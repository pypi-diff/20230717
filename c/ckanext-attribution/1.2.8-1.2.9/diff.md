# Comparing `tmp/ckanext-attribution-1.2.8.tar.gz` & `tmp/ckanext-attribution-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-attribution-1.2.8.tar", last modified: Tue Apr 11 08:13:36 2023, max compression
+gzip compressed data, was "ckanext-attribution-1.2.9.tar", last modified: Mon Jul 17 08:13:08 2023, max compression
```

## Comparing `ckanext-attribution-1.2.8.tar` & `ckanext-attribution-1.2.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/combiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.417134 ckanext-attribution-1.2.8/ckanext/attribution/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/lib/orcid_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/lib/ror_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.417134 ckanext-attribution-1.2.8/ckanext/attribution/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.417134 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.417134 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/meta/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/meta/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.417134 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/show.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.417134 ckanext-attribution-1.2.8/ckanext/attribution/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/agent_affiliation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/agent_contribution_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/contribution_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.421134 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/agent_affiliation.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/agent_contribution_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/contribution_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/crud/package_contribution_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/package_contribution_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/model/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.421134 ckanext-attribution-1.2.8/ckanext/attribution/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/routes/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.421134 ckanext-attribution-1.2.8/ckanext/attribution/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.421134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.421134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/less/attribution-additional.less
--rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/less/attribution.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.421134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.425134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   634988 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/625.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    52396 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/citations.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-activity.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-agent.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/errors.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)   430357 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/main.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-activity.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-agent.package-edit.js
--rw-r--r--   0 runner    (1001) docker     (123)   591316 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.425134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/App.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/api.js
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.425134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/AgentSearch.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/CitationPreview.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ContributionBlock.vue
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditActivity.vue
--rw-r--r--   0 runner    (1001) docker     (123)    15923 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditAgent.vue
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/Errors.vue
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/Loader.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowActivity.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowAgent.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.425134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/Base.vue
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/EditBase.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.425134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AgentTypeField.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Autocomplete.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AutocompleteList.vue
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/DateField.vue
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Field.vue
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Help.vue
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/SelectField.vue
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/TextField.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/ValidatedField.vue
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/eventbus.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/activity.js
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/affiliation.js
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/agent.js
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/citation.js
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/meta.js
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/store/
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/store/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/chicago-author-date.csl
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/ieee.csl
--rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/modern-language-association.csl
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.common.js
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.dev.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.prod.js
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/webassets.yml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/package/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/package/snippets/additional_info.html
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/package/snippets/package_metadata_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/snippets/contribution_item.html
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/snippets/contribution_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/user/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/user/contributions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/user/read_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:13:36.000000 ckanext-attribution-1.2.8/ckanext_attribution.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.413134 ckanext-attribution-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:13:36.429134 ckanext-attribution-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-11 08:13:26.000000 ckanext-attribution-1.2.8/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18495 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/lib/orcid_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/lib/ror_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/meta/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/meta/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/agent_affiliation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/agent_contribution_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/contribution_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/agent_affiliation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/agent_contribution_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/contribution_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/crud/package_contribution_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/package_contribution_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/model/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/routes/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.694120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/less/attribution-additional.less
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/less/attribution.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.698120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.698120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   634988 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/625.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52396 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/citations.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-activity.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-agent.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/errors.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)   430357 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/main.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-activity.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-agent.package-edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)   591316 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.698120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/App.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/AgentSearch.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/CitationPreview.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ContributionBlock.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditActivity.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    15923 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditAgent.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/Errors.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/Loader.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowActivity.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowAgent.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/Base.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/EditBase.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AgentTypeField.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Autocomplete.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AutocompleteList.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/DateField.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Field.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Help.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/SelectField.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/TextField.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/ValidatedField.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/eventbus.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/activity.js
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/affiliation.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/agent.js
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/citation.js
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/meta.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/store/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/chicago-author-date.csl
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/ieee.csl
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/modern-language-association.csl
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.common.js
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.dev.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.prod.js
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/webassets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/package/snippets/additional_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/package/snippets/package_metadata_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.702120 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/snippets/contribution_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/snippets/contribution_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/user/contributions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/user/read_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:13:08.000000 ckanext-attribution-1.2.9/ckanext_attribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.690120 ckanext-attribution-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:08.706120 ckanext-attribution-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-17 08:12:48.000000 ckanext-attribution-1.2.9/tests/test_helpers.py
```

### Comparing `ckanext-attribution-1.2.8/LICENSE` & `ckanext-attribution-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/PKG-INFO` & `ckanext-attribution-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-attribution
-Version: 1.2.8
+Version: 1.2.9
 Summary: A CKAN extension that adds support for complex attribution.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-attribution
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-attribution/blob/main/CHANGELOG.md
 Keywords: CKAN,data,attribution
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-attribution/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-attribution
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-attribution/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-attribution/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-attribution/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-attribution)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-attribution-1.2.8/README.md` & `ckanext-attribution-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-attribution/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-attribution
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-attribution/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-attribution/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-attribution/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-attribution)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/commands/cli.py` & `ckanext-attribution-1.2.9/ckanext/attribution/commands/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/api_search.py` & `ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/api_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/combiner.py` & `ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/combiner.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/common.py` & `ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/common.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/commands/migration/parser.py` & `ckanext-attribution-1.2.9/ckanext/attribution/commands/migration/parser.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/lib/helpers.py` & `ckanext-attribution-1.2.9/ckanext/attribution/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/lib/orcid_api.py` & `ckanext-attribution-1.2.9/ckanext/attribution/lib/orcid_api.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/lib/ror_api.py` & `ckanext-attribution-1.2.9/ckanext/attribution/lib/ror_api.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/create.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/create.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/delete.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/delete.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/extra.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/extra.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/helpers.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/meta/help.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/meta/help.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/meta/schema.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/meta/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/show.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/show.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/actions/update.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/actions/update.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/create.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/create.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/delete.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/delete.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/extra.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/extra.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/show.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/show.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/logic/auth/update.py` & `ckanext-attribution-1.2.9/ckanext/attribution/logic/auth/update.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/agent.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/agent.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/agent_affiliation.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/agent_affiliation.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/agent_contribution_activity.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/agent_contribution_activity.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/contribution_activity.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/contribution_activity.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/crud/_base.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/crud/_base.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/crud/agent.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/crud/agent.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/crud/agent_affiliation.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/crud/agent_affiliation.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/crud/agent_contribution_activity.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/crud/agent_contribution_activity.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/crud/package.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/crud/package.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/crud/package_contribution_activity.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/crud/package_contribution_activity.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/package_contribution_activity.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/package_contribution_activity.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/model/relationships.py` & `ckanext-attribution-1.2.9/ckanext/attribution/model/relationships.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/plugin.py` & `ckanext-attribution-1.2.9/ckanext/attribution/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/routes/user.py` & `ckanext-attribution-1.2.9/ckanext/attribution/routes/user.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/less/attribution.less` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/less/attribution.less`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/625.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/625.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/citations.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/citations.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-activity.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-activity.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-agent.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/edit-agent.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/main.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/main.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-activity.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-activity.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-agent.package-edit.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/dist/show-agent.package-edit.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/package-lock.json` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/package-lock.json`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/package.json` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/package.json`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/App.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/App.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/api.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/api.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/app.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/app.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/AgentSearch.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/AgentSearch.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/CitationPreview.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/CitationPreview.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ContributionBlock.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ContributionBlock.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditActivity.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditActivity.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditAgent.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/EditAgent.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowActivity.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowActivity.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowAgent.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/ShowAgent.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/Base.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/Base.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/EditBase.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/bases/EditBase.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AgentTypeField.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AgentTypeField.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Autocomplete.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Autocomplete.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AutocompleteList.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/AutocompleteList.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/DateField.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/DateField.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Field.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/Field.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/SelectField.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/SelectField.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/TextField.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/TextField.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/ValidatedField.vue` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/components/fields/ValidatedField.vue`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/activity.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/activity.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/affiliation.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/affiliation.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/agent.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/agent.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/meta.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/meta.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/utils.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/models/utils.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/store/main.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/src/store/main.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/chicago-author-date.csl` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/chicago-author-date.csl`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/ieee.csl` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/ieee.csl`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/modern-language-association.csl` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/vendor/modern-language-association.csl`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.common.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.common.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.prod.js` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/assets/scripts/apps/package-edit/webpack.config.prod.js`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/package.json` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'1.2.9'"}*

```diff
@@ -10,9 +10,9 @@
     "homepage": "https://github.com/NaturalHistoryMuseum/ckanext-attribution",
     "license": "GPL-3.0-or-later",
     "name": "ckanext-attribution",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/NaturalHistoryMuseum/ckanext-attribution.git"
     },
