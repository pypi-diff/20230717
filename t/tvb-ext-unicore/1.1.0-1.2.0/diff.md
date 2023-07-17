# Comparing `tmp/tvb-ext-unicore-1.1.0.tar.gz` & `tmp/tvb-ext-unicore-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-ext-unicore-1.1.0.tar", last modified: Fri Feb 24 13:51:22 2023, max compression
+gzip compressed data, was "tvb-ext-unicore-1.2.0.tar", last modified: Mon Jul 17 11:41:37 2023, max compression
```

## Comparing `tvb-ext-unicore-1.1.0.tar` & `tvb-ext-unicore-1.2.0.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.344296 tvb-ext-unicore-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35181 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-02-24 13:51:22.344296 tvb-ext-unicore-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/jest.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.332296 tvb-ext-unicore-1.1.0/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.336296 tvb-ext-unicore-1.1.0/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/jupyter-config/nb-config/tvbextunicore.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.336296 tvb-ext-unicore-1.1.0/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/jupyter-config/server-config/tvbextunicore.json
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 13:51:22.344296 tvb-ext-unicore-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.336296 tvb-ext-unicore-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/JobOutputFiles.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/ModalComponent.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/PaginationComponent.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/SideButton.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/UnicoreJobsTable.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/UnicoreSites.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/constants.tests.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/__tests__/pyunicoreWidget.test.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/CheckBoxToggle.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/JobOutputFiles.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/ModalComponent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/PaginationComponent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/SideButton.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/UnicoreJobsTable.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/components/UnicoreSites.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/constants.ts
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/globals.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/src/pyunicoreWidget.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/style/base.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/style/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/style/icons/logo-unicore.svg
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/style/variables.css
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 13:50:41.000000 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/tvbextunicore/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.340296 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    17058 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/488.0f8ad58095bf1360be6b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/remoteEntry.10457d0adbf3941a60bb.js
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-24 13:51:20.000000 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-02-24 13:51:22.000000 tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.344296 tvb-ext-unicore-1.1.0/tvbextunicore/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.344296 tvb-ext-unicore-1.1.0/tvbextunicore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/tests/test_unicore_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 13:51:22.344296 tvb-ext-unicore-1.1.0/tvbextunicore/unicore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/unicore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/unicore_wrapper/job_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/tvbextunicore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   372706 2023-02-24 13:50:03.000000 tvb-ext-unicore-1.1.0/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35181 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/jest.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.473169 tvb-ext-unicore-1.2.0/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.481169 tvb-ext-unicore-1.2.0/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/jupyter-config/nb-config/tvbextunicore.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.481169 tvb-ext-unicore-1.2.0/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/jupyter-config/server-config/tvbextunicore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.481169 tvb-ext-unicore-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/JobOutputFiles.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/ModalComponent.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/PaginationComponent.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/SideButton.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/UnicoreJobsTable.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/UnicoreSites.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/constants.tests.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/pyunicoreWidget.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/__tests__/utils.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/CheckBoxToggle.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/JobOutputFiles.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/ModalComponent.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/PaginationComponent.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/SideButton.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/UnicoreJobsTable.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/components/UnicoreSites.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/constants.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/globals.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/pyunicoreWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/src/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/style/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/icons/logo-unicore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/style/variables.css
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.485169 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:40:55.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17540 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/774.f5b7ad80ab759770978c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/remoteEntry.c6b3242597cbbe03a95e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 11:41:35.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 11:41:37.000000 tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/tests/test_unicore_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:41:37.489169 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/job_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/tvbextunicore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   372706 2023-07-17 11:40:13.000000 tvb-ext-unicore-1.2.0/yarn.lock
```

### Comparing `tvb-ext-unicore-1.1.0/LICENSE` & `tvb-ext-unicore-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/MANIFEST.in` & `tvb-ext-unicore-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/PKG-INFO` & `tvb-ext-unicore-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-ext-unicore
-Version: 1.1.0
+Version: 1.2.0
 Summary: TVB Widgets - A Unicore Lab extension
 Home-page: https://github.com/the-virtual-brain/tvb-ext-unicore
 Author: TVB Widgets Team
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `tvb-ext-unicore-1.1.0/README.md` & `tvb-ext-unicore-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/RELEASE.md` & `tvb-ext-unicore-1.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/jest.config.js` & `tvb-ext-unicore-1.2.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/package.json` & `tvb-ext-unicore-1.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.2.0'"}*

```diff
@@ -100,9 +100,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.2.0"
 }
```

### Comparing `tvb-ext-unicore-1.1.0/pyproject.toml` & `tvb-ext-unicore-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/setup.py` & `tvb-ext-unicore-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     description=pkg_json["description"],
     license=pkg_json["license"],
     license_file="LICENSE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        "jupyter_server>=1.6,<2",
+        "jupyter_server",
         "pyunicore >= 0.11.1"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
```

### Comparing `tvb-ext-unicore-1.1.0/sonar-project.properties` & `tvb-ext-unicore-1.2.0/sonar-project.properties`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/JobOutputFiles.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/JobOutputFiles.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/ModalComponent.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/ModalComponent.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/PaginationComponent.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/PaginationComponent.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/SideButton.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/SideButton.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/UnicoreJobsTable.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/UnicoreJobsTable.test.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/UnicoreSites.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/UnicoreSites.test.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
   disabled: boolean,
   onChange: (site: string) => void = (s: string) => {
     return;
   }
 ) {
   const props = {
     sites: ['JUDAC', 'JUSUF', 'DAINT'],
+    defaultSite: 'JUDAC',
     onChangeSite: onChange,
     disableSelection: disabled,
     refreshSite: () => console.log('Refresh sites'),
     loading: false,
     setAutoReload: (val: boolean) => console.log(val)
   };
```

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/constants.tests.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/constants.tests.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/__tests__/pyunicoreWidget.test.tsx` & `tvb-ext-unicore-1.2.0/src/__tests__/pyunicoreWidget.test.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,32 @@
     generatedJobs.push(generateJob('failed', i));
   }
   return generatedJobs;
 }
 
 const RELOAD_RATE_S = RELOAD_RATE_MS / 1000;
 
