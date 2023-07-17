# Comparing `tmp/pop_create-7.3.1.tar.gz` & `tmp/pop_create-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_create-7.3.1.tar", last modified: Wed Oct 26 23:59:47 2022, max compression
+gzip compressed data, was "pop_create-8.0.0.tar", last modified: Mon Jul 17 13:35:07 2023, max compression
```

## Comparing `pop_create-7.3.1.tar` & `pop_create-8.0.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/
--rw-r--r--   0 root         (0) root         (0)    11344 2022-10-26 23:59:28.000000 pop_create-7.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2022-10-26 23:59:28.000000 pop_create-7.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4371 2022-10-26 23:59:47.348902 pop_create-7.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3278 2022-10-26 23:59:28.000000 pop_create-7.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.344902 pop_create-7.3.1/pop_create/
--rw-r--r--   0 root         (0) root         (0)     2280 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.344902 pop_create-7.3.1/pop_create/pop_create/cicd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)      653 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     1064 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     5136 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)       69 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
--rw-r--r--   0 root         (0) root         (0)     7977 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/
--rw-r--r--   0 root         (0) root         (0)      220 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)       37 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/
--rw-r--r--   0 root         (0) root         (0)     9591 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      781 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/index.rst
--rw-r--r--   0 root         (0) root         (0)      175 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/{{cookiecutter.version_number}}.rst
--rw-r--r--   0 root         (0) root         (0)       64 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/
--rw-r--r--   0 root         (0) root         (0)       55 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      227 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/
--rw-r--r--   0 root         (0) root         (0)      143 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
--rw-r--r--   0 root         (0) root         (0)       76 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)      125 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)     4737 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/seed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/seed/hooks/
--rw-r--r--   0 root         (0) root         (0)      473 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)      374 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)      301 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2390 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore
--rw-r--r--   0 root         (0) root         (0)      356 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     8748 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    11375 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3425 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       10 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)      118 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/run.py
--rw-r--r--   0 root         (0) root         (0)       34 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2927 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)     1243 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py
--rw-r--r--   0 root         (0) root         (0)      188 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/scripts.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      908 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.344902 pop_create-7.3.1/pop_create/pop_create/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/hooks/
--rw-r--r--   0 root         (0) root         (0)      899 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/hooks/post_gen_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)       49 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       67 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/tests.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.344902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)      881 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      166 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/test_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      766 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)      305 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/test_init.py
--rw-r--r--   0 root         (0) root         (0)      151 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create/tool/
--rw-r--r--   0 root         (0) root         (0)     2119 2022-10-26 23:59:28.000000 pop_create-7.3.1/pop_create/tool/path.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-10-26 23:59:46.000000 pop_create-7.3.1/pop_create/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 23:59:47.348902 pop_create-7.3.1/pop_create.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4371 2022-10-26 23:59:47.000000 pop_create-7.3.1/pop_create.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3280 2022-10-26 23:59:47.000000 pop_create-7.3.1/pop_create.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-26 23:59:47.000000 pop_create-7.3.1/pop_create.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2022-10-26 23:59:47.000000 pop_create-7.3.1/pop_create.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-10-26 23:59:47.000000 pop_create-7.3.1/pop_create.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-10-26 23:59:47.000000 pop_create-7.3.1/pop_create.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-26 23:59:47.348902 pop_create-7.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2813 2022-10-26 23:59:28.000000 pop_create-7.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-17 13:34:53.000000 pop_create-8.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-17 13:34:53.000000 pop_create-8.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-07-17 13:35:07.980431 pop_create-8.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-07-17 13:34:53.000000 pop_create-8.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.972431 pop_create-8.0.0/pop_create/pop_create/cicd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     5546 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/build.conf
+-rw-r--r--   0 root         (0) root         (0)     7978 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/.rstcheck.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/releases/{{cookiecutter.version_number}}.rst
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/sitevars.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/topics/license.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/example.rst
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/tutorial/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/hooks/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      366 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     8748 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)    11375 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/run.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/scripts.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      908 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.972431 pop_create-8.0.0/pop_create/pop_create/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/hooks/
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/hooks/post_gen_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/requirements/tests.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)      881 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      166 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/{{cookiecutter.clean_name}}/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      766 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/{{cookiecutter.clean_name}}/test_init.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.980431 pop_create-8.0.0/pop_create/tool/
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-07-17 13:34:53.000000 pop_create-8.0.0/pop_create/tool/path.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:35:07.976431 pop_create-8.0.0/pop_create.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-17 13:35:07.000000 pop_create-8.0.0/pop_create.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-17 13:35:07.980431 pop_create-8.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2814 2023-07-17 13:34:53.000000 pop_create-8.0.0/setup.py
```

### Comparing `pop_create-7.3.1/LICENSE` & `pop_create-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/PKG-INFO` & `pop_create-8.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pop_create
-Version: 7.3.1
+Version: 8.0.0
 Summary: Create new pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-create/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-create
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-create/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==========
 pop-create
 ==========
