# Comparing `tmp/dcm2bids-2.1.9.tar.gz` & `tmp/dcm2bids-3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm2bids-2.1.9.tar", last modified: Fri Jun 17 20:30:23 2022, max compression
+gzip compressed data, was "dcm2bids-3.0rc1.tar", last modified: Mon Jul 17 17:54:31 2023, max compression
```

## Comparing `dcm2bids-2.1.9.tar` & `dcm2bids-3.0rc1.tar`

### file list

```diff
@@ -1,109 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.548835 dcm2bids-2.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.github/workflows/publish_doc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)    11532 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    35235 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5234 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/containers/
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/containers/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/containers/singularity.def
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/dcm2bids/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8553 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/dcm2bids.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/dcm2niix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/dcm2bids/scaffold/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/scaffold/CHANGES
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/scaffold/README
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/scaffold/dataset_description.json
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/scaffold/participants.json
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/scaffold/participants.tsv
--rw-r--r--   0 runner    (1001) docker     (121)     8906 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (121)     8982 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/dcm2bids/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/dcm2bids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5234 2022-06-17 20:30:23.000000 dcm2bids-2.1.9/dcm2bids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-06-17 20:30:23.000000 dcm2bids-2.1.9/dcm2bids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 20:30:23.000000 dcm2bids-2.1.9/dcm2bids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-17 20:30:23.000000 dcm2bids-2.1.9/dcm2bids.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-17 20:30:23.000000 dcm2bids-2.1.9/dcm2bids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-17 20:30:23.000000 dcm2bids-2.1.9/dcm2bids.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    35235 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.552835 dcm2bids-2.1.9/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.556835 dcm2bids-2.1.9/docs/assets/img/
--rw-r--r--   0 runner    (1001) docker     (121)   189904 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/dcm_qa_nih_repo-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)   170653 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/dcm_qa_nih_repo-light.png
--rw-r--r--   0 runner    (1001) docker     (121)   190229 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/github-issue-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)   203981 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/github-issue-light.png
--rw-r--r--   0 runner    (1001) docker     (121)    87736 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-1-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    82140 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-1-light.png
--rw-r--r--   0 runner    (1001) docker     (121)   310960 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-2-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)   277609 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-2-light.png
--rw-r--r--   0 runner    (1001) docker     (121)    69988 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-3-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    65068 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-3-light.png
--rw-r--r--   0 runner    (1001) docker     (121)    43868 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-4-dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    39685 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/assets/img/neurostars-4-light.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.556835 dcm2bids-2.1.9/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/get-started/index.md
--rw-r--r--   0 runner    (1001) docker     (121)    15005 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/get-started/install.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.556835 dcm2bids-2.1.9/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/how-to/create-config-file.md
--rw-r--r--   0 runner    (1001) docker     (121)     7225 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/how-to/get-help.md
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/how-to/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/how-to/use-advanced-commands.md
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/how-to/use-main-commands.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)    46083 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/tutorial/first-steps.md
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs/tutorial/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.548835 dcm2bids-2.1.9/docs_helper/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.548835 dcm2bids-2.1.9/docs_helper/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/docs_helper/templates/partials/
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/docs_helper/templates/partials/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/example/
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/example/config.json
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2600 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/config_test.json
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/config_test_not_case_sensitive_option.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:30:23.560835 dcm2bids-2.1.9/tests/data/sidecars/
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/001_localizer_20100603125600_i00001.json
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/001_localizer_20100603125600_i00002.json
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/001_localizer_20100603125600_i00003.json
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/002_ep2d_bold_20100603125600.json
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/003_MPRAGE_20100603125600.json
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/004_DTI_20100603125600.json
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/005_DTI_20100603125600.json
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/006_DTI_20100603125600.json
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/007_DTI_20100603125600.json
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/010_gre_field_mapping_20100603125600_e1.json
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/010_gre_field_mapping_20100603125600_e2.json
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/data/sidecars/011_gre_field_mapping_20100603125600_e2_ph.json
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/test_dcm2bids.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/test_dcm2niix.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/test_sidecar.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-06-17 20:30:13.000000 dcm2bids-2.1.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.731131 dcm2bids-3.0rc1/dcm2bids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.731131 dcm2bids-3.0rc1/dcm2bids/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/cli/dcm2bids_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/dcm2bids_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/dcm2niix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/dcm2bids/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/dcm2bids/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:31.731131 dcm2bids-3.0rc1/dcm2bids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 17:54:31.000000 dcm2bids-3.0rc1/dcm2bids.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:54:31.735131 dcm2bids-3.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-07-17 17:54:20.000000 dcm2bids-3.0rc1/setup.py
```

### Comparing `dcm2bids-2.1.9/LICENSE.txt` & `dcm2bids-3.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcm2bids-2.1.9/PKG-INFO` & `dcm2bids-3.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: dcm2bids
-Version: 2.1.9
+Version: 3.0rc1
 Summary: Reorganising NIfTI files from dcm2niix into the Brain Imaging Data Structure
