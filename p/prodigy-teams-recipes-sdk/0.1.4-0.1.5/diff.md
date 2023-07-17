# Comparing `tmp/prodigy-teams-recipes-sdk-0.1.4.tar.gz` & `tmp/prodigy-teams-recipes-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodigy-teams-recipes-sdk-0.1.4.tar", last modified: Tue Jul 11 17:06:45 2023, max compression
+gzip compressed data, was "prodigy-teams-recipes-sdk-0.1.5.tar", last modified: Mon Jul 17 08:24:15 2023, max compression
```

## Comparing `prodigy-teams-recipes-sdk-0.1.4.tar` & `prodigy-teams-recipes-sdk-0.1.5.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.916122 prodigy-teams-recipes-sdk-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 17:06:45.916122 prodigy-teams-recipes-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19849 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.908122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.912122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/preview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.912122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/200.html
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.912122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/_nuxt/
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.4c35cb5b.css
--rw-r--r--   0 runner    (1001) docker     (123)   200330 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.d4386e81.js
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/recipe_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/recipe_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/teams_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.912122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.916122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/org.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    59908 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.916122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.916122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/0.1.0_2023-05-12-12-39-11_patch_699f4418-3c53-4c0f-8a27-f838383451b1
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/0.1.1_2023-05-17-11-05-43_patch_8e2fe949-3833-4639-84bf-bf1f5bcbe993
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/0.1.2_2023-06-16-09-48-01_patch_7cae2ccc-2549-44a9-bbcf-3f56fa93b58e
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/0.1.3_2023-07-11-16-31-00_patch_24a2b472-2a9d-4e0a-a76d-0816f2cecc76
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/read_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:06:45.912122 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 17:06:45.000000 prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:06:45.916122 prodigy-teams-recipes-sdk-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-11 17:06:37.000000 prodigy-teams-recipes-sdk-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.916475 prodigy-teams-recipes-sdk-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 08:24:15.916475 prodigy-teams-recipes-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19849 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.908475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.908475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.908475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/200.html
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.908475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/_nuxt/
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.4c35cb5b.css
+-rw-r--r--   0 runner    (1001) docker     (123)   200330 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.d4386e81.js
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/recipe_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/recipe_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/teams_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.912475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.912475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59995 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.916475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.916475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/0.1.0_2023-05-12-12-39-11_patch_699f4418-3c53-4c0f-8a27-f838383451b1
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/0.1.1_2023-05-17-11-05-43_patch_8e2fe949-3833-4639-84bf-bf1f5bcbe993
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/0.1.2_2023-06-16-09-48-01_patch_7cae2ccc-2549-44a9-bbcf-3f56fa93b58e
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/0.1.3_2023-07-11-16-31-00_patch_24a2b472-2a9d-4e0a-a76d-0816f2cecc76
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/0.1.4_2023-07-17-07-47-30_patch_22c5529b-7752-43bf-ac53-aaef678efb5d
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/read_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:24:15.908475 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 08:24:15.000000 prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:24:15.916475 prodigy-teams-recipes-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-17 08:24:05.000000 prodigy-teams-recipes-sdk-0.1.5/setup.py
```

### Comparing `prodigy-teams-recipes-sdk-0.1.4/README.md` & `prodigy-teams-recipes-sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/__init__.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/about.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/about.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/cli.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/cli.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/preview.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/preview.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/200.html` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/200.html`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/404.html` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/404.html`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.4c35cb5b.css` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.4c35cb5b.css`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.d4386e81.js` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.d4386e81.js`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/public/index.html` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/public/index.html`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/recipe.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/recipe.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/recipe_loader.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/recipe_loader.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/recipe_schema.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/recipe_schema.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/registry.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/registry.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/teams_type.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/teams_type.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/engine/util.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/engine/util.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/project.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/project.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/session.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/session.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,18 @@
 
 
 class JobType(Enum):
     task = "task"
     action = "action"
 
 
+class LoginBody(BaseModel):
+    org_id: Optional[UUID] = Field(None, title="Org Id")
+
+
 class MetricsCreating(BaseModel):
     id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
     job_id: UUID = Field(..., title="Job Id")
     execution_id: UUID = Field(..., title="Execution Id")
     metrics_schema: Dict[str, Any] = Field(..., title="Metrics Schema")
```

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_client.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_client.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/assets.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/assets.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/dataset.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/decorator.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/decorator.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/props.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/props.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/types.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/types.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/sdk/util.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/sdk/util.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/testing.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/testing.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/types.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/types.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk/version/read_version.py` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk/version/read_version.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.4/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt` & `prodigy-teams-recipes-sdk-0.1.5/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,9 +66,10 @@
 prodigy_teams_recipes_sdk/sdk/props.py
 prodigy_teams_recipes_sdk/sdk/types.py
 prodigy_teams_recipes_sdk/sdk/util.py
 prodigy_teams_recipes_sdk/version/0.1.0_2023-05-12-12-39-11_patch_699f4418-3c53-4c0f-8a27-f838383451b1
 prodigy_teams_recipes_sdk/version/0.1.1_2023-05-17-11-05-43_patch_8e2fe949-3833-4639-84bf-bf1f5bcbe993
 prodigy_teams_recipes_sdk/version/0.1.2_2023-06-16-09-48-01_patch_7cae2ccc-2549-44a9-bbcf-3f56fa93b58e
 prodigy_teams_recipes_sdk/version/0.1.3_2023-07-11-16-31-00_patch_24a2b472-2a9d-4e0a-a76d-0816f2cecc76
+prodigy_teams_recipes_sdk/version/0.1.4_2023-07-17-07-47-30_patch_22c5529b-7752-43bf-ac53-aaef678efb5d
 prodigy_teams_recipes_sdk/version/__init__.py
 prodigy_teams_recipes_sdk/version/read_version.py
```

### Comparing `prodigy-teams-recipes-sdk-0.1.4/setup.py` & `prodigy-teams-recipes-sdk-0.1.5/setup.py`

 * *Files identical despite different names*