```

### Comparing `pop_create-7.3.1/README.rst` & `pop_create-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/conf.py` & `pop_create-8.0.0/pop_create/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc` & `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.coveragerc`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml` & `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     when: always
     paths:
       - artifacts
     reports:
       junit: artifacts/junit-report.xml
     expire_in: 30 days
 
-tests-3.7:
-  extends: .test-suite
-  image: python:3.7
-
 tests-3.8:
   extends: .test-suite
   image: python:3.8
 
 tests-3.9:
   extends: .test-suite
   image: python:3.9
 
 tests-3.10:
   extends: .test-suite
   image: python:3.10
+
+tests-3.11:
+  extends: .test-suite
+  image: python:3.11
```

### Comparing `pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml` & `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -44,22 +44,22 @@
     hooks:
       - id: remove-import-headers
 
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.1.0
     hooks:
       - id: pyupgrade
-        name: Rewrite Code to be Py3.7+
-        args: [--py37-plus]
+        name: Rewrite Code to be Py3.8+
+        args: [--py38-plus]
 
   - repo: https://github.com/asottile/reorder_python_imports
     rev: v3.8.4
     hooks:
       - id: reorder-python-imports
-        args: [--py37-plus]
+        args: [--py38-plus]
 
   - repo: https://github.com/psf/black
     rev: 22.10.0
     hooks:
       - id: black
         args: []
 
@@ -79,25 +79,14 @@
   # <---- Formatting -----------------------------------------------------------------------------
 
   # ----- Testing Static Requirements ------------------------------------------------------------------------------------>
   - repo: https://github.com/saltstack/pip-tools-compile-impersonate
     rev: '4.5'
     hooks:
       - id: pip-tools-compile
-        alias: compile-3.7-test-requirements
-        name: Py3.7 Test Requirements
-        files: ^requirements/tests.in$
-        pass_filenames: false
-        args:
-          - -v
-          - --py-version=3.7
-          - --platform=linux
-          - requirements/tests.in
-
-      - id: pip-tools-compile
         alias: compile-3.8-test-requirements
         name: Py3.8 Test Requirements
         files: ^requirements/tests.in$
         pass_filenames: false
         args:
           - -v
           - --py-version=3.8
@@ -122,24 +111,36 @@
         pass_filenames: false
         args:
           - -v
           - --py-version=3.10
           - --platform=linux
           - requirements/tests.in
 
+      - id: pip-tools-compile
+        alias: compile-3.11-test-requirements
+        name: Py3.11 Test Requirements
+        files: ^requirements/tests.in$
+        pass_filenames: false
+        args:
+          - -v
+          - --py-version=3.11
+          - --platform=linux
+          - requirements/tests.in
+
   # <---- Testing Static Requirements -------------------------------------------------------------------------------------
 
   # ----- Docs -------------------------------------------------------------------------------------------------->
 
   - repo: https://github.com/saltstack/mirrors-nox
     rev: v2022.8.7
     hooks:
       - id: nox
         alias: Generate Sphinx docs
         description: Generate Sphinx docs, ensure they build
