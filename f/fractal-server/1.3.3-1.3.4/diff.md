# Comparing `tmp/fractal_server-1.3.3.tar.gz` & `tmp/fractal_server-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.3.tar", max compression
+gzip compressed data, was "fractal_server-1.3.4.tar", max compression
```

## Comparing `fractal_server-1.3.3.tar` & `fractal_server-1.3.4.tar`

### file list

```diff
@@ -1,109 +1,84 @@
--rw-r--r--   0        0        0     1576 2023-06-23 06:18:06.498772 fractal_server-1.3.3/LICENSE
--rw-r--r--   0        0        0     2100 2023-06-23 06:18:06.498772 fractal_server-1.3.3/README.md
--rw-r--r--   0        0        0       69 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/.gitignore
--rw-r--r--   0        0        0       22 2023-07-06 08:58:33.028530 fractal_server-1.3.3/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     1242 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     7622 2023-06-29 10:43:50.361229 fractal_server-1.3.3/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4990 2023-06-29 10:43:50.361229 fractal_server-1.3.3/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-06-27 14:30:25.873556 fractal_server-1.3.3/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0     5516 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    10831 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/task_collection.py
--rw-r--r--   0        0        0     9246 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     5165 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/workflowtask.py
--rw-r--r--   0        0        0     3081 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     2535 2023-07-06 07:41:28.191331 fractal_server-1.3.3/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5207 2023-06-30 07:20:38.331243 fractal_server-1.3.3/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0    10102 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-07-06 08:55:51.562302 fractal_server-1.3.3/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3245 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19766 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42317 2023-06-29 10:43:50.365229 fractal_server-1.3.3/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-06-26 06:59:30.472776 fractal_server-1.3.3/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       57 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     4082 2023-06-26 06:59:32.132763 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3551 2023-06-26 06:59:32.132763 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     1179 2023-06-26 06:59:32.140764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-06-26 06:59:32.140764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     3306 2023-06-26 06:59:32.144764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-06-26 06:59:32.148764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     3896 2023-06-26 06:59:32.152763 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-06-28 13:38:09.728212 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      620 2023-06-28 13:38:09.776211 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-06-28 13:38:09.800210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1255 2023-06-28 13:38:09.800210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1178 2023-06-28 13:38:09.800210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-06-28 13:38:09.804210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2806 2023-06-28 13:38:09.804210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1349 2023-06-28 13:38:09.808210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2685 2023-06-28 13:38:09.808210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2925 2023-06-28 13:38:09.812209 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12432 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-06-27 14:30:25.873556 fractal_server-1.3.3/fractal_server/logger.py
--rw-r--r--   0        0        0     5935 2023-07-06 07:41:28.191331 fractal_server-1.3.3/fractal_server/main.py
--rw-r--r--   0        0        0       59 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/migrations/README
--rw-r--r--   0        0        0     2666 2023-06-29 12:21:21.012806 fractal_server-1.3.3/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-29 13:31:45.976002 fractal_server-1.3.3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-07-06 07:41:28.195330 fractal_server-1.3.3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-29 13:31:45.976002 fractal_server-1.3.3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    17583 2023-06-29 10:43:50.365229 fractal_server-1.3.3/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/utils.py
--rw-r--r--   0        0        0     2703 2023-07-06 08:58:33.028530 fractal_server-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 fractal_server-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-06-23 06:18:06.498772 fractal_server-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2100 2023-06-23 06:18:06.498772 fractal_server-1.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-07-17 12:16:57.082415 fractal_server-1.3.4/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     1242 2023-06-29 10:31:41.253702 fractal_server-1.3.4/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     7622 2023-06-29 10:43:50.361229 fractal_server-1.3.4/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4990 2023-06-29 10:43:50.361229 fractal_server-1.3.4/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     9839 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0     5516 2023-06-29 10:31:41.253702 fractal_server-1.3.4/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    10919 2023-07-17 09:49:51.774757 fractal_server-1.3.4/fractal_server/app/api/v1/task_collection.py
+-rw-r--r--   0        0        0     9246 2023-06-29 10:31:41.253702 fractal_server-1.3.4/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     5418 2023-07-10 10:46:15.443828 fractal_server-1.3.4/fractal_server/app/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     3081 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-07-06 14:29:22.370788 fractal_server-1.3.4/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3483 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     2535 2023-07-06 07:41:28.191331 fractal_server-1.3.4/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5207 2023-06-30 07:20:38.331243 fractal_server-1.3.4/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0    10988 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    17868 2023-07-10 10:46:15.443828 fractal_server-1.3.4/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     6279 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     4396 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19766 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2930 2023-07-10 10:46:15.443828 fractal_server-1.3.4/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42317 2023-06-29 10:43:50.365229 fractal_server-1.3.4/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9338 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-07-17 08:20:42.168640 fractal_server-1.3.4/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0     1964 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-26 06:59:32.128764 fractal_server-1.3.4/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       59 2023-07-17 09:36:04.703494 fractal_server-1.3.4/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-26 06:59:32.128764 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-06-26 06:59:32.128764 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2698 2023-07-17 09:39:08.405559 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4082 2023-06-26 06:59:32.132763 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3551 2023-06-26 06:59:32.132763 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     1179 2023-06-26 06:59:32.140764 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-06-26 06:59:32.140764 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     3306 2023-06-26 06:59:32.144764 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-06-26 06:59:32.148764 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     3896 2023-06-26 06:59:32.152763 fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     2392 2023-07-17 09:36:04.703494 fractal_server-1.3.4/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-06-26 06:59:30.480776 fractal_server-1.3.4/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0    12432 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-06-27 14:30:25.873556 fractal_server-1.3.4/fractal_server/logger.py
+-rw-r--r--   0        0        0     5935 2023-07-06 07:41:28.191331 fractal_server-1.3.4/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2666 2023-06-29 12:21:21.012806 fractal_server-1.3.4/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-29 13:31:45.976002 fractal_server-1.3.4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-07-06 07:41:28.195330 fractal_server-1.3.4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     1070 2023-07-17 10:32:22.244735 fractal_server-1.3.4/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0      746 2023-06-29 13:31:45.976002 fractal_server-1.3.4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17583 2023-06-29 10:43:50.365229 fractal_server-1.3.4/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-06-23 06:18:06.502771 fractal_server-1.3.4/fractal_server/utils.py
+-rw-r--r--   0        0        0     2818 2023-07-17 12:16:57.082415 fractal_server-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 fractal_server-1.3.4/PKG-INFO
```

### Comparing `fractal_server-1.3.3/LICENSE` & `fractal_server-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/README.md` & `fractal_server-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/__main__.py` & `fractal_server-1.3.4/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/alembic.ini` & `fractal_server-1.3.4/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/__init__.py` & `fractal_server-1.3.4/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ...models import LinkUserProject
 from ...models import Project
 from ...models import ProjectCreate
 from ...models import ProjectRead
 from ...models import ProjectUpdate
 from ...runner import submit_workflow
 from ...runner import validate_workflow_compatibility