-function renderUnicoreComponent(sites: string[] = []) {
+function renderUnicoreComponent(
+  sites: string[] = [],
+  defaultSite: string = NO_SITE
+) {
   const columns = ['id', 'name', 'owner', 'site', 'status', 'start_time'];
   const tableFormat = {
     cols: columns,
     idField: 'id',
     buttonRenderConditionField: 'is_cancelable'
   };
 
   return render(
     <PyunicoreComponent
       tableFormat={tableFormat}
       data={data}
       buttonSettings={BUTTON_SETTINGS}
       sites={[...sites, JUSUF, JUDAC]}
+      defaultSite={defaultSite}
       reloadRate={RELOAD_RATE_MS}
       getKernel={getKernel}
       getJobCode={mockGetJob}
       getFileBrowser={() => jest.fn as unknown as FileBrowser}
     />
   );
 }
@@ -106,15 +110,15 @@
 describe('<PyunicoreComponent />', () => {
   it('renders component correctly', async () => {
     // jest.useFakeTimers();
     const mockDate = new Date();
     const mockLaterDate = new Date();
     jest.setSystemTime(mockDate.getTime());
 
-    const { findByTestId } = renderUnicoreComponent();
+    const { findByTestId } = renderUnicoreComponent([], JUSUF);
 
     // simulate 60 seconds passed in system time to trigger update
     mockLaterDate.setSeconds(mockLaterDate.getSeconds() + RELOAD_RATE_S);
     jest.setSystemTime(mockLaterDate.getTime());
     jest.advanceTimersByTime(RELOAD_CHECK_RATE_MS); // advance timer to trigger the chock for reloads
 
     const pagination = await findByTestId('pagination-component');
```

### Comparing `tvb-ext-unicore-1.1.0/src/components/CheckBoxToggle.tsx` & `tvb-ext-unicore-1.2.0/src/components/CheckBoxToggle.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/components/JobOutputFiles.tsx` & `tvb-ext-unicore-1.2.0/src/components/JobOutputFiles.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -75,19 +75,19 @@
 
   return (
     <tr className={'outputFiles'} data-testid={`output-${props.job_url}`}>
       {outputFiles ? (
         <td colSpan={100}>
           <p className={'unicoreMessage'}>{message}</p>
           Output Files:
-          {Object.entries(outputFiles).map(([output, outputType], index) => (
+          {Object.entries(outputFiles).map(([output, outputType]) => (
             <JobOutput
               output={output}
               outputType={outputType}
-              key={`${output}-${index}`}
+              key={`${output}`}
               jobUrl={props.job_url}
               jobId={props.jobId}
               getFileBrowser={props.getFileBrowser}
               getKernel={props.getKernel}
             />
           ))}
         </td>
```

### Comparing `tvb-ext-unicore-1.1.0/src/components/ModalComponent.tsx` & `tvb-ext-unicore-1.2.0/src/components/ModalComponent.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/components/PaginationComponent.tsx` & `tvb-ext-unicore-1.2.0/src/components/PaginationComponent.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/components/SideButton.ts` & `tvb-ext-unicore-1.2.0/src/components/SideButton.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/components/UnicoreJobsTable.tsx` & `tvb-ext-unicore-1.2.0/src/components/UnicoreJobsTable.tsx`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/components/UnicoreSites.tsx` & `tvb-ext-unicore-1.2.0/src/components/UnicoreSites.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import React, { useState } from 'react';
 import { CheckBoxToggle } from './CheckBoxToggle';
 
 namespace types {
   export type Props = {
     sites: string[];
+    defaultSite: string;
     onChangeSite: (site: string) => void;
     disableSelection: boolean;
     refreshSite: () => void;
     loading: boolean;
     setAutoReload: (active: boolean) => void;
   };
 }
@@ -38,14 +39,15 @@
     <div className={'pyunicoreSites'} data-testid={'pyunicore-sites'}>
       <div>
         <span>SITE:</span>
         <select
           onChange={handleSiteChange}
           disabled={props.disableSelection}
           data-testid={'select'}
+          defaultValue={props.defaultSite}
         >
           {props.sites.map(site => (
             <option key={site} id={site} value={site}>
               {site}
             </option>
           ))}
         </select>
```

### Comparing `tvb-ext-unicore-1.1.0/src/constants.ts` & `tvb-ext-unicore-1.2.0/src/constants.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/handler.ts` & `tvb-ext-unicore-1.2.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/src/index.ts` & `tvb-ext-unicore-1.2.0/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,20 @@
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import {
   ICommandPalette,
   MainAreaWidget,
+  showErrorMessage,
   WidgetTracker
 } from '@jupyterlab/apputils';
 
+import { validateDefaultSite } from './utils';
+
 import { FileBrowser, IFileBrowserFactory } from '@jupyterlab/filebrowser';
 
 import { INotebookTracker, NotebookPanel } from '@jupyterlab/notebook';
 
 import { PyunicoreWidget } from './pyunicoreWidget';
 
 import { requestAPI } from './handler';
@@ -69,31 +72,49 @@
   ) => {
     console.log('JupyterLab extension tvb-ext-unicore is activated!');
     let widget: MainAreaWidget<PyunicoreWidget>;
     const columns = ['id', 'name', 'owner', 'site', 'status', 'start_time'];
     const command = 'tvbextunicore:open';
     app.commands.addCommand(command, {
       label: 'PyUnicore Task Stream',
-      execute: async (): Promise<any> => {
+      execute: async (args = { defaultSite: NO_SITE }): Promise<any> => {
         if (!widget || widget.isDisposed) {
-          const sitesResponse = await requestAPI<SitesResponse>('sites');
+          let sitesResponse: SitesResponse;
+          let availableSites: string[] = [];
+          let defaultSite: string;
+          try {
+            sitesResponse = await requestAPI<SitesResponse>('sites');
+            availableSites = [...Object.keys(sitesResponse.sites)];
+            const desiredDefaultSite = args['defaultSite'] as string;
+            defaultSite = validateDefaultSite(
+              desiredDefaultSite,
+              availableSites
+            );
+          } catch (e) {
+            await showErrorMessage(
+              'ERROR',
+              'Unicore seems to be down at the moment. Please check service availability and try again later.'
+            );
+            return;
+          }
           const content = new PyunicoreWidget({
             tableFormat: {
               cols: columns,
               idField: 'id',
               buttonRenderConditionField: 'is_cancelable'
             },
             data: { message: sitesResponse.message, jobs: [] },
             buttonSettings: {
               onClick: cancelJob,
               onClickFieldArgs: ['resource_url'],
               isAsync: false,
               name: 'Cancel Job'
             },
-            sites: [NO_SITE, ...Object.keys(sitesResponse.sites)],
+            sites: [NO_SITE, ...availableSites],
+            defaultSite: defaultSite,
             reloadRate: 60000,
             getKernel: async () => {
               const kernel = Private.getCurrentKernel(
                 labShell,
                 notebookTracker,
                 consoleTracker
               );
```

### Comparing `tvb-ext-unicore-1.1.0/src/pyunicoreWidget.tsx` & `tvb-ext-unicore-1.2.0/src/pyunicoreWidget.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 namespace types {
   export type Props = {
     tableFormat: ITableFormat;
     data: IDataType;
     buttonSettings: IButtonSettings;
     sites: string[];
+    defaultSite: string;
     reloadRate: number;
     getKernel: () => Promise<Kernel.IKernelConnection | null | undefined>;
     getJobCode: (job_url: string) => string;
     getFileBrowser: () => FileBrowser;
   };
 
   export type State = {
@@ -97,14 +98,15 @@
   protected render(): JSX.Element {
     return (
       <PyunicoreComponent
         tableFormat={this.props.tableFormat}
         data={this.props.data}
         buttonSettings={this.props.buttonSettings}
         sites={this.props.sites}
+        defaultSite={this.props.defaultSite}
         reloadRate={RELOAD_RATE_MS}
         getKernel={this.props.getKernel}
         getJobCode={this.props.getJobCode}
         getFileBrowser={this.props.getFileBrowser}
       /> // see how we can wrap this to use signal
     );
   }
@@ -128,15 +130,15 @@
     this.getData = this.getData.bind(this);
     this.catchError = this.catchError.bind(this);
     this.setAutoReload = this.setAutoReload.bind(this);
     const lastUpdate = new Date();
     this.state = {
       jobs: [],
       message: props.data.message,
-      site: props.sites[0],
+      site: props.defaultSite,
       buttonSettings: props.buttonSettings,
       tableFormat: props.tableFormat,
       reloadRate: RELOAD_RATE_MS,
       loading: props.sites.length > 0,
       sites: props.sites,
       page: 1,
       itemsPerPage: 10,
@@ -358,14 +360,15 @@
             showNextButton={this.state.renderRightArrow}
             showPrevButton={this.state.renderLeftArrow}
             currentPage={this.state.page}
           />
           <UnicoreSites
             sites={this.state.sites}
             onChangeSite={this.setSiteState}
+            defaultSite={this.state.site}
             disableSelection={this.state.disableSitesSelection}
             refreshSite={() => this._triggerUpdate(true)}
             loading={this.state.loading}
             setAutoReload={this.setAutoReload}
           />
           {this.state.loading ? (
             <div>
```

### Comparing `tvb-ext-unicore-1.1.0/style/base.css` & `tvb-ext-unicore-1.2.0/style/base.css`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/style/icons/logo-unicore.svg` & `tvb-ext-unicore-1.2.0/style/icons/logo-unicore.svg`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/style/variables.css` & `tvb-ext-unicore-1.2.0/style/variables.css`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tsconfig.json` & `tvb-ext-unicore-1.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/PKG-INFO` & `tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-ext-unicore
-Version: 1.1.0
+Version: 1.2.0
 Summary: TVB Widgets - A Unicore Lab extension
 Home-page: https://github.com/the-virtual-brain/tvb-ext-unicore
 Author: TVB Widgets Team
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `tvb-ext-unicore-1.1.0/tvb_ext_unicore.egg-info/SOURCES.txt` & `tvb-ext-unicore-1.2.0/tvb_ext_unicore.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 jupyter-config/nb-config/tvbextunicore.json
 jupyter-config/server-config/tvbextunicore.json
 src/constants.ts
 src/globals.d.ts
 src/handler.ts
 src/index.ts
 src/pyunicoreWidget.tsx
+src/utils.ts
 src/__tests__/JobOutputFiles.test.tsx
 src/__tests__/ModalComponent.test.tsx
 src/__tests__/PaginationComponent.test.tsx
 src/__tests__/SideButton.test.tsx
 src/__tests__/UnicoreJobsTable.test.tsx
 src/__tests__/UnicoreSites.test.tsx
 src/__tests__/constants.tests.tsx
 src/__tests__/pyunicoreWidget.test.tsx
+src/__tests__/utils.test.ts
 src/components/CheckBoxToggle.tsx
 src/components/JobOutputFiles.tsx
 src/components/ModalComponent.tsx
 src/components/PaginationComponent.tsx
 src/components/SideButton.ts
 src/components/UnicoreJobsTable.tsx
 src/components/UnicoreSites.tsx
@@ -48,17 +50,17 @@
 tvb_ext_unicore.egg-info/top_level.txt
 tvbextunicore/__init__.py
 tvbextunicore/_version.py
 tvbextunicore/exceptions.py
 tvbextunicore/handlers.py
 tvbextunicore/utils.py
 tvbextunicore/labextension/package.json
-tvbextunicore/labextension/static/488.0f8ad58095bf1360be6b.js
 tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js
-tvbextunicore/labextension/static/remoteEntry.10457d0adbf3941a60bb.js
+tvbextunicore/labextension/static/774.f5b7ad80ab759770978c.js
+tvbextunicore/labextension/static/remoteEntry.c6b3242597cbbe03a95e.js
 tvbextunicore/labextension/static/style.js
 tvbextunicore/labextension/static/third-party-licenses.json
 tvbextunicore/logger/__init__.py
 tvbextunicore/logger/builder.py
 tvbextunicore/logger/logging.conf
 tvbextunicore/tests/__init__.py
 tvbextunicore/tests/test_unicore_wrapper.py
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/__init__.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/_version.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/_version.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/exceptions.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/handlers.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 LOGGER = get_logger(__name__)
 
 
 class SitesHandler(APIHandler):
     @tornado.web.authenticated
     def get(self):
-        LOGGER.info(f"Retrieving sites...")
+        LOGGER.info("Retrieving sites...")
         message = ''
         try:
             sites = UnicoreWrapper().get_sites()
         except SitesDownException as e:
             sites = list()
             message = e.message
         self.finish(json.dumps({'sites': sites, 'message': message}))
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/labextension/package.json` & `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c6b3242597cbbe03a95e.js'}}",*

 * * "'version'": "'1.2.0'"}*

```diff
@@ -48,15 +48,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.10457d0adbf3941a60bb.js",
+            "load": "static/remoteEntry.c6b3242597cbbe03a95e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "tvb-ext-unicore"
                 },
@@ -105,9 +105,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.2.0"
 }
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/488.0f8ad58095bf1360be6b.js` & `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/774.f5b7ad80ab759770978c.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,381 +1,383 @@
 "use strict";
 (self.webpackChunktvb_ext_unicore = self.webpackChunktvb_ext_unicore || []).push([
-    [488], {
-        488: (e, t, s) => {
-            s.r(t), s.d(t, {
+    [774], {
+        774: (e, t, a) => {
+            a.r(t), a.d(t, {
                 default: () => P
             });
-            var a = s(866),
-                n = s(510),
-                i = s(535),
-                r = s(767),
-                o = s(271),
-                l = s.n(o),
-                c = s(694),
-                d = s(526),
-                u = s(886),
-                g = s(258);
-            async function m(e = "", t = {}) {
-                const s = g.ServerConnection.makeSettings(),
-                    a = u.URLExt.join(s.baseUrl, "tvbextunicore", e);
+            var s = a(638),
+                n = a(303);
+            const i = "NONE",
+                r = "text/plain";
+
+            function o(e) {
+                return `from tvbextunicore.unicore_wrapper import unicore_wrapper\nunicore = unicore_wrapper.UnicoreWrapper()\njob = unicore.get_job('${e}')\njob`
+            }
+            var l = a(122),
+                c = a(127),
+                d = a(271),
+                u = a.n(d),
+                g = a(694),
+                m = a(526),
+                h = a(344),
+                b = a(139);
+            async function p(e = "", t = {}) {
+                const a = b.ServerConnection.makeSettings(),
+                    s = h.URLExt.join(a.baseUrl, "tvbextunicore", e);
                 let n;
-                console.log("req URL: ", a);
+                console.log("req URL: ", s);
                 try {
-                    n = await g.ServerConnection.makeRequest(a, t, s)
+                    n = await b.ServerConnection.makeRequest(s, t, a)
                 } catch (e) {
-                    throw new g.ServerConnection.NetworkError(e)
+                    throw new b.ServerConnection.NetworkError(e)
                 }
                 let i = await n.text();
                 if (i.length > 0) try {
                     i = JSON.parse(i)
                 } catch (e) {
                     console.log("Not a JSON response body.", n)
                 }
-                if (!n.ok) throw new g.ServerConnection.ResponseError(n, i.message || i);
+                if (!n.ok) throw new b.ServerConnection.ResponseError(n, i.message || i);
                 return i
             }
-            const h = "NONE",
-                b = "text/plain";
-
-            function p(e) {
-                return `from tvbextunicore.unicore_wrapper import unicore_wrapper\nunicore = unicore_wrapper.UnicoreWrapper()\njob = unicore.get_job('${e}')\njob`
-            }
-            var S = s(918);
+            var S = a(918);
             const E = e => {
-                    const [t, s] = (0, o.useState)(null), [a, n] = (0, o.useState)("");
-                    return (0, o.useEffect)((() => {
-                        m(`job_output?job_url=${encodeURIComponent(e.job_url)}`).then((e => s(e))).catch((e => {
+                    const [t, a] = (0, d.useState)(null), [s, n] = (0, d.useState)("");
+                    return (0, d.useEffect)((() => {
+                        p(`job_output?job_url=${encodeURIComponent(e.job_url)}`).then((e => a(e))).catch((e => {
                             console.log("err: ", e), n(e.message)
                         }))
-                    }), []), l().createElement("tr", {
+                    }), []), u().createElement("tr", {
                         className: "outputFiles",
                         "data-testid": `output-${e.job_url}`
-                    }, t ? l().createElement("td", {
+                    }, t ? u().createElement("td", {
                         colSpan: 100
-                    }, l().createElement("p", {
+                    }, u().createElement("p", {
                         className: "unicoreMessage"
-                    }, a), "Output Files:", Object.entries(t).map((([t, s], a) => l().createElement(w, {
+                    }, s), "Output Files:", Object.entries(t).map((([t, a]) => u().createElement(w, {
                         output: t,
-                        outputType: s,
-                        key: `${t}-${a}`,
+                        outputType: a,
+                        key: `${t}`,
                         jobUrl: e.job_url,
                         jobId: e.jobId,
                         getFileBrowser: e.getFileBrowser,
                         getKernel: e.getKernel
-                    })))) : l().createElement("td", {
+                    })))) : u().createElement("td", {
                         colSpan: 100
-                    }, a ? l().createElement("p", {
+                    }, s ? u().createElement("p", {
                         className: "unicoreMessage"
-                    }, a) : l().createElement("div", {
+                    }, s) : u().createElement("div", {
                         className: "loadingRoot"
-                    }, l().createElement("span", {
+                    }, u().createElement("span", {
                         className: "unicoreLoading"
                     }))))
                 },
                 w = e => {
                     const {
                         output: t,
-                        outputType: s,
-                        jobUrl: a,
+                        outputType: a,
+                        jobUrl: s,
                         getFileBrowser: i,
-                        jobId: r
-                    } = e, [u, g] = (0, o.useState)(!1), h = {
+                        jobId: o
+                    } = e, [l, c] = (0, d.useState)(!1), h = {
                         success: "unicoreMessage-success",
                         warning: "unicoreMessage-warning",
                         error: "unicoreMessage"
-                    }, [p, E] = (0, o.useState)({
+                    }, [b, E] = (0, d.useState)({
                         text: "",
                         className: h.success
                     });
                     let w;
                     async function f(e) {
                         let t = e = e.replace("/", "");
-                        if (["stdout", "stderr", "UNICORE_SCRIPT_EXIT_CODE"].includes(t) && (t = `${e}_${r}`), function(e) {
+                        if (["stdout", "stderr", "UNICORE_SCRIPT_EXIT_CODE"].includes(t) && (t = `${e}_${o}`), function(e) {
                                 const t = i().model.items();
-                                return (0, S.some)(t, ((t, s) => t.name === e))
+                                return (0, S.some)(t, ((t, a) => t.name === e))
                             }(t) && !await async function(e) {
                                 return (await (0, n.showDialog)({
                                     title: "File already exists!",
                                     body: `If you continue the file ${e}} will be re downloaded and overwritten!`,
                                     buttons: [n.Dialog.cancelButton({
                                         label: "Cancel"
                                     }), n.Dialog.okButton({
                                         label: "Continue"
                                     })]
                                 })).button.accept
                             }(t)) return;
-                        const s = i(),
-                            o = s.model.path;
-                        console.log("File browser path: ", o);
+                        const a = i(),
+                            r = a.model.path;
+                        console.log("File browser path: ", r);
                         const l = {
-                            job_url: a,
+                            job_url: s,
                             in_file: e,
-                            path: o,
+                            path: r,
                             out_file: t
                         };
                         try {
-                            g(!0);
-                            const t = await m(`drive/${encodeURIComponent(a)}/${e}`, {
+                            c(!0);
+                            const t = await p(`drive/${encodeURIComponent(s)}/${e}`, {
                                 method: "POST",
                                 body: JSON.stringify(l)
                             });
                             console.log("response: ", t), E({
                                 text: t.message,
                                 className: h[t.status]
-                            }), g(!1), s.update()
+                            }), c(!1), a.update()
                         } catch (e) {
                             await (0, n.showErrorMessage)("Error on request:", e), E({
                                 text: e.text,
                                 className: h.error
-                            }), g(!1)
+                            }), c(!1)
                         }
                     }
                     async function v(e) {
                         await f(t), j()
                     }
 
                     function j() {
                         i().node.removeEventListener("drop", v), null == w || w.dispose()
                     }
-                    return l().createElement("div", {
+                    return u().createElement("div", {
                         className: "unicore-jobOutput",
                         "data-testid": `output-${t}`
-                    }, s.is_file ? l().createElement("i", {
+                    }, a.is_file ? u().createElement("i", {
                         className: "fa fa-file"
-                    }) : l().createElement("i", {
+                    }) : u().createElement("i", {
                         className: "fas fa-folder"
-                    }), l().createElement("p", {
+                    }), u().createElement("p", {
                         draggable: !0,
                         className: "outputFileName",
                         onDragStart: async function(e) {
                             i().node.addEventListener("drop", v);
-                            const s = `from tvbextunicore.unicore_wrapper import unicore_wrapper\nunicore = unicore_wrapper.UnicoreWrapper()\ndownload_result = unicore.download_file('${a}', '${t}')\ndownload_result`;
-                            w = new c.Drag({
-                                mimeData: new d.MimeData,
+                            const a = `from tvbextunicore.unicore_wrapper import unicore_wrapper\nunicore = unicore_wrapper.UnicoreWrapper()\ndownload_result = unicore.download_file('${s}', '${t}')\ndownload_result`;
+                            w = new g.Drag({
+                                mimeData: new m.MimeData,
                                 supportedActions: "copy",
                                 proposedAction: "copy",
                                 source: t
-                            }), w.mimeData.setData(b, s), w.start(e.clientX, e.clientY).then((e => {
+                            }), w.mimeData.setData(r, a), w.start(e.clientX, e.clientY).then((e => {
                                 console.log("r: ", e), j()
                             }))
                         }
-                    }, t), s && l().createElement(l().Fragment, null, l().createElement("span", {
-                        className: p.className
-                    }, p.text), u ? l().createElement("div", {
+                    }, t), a && u().createElement(u().Fragment, null, u().createElement("span", {
+                        className: b.className
+                    }, b.text), l ? u().createElement("div", {
                         className: "loadingRoot"
-                    }, l().createElement("span", {
+                    }, u().createElement("span", {
                         className: "unicoreLoading"
-                    })) : l().createElement("i", {
+                    })) : u().createElement("i", {
                         "data-testid": "download-file",
                         className: "fa fa-download clickableIcon",
                         onClick: () => f(t)
                     })))
                 },
-                f = e => l().createElement("table", null, l().createElement(v, {
+                f = e => u().createElement("table", null, u().createElement(v, {
                     columns: e.columns
-                }), l().createElement(j, {
+                }), u().createElement(j, {
                     buttonSettings: e.buttonSettings,
                     columns: e.columns,
                     data: e.data,
                     setMessageState: e.setMessageState,
                     getKernel: e.getKernel,
                     getJob: e.getJob,
                     handleError: e.handleError,
                     getFileBrowser: e.getFileBrowser,
                     afterButtonSettingClick: e.afterButtonSettingClick
                 })),
-                v = e => l().createElement("thead", null, l().createElement("tr", null, e.columns.map((e => l().createElement("td", {
+                v = e => u().createElement("thead", null, u().createElement("tr", null, e.columns.map((e => u().createElement("td", {
                     key: e,
                     className: e
-                }, e.toUpperCase()))), l().createElement("td", null, "ACTIONS"))),
-                j = e => l().createElement("tbody", null, e.data.map((t => l().createElement(C, {
+                }, e.toUpperCase()))), u().createElement("td", null, "ACTIONS"))),
+                j = e => u().createElement("tbody", null, e.data.map((t => u().createElement(C, {
                     key: t.id,
                     id: t.id,
                     cols: e.columns,
                     job: t,
                     buttonSettings: e.buttonSettings,
                     setMessageState: e.setMessageState,
                     getKernel: e.getKernel,
                     getJob: e.getJob,
                     handleError: e.handleError,
                     getFileBrowser: e.getFileBrowser,
                     afterButtonSettingClick: e.afterButtonSettingClick
                 })))),
                 C = e => {
-                    const [t, s] = (0, o.useState)(!1), [a, n] = (0, o.useState)(!1);
-                    return l().createElement(l().Fragment, null, l().createElement("tr", {
-                        onClick: () => n(!a),
+                    const [t, a] = (0, d.useState)(!1), [s, n] = (0, d.useState)(!1);
+                    return u().createElement(u().Fragment, null, u().createElement("tr", {
+                        onClick: () => n(!s),
                         draggable: "true",
                         onDragStart: async function(t) {
-                            var s;
+                            var a;
                             if (!await e.getKernel()) return void e.handleError("Current kernel can't be used to handle this operation!");
-                            const a = e.getJob(e.job.resource_url),
-                                n = new c.Drag({
-                                    mimeData: new d.MimeData,
+                            const s = e.getJob(e.job.resource_url),
+                                n = new g.Drag({
+                                    mimeData: new m.MimeData,
                                     supportedActions: "copy",
                                     proposedAction: "copy",
-                                    dragImage: null === (s = document.getElementById(`${e.job.id}`)) || void 0 === s ? void 0 : s.cloneNode(!0),
+                                    dragImage: null === (a = document.getElementById(`${e.job.id}`)) || void 0 === a ? void 0 : a.cloneNode(!0),
                                     source: e.job
                                 });
-                            n.mimeData.setData(b, a), n.start(t.clientX, t.clientY).then((e => console.log("r: ", e)))
+                            n.mimeData.setData(r, s), n.start(t.clientX, t.clientY).then((e => console.log("r: ", e)))
                         },
                         "data-testid": `table-row-${e.job.id}`
-                    }, e.cols.map(((t, s) => l().createElement("td", {
-                        key: `${e.job.id}-${s}`
-                    }, e.job[t]))), t ? l().createElement("td", null, l().createElement("div", {
+                    }, e.cols.map(((t, a) => u().createElement("td", {
+                        key: `${e.job.id}-${a}`
+                    }, e.job[t]))), t ? u().createElement("td", null, u().createElement("div", {
                         className: "loadingRoot"
-                    }, l().createElement("span", {
+                    }, u().createElement("span", {
                         className: "unicoreLoading"
-                    }))) : l().createElement("td", null, e.job.is_cancelable && !t && l().createElement("button", {
+                    }))) : u().createElement("td", null, e.job.is_cancelable && !t && u().createElement("button", {
                         onClick: function(t) {
-                            t.stopPropagation(), s(!0), e.buttonSettings.onClick(...e.buttonSettings.onClickFieldArgs.map((t => e.job[t]))).then((t => {
-                                e.afterButtonSettingClick().then((() => s(!1))), e.setMessageState(t.message)
+                            t.stopPropagation(), a(!0), e.buttonSettings.onClick(...e.buttonSettings.onClickFieldArgs.map((t => e.job[t]))).then((t => {
+                                e.afterButtonSettingClick().then((() => a(!1))), e.setMessageState(t.message)
                             }))
                         }
-                    }, "Cancel Job"))), a && l().createElement(l().Fragment, null, l().createElement(E, {
+                    }, "Cancel Job"))), s && u().createElement(u().Fragment, null, u().createElement(E, {
                         job_url: e.job.resource_url,
                         getFileBrowser: e.getFileBrowser,
                         getKernel: e.getKernel,
                         jobId: e.job.id
-                    }), l().createElement("tr", {
+                    }), u().createElement("tr", {
                         className: "detailsRow"
-                    }, l().createElement("td", {
+                    }, u().createElement("td", {
                         colSpan: 100
-                    }, l().createElement("textarea", {
+                    }, u().createElement("textarea", {
                         value: e.job.logs.join("\n"),
                         readOnly: !0
                     })))))
                 },
-                y = e => l().createElement("div", {
+                y = e => u().createElement("div", {
                     className: "unicorePagination",
                     "data-testid": "pagination-component"
-                }, l().createElement("div", null, l().createElement("div", {
+                }, u().createElement("div", null, u().createElement("div", {
                     className: "btnLeftContainer"
-                }, e.showPrevButton && l().createElement("button", {
+                }, e.showPrevButton && u().createElement("button", {
                     onClick: function() {
                         e.setPageState(e.currentPage - 1)
                     },
                     "data-testid": "p-btn-left"
-                }, l().createElement("i", {
+                }, u().createElement("i", {
                     className: "fa fa-arrow-left"
-                }))), l().createElement("div", {
+                }))), u().createElement("div", {
                     className: "currentPageContainer"
-                }, l().createElement("span", null, `Page: ${e.currentPage}`)), l().createElement("div", {
+                }, u().createElement("span", null, `Page: ${e.currentPage}`)), u().createElement("div", {
                     className: "btnRightContainer"
-                }, e.showNextButton && l().createElement("button", {
+                }, e.showNextButton && u().createElement("button", {
                     onClick: function() {
                         e.setPageState(e.currentPage + 1)
                     },
                     "data-testid": "p-btn-right"
-                }, l().createElement("i", {
+                }, u().createElement("i", {
                     className: "fa fa-arrow-right"
                 })))));
 
-            function k({
+            function R({
                 onToggle: e,
                 initialCheckedState: t,
-                label: s
+                label: a
             }) {
-                const [a, n] = (0, o.useState)(t);
-                return l().createElement("div", null, l().createElement("input", {
+                const [s, n] = (0, d.useState)(t);
+                return u().createElement("div", null, u().createElement("input", {
                     id: "auto-refresh",
                     type: "checkbox",
-                    checked: a,
+                    checked: s,
                     onChange: t => {
                         n(t.target.checked), e(t.target.checked)
                     }
-                }), s && l().createElement("label", {
+                }), a && u().createElement("label", {
                     htmlFor: "auto-refresh"
-                }, s))
+                }, a))
             }
-            const N = e => {
-                const [t, s] = (0, o.useState)(!1);
-                return l().createElement("div", {
+            const k = e => {
+                const [t, a] = (0, d.useState)(!1);
+                return u().createElement("div", {
                     className: "pyunicoreSites",
                     "data-testid": "pyunicore-sites"
-                }, l().createElement("div", null, l().createElement("span", null, "SITE:"), l().createElement("select", {
+                }, u().createElement("div", null, u().createElement("span", null, "SITE:"), u().createElement("select", {
                     onChange: function(t) {
                         e.onChangeSite(t.target.value)
                     },
                     disabled: e.disableSelection,
-                    "data-testid": "select"
-                }, e.sites.map((e => l().createElement("option", {
+                    "data-testid": "select",
+                    defaultValue: e.defaultSite
+                }, e.sites.map((e => u().createElement("option", {
                     key: e,
                     id: e,
                     value: e
-                }, e))))), l().createElement("button", {
+                }, e))))), u().createElement("button", {
                     className: `refreshBtn ${t&&"spin"}`,
                     onClick: () => {
-                        s(!0), setTimeout((() => s(!1)), 500), e.refreshSite()
+                        a(!0), setTimeout((() => a(!1)), 500), e.refreshSite()
                     },
                     disabled: e.loading
-                }, l().createElement("i", {
+                }, u().createElement("i", {
                     className: "fa fa-refresh"
-                })), l().createElement(k, {
+                })), u().createElement(R, {
                     onToggle: e.setAutoReload,
                     initialCheckedState: !0,
                     label: "Auto refresh"
                 }))
             };
-            var _;
+            var N;
             ! function(e) {
                 e.Warning = "WARNING", e.Error = "ERROR", e.Success = "SUCCESS", e.Confirm = "CONFIRM"
-            }(_ || (_ = {}));
-            const O = e => l().createElement("div", {
+            }(N || (N = {}));
+            const O = e => u().createElement("div", {
                 className: "unicoreModal",
                 style: {
                     display: e.visible ? "flex" : "none"
                 },
                 "data-testid": "modal-widget"
-            }, l().createElement("div", null, l().createElement("div", null, l().createElement("h3", null, e.modalType)), l().createElement("div", null, l().createElement("p", null, String(e.message))), l().createElement("div", null, l().createElement("button", {
+            }, u().createElement("div", null, u().createElement("div", null, u().createElement("h3", null, e.modalType)), u().createElement("div", null, u().createElement("p", null, String(e.message))), u().createElement("div", null, u().createElement("button", {
                 onClick: () => e.setVisible(!1)
             }, "CLOSE"))));
-            class R extends n.ReactWidget {
+            class _ extends n.ReactWidget {
                 constructor(e) {
                     super(), this.addClass("tvb-pyunicoreWidget"), this.props = e
                 }
                 render() {
-                    return l().createElement(x, {
+                    return u().createElement(x, {
                         tableFormat: this.props.tableFormat,
                         data: this.props.data,
                         buttonSettings: this.props.buttonSettings,
                         sites: this.props.sites,
+                        defaultSite: this.props.defaultSite,
                         reloadRate: 6e4,
                         getKernel: this.props.getKernel,
                         getJobCode: this.props.getJobCode,
                         getFileBrowser: this.props.getFileBrowser
                     })
                 }
             }
-            class x extends l().Component {
+            class x extends u().Component {
                 constructor(e) {
                     super(e), this._triggerUpdate = (e = !1) => {
-                        this.state.site !== h && (e || this.state.autoReload && (new Date).valueOf() - this.state.lastUpdate.valueOf() >= this.state.reloadRate && !this.state.loading) && this.setState(Object.assign(Object.assign({}, this.state), {
+                        this.state.site !== i && (e || this.state.autoReload && (new Date).valueOf() - this.state.lastUpdate.valueOf() >= this.state.reloadRate && !this.state.loading) && this.setState(Object.assign(Object.assign({}, this.state), {
                             isRefresh: !0
                         }))
                     }, this.setPageState = this.setPageState.bind(this), this.setSiteState = this.setSiteState.bind(this), this.setModalSateVisible = this.setModalSateVisible.bind(this), this.getData = this.getData.bind(this), this.catchError = this.catchError.bind(this), this.setAutoReload = this.setAutoReload.bind(this);
                     const t = new Date;
                     this.state = {
                         jobs: [],
                         message: e.data.message,
-                        site: e.sites[0],
+                        site: e.defaultSite,
                         buttonSettings: e.buttonSettings,
                         tableFormat: e.tableFormat,
                         reloadRate: 6e4,
                         loading: e.sites.length > 0,
                         sites: e.sites,
                         page: 1,
                         itemsPerPage: 10,
                         lastUpdate: t,
                         renderLeftArrow: !1,
                         renderRightArrow: !1,
                         disableSitesSelection: !0,
                         modalState: {
-                            modalType: _.Error,
+                            modalType: N.Error,
                             message: "",
                             visible: !1,
                             setVisible: this.setModalSateVisible
                         },
                         autoReload: !0,
                         isRefresh: !1,
                         updateIntervalId: 0
@@ -387,15 +389,15 @@
                 async getData() {
                     this.setState(Object.assign(Object.assign({}, this.state), {
                         loading: !0,
                         renderLeftArrow: !1,
                         renderRightArrow: !1,
                         disableSitesSelection: !0
                     }));
-                    const e = await m(this._getEndpoint());
+                    const e = await p(this._getEndpoint());
                     return this.setState(Object.assign(Object.assign({}, this.state), {
                         jobs: e.jobs,
                         message: e.message,
                         loading: !1,
                         lastUpdate: new Date,
                         renderLeftArrow: this.state.page > 1,
                         renderRightArrow: e.jobs.length >= this.state.itemsPerPage,
@@ -417,28 +419,28 @@
                         modalState: Object.assign(Object.assign({}, this.state.modalState), {
                             visible: e
                         })
                     }))
                 }
                 setSiteState(e) {
                     let t = this.state.jobs;
-                    e === h && (t = []), this.setState(Object.assign(Object.assign({}, this.state), {
+                    e === i && (t = []), this.setState(Object.assign(Object.assign({}, this.state), {
                         page: 1,
                         site: e,
                         jobs: t
                     }))
                 }
                 setAutoReload(e) {
                     this.setState(Object.assign(Object.assign({}, this.state), {
                         autoReload: e
                     }))
                 }
                 componentDidUpdate(e, t) {
                     if ((this.state.isRefresh && !t.isRefresh || t.page !== this.state.page || t.site !== this.state.site) && this.state.sites.length > 0) {
-                        if (this.state.site === h) return void this.setState(Object.assign(Object.assign({}, this.state), {
+                        if (this.state.site === i) return void this.setState(Object.assign(Object.assign({}, this.state), {
                             loading: !1,
                             disableSitesSelection: !1,
                             jobs: [],
                             renderLeftArrow: !1,
                             renderRightArrow: !1,
                             isRefresh: !1
                         }));
@@ -456,48 +458,49 @@
                 componentWillUnmount() {
                     clearInterval(this.state.updateIntervalId)
                 }
                 componentDidMount() {
                     const e = setInterval(this._triggerUpdate, 1e4);
                     this.setState(Object.assign(Object.assign({}, this.state), {
                         updateIntervalId: e
-                    })), this.state.site !== h ? this.state.sites.length <= 0 || this.getData().catch(this.catchError) : this.setState(Object.assign(Object.assign({}, this.state), {
+                    })), this.state.site !== i ? this.state.sites.length <= 0 || this.getData().catch(this.catchError) : this.setState(Object.assign(Object.assign({}, this.state), {
                         loading: !1,
                         disableSitesSelection: !1
                     }))
                 }
                 render() {
-                    return l().createElement(l().Fragment, null, l().createElement(O, {
+                    return u().createElement(u().Fragment, null, u().createElement(O, {
                         modalType: this.state.modalState.modalType,
                         message: this.state.modalState.message,
                         visible: this.state.modalState.visible,
                         setVisible: this.state.modalState.setVisible
-                    }), l().createElement("div", {
+                    }), u().createElement("div", {
                         className: "unicoreTopBar"
-                    }, l().createElement(y, {
+                    }, u().createElement(y, {
                         setPageState: this.setPageState,
                         showNextButton: this.state.renderRightArrow,
                         showPrevButton: this.state.renderLeftArrow,
                         currentPage: this.state.page
-                    }), l().createElement(N, {
+                    }), u().createElement(k, {
                         sites: this.state.sites,
                         onChangeSite: this.setSiteState,
+                        defaultSite: this.state.site,
                         disableSelection: this.state.disableSitesSelection,
                         refreshSite: () => this._triggerUpdate(!0),
                         loading: this.state.loading,
                         setAutoReload: this.setAutoReload
-                    }), this.state.loading ? l().createElement("div", null, l().createElement("div", {
+                    }), this.state.loading ? u().createElement("div", null, u().createElement("div", {
                         className: "loadingRoot"
-                    }, l().createElement("span", {
+                    }, u().createElement("span", {
                         className: "unicoreLoading"
-                    }))) : l().createElement("div", null, l().createElement("span", {
+                    }))) : u().createElement("div", null, u().createElement("span", {
                         className: "unicoreMessage"
-                    }, this.state.message), l().createElement("span", {
+                    }, this.state.message), u().createElement("span", {
                         className: "lastUpdate"
-                    }, "Last update: ", this.state.lastUpdate.toLocaleTimeString()))), l().createElement(f, {
+                    }, "Last update: ", this.state.lastUpdate.toLocaleTimeString()))), u().createElement(f, {
                         buttonSettings: this.state.buttonSettings,
                         afterButtonSettingClick: this.getData,
                         columns: this.state.tableFormat.cols,
                         data: this.state.jobs,
                         setMessageState: e => {
                             this.setState(Object.assign(Object.assign({}, this.state), {
                                 message: e
@@ -506,129 +509,139 @@
                         getKernel: this.props.getKernel,
                         getJob: this.props.getJobCode,
                         handleError: this.catchError,
                         getFileBrowser: this.props.getFileBrowser
                     }))
                 }
             }
-            var F = s(468),
-                B = s(431);
-            class I extends B.Widget {
+            var F = a(543),
+                I = a(832);
+            class B extends I.Widget {
                 constructor(e) {
                     super(e), this._labShell = e.labShell, this._command = e.command, this._commands = e.commandRegistry, this._area = e.area, this._shellOptions = e.shellOptions, this.title.icon = e.icon, this.title.caption = e.caption, this.id = e.id ? e.id : "tvb-ext-unicore-side-btn", this.title.className = this.id
                 }
                 addToLabShell() {
                     this._labShell.add(this, this._area, this._shellOptions)
                 }
                 async onAfterShow(e) {
-                    console.log("after show"), super.onAfterShow(e), c.Drag.overrideCursor("wait"), await this._click(), c.Drag.overrideCursor("inherit")
+                    console.log("after show"), super.onAfterShow(e), g.Drag.overrideCursor("wait"), await this._click(), g.Drag.overrideCursor("inherit")
                 }
                 async _click() {
                     switch (this._area) {
                         case "left":
                             this._labShell.collapseLeft();
                             break;
                         case "right":
                             this._labShell.collapseRight()
                     }
                     await this._commands.execute(this._command)
                 }
             }
-            var D = s(591);
+            var D = a(745);
             async function A(e) {
                 const t = {
                     resource_url: e
                 };
-                return m("jobs", {
+                return p("jobs", {
                     method: "POST",
                     body: JSON.stringify(t)
                 })
             }
             const P = {
                 id: "tvbextunicore:plugin",
                 autoStart: !0,
-                requires: [n.ICommandPalette, a.ILayoutRestorer, F.IConsoleTracker, a.ILabShell, r.INotebookTracker, i.IFileBrowserFactory],
-                activate: async (e, t, s, a, i, r, o) => {
-                    let l;
+                requires: [n.ICommandPalette, s.ILayoutRestorer, F.IConsoleTracker, s.ILabShell, c.INotebookTracker, l.IFileBrowserFactory],
+                activate: async (e, t, a, s, r, l, c) => {
+                    let d;
                     console.log("JupyterLab extension tvb-ext-unicore is activated!");
-                    const c = ["id", "name", "owner", "site", "status", "start_time"],
-                        d = "tvbextunicore:open";
-                    e.commands.addCommand(d, {
+                    const u = ["id", "name", "owner", "site", "status", "start_time"],
+                        g = "tvbextunicore:open";
+                    e.commands.addCommand(g, {
                         label: "PyUnicore Task Stream",
-                        execute: async () => {
-                            if (!l || l.isDisposed) {
-                                const e = await m("sites"),
-                                    t = new R({
-                                        tableFormat: {
-                                            cols: c,
-                                            idField: "id",
-                                            buttonRenderConditionField: "is_cancelable"
-                                        },
-                                        data: {
-                                            message: e.message,
-                                            jobs: []
-                                        },
-                                        buttonSettings: {
-                                            onClick: A,
-                                            onClickFieldArgs: ["resource_url"],
-                                            isAsync: !1,
-                                            name: "Cancel Job"
-                                        },
-                                        sites: [h, ...Object.keys(e.sites)],
-                                        reloadRate: 6e4,
-                                        getKernel: async () => {
-                                            const e = T.getCurrentKernel(i, r, a);
-                                            return await T.shouldUseKernel(e) ? e : null
-                                        },
-                                        getJobCode: p,
-                                        getFileBrowser: () => T.getFileBrowser(o)
-                                    });
-                                l = new n.MainAreaWidget({
-                                    content: t
-                                }), l.id = "tvbextunicore", l.title.label = "PyUnicore Task Stream", l.title.closable = !0
+                        execute: async (t = {
+                            defaultSite: i
+                        }) => {
+                            if (!d || d.isDisposed) {
+                                let e, a, g = [];
+                                try {
+                                    e = await p("sites"), g = [...Object.keys(e.sites)], a = function(e, t) {
+                                        return e !== i && null != e ? t.includes(e) ? e : ((0, n.showErrorMessage)("SITE ERROR", `Site ${e} is not available at this time! Available sites: ${t}`), i) : i
+                                    }(t.defaultSite, g)
+                                } catch (e) {
+                                    return void await (0, n.showErrorMessage)("ERROR", "Unicore seems to be down at the moment. Please check service availability and try again later.")
+                                }
+                                const m = new _({
+                                    tableFormat: {
+                                        cols: u,
+                                        idField: "id",
+                                        buttonRenderConditionField: "is_cancelable"
+                                    },
+                                    data: {
+                                        message: e.message,
+                                        jobs: []
+                                    },
+                                    buttonSettings: {
+                                        onClick: A,
+                                        onClickFieldArgs: ["resource_url"],
+                                        isAsync: !1,
+                                        name: "Cancel Job"
+                                    },
+                                    sites: [i, ...g],
+                                    defaultSite: a,
+                                    reloadRate: 6e4,
+                                    getKernel: async () => {
+                                        const e = T.getCurrentKernel(r, l, s);
+                                        return await T.shouldUseKernel(e) ? e : null
+                                    },
+                                    getJobCode: o,
+                                    getFileBrowser: () => T.getFileBrowser(c)
+                                });
+                                d = new n.MainAreaWidget({
+                                    content: m
+                                }), d.id = "tvbextunicore", d.title.label = "PyUnicore Task Stream", d.title.closable = !0
                             }
-                            u.has(l) || u.add(l), l.isAttached || e.shell.add(l, "main"), e.shell.activateById(l.id)
+                            m.has(d) || m.add(d), d.isAttached || e.shell.add(d, "main"), e.shell.activateById(d.id)
                         }
                     }), t.addItem({
-                        command: d,
+                        command: g,
                         category: "PyUnicore"
                     });
-                    const u = new n.WidgetTracker({
+                    const m = new n.WidgetTracker({
                             namespace: "pyunicore"
                         }),
-                        g = new D.LabIcon({
+                        h = new D.LabIcon({
                             name: "unicoreIcon",
                             svgstr: '<?xml version="1.0" standalone="no"?>\n<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 20010904//EN"\n "http://www.w3.org/TR/2001/REC-SVG-20010904/DTD/svg10.dtd">\n<svg version="1.0" xmlns="http://www.w3.org/2000/svg"\n width="37.000000pt" height="45.000000pt" viewBox="0 0 37.000000 45.000000"\n preserveAspectRatio="xMidYMid meet">\n\n<g transform="translate(7.000000,35.000000) scale(0.0700000,-0.0700000)"\nfill="#616161" stroke="none">\n<path d="M2 373 c3 -144 6 -173 22 -200 28 -46 83 -73 148 -73 72 0 117 25\n145 80 21 40 23 58 23 202 l0 158 -40 0 -40 0 0 -160 c0 -157 -1 -161 -25\n-185 -17 -18 -35 -25 -62 -25 -80 1 -93 31 -93 219 l0 151 -41 0 -41 0 4 -167z"/>\n<path d="M10 25 l0 -25 165 0 165 0 0 25 0 25 -165 0 -165 0 0 -25z"/>\n</g>\n</svg>\n'
                         });
-                    new I({
-                        command: d,
+                    new B({
+                        command: g,
                         commandRegistry: e.commands,
-                        labShell: i,
+                        labShell: r,
                         caption: "PyUnicore Tasks Stream",
-                        icon: g,
+                        icon: h,
                         area: "right",
                         shellOptions: {
                             rank: 10
                         }
-                    }).addToLabShell(), s.restore(u, {
-                        command: d,
+                    }).addToLabShell(), a.restore(m, {
+                        command: g,
                         name: () => "pyunicore"
                     })
                 }
             };
             var T;
             ! function(e) {
                 e.shouldUseKernel = async function(e) {
                     if (!e) return !1;
                     const t = await e.spec;
                     return !!t && -1 !== t.language.toLowerCase().indexOf("python")
-                }, e.getCurrentKernel = function(e, t, s) {
-                    var a, n, i, r;
+                }, e.getCurrentKernel = function(e, t, a) {
+                    var s, n, i, r;
                     let o, l = e.currentWidget;
-                    return l && t.has(l) ? o = null === (a = l.sessionContext.session) || void 0 === a ? void 0 : a.kernel : l && s.has(l) ? o = null === (n = l.sessionContext.session) || void 0 === n ? void 0 : n.kernel : t.currentWidget ? (l = t.currentWidget, o = null === (i = l.sessionContext.session) || void 0 === i ? void 0 : i.kernel) : s.currentWidget && (l = s.currentWidget, o = null === (r = l.sessionContext.session) || void 0 === r ? void 0 : r.kernel), o
+                    return l && t.has(l) ? o = null === (s = l.sessionContext.session) || void 0 === s ? void 0 : s.kernel : l && a.has(l) ? o = null === (n = l.sessionContext.session) || void 0 === n ? void 0 : n.kernel : t.currentWidget ? (l = t.currentWidget, o = null === (i = l.sessionContext.session) || void 0 === i ? void 0 : i.kernel) : a.currentWidget && (l = a.currentWidget, o = null === (r = l.sessionContext.session) || void 0 === r ? void 0 : r.kernel), o
                 }, e.getFileBrowser = function(e) {
                     return e.defaultBrowser
                 }
             }(T || (T = {}))
         }
     }
 ]);
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js` & `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/747.c26c9bf4f7bddc1ea1c7.js`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/remoteEntry.10457d0adbf3941a60bb.js` & `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/remoteEntry.c6b3242597cbbe03a95e.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, f, d, s, c, p, h, v = {
             675: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(488).then((() => () => t(488))),
-                        "./extension": () => t.e(488).then((() => () => t(488))),
+                        "./index": () => t.e(774).then((() => () => t(774))),
+                        "./extension": () => t.e(774).then((() => () => t(774))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,49 +43,49 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        488: "0f8ad58095bf1360be6b",
-        747: "c26c9bf4f7bddc1ea1c7"
+        747: "c26c9bf4f7bddc1ea1c7",
+        774: "f5b7ad80ab759770978c"
     } [e] + ".js?v=" + {
-        488: "0f8ad58095bf1360be6b",
-        747: "c26c9bf4f7bddc1ea1c7"
+        747: "c26c9bf4f7bddc1ea1c7",
+        774: "f5b7ad80ab759770978c"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "tvb-ext-unicore:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                    var d = l[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var s = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -102,19 +102,19 @@
                 var a = g.S[t],
                     i = "tvb-ext-unicore",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => g.e(488).then((() => () => g(488))),
+                        get: () => g.e(774).then((() => () => g(774))),
                         from: i,
                         eager: !1
                     })
-                })("tvb-ext-unicore", "1.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("tvb-ext-unicore", "1.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -163,87 +163,87 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == s) {
-                    if (!l || "u" != d) return !1
+                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
+                if ("u" == d) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (d == s)
+                    if (s == d)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (o ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != s && "n" != s) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
+                    if (u <= n || d < s != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = g.S[e];
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
+    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
-        258: () => d("default", "@jupyterlab/services", [1, 6, 6, 1]),
-        271: () => d("default", "react", [1, 17, 0, 1]),
-        431: () => d("default", "@lumino/widgets", [1, 1, 37, 1]),
-        468: () => d("default", "@jupyterlab/console", [1, 3, 6, 1]),
-        510: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        526: () => d("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        535: () => d("default", "@jupyterlab/filebrowser", [1, 3, 6, 1]),
-        591: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        694: () => d("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        767: () => d("default", "@jupyterlab/notebook", [1, 3, 6, 1]),
-        866: () => d("default", "@jupyterlab/application", [1, 3, 6, 1]),
-        886: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 1]),
-        918: () => d("default", "@lumino/algorithm", [1, 1, 9, 0])
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, p = {
+        122: () => s("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        127: () => s("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
+        139: () => s("default", "@jupyterlab/services", [1, 6, 6, 5]),
+        271: () => s("default", "react", [1, 17, 0, 1]),
+        303: () => s("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        344: () => s("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
+        526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        543: () => s("default", "@jupyterlab/console", [1, 3, 6, 5]),
+        638: () => s("default", "@jupyterlab/application", [1, 3, 6, 5]),
+        694: () => s("default", "@lumino/dragdrop", [1, 1, 13, 0]),
+        745: () => s("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
+        832: () => s("default", "@lumino/widgets", [1, 1, 37, 2]),
+        918: () => s("default", "@lumino/algorithm", [1, 1, 9, 0])
     }, h = {
-        488: [258, 271, 431, 468, 510, 526, 535, 591, 694, 767, 866, 886, 918]
+        774: [122, 127, 139, 271, 303, 344, 526, 543, 638, 694, 745, 832, 918]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
-            if (g.o(p, e)) return r.push(p[e]);
+            if (g.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, g.m[e] = t => {
+                    c[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], g.m[e] = t => {
+                    delete c[e], g.m[e] = t => {
                         throw delete g.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                var o = p[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             899: 0
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/labextension/static/third-party-licenses.json` & `tvb-ext-unicore-1.2.0/tvbextunicore/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/logger/builder.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/logger/logging.conf` & `tvb-ext-unicore-1.2.0/tvbextunicore/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/tests/test_unicore_wrapper.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/tests/test_unicore_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 import json
 import os
 import pytest
 from datetime import datetime
 
 from tvbextunicore.exceptions import TVBExtUnicoreException, SitesDownException, \
     FileNotExistsException, JobRunningException
-from tvbextunicore.unicore_wrapper.unicore_wrapper import UnicoreWrapper
+from tvbextunicore.unicore_wrapper.unicore_wrapper import UnicoreWrapper, DOWNLOAD_MESSAGE
 from tvbextunicore.unicore_wrapper.job_dto import JobDTO, NAME, OWNER, SITE_NAME, STATUS, SUBMISSION_TIME, \
     TERMINATION_TIME, \
     MOUNT_POINT
 from tvbextunicore.utils import build_response, DownloadStatus
 
 GET_JOB = 'tvbextunicore.unicore_wrapper.unicore_wrapper.UnicoreWrapper.get_job'
 SHUTIL_MOVE = 'shutil.move'
-DOWNLOAD_MESSAGE = 'Downloaded successfully!'
 
 
 class MockFilePath:
     def __init__(self, is_file=True):
         self.is_file = is_file
 
     def isfile(self):
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/unicore_wrapper/job_dto.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/job_dto.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/unicore_wrapper/unicore_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from tvbextunicore.exceptions import TVBExtUnicoreException, ClientAuthException, \
     SitesDownException, FileNotExistsException, JobRunningException
 from tvbextunicore.logger.builder import get_logger
 from tvbextunicore.unicore_wrapper.job_dto import JobDTO
 
 LOGGER = get_logger(__name__)
+DOWNLOAD_MESSAGE = 'Downloaded successfully!'
 
 
 class UnicoreWrapper(object):
 
     def __init__(self):
         token = self.__retrieve_token()
         self.transport = self.__build_transport(token)
@@ -148,42 +149,42 @@
     def download_file(self, job_url, file_name, path=None):
         # type: (str, str, str) -> str
         """
         Helper method to download a file from a job output
         """
         job = self.get_job(job_url)
         if job.is_running():
-            raise JobRunningException(f'Cannot download file while the job is still running!')
+            raise JobRunningException('Cannot download file while the job is still running!')
 
         # We need the 'if' below to support download from cell
         if path is None:
             path = file_name
 
         wd = job.working_dir.listdir()
         if not wd.get(file_name, False):
             # Try with folder suffix
             file_name += '/'
             if not wd.get(file_name, False):
                 raise FileNotExistsException(f'{file_name} does not exist as output of {job_url}!')
 
         if isinstance(wd[file_name], unicore_client.PathFile):
             wd[file_name].download(path)
-            return 'Downloaded successfully!'
+            return DOWNLOAD_MESSAGE
 
         # In case the file to download is a directory:
         if not os.path.isdir(path):
             os.mkdir(path)
 
         LOGGER.info(f"Downloading results to {path}...")
         results_content = job.working_dir.listdir(file_name)
 
         for fname, fpath in results_content.items():
             if isinstance(fpath, unicore_client.PathFile):
                 fpath.download(os.path.join(path, os.path.basename(fname)))
-        return 'Downloaded successfully!'
+        return DOWNLOAD_MESSAGE
 
     def stream_file(self, job_url, file, offset=0, size=-1):
         # type: (str, str, int, int) -> stream
         """
         Method to download a file as an octet stream
         """
         job = self.get_job(job_url)
```

### Comparing `tvb-ext-unicore-1.1.0/tvbextunicore/utils.py` & `tvb-ext-unicore-1.2.0/tvbextunicore/utils.py`

 * *Files identical despite different names*

### Comparing `tvb-ext-unicore-1.1.0/yarn.lock` & `tvb-ext-unicore-1.2.0/yarn.lock`

 * *Files identical despite different names*

