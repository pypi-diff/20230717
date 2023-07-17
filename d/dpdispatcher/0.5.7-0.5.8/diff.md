# Comparing `tmp/dpdispatcher-0.5.7.tar.gz` & `tmp/dpdispatcher-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpdispatcher-0.5.7.tar", last modified: Tue Jun 27 23:33:24 2023, max compression
+gzip compressed data, was "dpdispatcher-0.5.8.tar", last modified: Mon Jul 17 08:13:01 2023, max compression
```

## Comparing `dpdispatcher-0.5.7.tar` & `dpdispatcher-0.5.8.tar`

### file list

```diff
@@ -1,298 +1,301 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.163883 dpdispatcher-0.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.167883 dpdispatcher-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/machines.yml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/publish_conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/pyright.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/ci/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/ci/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/pbs/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/pbs/start-pbs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/pbs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/ci/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/slurm/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/slurm/register_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/slurm/start-slurm.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/slurm.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/ci/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/ssh/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/ssh/start-ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/ci/ssh_rsync.sh
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/conda/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/conda/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/batch.md
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/context.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/dpdispatcher_on_yarn.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.171883 dpdispatcher-0.5.7/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/examples/expanse.md
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/examples/g16.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/examples/shell.md
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/doc/task.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.175883 dpdispatcher-0.5.7/dpdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/JobStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/arginfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/base_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/distributed_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dp_cloud_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dp_cloud_server_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.175883 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/retcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/temp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/zip_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/dpdisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/hdfs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/hdfs_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/ssh_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    44077 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/dpdispatcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.175883 dpdispatcher-0.5.7/dpdispatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 23:33:24.000000 dpdispatcher-0.5.7/dpdispatcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.163883 dpdispatcher-0.5.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.175883 dpdispatcher-0.5.7/examples/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/machine/expanse.json
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/machine/lazy_local.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/machine/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.175883 dpdispatcher-0.5.7/examples/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/resources/expanse_cpu.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/resources/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.179884 dpdispatcher-0.5.7/examples/task/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/task/deepmd-kit.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/examples/task/g16.json
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.179884 dpdispatcher-0.5.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/scripts/script_gen_dargs_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/scripts/script_gen_dargs_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.183884 dpdispatcher-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/batch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/debug_test_class_submission_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_dp_cloud_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_lazy_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_lsf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_slurm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2629 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/devel_test_ssh_ali_ehpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.183884 dpdispatcher-0.5.7/tests/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/job.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine.json
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_ali_ehpc.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_center.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_diffenert.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_dp_cloud_server.json
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_if_cuda_multi_devices.json
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_lazy_local_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_lazy_local_slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_lazylocal_shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_local_shell.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/machine_yarn.json
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/resources.json
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/submission.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/jsons/task.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.183884 dpdispatcher-0.5.7/tests/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/lsf/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/lsf/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/lsf/test_lsf_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.183884 dpdispatcher-0.5.7/tests/old/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/old/test_dispatcher_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/old/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/old/test_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/old/test_local_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/old/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.183884 dpdispatcher-0.5.7/tests/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/pbs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/pbs/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/pbs/test_pbs_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/sample_class.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/script_gen_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.183884 dpdispatcher-0.5.7/tests/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/shell/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/shell/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/shell/test_shell_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/shell/test_shell_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm/test_dispatcher_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm/test_slurm_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm/test_slurm_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm/test_slurm_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/slurm_test.env
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_argcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_machine_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_submission_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_class_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.163883 dpdispatcher-0.5.7/tests/test_context_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-1/some_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-1/some_dir/some_file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-4/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/dir with space/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/dir with space/file with space
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_context_dir/0_md/some_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_context_dir/0_md/some_dir/some_file
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.163883 dpdispatcher-0.5.7/tests/test_hdfs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.167883 dpdispatcher-0.5.7/tests/test_if_cuda_multi_devices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_if_cuda_multi_devices/test_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_if_cuda_multi_devices/test_dir/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_import_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_local_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.167883 dpdispatcher-0.5.7/tests/test_lsf_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.187884 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_lsf_script_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.167883 dpdispatcher-0.5.7/tests/test_pbs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_run_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_run_submission_ratio_unfinished.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1913 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_cuda_multi_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4895 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.167883 dpdispatcher-0.5.7/tests/test_shell_trival_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/fail_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir with space/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir3/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir4/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/parent_dir/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_shell_trival_dir/recover_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.167883 dpdispatcher-0.5.7/tests/test_slurm_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2349 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_slurm_script_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:24.191884 dpdispatcher-0.5.7/tests/test_work_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 23:33:14.000000 dpdispatcher-0.5.7/tests/test_work_path/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/machines.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/publish_conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/pyright.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/pbs/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/pbs/start-pbs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/pbs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm/register_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm/start-slurm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh/start-ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh_rsync.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/conda/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/batch.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/context.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/dpdispatcher_on_yarn.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/examples/expanse.md
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/examples/g16.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/examples/shell.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/task.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/dpdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/JobStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 08:13:00.000000 dpdispatcher-0.5.8/dpdispatcher/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/arginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/base_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/distributed_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/retcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/temp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/zip_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpdisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/fugaku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/hdfs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/hdfs_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/ssh_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/dpdispatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/examples/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/machine/expanse.json
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/machine/lazy_local.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/machine/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/resources/expanse_cpu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/resources/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/examples/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/task/deepmd-kit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/task/g16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.086121 dpdispatcher-0.5.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/scripts/script_gen_dargs_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/scripts/script_gen_dargs_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.090122 dpdispatcher-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/debug_test_class_submission_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_dp_cloud_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_lazy_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_lsf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_slurm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2629 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_ssh_ali_ehpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_ali_ehpc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_center.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_diffenert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_dp_cloud_server.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_fugaku.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_if_cuda_multi_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lazylocal_shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_local_fugaku.json
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_local_shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_yarn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/resources.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/submission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/task.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/lsf/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/lsf/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/lsf/test_lsf_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_dispatcher_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_local_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/pbs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/pbs/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/pbs/test_pbs_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/sample_class.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/script_gen_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/test_shell_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/test_shell_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_dispatcher_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_slurm_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_slurm_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_slurm_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm_test.env
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_argcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_machine_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_submission_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/tests/test_context_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/some_dir/some_file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/dir with space/file with space
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/some_dir/some_file
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/tests/test_hdfs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/tests/test_if_cuda_multi_devices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_if_cuda_multi_devices/test_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_if_cuda_multi_devices/test_dir/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_import_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_local_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_lsf_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_script_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_pbs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_run_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_run_submission_ratio_unfinished.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1913 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_cuda_multi_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4895 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_shell_trival_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/fail_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir3/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir4/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/recover_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_slurm_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2349 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_script_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_work_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_work_path/.gitkeep
```

### Comparing `dpdispatcher-0.5.7/.github/workflows/ci-docker.yml` & `dpdispatcher-0.5.8/.github/workflows/ci-docker.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/.github/workflows/test.yml` & `dpdispatcher-0.5.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/.pre-commit-config.yaml` & `dpdispatcher-0.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/CONTRIBUTING.md` & `dpdispatcher-0.5.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/LICENSE` & `dpdispatcher-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/PKG-INFO` & `dpdispatcher-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.5.7
+Version: 0.5.8
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dpdispatcher-0.5.7/README.md` & `dpdispatcher-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/LICENSE` & `dpdispatcher-0.5.8/ci/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/pbs/docker-compose.yml` & `dpdispatcher-0.5.8/ci/pbs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/pbs.sh` & `dpdispatcher-0.5.8/ci/pbs.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/slurm/docker-compose.yml` & `dpdispatcher-0.5.8/ci/slurm/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/slurm/start-slurm.sh` & `dpdispatcher-0.5.8/ci/slurm/start-slurm.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/ssh/docker-compose.yml` & `dpdispatcher-0.5.8/ci/ssh/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/ci/ssh_rsync.sh` & `dpdispatcher-0.5.8/ci/ssh_rsync.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/conda/meta.yaml` & `dpdispatcher-0.5.8/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/.gitignore` & `dpdispatcher-0.5.8/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/Makefile` & `dpdispatcher-0.5.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/batch.md` & `dpdispatcher-0.5.8/doc/batch.md`

 * *Files 25% similar despite different names*

```diff
@@ -58,7 +58,15 @@
 
 ## DistributedShell
 
 {dargs:argument}`batch_type <resources/batch_type>`: `DistributedShell`
 
 `DistributedShell` is used to submit yarn jobs.
 Read [Support DPDispatcher on Yarn](dpdispatcher_on_yarn.md) for details.