+from ...runner.common import set_start_and_last_task_index
 from ...security import current_active_user
 from ...security import User
 from ._aux_functions import _get_dataset_check_owner
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_workflow_check_owner
 
 
@@ -219,14 +220,34 @@
 
     if not workflow.task_list:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=f"Workflow {workflow_id} has empty task list",
         )
 
+    # Set values of first_task_index and last_task_index
+    num_tasks = len(workflow.task_list)
+    try:
+        first_task_index, last_task_index = set_start_and_last_task_index(
+            num_tasks,
+            first_task_index=apply_workflow.first_task_index,
+            last_task_index=apply_workflow.last_task_index,
+        )
+        apply_workflow.first_task_index = first_task_index
+        apply_workflow.last_task_index = last_task_index
+    except ValueError as e:
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                "Invalid values for first_task_index or last_task_index "
+                f"(with {num_tasks=}).\n"
+                f"Original error: {str(e)}"
+            ),
+        )
+
     # If backend is SLURM, check that the user has required attributes
     settings = Inject(get_settings)
     backend = settings.FRACTAL_RUNNER_BACKEND
     if backend == "slurm":
         if not user.slurm_user:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
@@ -260,14 +281,16 @@
         )
 
     try:
         validate_workflow_compatibility(
             workflow=workflow,
             input_dataset=input_dataset,
             output_dataset=output_dataset,
+            first_task_index=apply_workflow.first_task_index,
+            last_task_index=apply_workflow.last_task_index,
         )
     except TypeError as e:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e)
         )
 
     job = ApplyWorkflow(
```

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/task_collection.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/task_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,25 @@
 
     Install a python package and collect the tasks it provides according to
     the manifest.
 
     In case of error, copy the log into the state and delete the package
     directory.
     """
+    logger_name = task_pkg.package.replace("/", "_")
+    logger = set_logger(
+        logger_name=logger_name,
+        log_file_path=get_log_path(venv_path),
+    )
+    logger.debug("Start background task collection")
+    for key, value in task_pkg.dict(exclude={"package_manifest"}).items():
+        logger.debug(f"{key}: {value}")
 
     with next(get_sync_db()) as db:
-
         state: State = db.get(State, state_id)
-
-        logger_name = task_pkg.package.replace("/", "_")
-        logger = set_logger(
-            logger_name=logger_name,
-            log_file_path=get_log_path(venv_path),
-        )
-
-        logger.debug("Start background task collection")
         data = TaskCollectStatus(**state.data)
         data.info = None
 
         try:
             # install
             logger.debug("Task-collection status: installing")
             data.status = "installing"
```

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/api/v1/workflowtask.py` & `fractal_server-1.3.4/fractal_server/app/api/v1/workflowtask.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 
 from ...db import AsyncSession
 from ...db import get_db
+from ...models import Task
 from ...models import WorkflowTaskCreate
 from ...models import WorkflowTaskRead
 from ...models import WorkflowTaskUpdate
 from ...security import current_active_user
 from ...security import User
 from ._aux_functions import _get_workflow_check_owner
 from ._aux_functions import _get_workflow_task_check_owner
@@ -49,14 +50,23 @@
     """
     Add a WorkflowTask to a Workflow
     """
 
     workflow = await _get_workflow_check_owner(
         project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
     )
+
+    # Check that task exists
+    task = await db.get(Task, task_id)
+    if not task:
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND,
+            detail=f"Task {task_id} not found.",
+        )
+
     async with db:
         workflow_task = await workflow.insert_task(
             **new_task.dict(),
             task_id=task_id,
             db=db,
         )
```

### Comparing `fractal_server-1.3.3/fractal_server/app/db/__init__.py` & `fractal_server-1.3.4/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/models/job.py` & `fractal_server-1.3.4/fractal_server/app/models/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     id: Optional[int] = Field(default=None, primary_key=True)
     project_id: int = Field(foreign_key="project.id")
     input_dataset_id: int = Field(foreign_key="dataset.id")
     output_dataset_id: int = Field(foreign_key="dataset.id")
     workflow_id: int = Field(foreign_key="workflow.id")
     working_dir: Optional[str]
     working_dir_user: Optional[str]
+    first_task_index: Optional[int]
+    last_task_index: Optional[int]
 
     input_dataset: Dataset = Relationship(
         sa_relationship_kwargs=dict(
             lazy="selectin",
             primaryjoin="ApplyWorkflow.input_dataset_id==Dataset.id",
         )
     )
