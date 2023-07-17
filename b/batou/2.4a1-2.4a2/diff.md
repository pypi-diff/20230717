# Comparing `tmp/batou-2.4a1.tar.gz` & `tmp/batou-2.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batou-2.4a1.tar", last modified: Tue Jun 27 10:23:48 2023, max compression
+gzip compressed data, was "batou-2.4a2.tar", last modified: Fri Jul  7 13:32:54 2023, max compression
```

## Comparing `batou-2.4a1.tar` & `batou-2.4a2.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249645 batou-2.4a1/
--rw-r--r--   0 elikoga    (501) staff       (20)    31241 2023-06-27 10:23:47.000000 batou-2.4a1/CHANGES.history.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1608 2023-06-27 10:23:47.000000 batou-2.4a1/LICENSE.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      212 2023-06-27 10:23:47.000000 batou-2.4a1/MANIFEST.in
--rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-06-27 10:23:48.249710 batou-2.4a1/PKG-INFO
--rw-r--r--   0 elikoga    (501) staff       (20)     2636 2023-06-27 10:23:47.000000 batou-2.4a1/README.md
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.222552 batou-2.4a1/doc/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.228299 batou-2.4a1/doc/source/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.228745 batou-2.4a1/doc/source/api/
--rw-r--r--   0 elikoga    (501) staff       (20)      886 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/component.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1717 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/environment.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       48 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/templates.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       63 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/api/utilities.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.228850 batou-2.4a1/doc/source/cli/
--rw-r--r--   0 elikoga    (501) staff       (20)     4211 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/cli/index.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.229392 batou-2.4a1/doc/source/components/
--rw-r--r--   0 elikoga    (501) staff       (20)     1025 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/cmmi.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2941 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/downloads-vcs.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     5657 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/files.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     4820 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/python.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     3050 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/components/services.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.229847 batou-2.4a1/doc/source/dev/
--rw-r--r--   0 elikoga    (501) staff       (20)      718 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/authors.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     8555 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/contributing.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1711 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/testing.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2809 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/dev/todo.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     8488 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/index.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     4799 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/upgrading.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230489 batou-2.4a1/doc/source/user/
--rw-r--r--   0 elikoga    (501) staff       (20)    10870 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/advanced.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2565 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/install.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     3848 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/installation-deb.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     3798 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/installation-rpm.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     2907 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/intro.txt
--rw-r--r--   0 elikoga    (501) staff       (20)    47489 2023-06-27 10:23:47.000000 batou-2.4a1/doc/source/user/quickstart.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.224177 batou-2.4a1/examples/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230728 batou-2.4a1/examples/api/
--rw-r--r--   0 elikoga    (501) staff       (20)      349 2023-06-27 10:23:47.000000 batou-2.4a1/examples/api/index.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/api/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230831 batou-2.4a1/examples/django/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/django/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.230943 batou-2.4a1/examples/durations/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/durations/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231047 batou-2.4a1/examples/errors/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/errors/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231149 batou-2.4a1/examples/errors2/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/errors2/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231257 batou-2.4a1/examples/ignores/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/ignores/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231362 batou-2.4a1/examples/largetempl/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/largetempl/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231477 batou-2.4a1/examples/package/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/package/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231582 batou-2.4a1/examples/sync_async/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/sync_async/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231687 batou-2.4a1/examples/tutorial-buildout/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-buildout/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231798 batou-2.4a1/examples/tutorial-component/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-component/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.231908 batou-2.4a1/examples/tutorial-helloworld/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-helloworld/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232021 batou-2.4a1/examples/tutorial-parallelize/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-parallelize/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232129 batou-2.4a1/examples/tutorial-provision-container/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-provision-container/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232240 batou-2.4a1/examples/tutorial-secrets/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.223989 batou-2.4a1/examples/tutorial-secrets/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232360 batou-2.4a1/examples/tutorial-secrets/environments/age/
--rw-r--r--   0 elikoga    (501) staff       (20)     2431 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-secrets/environments/age/age_keys.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/tutorial-secrets/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232474 batou-2.4a1/examples/vagrant/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/vagrant/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232588 batou-2.4a1/examples/vagrant-multi/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/vagrant-multi/requirements.txt
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232694 batou-2.4a1/examples/venvs/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.232801 batou-2.4a1/examples/venvs/environments/
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/venvs/environments/requirements.txt
--rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-06-27 10:23:47.000000 batou-2.4a1/examples/venvs/requirements.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      129 2023-06-27 10:23:47.000000 batou-2.4a1/pyproject.toml
--rw-r--r--   0 elikoga    (501) staff       (20)      275 2023-06-27 10:23:47.000000 batou-2.4a1/requirements-dev.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      139 2023-06-27 10:23:48.249930 batou-2.4a1/setup.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)     2187 2023-06-27 10:23:47.000000 batou-2.4a1/setup.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.224422 batou-2.4a1/src/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.235088 batou-2.4a1/src/batou/
--rw-r--r--   0 elikoga    (501) staff       (20)    21062 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)      997 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/_output.py
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/agent.py
--rw-r--r--   0 elikoga    (501) staff       (20)      163 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/c.py
--rw-r--r--   0 elikoga    (501) staff       (20)    40510 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/component.py
--rw-r--r--   0 elikoga    (501) staff       (20)      795 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/conftest.py
--rw-r--r--   0 elikoga    (501) staff       (20)    14630 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/deploy.py
--rw-r--r--   0 elikoga    (501) staff       (20)    20522 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/environment.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1507 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/fixtures.py
--rw-r--r--   0 elikoga    (501) staff       (20)    11006 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/host.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.236056 batou-2.4a1/src/batou/init-template/
--rw-r--r--   0 elikoga    (501) staff       (20)       44 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/init-template/.hgignore
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.224602 batou-2.4a1/src/batou/init-template/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.236185 batou-2.4a1/src/batou/init-template/components/example/
--rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/init-template/components/example/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.236306 batou-2.4a1/src/batou/init-template/environments/
--rw-r--r--   0 elikoga    (501) staff       (20)       66 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/init-template/environments/dev.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      411 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/insecure-private.key
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.238659 batou-2.4a1/src/batou/lib/
--rw-r--r--   0 elikoga    (501) staff       (20)       29 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3983 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/appenv.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6457 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/archive.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3297 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/buildout.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2211 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/cmmi.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2524 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/cron.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1224 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/debian.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2286 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/download.py
--rw-r--r--   0 elikoga    (501) staff       (20)    22046 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/file.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6368 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/git.py
--rw-r--r--   0 elikoga    (501) staff       (20)      854 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/goceptnet.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1388 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/logrotate.py
--rw-r--r--   0 elikoga    (501) staff       (20)     4541 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/mercurial.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3647 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/mysql.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2814 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/nagios.py
--rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/package.py
--rw-r--r--   0 elikoga    (501) staff       (20)     8150 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/python.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.239663 batou-2.4a1/src/batou/lib/resources/
--rw-r--r--   0 elikoga    (501) staff       (20)     2120 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/check_supervisor.py.in
--rw-r--r--   0 elikoga    (501) staff       (20)      244 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/crontab
--rw-r--r--   0 elikoga    (501) staff       (20)      548 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/init.sh
--rw-r--r--   0 elikoga    (501) staff       (20)      299 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/logrotate.in
--rw-r--r--   0 elikoga    (501) staff       (20)      840 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/nagios.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      153 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/nrpe.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      380 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/supervisor.buildout.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      609 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/resources/supervisor.conf
--rw-r--r--   0 elikoga    (501) staff       (20)      932 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/service.py
--rw-r--r--   0 elikoga    (501) staff       (20)    10273 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/supervisor.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1172 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/svn.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.241720 batou-2.4a1/src/batou/lib/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3083 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_appenv.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3858 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_archive.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1689 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_buildout.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3261 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_cmmi.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2110 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_cron.py
--rw-r--r--   0 elikoga    (501) staff       (20)      639 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_debian.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2158 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_download.py
--rw-r--r--   0 elikoga    (501) staff       (20)    31505 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_file.py
--rw-r--r--   0 elikoga    (501) staff       (20)    10383 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_git.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6165 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_mercurial.py
--rw-r--r--   0 elikoga    (501) staff       (20)      121 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_mysql.py
--rw-r--r--   0 elikoga    (501) staff       (20)      847 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_nagios.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1165 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_python.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1693 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_service.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3106 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_supervisor.py
--rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/lib/tests/test_svn.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6247 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/main.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.241842 batou-2.4a1/src/batou/migrate/
--rw-r--r--   0 elikoga    (501) staff       (20)     3377 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/__init__.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.242578 batou-2.4a1/src/batou/migrate/migrations/
--rw-r--r--   0 elikoga    (501) staff       (20)      389 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2300.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1775 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2301.py
--rw-r--r--   0 elikoga    (501) staff       (20)      874 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2302.py
--rw-r--r--   0 elikoga    (501) staff       (20)      790 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2303.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1282 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/2400.py
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/migrations/__init__.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.242784 batou-2.4a1/src/batou/migrate/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     4532 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/migrate/tests/test_migrate.py
--rw-r--r--   0 elikoga    (501) staff       (20)    12756 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/provision.py
--rw-r--r--   0 elikoga    (501) staff       (20)    11713 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/remote_core.py
--rw-r--r--   0 elikoga    (501) staff       (20)    11793 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/repository.py
--rw-r--r--   0 elikoga    (501) staff       (20)     6424 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/resources.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.243284 batou-2.4a1/src/batou/secrets/
--rw-r--r--   0 elikoga    (501) staff       (20)    21705 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3872 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/edit.py
--rw-r--r--   0 elikoga    (501) staff       (20)    12486 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/encryption.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2695 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/manage.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.243775 batou-2.4a1/src/batou/secrets/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)       23 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/test_editor.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1566 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/test_manage.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2736 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/secrets/tests/test_secrets.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2429 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/template.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246239 batou-2.4a1/src/batou/tests/
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/__init__.py
--rw-r--r--   0 elikoga    (501) staff       (20)      666 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/conftest.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3012 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/ellipsis.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.227122 batou-2.4a1/src/batou/tests/fixture/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246369 batou-2.4a1/src/batou/tests/fixture/basic_service/
--rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/.batou.json
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.225530 batou-2.4a1/src/batou/tests/fixture/basic_service/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246503 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zeo/
--rw-r--r--   0 elikoga    (501) staff       (20)      178 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zeo/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246641 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zope/
--rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/components/zope/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.225713 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246787 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/dev/
--rw-r--r--   0 elikoga    (501) staff       (20)       79 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.246924 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/production/
--rw-r--r--   0 elikoga    (501) staff       (20)      128 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247058 batou-2.4a1/src/batou/tests/fixture/component/
--rw-r--r--   0 elikoga    (501) staff       (20)       40 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/component/haproxy.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247196 batou-2.4a1/src/batou/tests/fixture/sample_service/
--rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/.batou.json
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.225954 batou-2.4a1/src/batou/tests/fixture/sample_service/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247343 batou-2.4a1/src/batou/tests/fixture/sample_service/components/hello/
--rw-r--r--   0 elikoga    (501) staff       (20)      973 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/components/hello/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.226690 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247480 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
--rw-r--r--   0 elikoga    (501) staff       (20)      144 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247621 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
--rw-r--r--   0 elikoga    (501) staff       (20)       88 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247767 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
--rw-r--r--   0 elikoga    (501) staff       (20)      110 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.247907 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver/
--rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248037 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
--rw-r--r--   0 elikoga    (501) staff       (20)       90 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248169 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
--rw-r--r--   0 elikoga    (501) staff       (20)      191 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248305 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
--rw-r--r--   0 elikoga    (501) staff       (20)       94 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248454 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
--rw-r--r--   0 elikoga    (501) staff       (20)       85 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248597 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
--rw-r--r--   0 elikoga    (501) staff       (20)       64 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248731 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
--rw-r--r--   0 elikoga    (501) staff       (20)       26 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248860 batou-2.4a1/src/batou/tests/fixture/service_early_resource/
--rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/.batou.json
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.226940 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.248995 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zeo/
--rw-r--r--   0 elikoga    (501) staff       (20)      346 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249130 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zope/
--rw-r--r--   0 elikoga    (501) staff       (20)      116 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/components/zope/component.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.227053 batou-2.4a1/src/batou/tests/fixture/service_early_resource/environments/
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249262 batou-2.4a1/src/batou/tests/fixture/service_early_resource/environments/dev/
--rw-r--r--   0 elikoga    (501) staff       (20)       62 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.249513 batou-2.4a1/src/batou/tests/fixture/template/
--rw-r--r--   0 elikoga    (501) staff       (20)       84 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/template/haproxy.cfg
--rw-r--r--   0 elikoga    (501) staff       (20)      119 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/fixture/template/haproxy.cfg.jinja2
--rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_bootstrap.py
--rw-r--r--   0 elikoga    (501) staff       (20)    18479 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_component.py
--rw-r--r--   0 elikoga    (501) staff       (20)     4776 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_config.py
--rw-r--r--   0 elikoga    (501) staff       (20)     5707 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_dependencies.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1725 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_deploy.py
--rw-r--r--   0 elikoga    (501) staff       (20)    10550 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_endtoend.py
--rw-r--r--   0 elikoga    (501) staff       (20)     8674 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_environment.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2305 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_exceptions.py
--rw-r--r--   0 elikoga    (501) staff       (20)      606 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_host.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1488 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_main.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1326 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_remote.py
--rw-r--r--   0 elikoga    (501) staff       (20)     9398 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_remote_core.py
--rw-r--r--   0 elikoga    (501) staff       (20)     3648 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_repository.py
--rw-r--r--   0 elikoga    (501) staff       (20)      743 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_resources.py
--rw-r--r--   0 elikoga    (501) staff       (20)     2602 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_template.py
--rw-r--r--   0 elikoga    (501) staff       (20)    14060 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_utils.py
--rw-r--r--   0 elikoga    (501) staff       (20)     1169 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/tests/test_vfs.py
--rw-r--r--   0 elikoga    (501) staff       (20)    18387 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/utils.py
--rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/version.txt
--rw-r--r--   0 elikoga    (501) staff       (20)     1009 2023-06-27 10:23:47.000000 batou-2.4a1/src/batou/vfs.py
-drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-06-27 10:23:48.235937 batou-2.4a1/src/batou.egg-info/
--rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/PKG-INFO
--rw-r--r--   0 elikoga    (501) staff       (20)     6796 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/SOURCES.txt
--rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/dependency_links.txt
--rw-r--r--   0 elikoga    (501) staff       (20)      241 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/entry_points.txt
--rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/not-zip-safe
--rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/requires.txt
--rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-06-27 10:23:48.000000 batou-2.4a1/src/batou.egg-info/top_level.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.948596 batou-2.4a2/
+-rw-r--r--   0 elikoga    (501) staff       (20)    31241 2023-07-07 13:32:54.000000 batou-2.4a2/CHANGES.history.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1608 2023-07-07 13:32:54.000000 batou-2.4a2/LICENSE.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      212 2023-07-07 13:32:54.000000 batou-2.4a2/MANIFEST.in
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-07 13:32:54.948660 batou-2.4a2/PKG-INFO
+-rw-r--r--   0 elikoga    (501) staff       (20)     2636 2023-07-07 13:32:54.000000 batou-2.4a2/README.md
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.921559 batou-2.4a2/doc/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.928338 batou-2.4a2/doc/source/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.928889 batou-2.4a2/doc/source/api/
+-rw-r--r--   0 elikoga    (501) staff       (20)      886 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/api/component.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1717 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/api/environment.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       48 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/api/templates.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       63 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/api/utilities.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.929023 batou-2.4a2/doc/source/cli/
+-rw-r--r--   0 elikoga    (501) staff       (20)     4211 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/cli/index.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.929749 batou-2.4a2/doc/source/components/
+-rw-r--r--   0 elikoga    (501) staff       (20)     1025 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/components/cmmi.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2941 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/components/downloads-vcs.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     5657 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/components/files.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     4820 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/components/python.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3050 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/components/services.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.930244 batou-2.4a2/doc/source/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)      718 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/dev/authors.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     8555 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/dev/contributing.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1711 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/dev/testing.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2809 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/dev/todo.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     8500 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/index.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     4799 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/upgrading.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.930976 batou-2.4a2/doc/source/user/
+-rw-r--r--   0 elikoga    (501) staff       (20)    10870 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/user/advanced.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2565 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/user/install.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3848 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/user/installation-deb.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     3798 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/user/installation-rpm.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     2907 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/user/intro.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)    47489 2023-07-07 13:32:54.000000 batou-2.4a2/doc/source/user/quickstart.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.923210 batou-2.4a2/examples/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931250 batou-2.4a2/examples/api/
+-rw-r--r--   0 elikoga    (501) staff       (20)      349 2023-07-07 13:32:54.000000 batou-2.4a2/examples/api/index.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/api/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931370 batou-2.4a2/examples/django/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/django/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931490 batou-2.4a2/examples/durations/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/durations/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931606 batou-2.4a2/examples/errors/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/errors/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931734 batou-2.4a2/examples/errors2/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/errors2/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931861 batou-2.4a2/examples/ignores/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/ignores/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.931976 batou-2.4a2/examples/largetempl/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/largetempl/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932132 batou-2.4a2/examples/package/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/package/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932255 batou-2.4a2/examples/sync_async/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/sync_async/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932380 batou-2.4a2/examples/tutorial-buildout/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-buildout/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932506 batou-2.4a2/examples/tutorial-component/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-component/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932629 batou-2.4a2/examples/tutorial-helloworld/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-helloworld/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932756 batou-2.4a2/examples/tutorial-parallelize/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-parallelize/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.932916 batou-2.4a2/examples/tutorial-provision-container/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-provision-container/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.933046 batou-2.4a2/examples/tutorial-secrets/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.923014 batou-2.4a2/examples/tutorial-secrets/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.933176 batou-2.4a2/examples/tutorial-secrets/environments/age/
+-rw-r--r--   0 elikoga    (501) staff       (20)     2431 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-secrets/environments/age/age_keys.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/tutorial-secrets/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.933287 batou-2.4a2/examples/vagrant/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/vagrant/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.933405 batou-2.4a2/examples/vagrant-multi/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/vagrant-multi/requirements.txt
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.933513 batou-2.4a2/examples/venvs/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.933624 batou-2.4a2/examples/venvs/environments/
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/venvs/environments/requirements.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)       54 2023-07-07 13:32:54.000000 batou-2.4a2/examples/venvs/requirements.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      129 2023-07-07 13:32:54.000000 batou-2.4a2/pyproject.toml
+-rw-r--r--   0 elikoga    (501) staff       (20)      275 2023-07-07 13:32:54.000000 batou-2.4a2/requirements-dev.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      139 2023-07-07 13:32:54.948880 batou-2.4a2/setup.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)     2187 2023-07-07 13:32:54.000000 batou-2.4a2/setup.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.923446 batou-2.4a2/src/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.935724 batou-2.4a2/src/batou/
+-rw-r--r--   0 elikoga    (501) staff       (20)    21062 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      997 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/_output.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/agent.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      163 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/c.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    40510 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/component.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      795 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/conftest.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    14630 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/deploy.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    20522 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/environment.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1507 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/fixtures.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11006 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/host.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.936548 batou-2.4a2/src/batou/init-template/
+-rw-r--r--   0 elikoga    (501) staff       (20)       44 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/init-template/.hgignore
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.923632 batou-2.4a2/src/batou/init-template/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.936652 batou-2.4a2/src/batou/init-template/components/example/
+-rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/init-template/components/example/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.936763 batou-2.4a2/src/batou/init-template/environments/
+-rw-r--r--   0 elikoga    (501) staff       (20)       66 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/init-template/environments/dev.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      411 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/insecure-private.key
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.938848 batou-2.4a2/src/batou/lib/
+-rw-r--r--   0 elikoga    (501) staff       (20)       29 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3983 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/appenv.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6457 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/archive.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3297 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/buildout.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2211 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/cmmi.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2524 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/cron.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1224 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/debian.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2286 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/download.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    22046 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/file.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6368 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/git.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      854 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/goceptnet.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1388 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/logrotate.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4541 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/mercurial.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3647 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/mysql.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2814 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/nagios.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/package.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     8150 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/python.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.939695 batou-2.4a2/src/batou/lib/resources/
+-rw-r--r--   0 elikoga    (501) staff       (20)     2120 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/check_supervisor.py.in
+-rw-r--r--   0 elikoga    (501) staff       (20)      244 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/crontab
+-rw-r--r--   0 elikoga    (501) staff       (20)      548 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/init.sh
+-rw-r--r--   0 elikoga    (501) staff       (20)      299 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/logrotate.in
+-rw-r--r--   0 elikoga    (501) staff       (20)      840 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/nagios.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      153 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/nrpe.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      380 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/supervisor.buildout.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      609 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/resources/supervisor.conf
+-rw-r--r--   0 elikoga    (501) staff       (20)      932 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/service.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10273 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/supervisor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1172 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/svn.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.941495 batou-2.4a2/src/batou/lib/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3083 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_appenv.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3858 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_archive.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1689 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_buildout.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3261 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_cmmi.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2110 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_cron.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      639 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_debian.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2158 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_download.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    31505 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_file.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10383 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_git.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6165 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_mercurial.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      121 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_mysql.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      847 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_nagios.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1165 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_python.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1693 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_service.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3106 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_supervisor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      707 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/lib/tests/test_svn.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6247 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/main.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.941597 batou-2.4a2/src/batou/migrate/
+-rw-r--r--   0 elikoga    (501) staff       (20)     3377 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/__init__.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.942226 batou-2.4a2/src/batou/migrate/migrations/
+-rw-r--r--   0 elikoga    (501) staff       (20)      389 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/migrations/2300.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1775 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/migrations/2301.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      874 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/migrations/2302.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      790 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/migrations/2303.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1282 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/migrations/2400.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/migrations/__init__.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.942407 batou-2.4a2/src/batou/migrate/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4532 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/migrate/tests/test_migrate.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    12756 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/provision.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11713 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/remote_core.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    11793 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/repository.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     6424 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/resources.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.942841 batou-2.4a2/src/batou/secrets/
+-rw-r--r--   0 elikoga    (501) staff       (20)    22033 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3935 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/edit.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    12938 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/encryption.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2695 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/manage.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.943258 batou-2.4a2/src/batou/secrets/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)       23 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/tests/test_editor.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1566 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/tests/test_manage.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2736 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/secrets/tests/test_secrets.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2429 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/template.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.945367 batou-2.4a2/src/batou/tests/
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/__init__.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      666 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/conftest.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3012 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/ellipsis.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.926506 batou-2.4a2/src/batou/tests/fixture/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.945501 batou-2.4a2/src/batou/tests/fixture/basic_service/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/basic_service/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.924601 batou-2.4a2/src/batou/tests/fixture/basic_service/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.945629 batou-2.4a2/src/batou/tests/fixture/basic_service/components/zeo/
+-rw-r--r--   0 elikoga    (501) staff       (20)      178 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/basic_service/components/zeo/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.945754 batou-2.4a2/src/batou/tests/fixture/basic_service/components/zope/
+-rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/basic_service/components/zope/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.924784 batou-2.4a2/src/batou/tests/fixture/basic_service/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.945883 batou-2.4a2/src/batou/tests/fixture/basic_service/environments/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)       79 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/basic_service/environments/dev/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946007 batou-2.4a2/src/batou/tests/fixture/basic_service/environments/production/
+-rw-r--r--   0 elikoga    (501) staff       (20)      128 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/basic_service/environments/production/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946145 batou-2.4a2/src/batou/tests/fixture/component/
+-rw-r--r--   0 elikoga    (501) staff       (20)       40 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/component/haproxy.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946267 batou-2.4a2/src/batou/tests/fixture/sample_service/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.925054 batou-2.4a2/src/batou/tests/fixture/sample_service/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946392 batou-2.4a2/src/batou/tests/fixture/sample_service/components/hello/
+-rw-r--r--   0 elikoga    (501) staff       (20)      973 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/components/hello/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.925987 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946525 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-multiple-components/
+-rw-r--r--   0 elikoga    (501) staff       (20)      144 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-multiple-components/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946658 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/
+-rw-r--r--   0 elikoga    (501) staff       (20)       88 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-multiple-hosts/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946793 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/
+-rw-r--r--   0 elikoga    (501) staff       (20)      110 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-overlapping-components/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.946920 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-resolver/
+-rw-r--r--   0 elikoga    (501) staff       (20)       72 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-resolver/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947047 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/
+-rw-r--r--   0 elikoga    (501) staff       (20)       90 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-resolver-invalid/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947175 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-env-config/
+-rw-r--r--   0 elikoga    (501) staff       (20)      191 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-env-config/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947302 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-overrides/
+-rw-r--r--   0 elikoga    (501) staff       (20)       94 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-overrides/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947436 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/
+-rw-r--r--   0 elikoga    (501) staff       (20)       85 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-provide-require/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947564 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/
+-rw-r--r--   0 elikoga    (501) staff       (20)       64 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-with-vfs-sandbox/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947696 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-without-env-config/
+-rw-r--r--   0 elikoga    (501) staff       (20)       26 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/sample_service/environments/test-without-env-config/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947822 batou-2.4a2/src/batou/tests/fixture/service_early_resource/
+-rw-r--r--   0 elikoga    (501) staff       (20)       33 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/service_early_resource/.batou.json
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.926278 batou-2.4a2/src/batou/tests/fixture/service_early_resource/components/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.947952 batou-2.4a2/src/batou/tests/fixture/service_early_resource/components/zeo/
+-rw-r--r--   0 elikoga    (501) staff       (20)      346 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/service_early_resource/components/zeo/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.948083 batou-2.4a2/src/batou/tests/fixture/service_early_resource/components/zope/
+-rw-r--r--   0 elikoga    (501) staff       (20)      116 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/service_early_resource/components/zope/component.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.926421 batou-2.4a2/src/batou/tests/fixture/service_early_resource/environments/
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.948222 batou-2.4a2/src/batou/tests/fixture/service_early_resource/environments/dev/
+-rw-r--r--   0 elikoga    (501) staff       (20)       62 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/service_early_resource/environments/dev/environment.cfg
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.948475 batou-2.4a2/src/batou/tests/fixture/template/
+-rw-r--r--   0 elikoga    (501) staff       (20)       84 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/template/haproxy.cfg
+-rw-r--r--   0 elikoga    (501) staff       (20)      119 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/fixture/template/haproxy.cfg.jinja2
+-rw-r--r--   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_bootstrap.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    18479 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_component.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     4776 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_config.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     5707 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_dependencies.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1725 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_deploy.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    10550 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_endtoend.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     8674 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_environment.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2305 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_exceptions.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      606 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_host.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1488 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_main.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1326 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_remote.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     9398 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_remote_core.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     3648 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_repository.py
+-rw-r--r--   0 elikoga    (501) staff       (20)      743 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_resources.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     2602 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_template.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    14060 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_utils.py
+-rw-r--r--   0 elikoga    (501) staff       (20)     1169 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/tests/test_vfs.py
+-rw-r--r--   0 elikoga    (501) staff       (20)    18387 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/utils.py
+-rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/version.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)     1009 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou/vfs.py
+drwxr-xr-x   0 elikoga    (501) staff       (20)        0 2023-07-07 13:32:54.936447 batou-2.4a2/src/batou.egg-info/
+-rw-r--r--   0 elikoga    (501) staff       (20)     3465 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/PKG-INFO
+-rw-r--r--   0 elikoga    (501) staff       (20)     6796 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/SOURCES.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/dependency_links.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)      241 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/entry_points.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        1 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/not-zip-safe
+-rw-r--r--   0 elikoga    (501) staff       (20)      177 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/requires.txt
+-rw-r--r--   0 elikoga    (501) staff       (20)        6 2023-07-07 13:32:54.000000 batou-2.4a2/src/batou.egg-info/top_level.txt
```

### Comparing `batou-2.4a1/CHANGES.history.txt` & `batou-2.4a2/CHANGES.history.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/LICENSE.txt` & `batou-2.4a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/PKG-INFO` & `batou-2.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.4a1
+Version: 2.4a2
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Platform: UNKNOWN
```

### Comparing `batou-2.4a1/README.md` & `batou-2.4a2/README.md`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/api/component.txt` & `batou-2.4a2/doc/source/api/component.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/api/environment.txt` & `batou-2.4a2/doc/source/api/environment.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/cli/index.txt` & `batou-2.4a2/doc/source/cli/index.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/components/cmmi.txt` & `batou-2.4a2/doc/source/components/cmmi.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/components/downloads-vcs.txt` & `batou-2.4a2/doc/source/components/downloads-vcs.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/components/files.txt` & `batou-2.4a2/doc/source/components/files.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/components/python.txt` & `batou-2.4a2/doc/source/components/python.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/components/services.txt` & `batou-2.4a2/doc/source/components/services.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/dev/authors.txt` & `batou-2.4a2/doc/source/dev/authors.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/dev/contributing.txt` & `batou-2.4a2/doc/source/dev/contributing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/dev/testing.txt` & `batou-2.4a2/doc/source/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/dev/todo.txt` & `batou-2.4a2/doc/source/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/index.txt` & `batou-2.4a2/doc/source/index.txt`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 .. toctree::
    :maxdepth: 2
 
    user/intro
    user/install
    user/quickstart
    user/advanced
