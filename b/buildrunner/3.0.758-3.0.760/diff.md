# Comparing `tmp/buildrunner-3.0.758.tar.gz` & `tmp/buildrunner-3.0.760.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildrunner-3.0.758.tar", last modified: Wed Jun 28 22:38:01 2023, max compression
+gzip compressed data, was "buildrunner-3.0.760.tar", last modified: Mon Jul 17 17:37:17 2023, max compression
```

## Comparing `buildrunner-3.0.758.tar` & `buildrunner-3.0.760.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.654488 buildrunner-3.0.758/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-28 22:37:49.000000 buildrunner-3.0.758/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-28 22:37:49.000000 buildrunner-3.0.758/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-06-28 22:38:01.654488 buildrunner-3.0.758/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-06-28 22:37:49.000000 buildrunner-3.0.758/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.638488 buildrunner-3.0.758/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-28 22:37:49.000000 buildrunner-3.0.758/bin/buildrunner
--rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-06-28 22:37:49.000000 buildrunner-3.0.758/bin/buildrunner-cleanup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.642488 buildrunner-3.0.758/buildrunner/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/SourceDockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.646488 buildrunner-3.0.758/buildrunner/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/docker/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/docker/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/docker/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/docker/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.646488 buildrunner-3.0.758/buildrunner/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/fetch/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/fetch/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/fetch/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.646488 buildrunner-3.0.758/buildrunner/provisioners/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/provisioners/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/provisioners/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.650488 buildrunner-3.0.758/buildrunner/sshagent/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.650488 buildrunner-3.0.758/buildrunner/sshagent/SSHAgentProxyImage/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/sshagent/SSHAgentProxyImage/login.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/sshagent/SSHAgentProxyImage/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/sshagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.650488 buildrunner-3.0.758/buildrunner/steprunner/
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.654488 buildrunner-3.0.758/buildrunner/steprunner/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/tasks/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/tasks/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/tasks/pypipush.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/tasks/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    43785 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/steprunner/tasks/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-28 22:37:49.000000 buildrunner-3.0.758/buildrunner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-28 22:38:01.000000 buildrunner-3.0.758/buildrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.642488 buildrunner-3.0.758/buildrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-06-28 22:38:01.000000 buildrunner-3.0.758/buildrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-28 22:38:01.000000 buildrunner-3.0.758/buildrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:38:01.000000 buildrunner-3.0.758/buildrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-28 22:38:01.000000 buildrunner-3.0.758/buildrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 22:38:01.000000 buildrunner-3.0.758/buildrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-28 22:37:49.000000 buildrunner-3.0.758/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-28 22:38:01.658488 buildrunner-3.0.758/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-28 22:37:49.000000 buildrunner-3.0.758/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-28 22:37:49.000000 buildrunner-3.0.758/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:38:01.654488 buildrunner-3.0.758/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_buildrunner_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_push_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_util_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_utils_flock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-28 22:37:49.000000 buildrunner-3.0.758/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.541043 buildrunner-3.0.760/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-17 17:37:09.000000 buildrunner-3.0.760/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 17:37:09.000000 buildrunner-3.0.760/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-07-17 17:37:17.541043 buildrunner-3.0.760/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-07-17 17:37:09.000000 buildrunner-3.0.760/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.533043 buildrunner-3.0.760/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-07-17 17:37:09.000000 buildrunner-3.0.760/bin/buildrunner
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-07-17 17:37:09.000000 buildrunner-3.0.760/bin/buildrunner-cleanup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.533043 buildrunner-3.0.760/buildrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/SourceDockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/docker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/docker/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/docker/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/docker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/fetch/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/fetch/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/fetch/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/provisioners/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/provisioners/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/sshagent/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/sshagent/SSHAgentProxyImage/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/sshagent/SSHAgentProxyImage/login.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/sshagent/SSHAgentProxyImage/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/sshagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/steprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner/steprunner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/tasks/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/tasks/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/tasks/pypipush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/tasks/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44014 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/steprunner/tasks/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-17 17:37:09.000000 buildrunner-3.0.760/buildrunner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 17:37:17.000000 buildrunner-3.0.760/buildrunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.537043 buildrunner-3.0.760/buildrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-07-17 17:37:17.000000 buildrunner-3.0.760/buildrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-17 17:37:17.000000 buildrunner-3.0.760/buildrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:37:17.000000 buildrunner-3.0.760/buildrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-17 17:37:17.000000 buildrunner-3.0.760/buildrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 17:37:17.000000 buildrunner-3.0.760/buildrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-17 17:37:09.000000 buildrunner-3.0.760/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 17:37:17.541043 buildrunner-3.0.760/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-17 17:37:09.000000 buildrunner-3.0.760/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-17 17:37:09.000000 buildrunner-3.0.760/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:37:17.541043 buildrunner-3.0.760/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_buildrunner_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_push_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_util_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_utils_flock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-17 17:37:09.000000 buildrunner-3.0.760/tests/test_version.py
```

### Comparing `buildrunner-3.0.758/LICENSE` & `buildrunner-3.0.760/LICENSE`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/PKG-INFO` & `buildrunner-3.0.760/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.0.758
+Version: 3.0.760
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `buildrunner-3.0.758/README.rst` & `buildrunner-3.0.760/README.rst`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/__init__.py` & `buildrunner-3.0.760/buildrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/cli.py` & `buildrunner-3.0.760/buildrunner/cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/config.py` & `buildrunner-3.0.760/buildrunner/config.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/docker/__init__.py` & `buildrunner-3.0.760/buildrunner/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/docker/builder.py` & `buildrunner-3.0.760/buildrunner/docker/builder.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/docker/daemon.py` & `buildrunner-3.0.760/buildrunner/docker/daemon.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/docker/importer.py` & `buildrunner-3.0.760/buildrunner/docker/importer.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/docker/runner.py` & `buildrunner-3.0.760/buildrunner/docker/runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/errors.py` & `buildrunner-3.0.760/buildrunner/errors.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/fetch/__init__.py` & `buildrunner-3.0.760/buildrunner/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/fetch/github.py` & `buildrunner-3.0.760/buildrunner/fetch/github.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/provisioners/__init__.py` & `buildrunner-3.0.760/buildrunner/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/provisioners/salt.py` & `buildrunner-3.0.760/buildrunner/provisioners/salt.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/provisioners/shell.py` & `buildrunner-3.0.760/buildrunner/provisioners/shell.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile` & `buildrunner-3.0.760/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/sshagent/__init__.py` & `buildrunner-3.0.760/buildrunner/sshagent/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/__init__.py` & `buildrunner-3.0.760/buildrunner/steprunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/tasks/__init__.py` & `buildrunner-3.0.760/buildrunner/steprunner/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/tasks/build.py` & `buildrunner-3.0.760/buildrunner/steprunner/tasks/build.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/tasks/push.py` & `buildrunner-3.0.760/buildrunner/steprunner/tasks/push.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/tasks/pypipush.py` & `buildrunner-3.0.760/buildrunner/steprunner/tasks/pypipush.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/tasks/remote.py` & `buildrunner-3.0.760/buildrunner/steprunner/tasks/remote.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner/steprunner/tasks/run.py` & `buildrunner-3.0.760/buildrunner/steprunner/tasks/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1007,14 +1007,18 @@
             self.runner.restore_caches(container_meta_logger, caches)
 
             self.step_runner.log.write(
                 f'Started build container {container_id:.10}\n'
             )
 
             if _cmds:
+                # First ensure that the source directory is marked as safe for newer git versions
+                # Any errors are ignored here
+                self.runner.run("git config --global --add safe.directory /source")
+
                 # run each cmd
                 for _cmd in _cmds:
                     container_meta_logger.write(
                         f"cmd> {_cmd}\n"
                     )
                     exit_code = self.runner.run(
                         _cmd,
```