```

### Comparing `fractal_server-1.3.3/fractal_server/app/models/project.py` & `fractal_server-1.3.4/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/models/security.py` & `fractal_server-1.3.4/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/models/state.py` & `fractal_server-1.3.4/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/models/task.py` & `fractal_server-1.3.4/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/models/workflow.py` & `fractal_server-1.3.4/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.4/fractal_server/app/runner/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,34 +102,54 @@
             The username to impersonate for the workflow execution, for the
             slurm backend.
     """
     with next(DB.get_sync_db()) as db_sync:
 
         job: ApplyWorkflow = db_sync.get(ApplyWorkflow, job_id)
         if not job:
-            raise ValueError("Cannot fetch job from database")
+            raise ValueError(f"Cannot fetch job {job_id} from database")
+
         input_dataset: Dataset = db_sync.get(Dataset, input_dataset_id)
-        if not input_dataset:
-            raise ValueError("Cannot fetch input_dataset from database")
         output_dataset: Dataset = db_sync.get(Dataset, output_dataset_id)
-        if not output_dataset:
-            raise ValueError("Cannot fetch output_dataset from database")
         workflow: Workflow = db_sync.get(Workflow, workflow_id)
-        if not workflow:
-            raise ValueError("Cannot fetch workflow from database")
+        if not (input_dataset and output_dataset and workflow):
+            log_msg = ""
+            if not input_dataset:
+                log_msg += (
+                    f"Cannot fetch input_dataset {input_dataset_id} "
+                    "from database\n"
+                )
+            if not output_dataset:
+                log_msg += (
+                    f"Cannot fetch output_dataset {output_dataset_id} "
+                    "from database\n"
+                )
+            if not workflow:
+                log_msg += (
+                    f"Cannot fetch workflow {workflow_id} from database\n"
+                )
+            job.status = JobStatusType.FAILED
+            job.end_timestamp = get_timestamp()
+            job.log = log_msg
+            db_sync.merge(job)
+            db_sync.commit()
+            db_sync.close()
+            return
 
         # Select backend
         settings = Inject(get_settings)
         FRACTAL_RUNNER_BACKEND = settings.FRACTAL_RUNNER_BACKEND
         process_workflow = get_process_workflow()
 
         # Prepare some of process_workflow arguments
         input_paths = input_dataset.paths
         output_path = output_dataset.paths[0]
         workflow_id = workflow.id
+        first_task_index = job.first_task_index
+        last_task_index = job.last_task_index
 
         # Define and create server-side working folder
         project_id = workflow.project_id
         timestamp_string = get_timestamp().strftime("%Y%m%d_%H%M%S")
         WORKFLOW_DIR = (
             settings.FRACTAL_RUNNER_WORKING_BASE_DIR  # type: ignore
             / (
@@ -183,14 +203,16 @@
         logger.debug(f"worker_init: {worker_init}")
         logger.debug(f"input metadata: {input_dataset.meta}")
         logger.debug(f"input_paths: {input_paths}")
         logger.debug(f"output_path: {output_path}")
         logger.debug(f"job.id: {job.id}")
         logger.debug(f"job.working_dir: {str(WORKFLOW_DIR)}")
         logger.debug(f"job.workflow_dir_user: {str(WORKFLOW_DIR_USER)}")
+        logger.debug(f"job.first_task_index: {job.first_task_index}")
+        logger.debug(f"job.last_task_index: {job.last_task_index}")
         logger.debug(f'START workflow "{workflow.name}"')
 
     try:
         # "The Session.close() method does not prevent the Session from being
         # used again. The Session itself does not actually have a distinct
         # “closed” state; it merely means the Session will release all database
         # connections and ORM objects."
@@ -210,14 +232,16 @@
             input_metadata=input_dataset.meta,
             slurm_user=slurm_user,
             user_cache_dir=user_cache_dir,
             workflow_dir=WORKFLOW_DIR,
             workflow_dir_user=WORKFLOW_DIR_USER,
             logger_name=logger_name,
             worker_init=worker_init,
+            first_task_index=first_task_index,
+            last_task_index=last_task_index,
         )
 
         logger.info(
             f'End execution of workflow "{workflow.name}"; '
             f"more logs at {str(log_file_path)}"
         )
         logger.debug(f'END workflow "{workflow.name}"')
```

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_common.py` & `fractal_server-1.3.4/fractal_server/app/runner/_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 This module includes utilities and routines that are of use to implement
 runner backends and that should not be exposed outside of the runner
 subsystem.
 """
 import json
 import subprocess  # nosec
 from concurrent.futures import Executor
-from concurrent.futures import Future
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
 from shlex import split as shlex_split
 from typing import Callable
 from typing import Optional
 
@@ -265,15 +264,15 @@
     # This assumes that the new metadata is printed to stdout
     # and nothing else outputs to stdout
     with task_files.metadiff.open("r") as f_metadiff:
         diff_metadata = json.load(f_metadiff)
     updated_metadata = task_pars.metadata.copy()
     updated_metadata.update(diff_metadata)
 
-    # Assemble a Future[TaskParameter]
+    # Assemble a TaskParameter object
     history = f"{wftask.task.name}"
     try:
         updated_metadata["history"].append(history)
     except KeyError:
         updated_metadata["history"] = [history]
 
     out_task_parameters = TaskParameters(
@@ -371,28 +370,22 @@
     *,
     executor: Executor,
     wftask: WorkflowTask,
     task_pars_depend: TaskParameters,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
     submit_setup_call: Callable = no_op_submit_setup_call,
-) -> Future:  # py3.9 Future[TaskParameters]:
+) -> TaskParameters:
     """
     Collect results from the parallel instances of a parallel task
 
     Prepare and submit for execution all the single calls of a parallel task,
-    and return a single future with the TaskParameters to be passed on to the
+    and return a single TaskParameters instance to be passed on to the
     next task.
 
-    **Note**: This function returns a future which already has
-    `out_future.done()=True` (that is, this function is blocking and it
-    returns only after the task is over). The reason for returning a future
-    instead of a `TaskParameter` object is for compatibility with the output of
-    `executor.submit(call_single_task, ...)`.
-
     Args:
         executor:
             The `concurrent.futures.Executor`-compatible executor that will
             run the task.
         wftask:
             The parallel task to run.
         task_pars_depend:
@@ -403,17 +396,17 @@
             The user-side working directory for workflow execution (only
             relevant for multi-user executors).
         submit_setup_call:
             An optional function that computes configuration parameters for
             the executor.
 
     Returns:
-        out_future:
-            A future that resolves in the output task parameters of the
-            parallel task execution, ready to be passed on to the next task.
+        out_task_parameters:
+            The output task parameters of the parallel task execution, ready to
+            be passed on to the next task.
     """
 
     if not workflow_dir_user:
         workflow_dir_user = workflow_dir
 
     component_list = task_pars_depend.metadata[wftask.parallelization_level]
 
@@ -434,73 +427,60 @@
         workflow_dir_user=workflow_dir_user,
     )
 
     # Submit tasks for execution. Note that `for _ in map_iter:
     # pass` explicitly calls the .result() method for each future, and
     # therefore is blocking until the task are complete.
     map_iter = executor.map(partial_call_task, component_list, **extra_setup)
+
     # Wait for execution of this chunk of tasks. Note: this is required *also*
     # because otherwise the shutdown of a FractalSlurmExecutor while running
     # map() may not work
     for _ in map_iter:
         pass  # noqa: 701
 
-    # Assemble a Future[TaskParameter]
+    # Assemble a TaskParameter object
     history = f"{wftask.task.name}: {component_list}"
     try:
         task_pars_depend.metadata["history"].append(history)
     except KeyError:
         task_pars_depend.metadata["history"] = [history]
 
     out_task_parameters = TaskParameters(
         input_paths=[task_pars_depend.output_path],
         output_path=task_pars_depend.output_path,
         metadata=task_pars_depend.metadata,
     )
 