+   user/age
 
 Reference: Command line interface
 ---------------------------------
 
 If you are looking for information on what commands the batou CLI provides then this is for you.
 
 .. toctree::
```

### Comparing `batou-2.4a1/doc/source/upgrading.txt` & `batou-2.4a2/doc/source/upgrading.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/user/advanced.txt` & `batou-2.4a2/doc/source/user/advanced.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/user/install.txt` & `batou-2.4a2/doc/source/user/install.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/user/installation-deb.txt` & `batou-2.4a2/doc/source/user/installation-deb.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/user/installation-rpm.txt` & `batou-2.4a2/doc/source/user/installation-rpm.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/user/intro.txt` & `batou-2.4a2/doc/source/user/intro.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/doc/source/user/quickstart.txt` & `batou-2.4a2/doc/source/user/quickstart.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/examples/tutorial-secrets/environments/age/age_keys.txt` & `batou-2.4a2/examples/tutorial-secrets/environments/age/age_keys.txt`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/setup.py` & `batou-2.4a2/setup.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/__init__.py` & `batou-2.4a2/src/batou/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/_output.py` & `batou-2.4a2/src/batou/_output.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/component.py` & `batou-2.4a2/src/batou/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/conftest.py` & `batou-2.4a2/src/batou/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/deploy.py` & `batou-2.4a2/src/batou/deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/environment.py` & `batou-2.4a2/src/batou/environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/fixtures.py` & `batou-2.4a2/src/batou/fixtures.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/host.py` & `batou-2.4a2/src/batou/host.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/appenv.py` & `batou-2.4a2/src/batou/lib/appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/archive.py` & `batou-2.4a2/src/batou/lib/archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/buildout.py` & `batou-2.4a2/src/batou/lib/buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/cmmi.py` & `batou-2.4a2/src/batou/lib/cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/cron.py` & `batou-2.4a2/src/batou/lib/cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/debian.py` & `batou-2.4a2/src/batou/lib/debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/download.py` & `batou-2.4a2/src/batou/lib/download.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/file.py` & `batou-2.4a2/src/batou/lib/file.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/git.py` & `batou-2.4a2/src/batou/lib/git.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/goceptnet.py` & `batou-2.4a2/src/batou/lib/goceptnet.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/logrotate.py` & `batou-2.4a2/src/batou/lib/logrotate.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/mercurial.py` & `batou-2.4a2/src/batou/lib/mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/mysql.py` & `batou-2.4a2/src/batou/lib/mysql.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/nagios.py` & `batou-2.4a2/src/batou/lib/nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/package.py` & `batou-2.4a2/src/batou/lib/package.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/python.py` & `batou-2.4a2/src/batou/lib/python.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/resources/check_supervisor.py.in` & `batou-2.4a2/src/batou/lib/resources/check_supervisor.py.in`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/resources/init.sh` & `batou-2.4a2/src/batou/lib/resources/init.sh`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/resources/nagios.cfg` & `batou-2.4a2/src/batou/lib/resources/nagios.cfg`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/resources/supervisor.conf` & `batou-2.4a2/src/batou/lib/resources/supervisor.conf`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/service.py` & `batou-2.4a2/src/batou/lib/service.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/supervisor.py` & `batou-2.4a2/src/batou/lib/supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/svn.py` & `batou-2.4a2/src/batou/lib/svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_appenv.py` & `batou-2.4a2/src/batou/lib/tests/test_appenv.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_archive.py` & `batou-2.4a2/src/batou/lib/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_buildout.py` & `batou-2.4a2/src/batou/lib/tests/test_buildout.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_cmmi.py` & `batou-2.4a2/src/batou/lib/tests/test_cmmi.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_cron.py` & `batou-2.4a2/src/batou/lib/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_debian.py` & `batou-2.4a2/src/batou/lib/tests/test_debian.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_download.py` & `batou-2.4a2/src/batou/lib/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_file.py` & `batou-2.4a2/src/batou/lib/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_git.py` & `batou-2.4a2/src/batou/lib/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_mercurial.py` & `batou-2.4a2/src/batou/lib/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_nagios.py` & `batou-2.4a2/src/batou/lib/tests/test_nagios.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_python.py` & `batou-2.4a2/src/batou/lib/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_service.py` & `batou-2.4a2/src/batou/lib/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_supervisor.py` & `batou-2.4a2/src/batou/lib/tests/test_supervisor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/lib/tests/test_svn.py` & `batou-2.4a2/src/batou/lib/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/main.py` & `batou-2.4a2/src/batou/main.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/migrate/__init__.py` & `batou-2.4a2/src/batou/migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/migrate/migrations/2301.py` & `batou-2.4a2/src/batou/migrate/migrations/2301.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/migrate/migrations/2302.py` & `batou-2.4a2/src/batou/migrate/migrations/2302.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/migrate/migrations/2303.py` & `batou-2.4a2/src/batou/migrate/migrations/2303.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/migrate/migrations/2400.py` & `batou-2.4a2/src/batou/migrate/migrations/2400.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/migrate/tests/test_migrate.py` & `batou-2.4a2/src/batou/migrate/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/provision.py` & `batou-2.4a2/src/batou/provision.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/remote_core.py` & `batou-2.4a2/src/batou/remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/repository.py` & `batou-2.4a2/src/batou/repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/resources.py` & `batou-2.4a2/src/batou/resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/secrets/__init__.py` & `batou-2.4a2/src/batou/secrets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pathlib
+import re
 import urllib.request
 from typing import TYPE_CHECKING, Dict, List, Optional, Set
 
 from configupdater import ConfigUpdater
 
 from batou import DuplicateOverride, SuperfluousSecretsSection
 from batou._output import output
@@ -170,28 +171,24 @@
 
     def change_secret_provider(
         self,
         config: ConfigUpdater,
         old_secret_provider: "SecretProvider",
     ):
         new_secret_provider_str = config.get("batou", "secret_provider").value
-        # new_secret_provider: SecretProvider
-        # output.annotate(
-        #     f"Changing secret provider from {old_secret_provider} to {new_secret_provider}."
-        # )
         if new_secret_provider_str == "age":
             new_secret_provider = AGESecretProvider(self.environment)
         elif new_secret_provider_str == "gpg":
             new_secret_provider = GPGSecretProvider(self.environment)
         else:
             raise ValueError(
                 f"Invalid secret provider {new_secret_provider_str}.",
             )
         output.annotate(
-            f"Changing secret provider from {old_secret_provider} to {new_secret_provider}."
+            f"Changing secret provider from {old_secret_provider.secret_provider_str()} to {new_secret_provider.secret_provider_str()}."
         )
         new_secret_provider.write_config_new(str(config).encode("utf-8"))
         new_secret_provider.write_secret_files(
             old_secret_provider.read_secret_files()
         )
         self.environment.secret_provider = new_secret_provider
         old_secret_provider.purge()
@@ -201,14 +198,17 @@
 
     def purge(self):
         raise NotImplementedError("purge() not implemented.")
 
     def _get_recipients(self) -> List[str]:
         raise NotImplementedError("_get_recipients() not implemented.")
 
+    def secret_provider_str(self) -> str:
+        raise NotImplementedError("secret_provider_str() not implemented.")
+
 
 class SecretBlob:
     def __init__(
         self,
         host_data: Dict[str, Dict[str, str]],
         component_overrides: Dict[str, Dict[str, str]],
         secret_data: Set[str],
@@ -255,14 +255,17 @@
 
     def read_secret_files(self) -> Dict[str, bytes]:
         return {}
 
     def purge(self):
         pass
 
+    def secret_provider_str(self) -> str:
+        return "none"
+
 
 class ConfigFileSecretProvider(SecretProvider):
     config_file: EncryptedFile
 
     @property
     def config(self):
         return ConfigUpdater().read_string(self.config_file.cleartext)
@@ -322,17 +325,18 @@
         self.config_file.delete()
 
     def summary(self):
         print("\t members")
         with self.config_file:
             members = self.config.get("batou", "members")
             if members.value is not None:
-                for member in members.value.split(","):
+                for member in re.split(r"(\n|,)+", members.value):
                     member = member.strip()
-                    print(f"\t\t- {member}")
+                    if member:
+                        print(f"\t\t- {member}")
             else:
                 print("\t\tUndefined behavior.")
             if not members:
                 print("\t\t(none)")
             print("\t secret files")
             # Keys of self.f.files are strings, but self.path is pathlib.Path:
             files = self.read_secret_files().keys()
@@ -403,16 +407,16 @@
             writeable,
         )
 
     def _get_recipients(self) -> List[str]:
         recipients = self.config.get("batou", "members")
         if recipients.value is None:
             return []
-        recipients = recipients.value.split(",")
-        recipients = [r.strip() for r in recipients]
+        recipients = re.split(r"(\n|,)+", recipients.value)
+        recipients = [r.strip() for r in recipients if r.strip()]
         return recipients
 
     def write_config(self, content: bytes):
         config = ConfigUpdater().read_string(content.decode("utf-8"))
         secret_provider = config.get("batou", "secret_provider", fallback=None)
         if secret_provider is None or secret_provider.value is None:
             config.set("batou", "secret_provider", "gpg")
@@ -422,26 +426,29 @@
             self.change_secret_provider(config, self)
             return
         recipients_opt = config.get("batou", "members")
         if recipients_opt is None or recipients_opt.value is None:
             raise ValueError(
                 "Please add a 'batou.members' section to the secrets file."
             )
-        recipients = recipients_opt.value.split(",")
-        recipients = [r.strip() for r in recipients]
+        recipients = re.split(r"(\n|,)+", recipients_opt.value)
+        recipients = [r.strip() for r in recipients if r.strip()]
         if not recipients or len(recipients) == 0 or recipients[0] == "":
             raise ValueError(
                 "Please add at least one recipient to the secrets file."
             )
         self.config_file.write(
             str(config).encode("utf-8"),
             recipients,
         )
         self.write_secret_files(self.read_secret_files())
 
+    def secret_provider_str(self) -> str:
+        return "gpg"
+
 
 def process_age_recipients(members, environment_path):
     """Process the recipients list."""
     key_meta_file_path = os.path.join(
         environment_path,
         "age_keys.txt",
     )
@@ -537,16 +544,16 @@
             writeable,
         )
 
     def _get_recipients(self) -> List[str]:
         recipients = self.config.get("batou", "members")
         if recipients.value is None:
             return []
-        recipients = recipients.value.split(",")
-        recipients = [r.strip() for r in recipients]
+        recipients = re.split(r"(\n|,)+", recipients.value)
+        recipients = [r.strip() for r in recipients if r.strip()]
         return process_age_recipients(
             recipients,
             pathlib.Path(self.environment.base_dir)
             / pathlib.Path("environments")
             / self.environment.name,
         )
 
@@ -561,16 +568,16 @@
             self.change_secret_provider(config, self)
             return
         recipients_opt = config.get("batou", "members")
         if recipients_opt is None or recipients_opt.value is None:
             raise ValueError(
                 "Please add a 'batou.members' section to the secrets file."
             )
-        recipients = recipients_opt.value.split(",")
-        recipients = [r.strip() for r in recipients]
+        recipients = re.split(r"(\n|,)+", recipients_opt.value)
+        recipients = [r.strip() for r in recipients if r.strip()]
         if not recipients or len(recipients) == 0 or recipients[0] == "":
             raise ValueError(
                 "Please add at least one recipient to the secrets file."
             )
         recipients = process_age_recipients(
             recipients,
             pathlib.Path(self.environment.base_dir)
@@ -578,7 +585,10 @@
             / self.environment.name,
         )
         self.config_file.write(
             str(config).encode("utf-8"),
             recipients,
         )
         self.write_secret_files(self.read_secret_files())
+
+    def secret_provider_str(self) -> str:
+        return "age"
```