### Comparing `buildrunner-3.0.758/buildrunner/utils.py` & `buildrunner-3.0.760/buildrunner/utils.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner.egg-info/PKG-INFO` & `buildrunner-3.0.760/buildrunner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildrunner
-Version: 3.0.758
+Version: 3.0.760
 Summary: Docker-based build tool
 Home-page: https://github.com/adobe/buildrunner
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `buildrunner-3.0.758/buildrunner.egg-info/SOURCES.txt` & `buildrunner-3.0.760/buildrunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/buildrunner.egg-info/requires.txt` & `buildrunner-3.0.760/buildrunner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/requirements.txt` & `buildrunner-3.0.760/requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/setup.py` & `buildrunner-3.0.760/setup.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/test_requirements.txt` & `buildrunner-3.0.760/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_buildrunner_files.py` & `buildrunner-3.0.760/tests/test_buildrunner_files.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_caching.py` & `buildrunner-3.0.760/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_console_logger.py` & `buildrunner-3.0.760/tests/test_console_logger.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_dependencies.py` & `buildrunner-3.0.760/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_push_artifact.py` & `buildrunner-3.0.760/tests/test_push_artifact.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_runner.py` & `buildrunner-3.0.760/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_util_checksum.py` & `buildrunner-3.0.760/tests/test_util_checksum.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_utils_flock.py` & `buildrunner-3.0.760/tests/test_utils_flock.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.758/tests/test_version.py` & `buildrunner-3.0.760/tests/test_version.py`

 * *Files identical despite different names*

