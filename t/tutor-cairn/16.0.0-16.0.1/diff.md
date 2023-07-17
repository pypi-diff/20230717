# Comparing `tmp/tutor-cairn-16.0.0.tar.gz` & `tmp/tutor-cairn-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-cairn-16.0.0.tar", last modified: Wed Jun 14 22:26:22 2023, max compression
+gzip compressed data, was "tutor-cairn-16.0.1.tar", last modified: Mon Jul 17 08:22:59 2023, max compression
```

## Comparing `tutor-cairn-16.0.0.tar` & `tutor-cairn-16.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)       80 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)    17285 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)    16470 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 22:26:22.642980 tutor-cairn-16.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1631 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.626314 tutor-cairn-16.0.0/tutor_cairn.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)    17285 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     2802 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-14 22:26:22.000000 tutor-cairn-16.0.0/tutor_cairn.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.629647 tutor-cairn-16.0.0/tutorcairn/
--rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       87 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     9135 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)     3014 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      759 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      868 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/k8s-volumes
--rw-r--r--   0 ci        (1000) ci        (1000)      981 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)     1869 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      112 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-permissions-command
--rw-r--r--   0 ci        (1000) ci        (1000)      146 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-permissions-volumes
--rw-r--r--   0 ci        (1000) ci        (1000)     3157 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)     5783 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.619647 tutor-cairn-16.0.0/tutorcairn/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.622980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/
--rw-r--r--   0 ci        (1000) ci        (1000)      350 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/auth.json
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/
--rw-r--r--   0 ci        (1000) ci        (1000)      734 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
--rw-r--r--   0 ci        (1000) ci        (1000)      430 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
--rw-r--r--   0 ci        (1000) ci        (1000)     2121 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
--rw-r--r--   0 ci        (1000) ci        (1000)     2250 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
--rw-r--r--   0 ci        (1000) ci        (1000)      343 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0005_course_blocks.sql
--rw-r--r--   0 ci        (1000) ci        (1000)     1093 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql
--rw-r--r--   0 ci        (1000) ci        (1000)      985 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql
--rw-r--r--   0 ci        (1000) ci        (1000)     1277 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.632980 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/users.d/
--rw-r--r--   0 ci        (1000) ci        (1000)      269 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/users.d/cairn.xml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.619647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/scripts/
--rw-r--r--   0 ci        (1000) ci        (1000)     3245 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/bootstrap/
--rw-r--r--   0 ci        (1000) ci        (1000)   115036 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json
--rw-r--r--   0 ci        (1000) ci        (1000)     5936 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/superset_config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/
--rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/file.toml
--rw-r--r--   0 ci        (1000) ci        (1000)      413 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/k8s.toml
--rw-r--r--   0 ci        (1000) ci        (1000)      367 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/local.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)     1929 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
--rw-r--r--   0 ci        (1000) ci        (1000)      112 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.636314 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/
--rw-r--r--   0 ci        (1000) ci        (1000)      554 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     3422 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/
--rw-r--r--   0 ci        (1000) ci        (1000)     1342 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5499 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/bootstrap.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8407 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3299 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/sso.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-clickhouse/
--rw-r--r--   0 ci        (1000) ci        (1000)       57 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)      938 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-openedx/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 22:26:22.639647 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-superset/
--rw-r--r--   0 ci        (1000) ci        (1000)      390 2023-06-14 22:26:13.000000 tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-superset/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.104388 tutor-cairn-16.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)       80 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)    17297 2023-07-17 08:22:59.104388 tutor-cairn-16.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)    16470 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-07-17 08:22:59.104388 tutor-cairn-16.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1643 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.074388 tutor-cairn-16.0.1/tutor_cairn.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)    17297 2023-07-17 08:22:58.000000 tutor-cairn-16.0.1/tutor_cairn.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     2802 2023-07-17 08:22:58.000000 tutor-cairn-16.0.1/tutor_cairn.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-07-17 08:22:58.000000 tutor-cairn-16.0.1/tutor_cairn.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-07-17 08:22:58.000000 tutor-cairn-16.0.1/tutor_cairn.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-07-17 08:22:58.000000 tutor-cairn-16.0.1/tutor_cairn.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-07-17 08:22:58.000000 tutor-cairn-16.0.1/tutor_cairn.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.074388 tutor-cairn-16.0.1/tutorcairn/
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.087721 tutor-cairn-16.0.1/tutorcairn/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       87 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     9135 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)     3014 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      759 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      868 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/k8s-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)      981 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      313 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)     1869 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      112 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-permissions-command
+-rw-r--r--   0 ci        (1000) ci        (1000)      146 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-permissions-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)     3157 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)     5783 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.064388 tutor-cairn-16.0.1/tutorcairn/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.071054 tutor-cairn-16.0.1/tutorcairn/templates/cairn/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.087721 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.087721 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/
+-rw-r--r--   0 ci        (1000) ci        (1000)      350 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/auth.json
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.094388 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/
+-rw-r--r--   0 ci        (1000) ci        (1000)      734 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)      430 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0002_grades.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     2121 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     2250 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)      343 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0005_course_blocks.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     1093 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)      985 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql
+-rw-r--r--   0 ci        (1000) ci        (1000)     1277 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.094388 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/users.d/
+-rw-r--r--   0 ci        (1000) ci        (1000)      269 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/users.d/cairn.xml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.067721 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.094388 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/openedx/scripts/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3245 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.094388 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/superset/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.097721 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/superset/bootstrap/
+-rw-r--r--   0 ci        (1000) ci        (1000)   115036 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json
+-rw-r--r--   0 ci        (1000) ci        (1000)     5936 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/superset/superset_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.097721 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/
+-rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/file.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)      413 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/k8s.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)      367 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/local.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.097721 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1929 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)      112 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-clickhouse/
+-rw-r--r--   0 ci        (1000) ci        (1000)      554 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     3422 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1342 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5499 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/bootstrap.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8435 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3299 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/sso.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.101055 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-clickhouse/
+-rw-r--r--   0 ci        (1000) ci        (1000)       57 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-clickhouse/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.104388 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)      938 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-openedx/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-07-17 08:22:59.104388 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-superset/
+-rw-r--r--   0 ci        (1000) ci        (1000)      390 2023-07-17 08:22:49.000000 tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-superset/init
```

### Comparing `tutor-cairn-16.0.0/PKG-INFO` & `tutor-cairn-16.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tutor-cairn
-Version: 16.0.0
+Version: 16.0.1
 Summary: Scalable, real-time analytics for Open edX
 Home-page: https://github.com/overhangio/tutor-cairn
 Author: Overhang.IO
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-cairn
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-cairn/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tutor-cairn-16.0.0/README.rst` & `tutor-cairn-16.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/setup.py` & `tutor-cairn-16.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.7",
     install_requires=["tutor>=16.0.0,<17.0.0"],
     entry_points={"tutor.plugin.v1": ["cairn = tutorcairn.plugin"]},
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `tutor-cairn-16.0.0/tutor_cairn.egg-info/PKG-INFO` & `tutor-cairn-16.0.1/tutor_cairn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tutor-cairn
-Version: 16.0.0
+Version: 16.0.1
 Summary: Scalable, real-time analytics for Open edX
 Home-page: https://github.com/overhangio/tutor-cairn
 Author: Overhang.IO
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-cairn
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-cairn/issues
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tutor-cairn-16.0.0/tutor_cairn.egg-info/SOURCES.txt` & `tutor-cairn-16.0.1/tutor_cairn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/k8s-deployments` & `tutor-cairn-16.0.1/tutorcairn/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/k8s-jobs` & `tutor-cairn-16.0.1/tutorcairn/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/k8s-services` & `tutor-cairn-16.0.1/tutorcairn/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/k8s-volumes` & `tutor-cairn-16.0.1/tutorcairn/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/kustomization-configmapgenerator` & `tutor-cairn-16.0.1/tutorcairn/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-jobs-services` & `tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/patches/local-docker-compose-services` & `tutor-cairn-16.0.1/tutorcairn/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/plugin.py` & `tutor-cairn-16.0.1/tutorcairn/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0001_create.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0003_course_enrollments.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0004_video_views.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0006_course_block_completion.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0007_fix_video_segments.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/clickhouse/migrations.d/0008_rename_openedx_tables.sql`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/openedx/scripts/importcoursedata.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/superset/bootstrap/courseoverview.json`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/superset/superset_config.py` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/superset/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-clickhouse/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-clickhouse/scripts/cairn`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/bootstrap.py` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/bootstrap.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     else:
         print(f"Creating user '{args.username}'...")
         user = security_manager.add_user(
             args.username,
             args.firstname,
             args.lastname,
             args.email,
-            "Gamma",
+            security_manager.find_role("Gamma"),
         )
         if user is None or user is False:
             # This may happen for instance when the email address is already associated
             # to a different username
             raise RuntimeError(
                 f"Failed to create user '{args.username}' email='{args.email}'"
             )
```

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/build/cairn-superset/cairn/sso.py` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/build/cairn-superset/cairn/sso.py`

 * *Files identical despite different names*

### Comparing `tutor-cairn-16.0.0/tutorcairn/templates/cairn/tasks/cairn-openedx/init` & `tutor-cairn-16.0.1/tutorcairn/templates/cairn/tasks/cairn-openedx/init`

 * *Files identical despite different names*