### Comparing `batou-2.4a1/src/batou/secrets/edit.py` & `batou-2.4a2/src/batou/secrets/edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,16 @@
                 )
         else:
             self.environment.secret_provider.write_config(
                 self.cleartext.encode("utf-8")
             )
 
     def edit(self):
-        _, suffix = os.path.splitext(self.file.path.name)
+        filename, _encryption_ext = os.path.splitext(self.file.path.name)
+        _, suffix = os.path.splitext(filename)
         with tempfile.NamedTemporaryFile(
             prefix="edit", suffix=suffix, mode="w+", encoding="utf-8"
         ) as clearfile:
             clearfile.write(self.cleartext)
             clearfile.flush()
 
             args = [self.editor_cmd + " " + clearfile.name]
```

### Comparing `batou-2.4a1/src/batou/secrets/encryption.py` & `batou-2.4a2/src/batou/secrets/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,24 +325,34 @@
                 if matches:
                     passphrase = get_passphrase(identity)
                     os.write(fd, passphrase.encode("utf-8") + b"\n")
                     matches, out = expect(fd, b"\r\r\n")
                     if not matches:
                         exceptions.append(
                             Exception(
-                                "Unexpected output from age: {}".format(out)
+                                'Unexpected output from age, expected "\\r\\r\\n": {}'.format(
+                                    out
+                                )
                             )
                         )
                         continue
                     # also assert, that output is empty from now on