+
+## Fugaku
+
+{dargs:argument}`batch_type <resources/batch_type>`: `Fugaku`
+
+[Fujitsu cloud service](https://doc.cloud.global.fujitsu.com/lib/common/jp/hpc-user-manual/) is a job scheduling system used by Fujitsu's HPCs such as Fugaku, ITO and K computer. It should be noted that although the same job scheduling system is used, there are some differences in the details, Fagaku class cannot be directly used for other HPCs.
+
+Read Fujitsu cloud service documentation for details.
```

### Comparing `dpdispatcher-0.5.7/doc/conf.py` & `dpdispatcher-0.5.8/doc/conf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/context.md` & `dpdispatcher-0.5.8/doc/context.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/dpdispatcher_on_yarn.md` & `dpdispatcher-0.5.8/doc/dpdispatcher_on_yarn.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/examples/expanse.md` & `dpdispatcher-0.5.8/doc/examples/expanse.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/examples/shell.md` & `dpdispatcher-0.5.8/doc/examples/shell.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/getting-started.md` & `dpdispatcher-0.5.8/doc/getting-started.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/index.rst` & `dpdispatcher-0.5.8/doc/index.rst`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/doc/make.bat` & `dpdispatcher-0.5.8/doc/make.bat`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/__init__.py` & `dpdispatcher-0.5.8/dpdispatcher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     from ._version import version as __version__
 except ImportError:
     __version__ = "unkown"
 
 from .distributed_shell import DistributedShell
 from .dp_cloud_server import DpCloudServer, Lebesgue
 from .dp_cloud_server_context import DpCloudServerContext, LebesgueContext
+from .fugaku import Fugaku
 from .hdfs_context import HDFSContext
 from .lazy_local_context import LazyLocalContext
 from .local_context import LocalContext
 from .lsf import LSF
 from .machine import Machine
 from .pbs import PBS, Torque
 from .shell import Shell
@@ -81,14 +82,15 @@
     "LazyLocalContext",
     "LocalContext",
     "LSF",
     "Machine",
     "PBS",
     "Shell",
     "Slurm",
+    "Fugaku",
     "SSHContext",
     "Submission",
     "Task",
     "Torque",
     "info",
     "Lebesgue",
     "LebesgueContext",
```

### Comparing `dpdispatcher-0.5.7/dpdispatcher/base_context.py` & `dpdispatcher-0.5.8/dpdispatcher/base_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/distributed_shell.py` & `dpdispatcher-0.5.8/dpdispatcher/distributed_shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dp_cloud_server.py` & `dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dp_cloud_server_context.py` & `dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/client.py` & `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/client.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/config.py` & `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/config.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/retcode.py` & `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/retcode.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/temp_test.py` & `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/temp_test.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/dpcloudserver/zip_file.py` & `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/zip_file.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/hdfs_cli.py` & `dpdispatcher-0.5.8/dpdispatcher/hdfs_cli.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/hdfs_context.py` & `dpdispatcher-0.5.8/dpdispatcher/hdfs_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/lazy_local_context.py` & `dpdispatcher-0.5.8/dpdispatcher/lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/local_context.py` & `dpdispatcher-0.5.8/dpdispatcher/local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/lsf.py` & `dpdispatcher-0.5.8/dpdispatcher/lsf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/machine.py` & `dpdispatcher-0.5.8/dpdispatcher/machine.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/pbs.py` & `dpdispatcher-0.5.8/dpdispatcher/pbs.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/shell.py` & `dpdispatcher-0.5.8/dpdispatcher/shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/slurm.py` & `dpdispatcher-0.5.8/dpdispatcher/slurm.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/ssh_context.py` & `dpdispatcher-0.5.8/dpdispatcher/ssh_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher/submission.py` & `dpdispatcher-0.5.8/dpdispatcher/submission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # %%
+import asyncio
 import copy
+import functools
 import json
 import os
 import pathlib
 import random
 import time
 import uuid
 from hashlib import sha1
@@ -195,15 +197,17 @@
         for job in self.belonging_jobs:
             job.machine = machine
         if machine is not None:
             self.machine.context.bind_submission(self)
             self.local_root = machine.context.temp_local_root
         return self
 
-    def run_submission(self, *, dry_run=False, exit_on_submit=False, clean=True):
+    def run_submission(
+        self, *, dry_run=False, exit_on_submit=False, clean=True, check_interval=30
+    ):
         """Main method to execute the submission.
         First, check whether old Submission exists on the remote machine, and try to recover from it.
         Second, upload the local files to the remote machine where the tasks to be executed.
         Third, run the submission defined previously.
         Forth, wait until the tasks in the submission finished and download the result file to local directory.
         If dry_run is True, submission will be uploaded but not be executed and exit.
         If exit_on_submit is True, submission will exit.
@@ -236,34 +240,94 @@
                 dlog.info(f"at {self.machine.context.remote_root}")
                 return self.serialize()
             if ratio_unfinished > 0.0 and self.check_ratio_unfinished(ratio_unfinished):
                 self.remove_unfinished_tasks()
                 break
 
             try:
-                time.sleep(30)
+                time.sleep(check_interval)
             except (Exception, KeyboardInterrupt, SystemExit) as e:
                 self.submission_to_json()
                 dlog.exception(e)
                 dlog.info(f"submission exit: {self.submission_hash}")
                 dlog.info(f"at {self.machine.context.remote_root}")
                 dlog.debug(self.serialize())
                 raise e
             else:
                 self.update_submission_state()
                 self.handle_unexpected_submission_state()
             finally:
                 pass
         self.handle_unexpected_submission_state()
-        self.download_jobs()
+        self.try_download_result()
         self.submission_to_json()
         if clean:
             self.clean_jobs()
         return self.serialize()
 
+    def try_download_result(self):
+        start_time = time.time()
+        retry_interval = 60  # 每1分钟重试一次
+        success = False
+        while not success:
+            try:
+                self.download_jobs()
+                success = True
+            except (EOFError, Exception) as e:
+                dlog.exception(e)
+                elapsed_time = time.time() - start_time
+                if elapsed_time < 3600:  # 1小时内
+                    dlog.info("Retrying in 1 minute...")
+                    time.sleep(retry_interval)
+                elif elapsed_time < 86400:  # 1小时后，但在24小时内
+                    retry_interval = 600  # 每10分钟重试一次
+                    dlog.info("Retrying in 10 minutes...")
+                    time.sleep(retry_interval)
+                else:  # 超过24小时
+                    dlog.info("Maximum retries time reached. Exiting.")
+                    break
+
+    async def async_run_submission(self, **kwargs):
+        """Async interface of run_submission.
+
+        Examples
+        --------
+        >>> import asyncio
+        >>> from dpdispacher import Machine, Resource, Submission
+        >>> async def run_jobs():
+        ...     backgroud_task = set()
+        ...     # task1
+        ...     task1 = Task(...)
+        ...     submission1 = Submission(..., task_list=[task1])
+        ...     background_task = asyncio.create_task(
+        ...         submission1.async_run_submission(check_interval=2, clean=False)
+        ...     )
+        ...     # task2
+        ...     task2 = Task(...)
+        ...     submission2 = Submission(..., task_list=[task1])
+        ...     background_task = asyncio.create_task(
+        ...         submission2.async_run_submission(check_interval=2, clean=False)
+        ...     )
+        ...     background_tasks.add(background_task)
+        ...     result = await asyncio.gather(*background_tasks)
+        ...     return result
+        >>> run_jobs()
+
+        May raise Error if pass `clean=True` explicitly when submit to pbs or slurm.
+        """
+        kwargs = {**{"clean": False}, **kwargs}
+        if kwargs["clean"]:
+            dlog.warning(
+                "Using async submission with `clean=True`, "
+                "job may fail in queue system"
+            )
+        loop = asyncio.get_event_loop()
+        wrapped_submission = functools.partial(self.run_submission, **kwargs)
+        return await loop.run_in_executor(None, wrapped_submission)
+
     def update_submission_state(self):
         """Check whether all the jobs in the submission.
 
         Notes
         -----
         this method will not handle unexpected (like resubmit terminated) job state in the submission.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dpdispatcher-0.5.7/dpdispatcher/utils.py` & `dpdispatcher-0.5.8/dpdispatcher/utils.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/dpdispatcher.egg-info/PKG-INFO` & `dpdispatcher-0.5.8/dpdispatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.5.7
+Version: 0.5.8
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dpdispatcher-0.5.7/dpdispatcher.egg-info/SOURCES.txt` & `dpdispatcher-0.5.8/dpdispatcher.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 dpdispatcher/_version.py
 dpdispatcher/arginfo.py
 dpdispatcher/base_context.py
 dpdispatcher/distributed_shell.py
 dpdispatcher/dp_cloud_server.py
 dpdispatcher/dp_cloud_server_context.py
 dpdispatcher/dpdisp.py
+dpdispatcher/fugaku.py
 dpdispatcher/hdfs_cli.py
 dpdispatcher/hdfs_context.py
 dpdispatcher/lazy_local_context.py
 dpdispatcher/local_context.py
 dpdispatcher/lsf.py
 dpdispatcher/machine.py
 dpdispatcher/pbs.py
@@ -127,18 +128,20 @@
 tests/test_ssh_context.py
 tests/jsons/job.json
 tests/jsons/machine.json
 tests/jsons/machine_ali_ehpc.json
 tests/jsons/machine_center.json
 tests/jsons/machine_diffenert.json
 tests/jsons/machine_dp_cloud_server.json
+tests/jsons/machine_fugaku.json
 tests/jsons/machine_if_cuda_multi_devices.json
 tests/jsons/machine_lazy_local_lsf.json
 tests/jsons/machine_lazy_local_slurm.json
 tests/jsons/machine_lazylocal_shell.json
+tests/jsons/machine_local_fugaku.json
 tests/jsons/machine_local_shell.json
 tests/jsons/machine_lsf.json
 tests/jsons/machine_slurm.json
 tests/jsons/machine_yarn.json
 tests/jsons/resources.json
 tests/jsons/submission.json
 tests/jsons/task.json
```

### Comparing `dpdispatcher-0.5.7/examples/resources/expanse_cpu.json` & `dpdispatcher-0.5.8/examples/resources/expanse_cpu.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/pyproject.toml` & `dpdispatcher-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/scripts/script_gen_dargs_docs.py` & `dpdispatcher-0.5.8/scripts/script_gen_dargs_docs.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/context.py` & `dpdispatcher-0.5.8/tests/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/debug_test_class_submission_init.py` & `dpdispatcher-0.5.8/tests/debug_test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_ali_ehpc.py` & `dpdispatcher-0.5.8/tests/devel_test_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_dp_cloud_server.py` & `dpdispatcher-0.5.8/tests/devel_test_dp_cloud_server.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_lazy_ali_ehpc.py` & `dpdispatcher-0.5.8/tests/devel_test_lazy_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_lsf.py` & `dpdispatcher-0.5.8/tests/devel_test_lsf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_shell.py` & `dpdispatcher-0.5.8/tests/devel_test_shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_slurm.py` & `dpdispatcher-0.5.8/tests/devel_test_slurm.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/devel_test_ssh_ali_ehpc.py` & `dpdispatcher-0.5.8/tests/devel_test_ssh_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/job.json` & `dpdispatcher-0.5.8/tests/jsons/job.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_center.json` & `dpdispatcher-0.5.8/tests/jsons/machine_center.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_diffenert.json` & `dpdispatcher-0.5.8/tests/jsons/machine_diffenert.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_dp_cloud_server.json` & `dpdispatcher-0.5.8/tests/jsons/machine_dp_cloud_server.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_lazy_local_lsf.json` & `dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_lazy_local_slurm.json` & `dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_lsf.json` & `dpdispatcher-0.5.8/tests/jsons/machine_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_slurm.json` & `dpdispatcher-0.5.8/tests/jsons/machine_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/machine_yarn.json` & `dpdispatcher-0.5.8/tests/jsons/machine_yarn.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/jsons/submission.json` & `dpdispatcher-0.5.8/tests/jsons/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/lsf/context.py` & `dpdispatcher-0.5.8/tests/lsf/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/lsf/test_dispatcher.py` & `dpdispatcher-0.5.8/tests/lsf/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/lsf/test_lsf_local.py` & `dpdispatcher-0.5.8/tests/lsf/test_lsf_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/old/test_dispatcher_utils.py` & `dpdispatcher-0.5.8/tests/old/test_dispatcher_utils.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/old/test_lazy_local_context.py` & `dpdispatcher-0.5.8/tests/old/test_lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/old/test_local_context.py` & `dpdispatcher-0.5.8/tests/old/test_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/old/test_ssh_context.py` & `dpdispatcher-0.5.8/tests/old/test_ssh_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/pbs/context.py` & `dpdispatcher-0.5.8/tests/pbs/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/pbs/test_dispatcher.py` & `dpdispatcher-0.5.8/tests/pbs/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/pbs/test_pbs_local.py` & `dpdispatcher-0.5.8/tests/pbs/test_pbs_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/sample_class.py` & `dpdispatcher-0.5.8/tests/sample_class.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/script_gen_json.py` & `dpdispatcher-0.5.8/tests/script_gen_json.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/shell/context.py` & `dpdispatcher-0.5.8/tests/shell/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/shell/test_dispatcher.py` & `dpdispatcher-0.5.8/tests/shell/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/shell/test_shell_local.py` & `dpdispatcher-0.5.8/tests/shell/test_shell_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/shell/test_shell_ssh.py` & `dpdispatcher-0.5.8/tests/shell/test_shell_ssh.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/slurm/context.py` & `dpdispatcher-0.5.8/tests/slurm/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/slurm/test_dispatcher.py` & `dpdispatcher-0.5.8/tests/slurm/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/slurm/test_dispatcher_lazy_local.py` & `dpdispatcher-0.5.8/tests/slurm/test_dispatcher_lazy_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/slurm/test_slurm_lazy_local.py` & `dpdispatcher-0.5.8/tests/slurm/test_slurm_lazy_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/slurm/test_slurm_local.py` & `dpdispatcher-0.5.8/tests/slurm/test_slurm_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/slurm/test_slurm_ssh.py` & `dpdispatcher-0.5.8/tests/slurm/test_slurm_ssh.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_argcheck.py` & `dpdispatcher-0.5.8/tests/test_argcheck.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_job.py` & `dpdispatcher-0.5.8/tests/test_class_job.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_machine.py` & `dpdispatcher-0.5.8/tests/test_class_machine.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_machine_dispatch.py` & `dpdispatcher-0.5.8/tests/test_class_machine_dispatch.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_resources.py` & `dpdispatcher-0.5.8/tests/test_class_resources.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_submission.py` & `dpdispatcher-0.5.8/tests/test_class_submission.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_submission_init.py` & `dpdispatcher-0.5.8/tests/test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_class_task.py` & `dpdispatcher-0.5.8/tests/test_class_task.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_context_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_group_size.py` & `dpdispatcher-0.5.8/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_hdfs_context.py` & `dpdispatcher-0.5.8/tests/test_hdfs_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_hdfs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_import_classes.py` & `dpdispatcher-0.5.8/tests/test_import_classes.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lazy_local_context.py` & `dpdispatcher-0.5.8/tests/test_lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_local_context.py` & `dpdispatcher-0.5.8/tests/test_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lsf_dir/0_md/submission.json` & `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_lsf_script_generation.py` & `dpdispatcher-0.5.8/tests/test_lsf_script_generation.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_pbs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_retry.py` & `dpdispatcher-0.5.8/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_run_submission.py` & `dpdispatcher-0.5.8/tests/test_run_submission_ratio_unfinished.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Set ratio_unfinished to 1.0 to test killing jobs."""
+
 import os
 import shutil
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 __package__ = "tests"
 import unittest
@@ -29,14 +31,15 @@
         }
         self.resources_dict = {
             "number_node": 1,
             "cpu_per_node": 1,
             "gpu_per_node": 0,
             "queue_name": "?",
             "group_size": 2,
+            "strategy": {"ratio_unfinished": 0.67},  # 2/3
         }
         os.makedirs(
             os.path.join(self.machine_dict["local_root"], "test_dir"), exist_ok=True
         )
         os.makedirs(
             os.path.join(self.machine_dict["local_root"], "test_dir", "test space"),
             exist_ok=True,
@@ -66,15 +69,15 @@
                 outlog=f"out{ii}.txt",
             )
             task_list.append(task)
 
         # test space in file name
         task_list.append(
             Task(
-                command="echo dpdispatcher_unittest_space",
+                command="sleep 1000 && echo dpdispatcher_unittest_space",
                 task_work_path="test space/",
                 forward_files=["inp space.txt"],
                 backward_files=["out space.txt"],
                 outlog="out space.txt",
             )
         )
         submission = Submission(
@@ -83,23 +86,14 @@
             resources=resources,
             forward_common_files=[],
             backward_common_files=[],
             task_list=task_list,
         )
         submission.run_submission()
 
-        for ii in range(4):
-            self.assertTrue(
-                os.path.isfile(
-                    os.path.join(
-                        self.machine_dict["local_root"], "test_dir/", f"out{ii}.txt"
-                    )
-                )
-            )
-
     def tearDown(self):
         shutil.rmtree(os.path.join(self.machine_dict["local_root"]))
 
 
 @unittest.skipIf(
     os.environ.get("DPDISPATCHER_TEST") != "slurm",
     "outside the slurm testing environment",
```

### Comparing `dpdispatcher-0.5.7/tests/test_shell_cuda_multi_devices.py` & `dpdispatcher-0.5.8/tests/test_shell_cuda_multi_devices.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_shell_trival.py` & `dpdispatcher-0.5.8/tests/test_shell_trival.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json` & `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_dir/0_md/submission.json` & `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_slurm_script_generation.py` & `dpdispatcher-0.5.8/tests/test_slurm_script_generation.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.7/tests/test_ssh_context.py` & `dpdispatcher-0.5.8/tests/test_ssh_context.py`

 * *Files identical despite different names*