-Home-page: UNKNOWN
-Author: Christophe Bedetti
-Author-email: christophe.bedetti@umontreal.ca
+Maintainer: Arnaud Boré
+Maintainer-email: arnaud.bore@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://unfmontreal.github.io/Dcm2Bids
 Project-URL: Source Code, https://github.com/unfmontreal/Dcm2Bids
-Platform: UNKNOWN
+Platform: OS Independent
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dcm2bids
 Your friendly DICOM converter.
 
 [![Documentation badge](https://img.shields.io/badge/Documentation-dcm2bids-succes.svg)](https://unfmontreal.github.io/Dcm2Bids)
@@ -35,24 +35,36 @@
 
 [![Test status badge](https://github.com/unfmontreal/Dcm2Bids/workflows/Tests/badge.svg)](https://github.com/unfmontreal/Dcm2Bids/actionsk)
 [![Code coverage badge](https://codecov.io/gh/unfmontreal/Dcm2Bids/branch/master/graph/badge.svg)](https://codecov.io/gh/unfmontreal/Dcm2Bids)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![PyPI version badge](https://img.shields.io/pypi/v/dcm2bids?logo=pypi&logoColor=white)](https://pypi.org/project/dcm2bids)
+[![PyPI - Downloads](https://static.pepy.tech/badge/dcm2bids)](https://pypi.org/project/dcm2bids)
+
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/dcm2bids?logo=anaconda&logoColor=white)](https://anaconda.org/conda-forge/dcm2bids)
 [![Docker container badge](https://img.shields.io/docker/v/unfmontreal/dcm2bids?label=docker&logo=docker&logoColor=white)](https://hub.docker.com/r/unfmontreal/dcm2bids)
 
 
 [![License badge](https://img.shields.io/pypi/l/dcm2bids)](/docs/LICENSE.txt)
 
 ---
 
 `dcm2bids` reorganises NIfTI files using [dcm2niix][dcm2niix-github] into the [Brain Imaging Data Structure][bids] (BIDS).
 
+
+## Major upgrade with dcm2bids >=3.0.0
+
+⚠️ Breaking changes alert ⚠️
+
+**dcm2bids>=3.0.0 is not compatible with config files made for v2.1.9 and below**.
+In order to develop dcm2bids new features we had to rewrite some of its code.  
+Since v3.0.0, dcm2bids has become **more powerful** and **more flexible** while reducing the burden of creating config files. Porting your config file should be relatively easy by following the [How-to upgrade][dcm2bids-upgrade] page.
+If you have any issues with it don't hesitate to report it on [Neurostars][neurostars-dcm2bids].
+
 ## Scope
 
 `dcm2bids` is a community-centered project. It aims to be a friendly,
 easy-to-use tool to convert your dicoms. Our main goal is to make the dicom
 to BIDS conversion as effortless as possible. Even if in the near future
 more advanced features will be added, we'll keep the focus on your day
 to day use case without complicating anything. That's the promise of the `dcm2bids` project.
@@ -76,18 +88,17 @@
 - If you think you've found a bug :bug:, please open an issue on [our repository][dcm2bids-issues]. To do this, you'll need a GitHub account. See our [contributing guide](CONTRIBUTING/#open-an-issue-or-choose-one-to-fix) for more details.
 
 
 [bids]: http://bids.neuroimaging.io/
 [bids-examples]: https://github.com/bids-standard/bids-examples
 [bids-spec]: https://bids-specification.readthedocs.io/en/stable/
 [dcm2bids-doc]: https://unfmontreal.github.io/Dcm2Bids
-[dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/docs/get-started/install/
-[dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/docs/tutorial/first-steps/#tutorial-first-steps
-[dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/docs/advanced/
+[dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/latest/get-started/install/
+[dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/latest/tutorial/first-steps/#tutorial-first-steps
+[dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/latest/advanced/
+[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/latest/upgrade/
 [dcm2bids-issues]: https://github.com/UNFmontreal/Dcm2Bids/issues
 [dcm2niix-install]: https://github.com/rordenlab/dcm2niix#install
 [dcm2niix-github]: https://github.com/rordenlab/dcm2niix
 [neurostars]: https://neurostars.org/
 [neurostars-dcm2bids]: https://neurostars.org/tag/dcm2bids
-[dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/CONTRIBUTING
-
-
+[dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/latest/how-to/contributing/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcm2bids-2.1.9/README.md` & `dcm2bids-3.0rc1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,36 @@
 
 [![Test status badge](https://github.com/unfmontreal/Dcm2Bids/workflows/Tests/badge.svg)](https://github.com/unfmontreal/Dcm2Bids/actionsk)
 [![Code coverage badge](https://codecov.io/gh/unfmontreal/Dcm2Bids/branch/master/graph/badge.svg)](https://codecov.io/gh/unfmontreal/Dcm2Bids)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![PyPI version badge](https://img.shields.io/pypi/v/dcm2bids?logo=pypi&logoColor=white)](https://pypi.org/project/dcm2bids)
+[![PyPI - Downloads](https://static.pepy.tech/badge/dcm2bids)](https://pypi.org/project/dcm2bids)
+
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/dcm2bids?logo=anaconda&logoColor=white)](https://anaconda.org/conda-forge/dcm2bids)
 [![Docker container badge](https://img.shields.io/docker/v/unfmontreal/dcm2bids?label=docker&logo=docker&logoColor=white)](https://hub.docker.com/r/unfmontreal/dcm2bids)
 
 
 [![License badge](https://img.shields.io/pypi/l/dcm2bids)](/docs/LICENSE.txt)
 
 ---
 
 `dcm2bids` reorganises NIfTI files using [dcm2niix][dcm2niix-github] into the [Brain Imaging Data Structure][bids] (BIDS).
 
+
+## Major upgrade with dcm2bids >=3.0.0
+
+⚠️ Breaking changes alert ⚠️
+
+**dcm2bids>=3.0.0 is not compatible with config files made for v2.1.9 and below**.
+In order to develop dcm2bids new features we had to rewrite some of its code.  
+Since v3.0.0, dcm2bids has become **more powerful** and **more flexible** while reducing the burden of creating config files. Porting your config file should be relatively easy by following the [How-to upgrade][dcm2bids-upgrade] page.
+If you have any issues with it don't hesitate to report it on [Neurostars][neurostars-dcm2bids].
+
 ## Scope
 
 `dcm2bids` is a community-centered project. It aims to be a friendly,
 easy-to-use tool to convert your dicoms. Our main goal is to make the dicom
 to BIDS conversion as effortless as possible. Even if in the near future
 more advanced features will be added, we'll keep the focus on your day
 to day use case without complicating anything. That's the promise of the `dcm2bids` project.
@@ -49,16 +61,17 @@
 - If you think you've found a bug :bug:, please open an issue on [our repository][dcm2bids-issues]. To do this, you'll need a GitHub account. See our [contributing guide](CONTRIBUTING/#open-an-issue-or-choose-one-to-fix) for more details.
 
 
 [bids]: http://bids.neuroimaging.io/
 [bids-examples]: https://github.com/bids-standard/bids-examples
 [bids-spec]: https://bids-specification.readthedocs.io/en/stable/
 [dcm2bids-doc]: https://unfmontreal.github.io/Dcm2Bids
-[dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/docs/get-started/install/
-[dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/docs/tutorial/first-steps/#tutorial-first-steps
-[dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/docs/advanced/
+[dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/latest/get-started/install/
+[dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/latest/tutorial/first-steps/#tutorial-first-steps
+[dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/latest/advanced/
+[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/latest/upgrade/
 [dcm2bids-issues]: https://github.com/UNFmontreal/Dcm2Bids/issues
 [dcm2niix-install]: https://github.com/rordenlab/dcm2niix#install
 [dcm2niix-github]: https://github.com/rordenlab/dcm2niix
 [neurostars]: https://neurostars.org/
 [neurostars-dcm2bids]: https://neurostars.org/tag/dcm2bids
-[dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/CONTRIBUTING
+[dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/latest/how-to/contributing/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dcm2bids-2.1.9/dcm2bids/dcm2niix.py` & `dcm2bids-3.0rc1/dcm2bids/dcm2niix_gen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,110 @@
 # -*- coding: utf-8 -*-
 
 """Dcm2niix class"""
 
 import logging
 import os
-from pathlib import Path
 import shlex
 import shutil
 from glob import glob
-from .utils import DEFAULT, run_shell_command
 
+from dcm2bids.utils.utils import DEFAULT, run_shell_command
 
-class Dcm2niix(object):
+
+class Dcm2niixGen(object):
     """ Object to handle dcm2niix execution
 
     Args:
-        dicomDirs (list): A list of folder with dicoms to convert
-        bidsDir (str): A path to the root BIDS directory
+        dicom_dirs (list): A list of folder with dicoms to convert
+        bids_dir (str): A path to the root BIDS directory
         participant: Optional Participant object
         options (str): Optional arguments for dcm2niix
 
     Properties:
         sidecars (list): A list of sidecar path created by dcm2niix
     """
 
     def __init__(
-        self, dicomDirs, bidsDir, participant=None, options=DEFAULT.dcm2niixOptions
+        self,
+        dicom_dirs,
+        bids_dir,
+        participant=None,
+        options=DEFAULT.dcm2niixOptions,
+        helper=False
     ):
         self.logger = logging.getLogger(__name__)
-
         self.sidecarsFiles = []
-
-        self.dicomDirs = dicomDirs
-        self.bidsDir = bidsDir
+        self.dicom_dirs = dicom_dirs
+        self.bids_dir = bids_dir
         self.participant = participant
         self.options = options
+        self.helper = helper
 
     @property
-    def outputDir(self):
+    def output_dir(self):
         """
         Returns:
             A directory to save all the output files of dcm2niix
         """
-        tmpDir = self.participant.prefix if self.participant else DEFAULT.helperDir
-
-        return self.bidsDir / DEFAULT.tmpDirName / tmpDir
+        tmpDir = self.participant.prefix if self.participant else DEFAULT.helper_dir
+        tmpDir = self.bids_dir / DEFAULT.tmp_dir_name / tmpDir
+        if self.helper:
+            tmpDir = self.bids_dir
+        return tmpDir
 
-    def run(self, force=False):
+    def run(self, force=False, helper=False):
         """ Run dcm2niix if necessary
 
         Args:
             force (boolean): Forces a cleaning of a previous execution of
                              dcm2niix
 
         Sets:
             sidecarsFiles (list): A list of sidecar path created by dcm2niix
         """
         try:
-            oldOutput = os.listdir(self.outputDir) != []
-        except:
+            oldOutput = os.listdir(self.output_dir) != []
+        except Exception:
             oldOutput = False
 
         if oldOutput and force:
             self.logger.warning("Previous dcm2niix directory output found:")
-            self.logger.warning(self.outputDir)
+            self.logger.warning(self.output_dir)
             self.logger.warning("'force' argument is set to True")
             self.logger.warning("Cleaning the previous directory and running dcm2niix")
 
-            shutil.rmtree(self.outputDir, ignore_errors=True)
+            shutil.rmtree(self.output_dir, ignore_errors=True)
 
-            # os.makedirs(self.outputDir, exist_ok=True)
-            # python2 compatibility
-            if not os.path.exists(self.outputDir):
-                os.makedirs(self.outputDir)
+            if not os.path.exists(self.output_dir):
+                os.makedirs(self.output_dir)
 
             self.execute()
 
         elif oldOutput:
             self.logger.warning("Previous dcm2niix directory output found:")
-            self.logger.warning(self.outputDir)
-            self.logger.warning("Use --forceDcm2niix to rerun dcm2niix")
+            self.logger.warning(self.output_dir)
+            self.logger.warning("Use --force_dcm2niix to rerun dcm2niix\n")
 
         else:
-            # os.makedirs(self.outputDir, exist_ok=True)
-            # python2 compatibility
-            if not os.path.exists(self.outputDir):
-                os.makedirs(self.outputDir)
+            if not os.path.exists(self.output_dir):
+                os.makedirs(self.output_dir)
 
             self.execute()
 
-        self.sidecarFiles = glob(os.path.join(self.outputDir, "*.json"))
+        self.sidecarFiles = glob(os.path.join(self.output_dir, "*.json"))
 
     def execute(self):
-        """ Execute dcm2niix for each directory in dicomDirs
+        """ Execute dcm2niix for each directory in dicom_dirs
         """
-        for dicomDir in self.dicomDirs:
+        for dicomDir in self.dicom_dirs:
             cmd = ['dcm2niix', *shlex.split(self.options),
-                   '-o', self.outputDir, dicomDir]
+                   '-o', self.output_dir, dicomDir]
             output = run_shell_command(cmd)
 
             try:
                 output = output.decode()
-            except:
+            except Exception:
                 pass
 
-            self.logger.debug("\n%s", output)
-            self.logger.info("Check log file for dcm2niix output")
+            self.logger.debug(f"\n{output}")
+            self.logger.info("Check log file for dcm2niix output\n")
```

### Comparing `dcm2bids-2.1.9/dcm2bids/structure.py` & `dcm2bids-3.0rc1/dcm2bids/acquisition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,242 +1,168 @@
 # -*- coding: utf-8 -*-
 
 """Participant class"""
 
 import logging
 from os.path import join as opj
-from future.utils import iteritems
-from .utils import DEFAULT
-from .version import __version__
 
-
-class Participant(object):
-    """ Class representing a participant
-
-    Args:
-        name (str): Label of your participant
-        session (str): Optional label of a session
-    """
-
-    def __init__(self, name, session=DEFAULT.session):
-        self._name = ""
-        self._session = ""
-
-        self.name = name
-        self.session = session
-
-    @property
-    def name(self):
-        """
-        Returns:
-            A string 'sub-<subject_label>'
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """ Prepend 'sub-' if necessary"""
-        if name.startswith("sub-"):
-            self._name = name
-
-        else:
-            self._name = "sub-" + name
-
-    @property
-    def session(self):
-        """
-        Returns:
-            A string 'ses-<session_label>'
-        """
-        return self._session
-
-    @session.setter
-    def session(self, session):
-        """ Prepend 'ses-' if necessary"""
-        if session.strip() == "":
-            self._session = ""
-
-        elif session.startswith("ses-"):
-            self._session = session
-
-        else:
-            self._session = "ses-" + session
-
-    @property
-    def directory(self):
-        """ The directory of the participant
-
-        Returns:
-            A path 'sub-<subject_label>' or
-            'sub-<subject_label>/ses-<session_label>'
-        """
-        if self.hasSession():
-            return opj(self.name, self.session)
-        else:
-            return self.name
-
-    @property
-    def prefix(self):
-        """ The prefix to build filenames
-
-        Returns:
-            A string 'sub-<subject_label>' or
-            'sub-<subject_label>_ses-<session_label>'
-        """
-        if self.hasSession():
-            return self.name + "_" + self.session
-        else:
-            return self.name
-
-    def hasSession(self):
-        """ Check if a session is set
-
-        Returns:
-            Boolean
-        """
-        return self.session.strip() != DEFAULT.session
+from dcm2bids.utils.utils import DEFAULT
+from dcm2bids.version import __version__
 
 
 class Acquisition(object):
     """ Class representing an acquisition
 
     Args:
         participant (Participant): A participant object
-        dataType (str): A functional group of MRI data (ex: func, anat ...)
-        modalityLabel (str): The modality of the acquisition
+        datatype (str): A functional group of MRI data (ex: func, anat ...)
+        suffix (str): The modality of the acquisition
                 (ex: T1w, T2w, bold ...)
-        customLabels (str): Optional labels (ex: task-rest)
-        srcSidecar (Sidecar): Optional sidecar object
+        custom_entities (str): Optional entities (ex: task-rest)
+        src_sidecar (Sidecar): Optional sidecar object
     """
 
     def __init__(
         self,
         participant,
-        dataType,
-        modalityLabel,
-        indexSidecar=None,
-        customLabels="",
-        srcSidecar=None,
-        sidecarChanges=None,
-        intendedFor=None,
-        IntendedFor=None,
+        datatype,
+        suffix,
+        custom_entities="",
+        id=None,
+        src_sidecar=None,
+        sidecar_changes=None,
         **kwargs
     ):
         self.logger = logging.getLogger(__name__)
 
-        self._modalityLabel = ""
-        self._customLabels = ""
-        self._intendedFor = None
-        self._indexSidecar = None
+        self._suffix = ""
+        self._custom_entities = ""
+        self._id = ""
 
         self.participant = participant
-        self.dataType = dataType
-        self.modalityLabel = modalityLabel
-        self.customLabels = customLabels
-        self.srcSidecar = srcSidecar
+        self.datatype = datatype
+        self.suffix = suffix
+        self.custom_entities = custom_entities
+        self.src_sidecar = src_sidecar
 
-        if sidecarChanges is None:
-            self.sidecarChanges = {}
+        if sidecar_changes is None:
+            self.sidecar_changes = {}
         else:
-            self.sidecarChanges = sidecarChanges
+            self.sidecar_changes = sidecar_changes
 
-        if intendedFor is None:
-            self.intendedFor = IntendedFor
+        if id is None:
+            self.id = None
         else:
-            self.intendedFor = intendedFor
+            self.id = id
 
         self.dstFile = ''
 
     def __eq__(self, other):
         return (
-            self.dataType == other.dataType
+            self.datatype == other.datatype
             and self.participant.prefix == other.participant.prefix
-            and self.suffix == other.suffix
+            and self.build_suffix == other.build_suffix
         )
 
     @property
-    def modalityLabel(self):
+    def suffix(self):
         """
         Returns:
-            A string '_<modalityLabel>'
+            A string '_<suffix>'
         """
-        return self._modalityLabel
+        return self._suffix
 
-    @modalityLabel.setter
-    def modalityLabel(self, modalityLabel):
+    @suffix.setter
+    def suffix(self, suffix):
         """ Prepend '_' if necessary"""
-        self._modalityLabel = self.prepend(modalityLabel)
+        self._suffix = self.prepend(suffix)
+
+    @property
+    def id(self):
+        """
+        Returns:
+            A string '_<id>'
+        """
+        return self._id
+
+    @id.setter
+    def id(self, value):
+        self._id = value
 
     @property
-    def customLabels(self):
+    def custom_entities(self):
         """
         Returns:
-            A string '_<customLabels>'
+            A string '_<custom_entities>'
         """
-        return self._customLabels
+        return self._custom_entities
 
-    @customLabels.setter
-    def customLabels(self, customLabels):
+    @custom_entities.setter
+    def custom_entities(self, custom_entities):
         """ Prepend '_' if necessary"""
-        self._customLabels = self.prepend(customLabels)
+        if isinstance(custom_entities, list):
+            self._custom_entities = self.prepend('_'.join(custom_entities))
+        else:
+            self._custom_entities = self.prepend(custom_entities)
 
     @property
-    def suffix(self):
+    def build_suffix(self):
         """ The suffix to build filenames
 
         Returns:
-            A string '_<modalityLabel>' or '_<customLabels>_<modalityLabel>'
+            A string '_<suffix>' or '_<custom_entities>_<suffix>'
         """
-        if self.customLabels.strip() == "":
-            return self.modalityLabel
+        if self.custom_entities.strip() == "":
+            return self.suffix
         else:
-            return self.customLabels + self.modalityLabel
+            return self.custom_entities + self.suffix
 
     @property
     def srcRoot(self):
         """
         Return:
             The sidecar source root to move
         """
-        if self.srcSidecar:
-            return self.srcSidecar.root
+        if self.src_sidecar:
+            return self.src_sidecar.root
         else:
             return None
 
     @property
     def dstRoot(self):
         """
         Return:
             The destination root inside the BIDS structure
         """
         return opj(
             self.participant.directory,
-            self.dataType,
+            self.datatype,
             self.dstFile,
         )
 
     @property
-    def dstIntendedFor(self):
+    def dstId(self):
         """
         Return:
-            The destination root inside the BIDS structure for intendedFor
+            The destination root inside the BIDS structure for description
         """
         return opj(
             self.participant.session,
-            self.dataType,
+            self.datatype,
             self.dstFile,
         )
 
     def setDstFile(self):
         """
         Return:
-            The destination filename formatted following the v1.7.0 BIDS entity key table
-            https://bids-specification.readthedocs.io/en/v1.7.0/99-appendices/04-entity-table.html
+            The destination filename formatted following
+            the v1.8.0 BIDS entity key table
+            https://bids-specification.readthedocs.io/en/v1.8.0/99-appendices/04-entity-table.html
         """
-        current_name = self.participant.prefix + self.suffix
+        current_name = self.participant.prefix + self.build_suffix
         new_name = ''
         current_dict = dict(x.split("-") for x in current_name.split("_") if len(x.split('-')) == 2)
         suffix_list = [x for x in current_name.split("_") if len(x.split('-')) == 1]
 
         for current_key in DEFAULT.entityTableKeys:
             if current_key in current_dict and new_name != '':
                 new_name += f"_{current_key}-{current_dict[current_key]}"
@@ -244,18 +170,19 @@
                 new_name = f"{current_key}-{current_dict[current_key]}"
             current_dict.pop(current_key, None)
 
         for current_key in current_dict:
             new_name += f"_{current_key}-{current_dict[current_key]}"
 
         if current_dict:
-            self.logger.warning("Entity \"{}\"".format(list(current_dict.keys())) +
-                                " is not a valid BIDS entity.")
+            self.logger.warning(f'Entity \"{list(current_dict.keys())}\"'
+                                ' is not a valid BIDS entity.')
 
-        new_name += f"_{'_'.join(suffix_list)}"  # Allow multiple single keys (without value)
+        # Allow multiple single keys (without value)
+        new_name += f"_{'_'.join(suffix_list)}"
 
         if len(suffix_list) != 1:
             self.logger.warning("There was more than one suffix found "
                                 f"({suffix_list}). This is not BIDS "
                                 "compliant. Make sure you know what "
                                 "you are doing.")
 
@@ -263,62 +190,53 @@
             self.logger.warning(
                 f"""✅ Filename was reordered according to BIDS entity table order:
                 from:   {current_name}
                 to:     {new_name}""")
 
         self.dstFile = new_name
 
-    @property
-    def intendedFor(self):
-        return self._intendedFor
-
-    @intendedFor.setter
-    def intendedFor(self, value):
-        if isinstance(value, list):
-            self._intendedFor = value
-        else:
-            self._intendedFor = [value]
-
-    @property
-    def indexSidecar(self):
+    def dstSidecarData(self, idList):
         """
-        Returns:
-            A int '_<indexSidecar>'
         """
-        return self._indexSidecar
-
-    @indexSidecar.setter
-    def indexSidecar(self, value):
-        """
-        Returns:
-            A int '_<indexSidecar>'
-        """
-        self._indexSidecar = value
-
-    def dstSidecarData(self, descriptions, intendedForList):
-        """
-        """
-        data = self.srcSidecar.origData
+        data = self.src_sidecar.origData
         data["Dcm2bidsVersion"] = __version__
 
-        # intendedFor key
-        if self.intendedFor != [None]:
-            intendedValue = []
-
-            for index in self.intendedFor:
-                intendedValue = intendedValue + intendedForList[index]
-
-            if len(intendedValue) == 1:
-                data["IntendedFor"] = intendedValue[0]
-            else:
-                data["IntendedFor"] = intendedValue
-
-        # sidecarChanges
-        for key, value in iteritems(self.sidecarChanges):
-            data[key] = value
+        # TaskName
+        if 'TaskName' in self.src_sidecar.data:
+            data["TaskName"] = self.src_sidecar.data["TaskName"]
+
+        # sidecar_changes
+        for key, value in self.sidecar_changes.items():
+            values = []
+
+            if not isinstance(value, list):
+                value = [value]
+
+            for val in value:
+                if isinstance(val, str):
+                    if val not in idList and key in DEFAULT.keyWithPathsidecar_changes:
+                        logging.warning(f"No id found for '{key}' value '{val}'.")
+                        logging.warning(f"No sidecar changes for field '{key}' "
+                                        f"will be made "
+                                        f"for json file '{self.dstFile}.json' "
+                                        "with this id.")
+                    else:
+                        values.append(idList.get(val, val))
+
+            # handle if nested list vs str
+            flat_value_list = []
+            for item in values:
+                if isinstance(item, list):
+                    flat_value_list += item
+                else:
+                    flat_value_list.append(item)
+            if len(flat_value_list) == 1:
+                flat_value_list = flat_value_list[0]
+
+            data[key] = flat_value_list
 
         return data
 
     @staticmethod
     def prepend(value, char="_"):
         """ Prepend `char` to `value` if necessary
```

### Comparing `dcm2bids-2.1.9/dcm2bids.egg-info/PKG-INFO` & `dcm2bids-3.0rc1/dcm2bids.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: dcm2bids
-Version: 2.1.9
+Version: 3.0rc1
 Summary: Reorganising NIfTI files from dcm2niix into the Brain Imaging Data Structure
-Home-page: UNKNOWN
-Author: Christophe Bedetti
-Author-email: christophe.bedetti@umontreal.ca
+Maintainer: Arnaud Boré
+Maintainer-email: arnaud.bore@gmail.com
 License: GPLv3+
 Project-URL: Documentation, https://unfmontreal.github.io/Dcm2Bids
 Project-URL: Source Code, https://github.com/unfmontreal/Dcm2Bids
-Platform: UNKNOWN
+Platform: OS Independent
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7
+Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # dcm2bids
 Your friendly DICOM converter.
 
 [![Documentation badge](https://img.shields.io/badge/Documentation-dcm2bids-succes.svg)](https://unfmontreal.github.io/Dcm2Bids)
@@ -35,24 +35,36 @@
 
 [![Test status badge](https://github.com/unfmontreal/Dcm2Bids/workflows/Tests/badge.svg)](https://github.com/unfmontreal/Dcm2Bids/actionsk)
 [![Code coverage badge](https://codecov.io/gh/unfmontreal/Dcm2Bids/branch/master/graph/badge.svg)](https://codecov.io/gh/unfmontreal/Dcm2Bids)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
 [![PyPI version badge](https://img.shields.io/pypi/v/dcm2bids?logo=pypi&logoColor=white)](https://pypi.org/project/dcm2bids)
+[![PyPI - Downloads](https://static.pepy.tech/badge/dcm2bids)](https://pypi.org/project/dcm2bids)
+
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/dcm2bids?logo=anaconda&logoColor=white)](https://anaconda.org/conda-forge/dcm2bids)
 [![Docker container badge](https://img.shields.io/docker/v/unfmontreal/dcm2bids?label=docker&logo=docker&logoColor=white)](https://hub.docker.com/r/unfmontreal/dcm2bids)
 
 
 [![License badge](https://img.shields.io/pypi/l/dcm2bids)](/docs/LICENSE.txt)
 
 ---
 
 `dcm2bids` reorganises NIfTI files using [dcm2niix][dcm2niix-github] into the [Brain Imaging Data Structure][bids] (BIDS).
 
+
+## Major upgrade with dcm2bids >=3.0.0
+
+⚠️ Breaking changes alert ⚠️
+
+**dcm2bids>=3.0.0 is not compatible with config files made for v2.1.9 and below**.
+In order to develop dcm2bids new features we had to rewrite some of its code.  
+Since v3.0.0, dcm2bids has become **more powerful** and **more flexible** while reducing the burden of creating config files. Porting your config file should be relatively easy by following the [How-to upgrade][dcm2bids-upgrade] page.
+If you have any issues with it don't hesitate to report it on [Neurostars][neurostars-dcm2bids].
+
 ## Scope
 
 `dcm2bids` is a community-centered project. It aims to be a friendly,
 easy-to-use tool to convert your dicoms. Our main goal is to make the dicom
 to BIDS conversion as effortless as possible. Even if in the near future
 more advanced features will be added, we'll keep the focus on your day
 to day use case without complicating anything. That's the promise of the `dcm2bids` project.
@@ -76,18 +88,17 @@
 - If you think you've found a bug :bug:, please open an issue on [our repository][dcm2bids-issues]. To do this, you'll need a GitHub account. See our [contributing guide](CONTRIBUTING/#open-an-issue-or-choose-one-to-fix) for more details.
 
 
 [bids]: http://bids.neuroimaging.io/
 [bids-examples]: https://github.com/bids-standard/bids-examples
 [bids-spec]: https://bids-specification.readthedocs.io/en/stable/
 [dcm2bids-doc]: https://unfmontreal.github.io/Dcm2Bids
-[dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/docs/get-started/install/
-[dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/docs/tutorial/first-steps/#tutorial-first-steps
-[dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/docs/advanced/
+[dcm2bids-install]: https://unfmontreal.github.io/Dcm2Bids/latest/get-started/install/
+[dcm2bids-tutorial]: https://unfmontreal.github.io/Dcm2Bids/latest/tutorial/first-steps/#tutorial-first-steps
+[dcm2bids-advanced]: https://unfmontreal.github.io/Dcm2Bids/latest/advanced/
+[dcm2bids-upgrade]: https://unfmontreal.github.io/Dcm2Bids/latest/upgrade/
 [dcm2bids-issues]: https://github.com/UNFmontreal/Dcm2Bids/issues
 [dcm2niix-install]: https://github.com/rordenlab/dcm2niix#install
 [dcm2niix-github]: https://github.com/rordenlab/dcm2niix
 [neurostars]: https://neurostars.org/
 [neurostars-dcm2bids]: https://neurostars.org/tag/dcm2bids
-[dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/CONTRIBUTING
-
-
+[dcm2bids-contributing]:  https://unfmontreal.github.io/Dcm2Bids/latest/how-to/contributing/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