-                    chunk = os.read(fd, 1024)
-                    if chunk:
+                    buffer = b""
+                    while True:
+                        chunk = os.read(fd, 1024)
+                        if not chunk:
+                            break
+                        buffer += chunk
+                    if buffer:
+                        magic_bytes = b"\x1b[F\x1b[K"
+                        if buffer.startswith(magic_bytes):
+                            buffer = buffer[len(magic_bytes) :]
                         exceptions.append(
                             Exception(
-                                "Unexpected output from age: {}".format(chunk)
+                                "Unexpected output from age: {}".format(buffer)
                             )
                         )
                         continue
 
                 # Wait for the child to exit
                 pid, exitcode = os.waitpid(child_pid, 0)
```

### Comparing `batou-2.4a1/src/batou/secrets/manage.py` & `batou-2.4a2/src/batou/secrets/manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/secrets/tests/test_editor.py` & `batou-2.4a2/src/batou/secrets/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/secrets/tests/test_manage.py` & `batou-2.4a2/src/batou/secrets/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/secrets/tests/test_secrets.py` & `batou-2.4a2/src/batou/secrets/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/template.py` & `batou-2.4a2/src/batou/template.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/conftest.py` & `batou-2.4a2/src/batou/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/ellipsis.py` & `batou-2.4a2/src/batou/tests/ellipsis.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/fixture/sample_service/components/hello/component.py` & `batou-2.4a2/src/batou/tests/fixture/sample_service/components/hello/component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_component.py` & `batou-2.4a2/src/batou/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_config.py` & `batou-2.4a2/src/batou/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_dependencies.py` & `batou-2.4a2/src/batou/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_deploy.py` & `batou-2.4a2/src/batou/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_endtoend.py` & `batou-2.4a2/src/batou/tests/test_endtoend.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_environment.py` & `batou-2.4a2/src/batou/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_exceptions.py` & `batou-2.4a2/src/batou/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_host.py` & `batou-2.4a2/src/batou/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_main.py` & `batou-2.4a2/src/batou/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_remote.py` & `batou-2.4a2/src/batou/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_remote_core.py` & `batou-2.4a2/src/batou/tests/test_remote_core.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_repository.py` & `batou-2.4a2/src/batou/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_resources.py` & `batou-2.4a2/src/batou/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_template.py` & `batou-2.4a2/src/batou/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_utils.py` & `batou-2.4a2/src/batou/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/tests/test_vfs.py` & `batou-2.4a2/src/batou/tests/test_vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/utils.py` & `batou-2.4a2/src/batou/utils.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou/vfs.py` & `batou-2.4a2/src/batou/vfs.py`

 * *Files identical despite different names*

### Comparing `batou-2.4a1/src/batou.egg-info/PKG-INFO` & `batou-2.4a2/src/batou.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batou
-Version: 2.4a1
+Version: 2.4a2
 Summary: A utility for automating multi-host, multi-environment software builds and deployments.
 Home-page: https://batou.readthedocs.io/en/latest/
 Author: Christian Theune
 Author-email: ct@flyingcircus.io
 License: BSD (2-clause)
 Keywords: deployment
 Platform: UNKNOWN
```

### Comparing `batou-2.4a1/src/batou.egg-info/SOURCES.txt` & `batou-2.4a2/src/batou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