-    "version": "1.2.8"
+    "version": "1.2.9"
 }
```

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/package/snippets/additional_info.html` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/package/snippets/additional_info.html`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/snippets/contribution_item.html` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/snippets/contribution_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/snippets/contribution_list.html` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/snippets/contribution_list.html`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext/attribution/theme/templates/user/read_base.html` & `ckanext-attribution-1.2.9/ckanext/attribution/theme/templates/user/read_base.html`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/ckanext_attribution.egg-info/PKG-INFO` & `ckanext-attribution-1.2.9/ckanext_attribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-attribution
-Version: 1.2.8
+Version: 1.2.9
 Summary: A CKAN extension that adds support for complex attribution.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-attribution
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-attribution/blob/main/CHANGELOG.md
 Keywords: CKAN,data,attribution
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--header-start-->
-<img src="https://github.com/NaturalHistoryMuseum/ckanext-attribution/raw/main/.github/nhm-logo.svg" align="left" width="150px" height="100px" hspace="40"/>
+<img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-attribution
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-attribution/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-attribution/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-attribution/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-attribution)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
```

### Comparing `ckanext-attribution-1.2.8/ckanext_attribution.egg-info/SOURCES.txt` & `ckanext-attribution-1.2.9/ckanext_attribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/docs/_scripts/gen_api_pages.py` & `ckanext-attribution-1.2.9/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-attribution-1.2.8/pyproject.toml` & `ckanext-attribution-1.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-attribution"
-version = "1.2.8"
+version = "1.2.9"
 description = "A CKAN extension that adds support for complex attribution."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -59,15 +59,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.attribution.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "1.2.8"
+version = "1.2.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "ckanext/attribution/theme/package.json",
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-attribution-1.2.8/tests/test_helpers.py` & `ckanext-attribution-1.2.9/tests/test_helpers.py`

 * *Files identical despite different names*