+        files: ^((CONTRIBUTING|README)|docs/.*)\.rst$
         pass_filenames: false
         args:
           - -e
           - 'docs-html(clean=True)'
           - --
 
   # <---- Docs ---------------------------------------------------------------------------------------------------
@@ -154,7 +155,14 @@
         files: .*\.py
         exclude: >
             (?x)^(
                 tests/.*
             )$
 
   # <---- Security ---------------------------------------------------------------------------------------------------
+
+  # ----- Build Test -------------------------------------------------------------------------------------------------->
+  - repo: https://github.com/miki725/pre-commit-twine-check
+    rev: '0.1'
+    hooks:
+      - id: twine-check
+  # <---- Build Test ---------------------------------------------------------------------------------------------------
```

### Comparing `pop_create-7.3.1/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py` & `pop_create-8.0.0/pop_create/pop_create/cicd/{{cookiecutter.root_dir}}/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # Nox options
 #  Reuse existing virtualenvs
 nox.options.reuse_existing_virtualenvs = True
 #  Don't fail on missing interpreters
 nox.options.error_on_missing_interpreters = False
 
 # Python versions to test against
-PYTHON_VERSIONS = ("3", "3.7", "3.8", "3.9", "3.10")
+PYTHON_VERSIONS = ("3", "3.8", "3.9", "3.10", "3.11")
 # Be verbose when runing under a CI context
 CI_RUN = os.environ.get("CI")
 PIP_INSTALL_SILENT = CI_RUN is False
 SKIP_REQUIREMENTS_INSTALL = "SKIP_REQUIREMENTS_INSTALL" in os.environ
 EXTRA_REQUIREMENTS_INSTALL = os.environ.get("EXTRA_REQUIREMENTS_INSTALL")
 
 COVERAGE_VERSION_REQUIREMENT = "coverage==5.5"
@@ -75,16 +75,16 @@
         )
         session._runner._real_python_version_info = version_info
     return version_info
 
 
 def _get_pydir(session):
     version_info = _get_session_python_version_info(session)
-    if version_info < (3, 7):
-        session.error("Only Python >= 3.7 is supported")
+    if version_info < (3, 8):
+        session.error("Only Python >= 3.8 is supported")
     return "py{}.{}".format(*version_info)
 
 
 @nox.session(python=PYTHON_VERSIONS)
 def tests(session):
     if SKIP_REQUIREMENTS_INSTALL is False:
         # Always have the wheel package installed
```

### Comparing `pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py` & `pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst` & `pop_create-8.0.0/pop_create/pop_create/docs/{{cookiecutter.root_dir}}/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/init.py` & `pop_create-8.0.0/pop_create/pop_create/init.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/LICENSE`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.6+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,26 +71,26 @@
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
     license = "Apache Software License 2.0",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": ["{{cookiecutter.entrypoint}}"]},
     cmdclass={"clean": Clean},
 )
```

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/conf.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py` & `pop_create-8.0.0/pop_create/pop_create/seed/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/{{cookiecutter.clean_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/tests/hooks/post_gen_project.py` & `pop_create-8.0.0/pop_create/pop_create/tests/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop_create-8.0.0/pop_create/pop_create/tests/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create/tool/path.py` & `pop_create-8.0.0/pop_create/tool/path.py`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/pop_create.egg-info/PKG-INFO` & `pop_create-8.0.0/pop_create.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pop-create
-Version: 7.3.1
+Version: 8.0.0
 Summary: Create new pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-create/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-create
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-create/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==========
 pop-create
 ==========
```

### Comparing `pop_create-7.3.1/pop_create.egg-info/SOURCES.txt` & `pop_create-8.0.0/pop_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop_create-7.3.1/setup.py` & `pop_create-8.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,27 +66,27 @@
     },
     version=VERSION,
     install_requires=REQUIREMENTS,
     description=DESC,
     include_package_data=True,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="Apache Software License 2.0",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=discover_packages(),
     entry_points={
         "console_scripts": [
             "pop-create= pop_create.scripts:start",
```