-    out_future: Future = Future()
-    out_future.set_result(out_task_parameters)
-    return out_future
+    return out_task_parameters
 
 
-def recursive_task_submission(
+def execute_tasks(
     *,
     executor: Executor,
     task_list: list[WorkflowTask],
     task_pars: TaskParameters,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
     submit_setup_call: Callable = no_op_submit_setup_call,
     logger_name: str,
-) -> Future:
+) -> TaskParameters:
     """
-    Recursively submit a list of tasks
-
-    This recursive function schedules a workflow task list in the correct
-    order, making sure to resolve dependency before proceeding to the next
-    task: each following task depends on the future.result() of the previous
-    one, thus assuring the dependency chain.
-
-    Induction process:
-
-    * `0`: return a future which resolves in the task parameters necessary for
-      the first task of the list.
-    * `n => n+1`: use output resulting from step `n` as input for the first
-      task in the list, i.e., the `n+1`st task.
+    Submit a list of WorkflowTasks for execution
 
     **Note:** At the end of each task, write current metadata to `working_dir /
     METADATA_FILENAME`, so that they can be read as part of the [`get_job`
     endpoint](../../api/v1/job/#fractal_server.app.api.v1.job.get_job).
 
     Arguments:
         executor:
             The `concurrent.futures.Executor`-compatible executor that will
             run the task.
         task_list:
-            The list of tasks to be run
+            The list of wftasks to be run
         task_pars:
             The task parameters to be passed on to the first task of the list.
         workflow_dir:
             The server-side working directory for workflow execution.
         workflow_dir_user:
             The user-side working directory for workflow execution (only
             relevant for multi-user executors). If `None`, it is set to be
@@ -508,81 +488,62 @@
         submit_setup_call:
             An optional function that computes configuration parameters for
             the executor.
         logger_name:
             Name of the logger
 
     Returns:
-        this_wftask_future:
-            a future that results to the task parameters which constitute the
-            input of the following task in the list.
+        current_task_pars:
+            A TaskParameters object which constitutes the output of the last
+            task in the list.
     """
     if not workflow_dir_user:
         workflow_dir_user = workflow_dir
 
-    try:
-        *dependencies, this_wftask = task_list
-    except ValueError:
-        # step 0: return future containing original task_pars
-        pseudo_future: Future = Future()
-        pseudo_future.set_result(task_pars)
-        return pseudo_future
-
     logger = get_logger(logger_name)
 
-    # step n => step n+1
-    task_pars_depend_future = recursive_task_submission(
-        executor=executor,
-        task_list=dependencies,
-        task_pars=task_pars,
-        workflow_dir=workflow_dir,
-        workflow_dir_user=workflow_dir_user,
-        submit_setup_call=submit_setup_call,
-        logger_name=logger_name,
-    )
-    # Wait for dependencies to be complete (NOTE: this is not necessary if we
-    # explicitly wait for the result of executor.submit(call_single_task, ...),
-    # see below
-    task_pars_depend = task_pars_depend_future.result()
-
-    logger.debug(
-        f'SUBMIT {this_wftask.order}-th task (name="{this_wftask.task.name}")'
-    )
-    if this_wftask.is_parallel:
-        # NOTE: call_parallel_task is blocking, i.e. the returned future always
-        # has `this_wftask_future.done() = True`
-        this_wftask_future = call_parallel_task(
-            executor=executor,
-            wftask=this_wftask,
-            task_pars_depend=task_pars_depend,
-            workflow_dir=workflow_dir,
-            workflow_dir_user=workflow_dir_user,
-            submit_setup_call=submit_setup_call,
-        )
-    else:
-        # NOTE: executor.submit(call_single_task, ...) is non-blocking, i.e.
-        # the returned future may have `this_wftask_future.done() = False`
-        extra_setup = submit_setup_call(
-            wftask=this_wftask,
-            task_pars=task_pars,
-            workflow_dir=workflow_dir,
-            workflow_dir_user=workflow_dir_user,
+    current_task_pars = task_pars.copy()
+
+    for this_wftask in task_list:
+        logger.debug(
+            f"SUBMIT {this_wftask.order}-th task "
+            f'(name="{this_wftask.task.name}")'
         )
-        this_wftask_future = executor.submit(
-            call_single_task,
-            wftask=this_wftask,
-            task_pars=task_pars_depend,
-            workflow_dir=workflow_dir,
-            workflow_dir_user=workflow_dir_user,
-            **extra_setup,
+        if this_wftask.is_parallel:
+            current_task_pars = call_parallel_task(
+                executor=executor,
+                wftask=this_wftask,
+                task_pars_depend=current_task_pars,
+                workflow_dir=workflow_dir,
+                workflow_dir_user=workflow_dir_user,
+                submit_setup_call=submit_setup_call,
+            )
+        else:
+            # NOTE: executor.submit(call_single_task, ...) is non-blocking,
+            # i.e. the returned future may have `this_wftask_future.done() =
+            # False`. We make it blocking right away, by calling `.result()`
+            extra_setup = submit_setup_call(
+                wftask=this_wftask,
+                task_pars=current_task_pars,
+                workflow_dir=workflow_dir,
+                workflow_dir_user=workflow_dir_user,
+            )
+            this_wftask_future = executor.submit(
+                call_single_task,
+                wftask=this_wftask,
+                task_pars=current_task_pars,
+                workflow_dir=workflow_dir,
+                workflow_dir_user=workflow_dir_user,
+                **extra_setup,
+            )
+            # Wait for the future result (blocking)
+            current_task_pars = this_wftask_future.result()
+        logger.debug(
+            f"END    {this_wftask.order}-th task "
+            f'(name="{this_wftask.task.name}")'
         )
-        # Wait for the future result (blocking)
-        this_wftask_future.result()
-    logger.debug(
-        f'END    {this_wftask.order}-th task (name="{this_wftask.task.name}")'
-    )
 
-    # Write most recent metadata to METADATA_FILENAME
-    with open(workflow_dir / METADATA_FILENAME, "w") as f:
-        json.dump(this_wftask_future.result().metadata, f, indent=2)
+        # Write most recent metadata to METADATA_FILENAME
+        with open(workflow_dir / METADATA_FILENAME, "w") as f:
+            json.dump(current_task_pars.metadata, f, indent=2)
 
-    return this_wftask_future
+    return current_task_pars
```

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.4/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.4/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.4/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,30 +17,33 @@
 """
 from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import Union
 
 from ...models import Workflow
-from .._common import recursive_task_submission
+from .._common import execute_tasks
 from ..common import async_wrap
+from ..common import set_start_and_last_task_index
 from ..common import TaskParameters
 from ._submit_setup import _slurm_submit_setup
 from .executor import FractalSlurmExecutor
 
 
 def _process_workflow(
     *,
     workflow: Workflow,
     input_paths: list[Path],
     output_path: Path,
     input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Path,
+    first_task_index: int,
+    last_task_index: int,
     slurm_user: Optional[str] = None,
     user_cache_dir: str,
     worker_init: Optional[Union[str, list[str]]] = None,
 ) -> dict[str, Any]:
     """
     Internal processing routine for the SLURM backend
 
@@ -67,28 +70,29 @@
         keep_logs=True,
         slurm_user=slurm_user,
         user_cache_dir=user_cache_dir,
         working_dir=workflow_dir,
         working_dir_user=workflow_dir_user,
         common_script_lines=worker_init,
     ) as executor:
-        output_task_pars_fut = recursive_task_submission(
+        output_task_pars = execute_tasks(
             executor=executor,
-            task_list=workflow.task_list,
+            task_list=workflow.task_list[
+                first_task_index : (last_task_index + 1)  # noqa
+            ],  # noqa
             task_pars=TaskParameters(
                 input_paths=input_paths,
                 output_path=output_path,
                 metadata=input_metadata,
             ),
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir_user,
             submit_setup_call=_slurm_submit_setup,
             logger_name=logger_name,
         )
-        output_task_pars = output_task_pars_fut.result()
     output_dataset_metadata = output_task_pars.metadata
     return output_dataset_metadata
 
 
 async def process_workflow(
     *,
     workflow: Workflow,
@@ -97,26 +101,39 @@
     input_metadata: dict[str, Any],
     logger_name: str,
     workflow_dir: Path,
     workflow_dir_user: Optional[Path] = None,
     user_cache_dir: Optional[str] = None,
     slurm_user: Optional[str] = None,
     worker_init: Optional[str] = None,
+    first_task_index: Optional[int] = None,
+    last_task_index: Optional[int] = None,
 ) -> dict[str, Any]:
     """
     Process workflow (SLURM backend public interface)
 
     Cf. [process_workflow][fractal_server.app.runner._local.process_workflow]
     """
+
+    # Set values of first_task_index and last_task_index
+    num_tasks = len(workflow.task_list)
+    first_task_index, last_task_index = set_start_and_last_task_index(
+        num_tasks,
+        first_task_index=first_task_index,
+        last_task_index=last_task_index,
+    )
+
     output_dataset_metadata = await async_wrap(_process_workflow)(
         workflow=workflow,
         input_paths=input_paths,
         output_path=output_path,
         input_metadata=input_metadata,
         logger_name=logger_name,
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
         slurm_user=slurm_user,
         user_cache_dir=user_cache_dir,
         worker_init=worker_init,
+        first_task_index=first_task_index,
+        last_task_index=last_task_index,
     )
     return output_dataset_metadata
```

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     Here goes all the logic for reading attributes from the appropriate sources
     and transforming them into an appropriate `SlurmConfig` object (encoding
     SLURM configuration) and `TaskFiles` object (with details e.g. about file
     paths or filename prefixes).
 
     For now, this is the reference implementation for the argument
     `submit_setup_call` of
-    [fractal_server.app.runner._common.recursive_task_submission][].
+    [fractal_server.app.runner._common.execute_tasks][].
 
     Arguments:
         wftask:
             WorkflowTask for which the configuration is to be assembled
         task_pars:
             Task parameters to be passed to the task
             (not used in this function)
```

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.4/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/app/runner/common.py` & `fractal_server-1.3.4/fractal_server/app/runner/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -188,36 +188,40 @@
 
 
 def validate_workflow_compatibility(
     *,
     input_dataset: Dataset,
     workflow: Workflow,
     output_dataset: Dataset,
+    first_task_index: int,
+    last_task_index: int,
 ) -> None:
     """
     Check compatibility of workflow and input / ouptut dataset
     """
     # Check input_dataset type
+    workflow_input_type = workflow.task_list[first_task_index].task.input_type
     if (
-        workflow.input_type != "Any"
-        and workflow.input_type != input_dataset.type
+        workflow_input_type != "Any"
+        and workflow_input_type != input_dataset.type
     ):
         raise TypeError(
-            f"Incompatible types `{workflow.input_type}` of workflow "
+            f"Incompatible types `{workflow_input_type}` of workflow "
             f"`{workflow.name}` and `{input_dataset.type}` of dataset "
             f"`{input_dataset.name}`"
         )
 
     # Check output_dataset type
+    workflow_output_type = workflow.task_list[last_task_index].task.output_type
     if (
-        workflow.output_type != "Any"
-        and workflow.output_type != output_dataset.type
+        workflow_output_type != "Any"
+        and workflow_output_type != output_dataset.type
     ):
         raise TypeError(
-            f"Incompatible types `{workflow.output_type}` of workflow "
+            f"Incompatible types `{workflow_output_type}` of workflow "
             f"`{workflow.name}` and `{output_dataset.type}` of dataset "
             f"`{output_dataset.name}`"
         )
 
 
 def async_wrap(func: Callable) -> Callable:
     """
@@ -255,7 +259,45 @@
             Destination for serialised file.
     """
     out = {}
     for d in args:
         out.update(d)
     with open(path, "w") as f:
         json.dump(out, f, cls=TaskParameterEncoder, indent=4)
+
+
+def set_start_and_last_task_index(
+    num_tasks: int,
+    first_task_index: Optional[int] = None,
+    last_task_index: Optional[int] = None,
+) -> tuple[int, int]:
+    """
+    Handle `first_task_index` and `last_task_index`, by setting defaults and
+    validating values.
+
+    num_tasks:
+        Total number of tasks in a workflow task list
+    first_task_index:
+        Positional index of the first task to execute
+    last_task_index:
+        Positional index of the last task to execute
+    """
+    # Set default values
+    if first_task_index is None:
+        first_task_index = 0
+    if last_task_index is None:
+        last_task_index = num_tasks - 1
+
+    # Perform checks
+    if first_task_index < 0:
+        raise ValueError(f"{first_task_index=} cannot be negative")
+    if last_task_index < 0:
+        raise ValueError(f"{last_task_index=} cannot be negative")
+    if last_task_index > num_tasks - 1:
+        raise ValueError(
+            f"{last_task_index=} cannot be larger than {(num_tasks-1)=}"
+        )
+    if first_task_index > last_task_index:
+        raise ValueError(
+            f"{first_task_index=} cannot be larger than {last_task_index=}"
+        )
+    return (first_task_index, last_task_index)
```

### Comparing `fractal_server-1.3.3/fractal_server/app/security/__init__.py` & `fractal_server-1.3.4/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/README.md` & `fractal_server-1.3.4/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.4/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 26 06:59:30 2023 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5237 9964 5d04 0000  o.......R7.d]...
+00000000: 6f0d 0d0a 0000 0000 840b b564 5809 0000  o..........dX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d07 5a07 0100 6407 5a08 4700  d.l.m.Z...d.Z.G.
 00000070: 6408 6409 8400 6409 6504 8303 5a09 4700  d.d...d.e...Z.G.
@@ -36,67 +36,134 @@
 00000230: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
 00000240: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
 00000250: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7363  server/common/sc
 00000260: 6865 6d61 732f 6170 706c 7977 6f72 6b66  hemas/applyworkf
 00000270: 6c6f 772e 7079 7208 0000 0010 0000 0073  low.pyr........s
 00000280: 0600 0000 0a00 0401 1007 7208 0000 0063  ..........r....c
 00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
-000002b0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
-000002c0: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
-000002d0: 0900 0000 720b 0000 0054 2901 da0b 616c  ....r....T)...al
-000002e0: 6c6f 775f 7265 7573 654e 2906 720c 0000  low_reuseN).r...
-000002f0: 0072 0d00 0000 720e 0000 0072 0500 0000  .r....r....r....
-00000300: 7207 0000 00da 0c5f 776f 726b 6572 5f69  r......_worker_i
-00000310: 6e69 7472 1200 0000 7212 0000 0072 1200  nitr....r....r..
-00000320: 0000 7213 0000 0072 0900 0000 1b00 0000  ..r....r........
-00000330: 7308 0000 0008 000a 0306 0108 ff72 0900  s............r..
-00000340: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000350: 0000 0003 0000 0040 0000 0073 8e00 0000  .......@...s....
-00000360: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
-00000370: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
-00000380: 3c00 6503 6504 6404 3c00 6503 6504 6405  <.e.e.d.<.e.e.d.
-00000390: 3c00 6505 6504 6406 3c00 6506 6505 1900  <.e.e.d.<.e.e...
-000003a0: 6504 6407 3c00 6507 6504 6408 3c00 6506  e.d.<.e.e.d.<.e.
-000003b0: 6507 1900 6504 6409 3c00 6506 6508 6507  e...e.d.<.e.e.e.
-000003c0: 1900 1900 6504 640a 3c00 6506 6507 1900  ....e.d.<.e.e...
-000003d0: 6504 640b 3c00 6506 6507 1900 6504 640c  e.d.<.e.e...e.d.
-000003e0: 3c00 640d 640e 8400 5a09 640f 5300 2910  <.d.d...Z.d.S.).
-000003f0: 720a 0000 00da 0269 64da 0a70 726f 6a65  r......id..proje
-00000400: 6374 5f69 64da 0b77 6f72 6b66 6c6f 775f  ct_id..workflow_
-00000410: 6964 da10 696e 7075 745f 6461 7461 7365  id..input_datase
-00000420: 745f 6964 da11 6f75 7470 7574 5f64 6174  t_id..output_dat
-00000430: 6173 6574 5f69 64da 0f73 7461 7274 5f74  aset_id..start_t
-00000440: 696d 6573 7461 6d70 da0d 656e 645f 7469  imestamp..end_ti
-00000450: 6d65 7374 616d 70da 0673 7461 7475 73da  mestamp..status.
-00000460: 036c 6f67 da07 6869 7374 6f72 79da 0b77  .log..history..w
-00000470: 6f72 6b69 6e67 5f64 6972 da10 776f 726b  orking_dir..work
-00000480: 696e 675f 6469 725f 7573 6572 6301 0000  ing_dir_userc...
-00000490: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-000004a0: 0043 0000 0073 2800 0000 7c00 a000 a100  .C...s(...|.....
-000004b0: 7d01 7401 7c00 6a02 8301 7c01 6401 3c00  }.t.|.j...|.d.<.
-000004c0: 7401 7c00 6a03 8301 7c01 6402 3c00 7c01  t.|.j...|.d.<.|.
-000004d0: 5300 2903 4e72 1b00 0000 721c 0000 0029  S.).Nr....r....)
-000004e0: 04da 0464 6963 7472 1000 0000 721b 0000  ...dictr....r...
-000004f0: 0072 1c00 0000 2902 da04 7365 6c66 da01  .r....)...self..
-00000500: 6472 1200 0000 7212 0000 0072 1300 0000  dr....r....r....
-00000510: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
-00000520: 3100 0000 7308 0000 0008 010e 010e 0104  1...s...........
-00000530: 017a 2041 7070 6c79 576f 726b 666c 6f77  .z ApplyWorkflow
-00000540: 5265 6164 2e73 616e 6974 6973 6564 5f64  Read.sanitised_d
-00000550: 6963 744e 290a 720c 0000 0072 0d00 0000  ictN).r....r....
-00000560: 720e 0000 00da 0369 6e74 7211 0000 0072  r......intr....r
-00000570: 0200 0000 7203 0000 0072 1000 0000 da04  ....r....r......
-00000580: 6c69 7374 7225 0000 0072 1200 0000 7212  listr%...r....r.
-00000590: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
-000005a0: 0000 2300 0000 731c 0000 000a 0008 0108  ..#...s.........
-000005b0: 0108 0108 0108 0108 010c 0108 010c 0110  ................
-000005c0: 010c 010c 010c 0272 0a00 0000 4e29 0c72  .......r....N).r
-000005d0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-000005e0: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
-000005f0: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
-00000600: 7273 7207 0000 00da 075f 5f61 6c6c 5f5f  rsr......__all__
-00000610: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000620: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000630: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000640: 0073 1200 0000 0c00 0c01 0c02 0c01 0c02  .s..............
-00000650: 0402 1007 100b 1408                      ........
+000002a0: 0400 0000 4000 0000 736a 0000 0065 005a  ....@...sj...e.Z
+000002b0: 0164 005a 0255 0064 015a 0365 0465 0519  .d.Z.U.d.Z.e.e..
+000002c0: 0065 0664 023c 0064 015a 0765 0465 0519  .e.d.<.d.Z.e.e..
+000002d0: 0065 0664 033c 0065 0864 0464 0564 068d  .e.d.<.e.d.d.d..
+000002e0: 0265 0964 0483 0183 015a 0a65 0864 0264  .e.d.....Z.e.d.d
+000002f0: 0564 078d 0264 0864 0984 0083 015a 0b65  .d...d.d.....Z.e
+00000300: 0864 0364 0564 078d 0264 0a64 0b84 0083  .d.d.d...d.d....
+00000310: 015a 0c64 0153 0029 0c72 0900 0000 4eda  .Z.d.S.).r....N.
+00000320: 1066 6972 7374 5f74 6173 6b5f 696e 6465  .first_task_inde
+00000330: 78da 0f6c 6173 745f 7461 736b 5f69 6e64  x..last_task_ind
+00000340: 6578 720b 0000 0054 2901 da0b 616c 6c6f  exr....T)...allo
+00000350: 775f 7265 7573 6529 01da 0661 6c77 6179  w_reuse)...alway
+00000360: 7363 0300 0000 0000 0000 0000 0000 0300  sc..............
+00000370: 0000 0400 0000 4300 0000 7324 0000 007c  ......C...s$...|
+00000380: 0164 0175 0172 107c 0164 026b 0072 1074  .d.u.r.|.d.k.r.t
+00000390: 0064 037c 019b 0064 049d 0383 0182 017c  .d.|...d.......|
+000003a0: 0153 0029 057a 400a 2020 2020 2020 2020  .S.).z@.        
+000003b0: 4368 6563 6b20 7468 6174 2060 6669 7273  Check that `firs
+000003c0: 745f 7461 736b 5f69 6e64 6578 6020 6973  t_task_index` is
+000003d0: 206e 6f6e 2d6e 6567 6174 6976 652e 0a20   non-negative.. 
+000003e0: 2020 2020 2020 204e 7201 0000 007a 2c66         Nr....z,f
+000003f0: 6972 7374 5f74 6173 6b5f 696e 6465 7820  irst_task_index 
+00000400: 6361 6e6e 6f74 2062 6520 6e65 6761 7469  cannot be negati
+00000410: 7665 2028 6769 7665 6e3a 20fa 0129 2901  ve (given: ..)).
+00000420: da0a 5661 6c75 6545 7272 6f72 2903 da03  ..ValueError)...
+00000430: 636c 73da 0176 da06 7661 6c75 6573 7212  cls..v..valuesr.
+00000440: 0000 0072 1200 0000 7213 0000 00da 1d66  ...r....r......f
+00000450: 6972 7374 5f74 6173 6b5f 696e 6465 785f  irst_task_index_
+00000460: 6e6f 6e5f 6e65 6761 7469 7665 2500 0000  non_negative%...
+00000470: 730a 0000 0010 0502 010a 0104 ff04 037a  s..............z
+00000480: 3141 7070 6c79 576f 726b 666c 6f77 4372  1ApplyWorkflowCr
+00000490: 6561 7465 2e66 6972 7374 5f74 6173 6b5f  eate.first_task_
+000004a0: 696e 6465 785f 6e6f 6e5f 6e65 6761 7469  index_non_negati
+000004b0: 7665 6303 0000 0000 0000 0000 0000 0005  vec.............
+000004c0: 0000 0005 0000 0043 0000 0073 5e00 0000  .......C...s^...
+000004d0: 7c01 6401 7501 7210 7c01 6402 6b00 7210  |.d.u.r.|.d.k.r.
+000004e0: 7400 6403 7c01 9b00 6404 9d03 8301 8201  t.d.|...d.......
+000004f0: 7c02 a001 6405 a101 7d03 7c01 7d04 7c03  |...d...}.|.}.|.
+00000500: 6401 7501 722d 7c04 6401 7501 722d 7c03  d.u.r-|.d.u.r-|.
+00000510: 7c04 6b04 722d 7400 6406 7c03 9b02 6407  |.k.r-t.d.|...d.
+00000520: 7c04 9b02 9d04 8301 8201 7c01 5300 2908  |.........|.S.).
+00000530: 7a7b 0a20 2020 2020 2020 2043 6865 636b  z{.        Check
+00000540: 2074 6861 7420 606c 6173 745f 7461 736b   that `last_task
+00000550: 5f69 6e64 6578 6020 6973 206e 6f6e 2d6e  _index` is non-n
+00000560: 6567 6174 6976 652c 2061 6e64 2074 6861  egative, and tha
+00000570: 7420 6974 2069 7320 6e6f 740a 2020 2020  t it is not.    
+00000580: 2020 2020 736d 616c 6c65 7220 7468 616e      smaller than
+00000590: 2060 6669 7273 745f 7461 736b 5f69 6e64   `first_task_ind
+000005a0: 6578 602e 0a20 2020 2020 2020 204e 7201  ex`..        Nr.
+000005b0: 0000 007a 2b6c 6173 745f 7461 736b 5f69  ...z+last_task_i
+000005c0: 6e64 6578 2063 616e 6e6f 7420 6265 206e  ndex cannot be n
+000005d0: 6567 6174 6976 6520 2867 6976 656e 3a20  egative (given: 
+000005e0: 7218 0000 0072 1400 0000 7a11 6669 7273  r....r....z.firs
+000005f0: 745f 7461 736b 5f69 6e64 6578 3d7a 2720  t_task_index=z' 
+00000600: 6361 6e6e 6f74 2062 6520 6c61 7267 6572  cannot be larger
+00000610: 2074 6861 6e20 6c61 7374 5f74 6173 6b5f   than last_task_
+00000620: 696e 6465 783d 2902 7219 0000 00da 0367  index=).r......g
+00000630: 6574 2905 721a 0000 0072 1b00 0000 721c  et).r....r....r.
+00000640: 0000 0072 1400 0000 7215 0000 0072 1200  ...r....r....r..
+00000650: 0000 7212 0000 0072 1300 0000 da17 6669  ..r....r......fi
+00000660: 7273 745f 6c61 7374 5f74 6173 6b5f 696e  rst_last_task_in
+00000670: 6469 6365 7330 0000 0073 1c00 0000 1006  dices0...s......
+00000680: 0201 0a01 04ff 0a04 0401 1001 0801 0201  ................
+00000690: 0801 0201 04ff 04ff 0404 7a2b 4170 706c  ..........z+Appl
+000006a0: 7957 6f72 6b66 6c6f 7743 7265 6174 652e  yWorkflowCreate.
+000006b0: 6669 7273 745f 6c61 7374 5f74 6173 6b5f  first_last_task_
+000006c0: 696e 6469 6365 7329 0d72 0c00 0000 720d  indices).r....r.
+000006d0: 0000 0072 0e00 0000 7214 0000 0072 0300  ...r....r....r..
+000006e0: 0000 da03 696e 7472 1100 0000 7215 0000  ....intr....r...
+000006f0: 0072 0500 0000 7207 0000 00da 0c5f 776f  .r....r......_wo
+00000700: 726b 6572 5f69 6e69 7472 1d00 0000 721f  rker_initr....r.
+00000710: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+00000720: 0000 7213 0000 0072 0900 0000 1b00 0000  ..r....r........
+00000730: 7314 0000 000a 0010 0210 010a 0306 0104  s...............
+00000740: ff0a 040a 010a 0a0e 0172 0900 0000 6300  .........r....c.
+00000750: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000760: 0000 0040 0000 0073 a600 0000 6500 5a01  ...@...s....e.Z.
+00000770: 6400 5a02 5500 6503 6504 6401 3c00 6503  d.Z.U.e.e.d.<.e.
+00000780: 6504 6402 3c00 6503 6504 6403 3c00 6503  e.d.<.e.e.d.<.e.
+00000790: 6504 6404 3c00 6503 6504 6405 3c00 6505  e.d.<.e.e.d.<.e.
+000007a0: 6504 6406 3c00 6506 6505 1900 6504 6407  e.d.<.e.e...e.d.
+000007b0: 3c00 6507 6504 6408 3c00 6506 6507 1900  <.e.e.d.<.e.e...
+000007c0: 6504 6409 3c00 6506 6508 6507 1900 1900  e.d.<.e.e.e.....
+000007d0: 6504 640a 3c00 6506 6507 1900 6504 640b  e.d.<.e.e...e.d.
+000007e0: 3c00 6506 6507 1900 6504 640c 3c00 6506  <.e.e...e.d.<.e.
+000007f0: 6503 1900 6504 640d 3c00 6506 6503 1900  e...e.d.<.e.e...
+00000800: 6504 640e 3c00 640f 6410 8400 5a09 6411  e.d.<.d.d...Z.d.
+00000810: 5300 2912 720a 0000 00da 0269 64da 0a70  S.).r......id..p
+00000820: 726f 6a65 6374 5f69 64da 0b77 6f72 6b66  roject_id..workf
+00000830: 6c6f 775f 6964 da10 696e 7075 745f 6461  low_id..input_da
+00000840: 7461 7365 745f 6964 da11 6f75 7470 7574  taset_id..output
+00000850: 5f64 6174 6173 6574 5f69 64da 0f73 7461  _dataset_id..sta
+00000860: 7274 5f74 696d 6573 7461 6d70 da0d 656e  rt_timestamp..en
+00000870: 645f 7469 6d65 7374 616d 70da 0673 7461  d_timestamp..sta
+00000880: 7475 73da 036c 6f67 da07 6869 7374 6f72  tus..log..histor
+00000890: 79da 0b77 6f72 6b69 6e67 5f64 6972 da10  y..working_dir..
+000008a0: 776f 726b 696e 675f 6469 725f 7573 6572  working_dir_user
+000008b0: 7214 0000 0072 1500 0000 6301 0000 0000  r....r....c.....
+000008c0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+000008d0: 0000 0073 2800 0000 7c00 a000 a100 7d01  ...s(...|.....}.
+000008e0: 7401 7c00 6a02 8301 7c01 6401 3c00 7401  t.|.j...|.d.<.t.
+000008f0: 7c00 6a03 8301 7c01 6402 3c00 7c01 5300  |.j...|.d.<.|.S.
+00000900: 2903 4e72 2700 0000 7228 0000 0029 04da  ).Nr'...r(...)..
+00000910: 0464 6963 7472 1000 0000 7227 0000 0072  .dictr....r'...r
+00000920: 2800 0000 2902 da04 7365 6c66 da01 6472  (...)...self..dr
+00000930: 1200 0000 7212 0000 0072 1300 0000 da0e  ....r....r......
+00000940: 7361 6e69 7469 7365 645f 6469 6374 5600  sanitised_dictV.
+00000950: 0000 7308 0000 0008 010e 010e 0104 017a  ..s............z
+00000960: 2041 7070 6c79 576f 726b 666c 6f77 5265   ApplyWorkflowRe
+00000970: 6164 2e73 616e 6974 6973 6564 5f64 6963  ad.sanitised_dic
+00000980: 744e 290a 720c 0000 0072 0d00 0000 720e  tN).r....r....r.
+00000990: 0000 0072 2000 0000 7211 0000 0072 0200  ...r ...r....r..
+000009a0: 0000 7203 0000 0072 1000 0000 da04 6c69  ..r....r......li
+000009b0: 7374 7231 0000 0072 1200 0000 7212 0000  str1...r....r...
+000009c0: 0072 1200 0000 7213 0000 0072 0a00 0000  .r....r....r....
+000009d0: 4600 0000 7320 0000 000a 0008 0108 0108  F...s ..........
+000009e0: 0108 0108 0108 010c 0108 010c 0110 010c  ................
+000009f0: 010c 010c 010c 010c 0272 0a00 0000 4e29  .........r....N)
+00000a00: 0c72 0200 0000 da06 7479 7069 6e67 7203  .r......typingr.
+00000a10: 0000 00da 0870 7964 616e 7469 6372 0400  .....pydanticr..
+00000a20: 0000 7205 0000 00da 0b5f 7661 6c69 6461  ..r......_valida
+00000a30: 746f 7273 7207 0000 00da 075f 5f61 6c6c  torsr......__all
+00000a40: 5f5f 7208 0000 0072 0900 0000 720a 0000  __r....r....r...
+00000a50: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000a60: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000a70: 0000 0073 1200 0000 0c00 0c01 0c02 0c01  ...s............
+00000a80: 0c02 0402 1007 100b 142b                 .........+
```

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.4/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.4/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/project.py` & `fractal_server-1.3.4/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/state.py` & `fractal_server-1.3.4/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/task.py` & `fractal_server-1.3.4/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.4/fractal_server/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/user.py` & `fractal_server-1.3.4/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.4/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/config.py` & `fractal_server-1.3.4/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/logger.py` & `fractal_server-1.3.4/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/main.py` & `fractal_server-1.3.4/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/migrations/env.py` & `fractal_server-1.3.4/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.4/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/syringe.py` & `fractal_server-1.3.4/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/tasks/collection.py` & `fractal_server-1.3.4/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/fractal_server/utils.py` & `fractal_server-1.3.4/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.3/pyproject.toml` & `fractal_server-1.3.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.3"
+version = "1.3.4"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
 homepage = "https://github.com/fractal-analytics-platform/fractal-server"
 license = "BSD-3-Clause"
+exclude = [
+"fractal_server/.gitignore",
+"fractal_server/common/tests",
+"fractal_server/common/.git*",
+"fractal_server/common/.pre-commit-config.yaml",
+]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.20.0"
 fastapi = "^0.95.0"
 sqlmodel = "^0.0.8"
@@ -41,16 +47,14 @@
 [tool.poetry.group.dev.dependencies]
 asgi-lifespan = "^2"
 pytest = "^7.2"
 httpx = "^0.23"
 devtools = "^0.10"
 pytest-asyncio = "^0.20"
 bumpver = "^2022.1120"
-Pillow = "^9.1.1"
-pytest-mock = "^3.8"
 pre-commit = "^2.19"
 coverage = {extras = ["toml"], version = "^6.4.4"}
 mypy = "^0.982"
 pytest-subprocess = "^1.4"
 pytest-docker = {extras = ["docker-compose-v1"], version = "^1.0"}
 pytest-pretty = "^1.0.1"
 
@@ -73,15 +77,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.3"
+current_version = "1.3.4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.3/PKG-INFO` & `fractal_server-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.3
+Version: 1.3.4
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

