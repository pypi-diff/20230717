# Comparing `tmp/dbt-core-1.6.0b8.tar.gz` & `tmp/dbt-core-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.6.0b8.tar", last modified: Fri Jun 30 19:21:38 2023, max compression
+gzip compressed data, was "dbt-core-1.6.0rc1.tar", last modified: Mon Jul 17 21:04:32 2023, max compression
```

## Comparing `dbt-core-1.6.0b8.tar` & `dbt-core-1.6.0rc1.tar`

### file list

```diff
@@ -1,343 +1,345 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.491028 dbt-core-1.6.0b8/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.495028 dbt-core-1.6.0b8/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.499029 dbt-core-1.6.0b8/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.499029 dbt-core-1.6.0b8/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.499029 dbt-core-1.6.0b8/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    60992 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55058 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    53205 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/semantic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22434 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.503028 dbt-core-1.6.0b8/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    62526 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   115121 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    79375 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    30457 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.507029 dbt-core-1.6.0b8/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/drop_relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/clone.sql
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.511029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.515029 dbt-core-1.6.0b8/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.487028 dbt-core-1.6.0b8/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.519029 dbt-core-1.6.0b8/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.523029 dbt-core-1.6.0b8/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    68817 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    48426 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/parser/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.523029 dbt-core-1.6.0b8/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-30 19:21:38.000000 dbt-core-1.6.0b8/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 19:21:38.527029 dbt-core-1.6.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-30 19:21:26.000000 dbt-core-1.6.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.934350 dbt-core-1.6.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.934350 dbt-core-1.6.0rc1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57217 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18265 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.938350 dbt-core-1.6.0rc1/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23217 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.942350 dbt-core-1.6.0rc1/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27182 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.942350 dbt-core-1.6.0rc1/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60992 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.942350 dbt-core-1.6.0rc1/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55911 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54904 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.946350 dbt-core-1.6.0rc1/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62873 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105768 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79543 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30501 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.950350 dbt-core-1.6.0rc1/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/drop_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/validate_sql.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.954350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/create_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/refresh_materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.958351 dbt-core-1.6.0rc1/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497953 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.930350 dbt-core-1.6.0rc1/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.962350 dbt-core-1.6.0rc1/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.966350 dbt-core-1.6.0rc1/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48426 2023-07-17 21:04:19.000000 dbt-core-1.6.0rc1/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20475 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38427 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/parser/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.966350 dbt-core-1.6.0rc1/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18745 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22958 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19598 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 21:04:32.000000 dbt-core-1.6.0rc1/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:04:32.970351 dbt-core-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-17 21:04:20.000000 dbt-core-1.6.0rc1/setup.py
```

### Comparing `dbt-core-1.6.0b8/PKG-INFO` & `dbt-core-1.6.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b8
+Version: 1.6.0rc1
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b8 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0rc1 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b8/README.md` & `dbt-core-1.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/__init__.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/column.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/connections.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/impl.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,25 @@
         :param bool fetch: If set, fetch results.
         :param Optional[int] limit: If set, only fetch n number of rows
         :return: A tuple of the query status and results (empty if fetch=False).
         :rtype: Tuple[AdapterResponse, agate.Table]
         """
         return self.connections.execute(sql=sql, auto_begin=auto_begin, fetch=fetch, limit=limit)
 
+    def validate_sql(self, sql: str) -> AdapterResponse:
+        """Submit the given SQL to the engine for validation, but not execution.
+
+        This should throw an appropriate exception if the input SQL is invalid, although
+        in practice that will generally be handled by delegating to an existing method
+        for execution and allowing the error handler to take care of the rest.
+
+        :param str sql: The sql to validate
+        """
+        raise NotImplementedError("`validate_sql` is not implemented for this adapter!")
+
     @available.parse(lambda *a, **k: [])
     def get_column_schema_from_query(self, sql: str) -> List[BaseColumn]:
         """Get a list of the Columns with names and data types from the given sql."""
         _, cursor = self.connections.add_select_query(sql)
         columns = [
             self.Column.create(
                 column_name, self.connections.data_type_code_to_name(column_type_code)
@@ -781,15 +792,14 @@
     def _make_match(
         self,
         relations_list: List[BaseRelation],
         database: str,
         schema: str,
         identifier: str,
     ) -> List[BaseRelation]:
-
         matches = []
 
         search = self._make_match_kwargs(database, schema, identifier)
 
         for relation in relations_list:
             if relation.matches(**search):
                 matches.append(relation)
@@ -1059,15 +1069,14 @@
 
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Set[str],
         manifest: Manifest,
     ) -> agate.Table:
-
         kwargs = {"information_schema": information_schema, "schemas": schemas}
         table = self.execute_macro(
             GET_CATALOG_MACRO_NAME,
             kwargs=kwargs,
             # pass in the full manifest so we get any local project
             # overrides
             manifest=manifest,
@@ -1449,15 +1458,14 @@
 join diff_count using (id)
 """.strip()
 
 
 def catch_as_completed(
     futures,  # typing: List[Future[agate.Table]]
 ) -> Tuple[agate.Table, List[Exception]]:
-
     # catalogs: agate.Table = agate.Table(rows=[])
     tables: List[agate.Table] = []
     exceptions: List[Exception] = []
 
     for future in as_completed(futures):
         exc = future.exception()
         # we want to re-raise on ctrl+c and BaseException
```

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/meta.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/plugin.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/query_headers.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/base/relation.py` & `dbt-core-1.6.0rc1/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/cache.py` & `dbt-core-1.6.0rc1/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/factory.py` & `dbt-core-1.6.0rc1/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/protocol.py` & `dbt-core-1.6.0rc1/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/reference_keys.py` & `dbt-core-1.6.0rc1/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_base.py` & `dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_change.py` & `dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/relation_configs/config_validation.py` & `dbt-core-1.6.0rc1/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/adapters/sql/connections.py` & `dbt-core-1.6.0rc1/dbt/adapters/sql/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     def add_query(
         self,
         sql: str,
         auto_begin: bool = True,
         bindings: Optional[Any] = None,
         abridge_sql_log: bool = False,
     ) -> Tuple[Connection, Any]:
-
         connection = self.get_thread_connection()
         if auto_begin and connection.transaction_open is False:
             self.begin()
         fire_event(
             ConnectionUsed(
                 conn_type=self.TYPE,
                 conn_name=cast_to_str(connection.name),
```

### Comparing `dbt-core-1.6.0b8/dbt/adapters/sql/impl.py` & `dbt-core-1.6.0rc1/dbt/adapters/sql/impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import agate
 from typing import Any, Optional, Tuple, Type, List
 
-from dbt.contracts.connection import Connection
+from dbt.contracts.connection import Connection, AdapterResponse
 from dbt.exceptions import RelationTypeNullError
 from dbt.adapters.base import BaseAdapter, available
 from dbt.adapters.cache import _make_ref_key_dict
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.events.functions import fire_event
 from dbt.events.types import ColTypeChange, SchemaCreation, SchemaDrop
 
@@ -18,14 +18,15 @@
 CHECK_SCHEMA_EXISTS_MACRO_NAME = "check_schema_exists"
 CREATE_SCHEMA_MACRO_NAME = "create_schema"
 DROP_SCHEMA_MACRO_NAME = "drop_schema"
 RENAME_RELATION_MACRO_NAME = "rename_relation"
 TRUNCATE_RELATION_MACRO_NAME = "truncate_relation"
 DROP_RELATION_MACRO_NAME = "drop_relation"
 ALTER_COLUMN_TYPE_MACRO_NAME = "alter_column_type"
+VALIDATE_SQL_MACRO_NAME = "validate_sql"
 
 
 class SQLAdapter(BaseAdapter):
     """The default adapter with the common agate conversions and some SQL
     methods was implemented. This adapter has a different much shorter list of
     methods to implement, but some more macros that must be implemented.
 
@@ -214,14 +215,42 @@
             quote_policy=self.config.quoting,
         ).information_schema()
 
         kwargs = {"information_schema": information_schema, "schema": schema}
         results = self.execute_macro(CHECK_SCHEMA_EXISTS_MACRO_NAME, kwargs=kwargs)
         return results[0][0] > 0
 
+    def validate_sql(self, sql: str) -> AdapterResponse:
+        """Submit the given SQL to the engine for validation, but not execution.
+
+        By default we simply prefix the query with the explain keyword and allow the
+        exceptions thrown by the underlying engine on invalid SQL inputs to bubble up
+        to the exception handler. For adjustments to the explain statement - such as
+        for adapters that have different mechanisms for hinting at query validation
+        or dry-run - callers may be able to override the validate_sql_query macro with
+        the addition of an <adapter>__validate_sql implementation.
+
+        :param sql str: The sql to validate
+        """
+        kwargs = {
+            "sql": sql,
+        }
+        result = self.execute_macro(VALIDATE_SQL_MACRO_NAME, kwargs=kwargs)
+        # The statement macro always returns an AdapterResponse in the output AttrDict's
+        # `response` property, and we preserve the full payload in case we want to
+        # return fetched output for engines where explain plans are emitted as columnar
+        # results. Any macro override that deviates from this behavior may encounter an
+        # assertion error in the runtime.
+        adapter_response = result.response  # type: ignore[attr-defined]
+        assert isinstance(adapter_response, AdapterResponse), (
+            f"Expected AdapterResponse from validate_sql macro execution, "
+            f"got {type(adapter_response)}."
+        )
+        return adapter_response
+
     # This is for use in the test suite
     def run_sql_for_tests(self, sql, fetch, conn):
         cursor = conn.handle.cursor()
         try:
             cursor.execute(sql)
             if hasattr(conn.handle, "commit"):
                 conn.handle.commit()
```

### Comparing `dbt-core-1.6.0b8/dbt/cli/exceptions.py` & `dbt-core-1.6.0rc1/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/cli/flags.py` & `dbt-core-1.6.0rc1/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/cli/main.py` & `dbt-core-1.6.0rc1/dbt/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 @p.log_format
 @p.log_format_file
 @p.log_level
 @p.log_level_file
 @p.log_path
 @p.macro_debugging
 @p.partial_parse
+@p.partial_parse_file_path
 @p.populate_cache
 @p.print
 @p.printer_width
 @p.quiet
 @p.record_timing_info
 @p.send_anonymous_usage_stats
 @p.single_threaded
```

### Comparing `dbt-core-1.6.0b8/dbt/cli/option_types.py` & `dbt-core-1.6.0rc1/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/cli/options.py` & `dbt-core-1.6.0rc1/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/cli/params.py` & `dbt-core-1.6.0rc1/dbt/cli/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,14 +235,23 @@
 partial_parse = click.option(
     "--partial-parse/--no-partial-parse",
     envvar="DBT_PARTIAL_PARSE",
     help="Allow for partial parsing by looking for and writing to a pickle file in the target directory. This overrides the user configuration file.",
     default=True,
 )
 
+partial_parse_file_path = click.option(
+    "--partial-parse-file-path",
+    envvar="DBT_PARTIAL_PARSE_FILE_PATH",
+    help="Internal flag for path to partial_parse.manifest file.",
+    default=None,
+    hidden=True,
+    type=click.Path(exists=True, dir_okay=False, resolve_path=True),
+)
+
 populate_cache = click.option(
     "--populate-cache/--no-populate-cache",
     envvar="DBT_POPULATE_CACHE",
     help="At start of run, use `show` or `information_schema` queries to populate a relational cache, which can speed up subsequent materializations.",
     default=True,
 )
```

### Comparing `dbt-core-1.6.0b8/dbt/cli/requires.py` & `dbt-core-1.6.0rc1/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/cli/resolvers.py` & `dbt-core-1.6.0rc1/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/cli/types.py` & `dbt-core-1.6.0rc1/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/_jinja_blocks.py` & `dbt-core-1.6.0rc1/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/agate_helper.py` & `dbt-core-1.6.0rc1/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/git.py` & `dbt-core-1.6.0rc1/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/jinja.py` & `dbt-core-1.6.0rc1/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/jinja_static.py` & `dbt-core-1.6.0rc1/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/registry.py` & `dbt-core-1.6.0rc1/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/system.py` & `dbt-core-1.6.0rc1/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/clients/yaml_helper.py` & `dbt-core-1.6.0rc1/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/compilation.py` & `dbt-core-1.6.0rc1/dbt/compilation.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,30 +44,32 @@
     names = {
         NodeType.Model: "model",
         NodeType.Test: "test",
         NodeType.Snapshot: "snapshot",
         NodeType.Analysis: "analysis",
         NodeType.Macro: "macro",
         NodeType.Operation: "operation",
-        NodeType.Seed: "seed file",
+        NodeType.Seed: "seed",
         NodeType.Source: "source",
         NodeType.Exposure: "exposure",
+        NodeType.SemanticModel: "semantic model",
         NodeType.Metric: "metric",
         NodeType.Group: "group",
     }
 
     results = {k: 0 for k in names.keys()}
     results.update(stats)
 
     # create tracking event for resource_counts
     if dbt.tracking.active_user is not None:
         resource_counts = {k.pluralize(): v for k, v in results.items()}
         dbt.tracking.track_resource_counts(resource_counts)
 
-    stat_line = ", ".join([pluralize(ct, names.get(t)) for t, ct in results.items() if t in names])
+    # do not include resource types that are not actually defined in the project
+    stat_line = ", ".join([pluralize(ct, names.get(t)) for t, ct in stats.items() if t in names])
 
     fire_event(FoundStats(stat_line=stat_line))
 
 
 def _node_enabled(node: ManifestNode):
     # Disabled models are already excluded from the manifest
     if node.resource_type == NodeType.Test and not node.config.enabled:
@@ -78,24 +80,24 @@
 
 def _generate_stats(manifest: Manifest):
     stats: Dict[NodeType, int] = defaultdict(int)
     for node in manifest.nodes.values():
         if _node_enabled(node):
             stats[node.resource_type] += 1
 
-    for source in manifest.sources.values():
-        stats[source.resource_type] += 1
-    for exposure in manifest.exposures.values():
-        stats[exposure.resource_type] += 1
-    for metric in manifest.metrics.values():
-        stats[metric.resource_type] += 1
-    for macro in manifest.macros.values():
-        stats[macro.resource_type] += 1
-    for group in manifest.groups.values():
-        stats[group.resource_type] += 1
+    # Disabled nodes don't appear in the following collections, so we don't check.
+    stats[NodeType.Source] += len(manifest.sources)
+    stats[NodeType.Exposure] += len(manifest.exposures)
+    stats[NodeType.Metric] += len(manifest.metrics)
+    stats[NodeType.Macro] += len(manifest.macros)
+    stats[NodeType.Group] += len(manifest.groups)
+    stats[NodeType.SemanticModel] += len(manifest.semantic_models)
+
+    # TODO: should we be counting dimensions + entities?
+
     return stats
 
 
 def _add_prepended_cte(prepended_ctes, new_cte):
     for cte in prepended_ctes:
         if cte.id == new_cte.id and new_cte.sql:
             cte.sql = new_cte.sql
@@ -169,14 +171,16 @@
         for dependency in node.depends_on_nodes:
             if dependency in manifest.nodes:
                 self.dependency(node.unique_id, (manifest.nodes[dependency].unique_id))
             elif dependency in manifest.sources:
                 self.dependency(node.unique_id, (manifest.sources[dependency].unique_id))
             elif dependency in manifest.metrics:
                 self.dependency(node.unique_id, (manifest.metrics[dependency].unique_id))
+            elif dependency in manifest.semantic_models:
+                self.dependency(node.unique_id, (manifest.semantic_models[dependency].unique_id))
             else:
                 raise GraphDependencyNotFoundError(node, dependency)
 
     def link_graph(self, manifest: Manifest):
         for source in manifest.sources.values():
             self.add_node(source.unique_id)
         for semantic_model in manifest.semantic_models.values():
```

### Comparing `dbt-core-1.6.0b8/dbt/config/profile.py` & `dbt-core-1.6.0rc1/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/config/project.py` & `dbt-core-1.6.0rc1/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/config/renderer.py` & `dbt-core-1.6.0rc1/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/config/runtime.py` & `dbt-core-1.6.0rc1/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/config/selectors.py` & `dbt-core-1.6.0rc1/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/config/utils.py` & `dbt-core-1.6.0rc1/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/constants.py` & `dbt-core-1.6.0rc1/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/base.py` & `dbt-core-1.6.0rc1/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/configured.py` & `dbt-core-1.6.0rc1/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/context_config.py` & `dbt-core-1.6.0rc1/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/docs.py` & `dbt-core-1.6.0rc1/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/exceptions_jinja.py` & `dbt-core-1.6.0rc1/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/macro_resolver.py` & `dbt-core-1.6.0rc1/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/macros.py` & `dbt-core-1.6.0rc1/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/manifest.py` & `dbt-core-1.6.0rc1/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/providers.py` & `dbt-core-1.6.0rc1/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/secret.py` & `dbt-core-1.6.0rc1/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/context/target.py` & `dbt-core-1.6.0rc1/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/connection.py` & `dbt-core-1.6.0rc1/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/files.py` & `dbt-core-1.6.0rc1/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/manifest.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import enum
+from collections import defaultdict
 from dataclasses import dataclass, field
 from itertools import chain, islice
 from mashumaro.mixins.msgpack import DataClassMessagePackMixin
 from multiprocessing.synchronize import Lock
 from typing import (
+    DefaultDict,
     Dict,
     List,
     Optional,
     Union,
     Mapping,
     MutableMapping,
     Any,
@@ -46,34 +48,24 @@
 from dbt.dataclass_schema import dbtClassMixin
 from dbt.exceptions import (
     CompilationError,
     DuplicateResourceNameError,
     DuplicateMacroInPackageError,
     DuplicateMaterializationNameError,
     AmbiguousResourceNameRefError,
-    ParsingError,
 )
 from dbt.helper_types import PathSet
 from dbt.events.functions import fire_event
 from dbt.events.types import MergedFromState, UnpinnedRefNewVersionAvailable
 from dbt.events.contextvars import get_node_info
 from dbt.node_types import NodeType, AccessType
 from dbt.flags import get_flags, MP_CONTEXT
 from dbt import tracking
 import dbt.utils
-from dbt_semantic_interfaces.implementations.metric import PydanticMetric
-from dbt_semantic_interfaces.implementations.semantic_manifest import PydanticSemanticManifest
-from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
-from dbt_semantic_interfaces.implementations.project_configuration import (
-    PydanticProjectConfiguration,
-)
-from dbt_semantic_interfaces.implementations.time_spine_table_configuration import (
-    PydanticTimeSpineTableConfiguration,
-)
-from dbt_semantic_interfaces.type_enums import TimeGranularity
+
 
 NodeEdgeMap = Dict[str, List[str]]
 PackageName = str
 DocName = str
 RefName = str
 UniqueID = str
 
@@ -303,14 +295,57 @@
         if unique_id not in manifest.metrics:
             raise dbt.exceptions.DbtInternalError(
                 f"Metric {unique_id} found in cache but not found in manifest"
             )
         return manifest.metrics[unique_id]
 
 
+class SemanticModelByMeasureLookup(dbtClassMixin):
+    """Lookup utility for finding SemanticModel by measure
+
+    This is possible because measure names are supposed to be unique across
+    the semantic models in a manifest.
+    """
+
+    def __init__(self, manifest: "Manifest"):
+        self.storage: DefaultDict[str, Dict[PackageName, UniqueID]] = defaultdict(dict)
+        self.populate(manifest)
+
+    def get_unique_id(self, search_name: str, package: Optional[PackageName]):
+        return find_unique_id_for_package(self.storage, search_name, package)
+
+    def find(
+        self, search_name: str, package: Optional[PackageName], manifest: "Manifest"
+    ) -> Optional[SemanticModel]:
+        """Tries to find a SemanticModel based on a measure name"""
+        unique_id = self.get_unique_id(search_name, package)
+        if unique_id is not None:
+            return self.perform_lookup(unique_id, manifest)
+        return None
+
+    def add(self, semantic_model: SemanticModel):
+        """Sets all measures for a SemanticModel as paths to the SemanticModel's `unique_id`"""
+        for measure in semantic_model.measures:
+            self.storage[measure.name][semantic_model.package_name] = semantic_model.unique_id
+
+    def populate(self, manifest: "Manifest"):
+        """Populate storage with all the measure + package paths to the Manifest's SemanticModels"""
+        for semantic_model in manifest.semantic_models.values():
+            self.add(semantic_model=semantic_model)
+
+    def perform_lookup(self, unique_id: UniqueID, manifest: "Manifest") -> SemanticModel:
+        """Tries to get a SemanticModel from the Manifest"""
+        semantic_model = manifest.semantic_models.get(unique_id)
+        if semantic_model is None:
+            raise dbt.exceptions.DbtInternalError(
+                f"Semantic model `{unique_id}` found in cache but not found in manifest"
+            )
+        return semantic_model
+
+
 # This handles both models/seeds/snapshots and sources/metrics/exposures
 class DisabledLookup(dbtClassMixin):
     def __init__(self, manifest: "Manifest"):
         self.storage: Dict[str, Dict[PackageName, List[Any]]] = {}
         self.populate(manifest)
 
     def populate(self, manifest):
@@ -716,14 +751,17 @@
     )
     _ref_lookup: Optional[RefableLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
     _metric_lookup: Optional[MetricLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
+    _semantic_model_by_measure_lookup: Optional[SemanticModelByMeasureLookup] = field(
+        default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
+    )
     _disabled_lookup: Optional[DisabledLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
     _analysis_lookup: Optional[AnalysisLookup] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
     _parsing_info: ParsingInfo = field(
@@ -966,14 +1004,21 @@
 
     @property
     def metric_lookup(self) -> MetricLookup:
         if self._metric_lookup is None:
             self._metric_lookup = MetricLookup(self)
         return self._metric_lookup
 
+    @property
+    def semantic_model_by_measure_lookup(self) -> SemanticModelByMeasureLookup:
+        """Gets (and creates if necessary) the lookup utility for getting SemanticModels by measures"""
+        if self._semantic_model_by_measure_lookup is None:
+            self._semantic_model_by_measure_lookup = SemanticModelByMeasureLookup(self)
+        return self._semantic_model_by_measure_lookup
+
     def rebuild_ref_lookup(self):
         self._ref_lookup = RefableLookup(self)
 
     @property
     def disabled_lookup(self) -> DisabledLookup:
         if self._disabled_lookup is None:
             self._disabled_lookup = DisabledLookup(self)
@@ -985,52 +1030,14 @@
     @property
     def analysis_lookup(self) -> AnalysisLookup:
         if self._analysis_lookup is None:
             self._analysis_lookup = AnalysisLookup(self)
         return self._analysis_lookup
 
     @property
-    def pydantic_semantic_manifest(self) -> PydanticSemanticManifest:
-        project_config = PydanticProjectConfiguration(
-            time_spine_table_configurations=[],
-        )
-        pydantic_semantic_manifest = PydanticSemanticManifest(
-            metrics=[], semantic_models=[], project_configuration=project_config
-        )
-
-        for semantic_model in self.semantic_models.values():
-            pydantic_semantic_manifest.semantic_models.append(
-                PydanticSemanticModel.parse_obj(semantic_model.to_dict())
-            )
-
-        for metric in self.metrics.values():
-            pydantic_semantic_manifest.metrics.append(PydanticMetric.parse_obj(metric.to_dict()))
-
-        # Look for time-spine table model and create time spine table configuration
-        if self.semantic_models:
-            # Get model for time_spine_table
-            time_spine_model_name = "metricflow_time_spine"
-            model = self.ref_lookup.find(time_spine_model_name, None, None, self)
-            if not model:
-                raise ParsingError(
-                    "The semantic layer requires a 'metricflow_time_spine' model in the project, but none was found. Guidance on creating this model can be found on our docs site (https://docs.getdbt.com/docs/build/metricflow-time-spine)"
-                )
-            # Create time_spine_table_config, set it in project_config, and add to semantic manifest
-            time_spine_table_config = PydanticTimeSpineTableConfiguration(
-                location=model.relation_name,
-                column_name="date_day",
-                grain=TimeGranularity.DAY,
-            )
-            pydantic_semantic_manifest.project_configuration.time_spine_table_configurations = [
-                time_spine_table_config
-            ]
-
-        return pydantic_semantic_manifest
-
-    @property
     def external_node_unique_ids(self):
         return [node.unique_id for node in self.nodes.values() if node.is_external_node]
 
     def resolve_refs(
         self,
         source_node: ModelNode,
         current_project: str,  # TODO: ModelNode is overly restrictive typing
@@ -1131,14 +1138,33 @@
             # it's possible that the node is disabled
             if disabled is None:
                 disabled = self.disabled_lookup.find(f"{target_metric_name}", pkg)
         if disabled:
             return Disabled(disabled[0])
         return None
 
+    def resolve_semantic_model_for_measure(
+        self,
+        target_measure_name: str,
+        current_project: str,
+        node_package: str,
+        target_package: Optional[str] = None,
+    ) -> Optional[SemanticModel]:
+        """Tries to find the SemanticModel that a measure belongs to"""
+        candidates = _packages_to_search(current_project, node_package, target_package)
+
+        for pkg in candidates:
+            semantic_model = self.semantic_model_by_measure_lookup.find(
+                target_measure_name, pkg, self
+            )
+            if semantic_model is not None:
+                return semantic_model
+
+        return None
+
     # Called by DocsRuntimeContext.doc
     def resolve_doc(
         self,
         name: str,
         package: Optional[str],
         current_project: str,
         node_package: str,
@@ -1372,14 +1398,15 @@
             self.disabled,
             self.env_vars,
             self.semantic_models,
             self._doc_lookup,
             self._source_lookup,
             self._ref_lookup,
             self._metric_lookup,
+            self._semantic_model_by_measure_lookup,
             self._disabled_lookup,
             self._analysis_lookup,
         )
         return self.__class__, args
 
 
 class MacroManifest(MacroMethods):
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/metrics.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/model_config.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,14 +383,19 @@
         for key, value in kwargs.items():
             new_key = mapping.get(key, key)
             dct[new_key] = value
         return self.from_dict(dct)
 
 
 @dataclass
+class SemanticModelConfig(BaseConfig):
+    enabled: bool = True
+
+
+@dataclass
 class MetricConfig(BaseConfig):
     enabled: bool = True
     group: Optional[str] = None
 
 
 @dataclass
 class ExposureConfig(BaseConfig):
@@ -546,14 +551,16 @@
         super().validate(data)
         if data.get("materialized") and data.get("materialized") != "seed":
             raise ValidationError("A seed must have a materialized value of 'seed'")
 
 
 @dataclass
 class TestConfig(NodeAndTestConfig):
+    __test__ = False
+
     # this is repeated because of a different default
     schema: Optional[str] = field(
         default="dbt_test__audit",
         metadata=CompareBehavior.Exclude.meta(),
     )
     materialized: str = "test"
     severity: Severity = Severity("ERROR")
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/node_args.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/node_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     depends_on_nodes: List[str] = field(default_factory=list)
     enabled: bool = True
 
     @property
     def unique_id(self) -> str:
         unique_id = f"{NodeType.Model}.{self.package_name}.{self.name}"
         if self.version:
-            unique_id = f"{unique_id}.{self.version}"
+            unique_id = f"{unique_id}.v{self.version}"
 
         return unique_id
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/nodes.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,35 @@
     SeedExceedsLimitSamePath,
     SeedExceedsLimitAndPathChanged,
     SeedExceedsLimitChecksumChanged,
 )
 from dbt.events.contextvars import set_log_contextvars
 from dbt.flags import get_flags
 from dbt.node_types import ModelLanguage, NodeType, AccessType
+from dbt_semantic_interfaces.call_parameter_sets import FilterCallParameterSets
 from dbt_semantic_interfaces.references import (
     MeasureReference,
     LinkableElementReference,
     SemanticModelReference,
+    TimeDimensionReference,
 )
 from dbt_semantic_interfaces.references import MetricReference as DSIMetricReference
 from dbt_semantic_interfaces.type_enums import MetricType, TimeGranularity
+from dbt_semantic_interfaces.parsing.where_filter_parser import WhereFilterParser
 
 from .model_config import (
     NodeConfig,
     SeedConfig,
     TestConfig,
     SourceConfig,
     MetricConfig,
     ExposureConfig,
     EmptySnapshotConfig,
     SnapshotConfig,
+    SemanticModelConfig,
 )
 
 
 # =====================================================================
 # This contains the classes for all of the nodes and node-like objects
 # in the manifest. In the "nodes" dictionary of the manifest we find
 # all of the objects in the ManifestNode union below. In addition the
@@ -621,14 +625,19 @@
     def materialization_enforces_constraints(self) -> bool:
         return self.config.materialized in ["table", "incremental"]
 
     def build_contract_checksum(self):
         # We don't need to construct the checksum if the model does not
         # have contract enforced, because it won't be used.
         # This needs to be executed after contract config is set
+
+        # Avoid rebuilding the checksum if it has already been set.
+        if self.contract.checksum is not None:
+            return
+
         if self.contract.enforced is True:
             contract_state = ""
             # We need to sort the columns so that order doesn't matter
             # columns is a str: ColumnInfo dictionary
             sorted_columns = sorted(self.columns.values(), key=lambda col: col.name)
             for column in sorted_columns:
                 contract_state += f"|{column.name}"
@@ -919,14 +928,16 @@
 # ====================================
 # Generic Test node
 # ====================================
 
 
 @dataclass
 class TestMetadata(dbtClassMixin, Replaceable):
+    __test__ = False
+
     name: str
     # kwargs are the args that are left in the test builder after
     # removing configs. They are set from the test builder when
     # the test node is created.
     kwargs: Dict[str, Any] = field(default_factory=dict)
     namespace: Optional[str] = None
 
@@ -1304,14 +1315,18 @@
 # ====================================
 
 
 @dataclass
 class WhereFilter(dbtClassMixin):
     where_sql_template: str
 
+    @property
+    def call_parameter_sets(self) -> FilterCallParameterSets:
+        return WhereFilterParser.parse_call_parameter_sets(self.where_sql_template)
+
 
 @dataclass
 class MetricInputMeasure(dbtClassMixin):
     name: str
     filter: Optional[WhereFilter] = None
     alias: Optional[str] = None
 
@@ -1478,14 +1493,15 @@
     entities: Sequence[Entity] = field(default_factory=list)
     measures: Sequence[Measure] = field(default_factory=list)
     dimensions: Sequence[Dimension] = field(default_factory=list)
     metadata: Optional[SourceFileMetadata] = None
     depends_on: DependsOn = field(default_factory=DependsOn)
     refs: List[RefArgs] = field(default_factory=list)
     created_at: float = field(default_factory=lambda: time.time())
+    config: SemanticModelConfig = field(default_factory=SemanticModelConfig)
 
     @property
     def entity_references(self) -> List[LinkableElementReference]:
         return [entity.reference for entity in self.entities]
 
     @property
     def dimension_references(self) -> List[LinkableElementReference]:
@@ -1536,14 +1552,37 @@
     def depends_on_nodes(self):
         return self.depends_on.nodes
 
     @property
     def depends_on_macros(self):
         return self.depends_on.macros
 
+    def checked_agg_time_dimension_for_measure(
+        self, measure_reference: MeasureReference
+    ) -> TimeDimensionReference:
+        measure: Optional[Measure] = None
+        for measure in self.measures:
+            if measure.reference == measure_reference:
+                measure = measure
+
+        assert (
+            measure is not None
+        ), f"No measure with name ({measure_reference.element_name}) in semantic_model with name ({self.name})"
+
+        if self.defaults is not None:
+            default_agg_time_dimesion = self.defaults.agg_time_dimension
+
+        agg_time_dimension_name = measure.agg_time_dimension or default_agg_time_dimesion
+        assert agg_time_dimension_name is not None, (
+            f"Aggregation time dimension for measure {measure.name} is not set! This should either be set directly on "
+            f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
+            f"source containing the measure."
+        )
+        return TimeDimensionReference(element_name=agg_time_dimension_name)
+
 
 # ====================================
 # Patches
 # ====================================
 
 
 @dataclass
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/semantic_models.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/semantic_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,31 +124,24 @@
     use_approximate_percentile: bool = False
 
 
 @dataclass
 class NonAdditiveDimension(dbtClassMixin):
     name: str
     window_choice: AggregationType
-    window_grouples: List[str]
+    window_groupings: List[str]
 
 
 @dataclass
 class Measure(dbtClassMixin):
     name: str
     agg: AggregationType
     description: Optional[str] = None
     create_metric: bool = False
     expr: Optional[str] = None
     agg_params: Optional[MeasureAggregationParameters] = None
     non_additive_dimension: Optional[NonAdditiveDimension] = None
     agg_time_dimension: Optional[str] = None
 
     @property
-    def checked_agg_time_dimension(self) -> TimeDimensionReference:
-        if self.agg_time_dimension is not None:
-            return TimeDimensionReference(element_name=self.agg_time_dimension)
-        else:
-            raise Exception("Measure is missing agg_time_dimension!")
-
-    @property
     def reference(self) -> MeasureReference:
         return MeasureReference(element_name=self.name)
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/unparsed.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/unparsed.py`

 * *Files 0% similar despite different names*

```diff
@@ -685,23 +685,22 @@
     expr: Optional[str] = None
 
 
 @dataclass
 class UnparsedNonAdditiveDimension(dbtClassMixin):
     name: str
     window_choice: str  # AggregationType enum
-    window_grouples: List[str]
+    window_groupings: List[str]
 
 
 @dataclass
 class UnparsedMeasure(dbtClassMixin):
     name: str
     agg: str  # actually an enum
     description: Optional[str] = None
-    create_metric: bool = False
     expr: Optional[Union[str, bool, int]] = None
     agg_params: Optional[MeasureAggregationParameters] = None
     non_additive_dimension: Optional[UnparsedNonAdditiveDimension] = None
     agg_time_dimension: Optional[str] = None
 
 
 @dataclass
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/graph/utils.py` & `dbt-core-1.6.0rc1/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/project.py` & `dbt-core-1.6.0rc1/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/relation.py` & `dbt-core-1.6.0rc1/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/results.py` & `dbt-core-1.6.0rc1/dbt/contracts/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import threading
+
 from dbt.contracts.graph.unparsed import FreshnessThreshold
 from dbt.contracts.graph.nodes import SourceDefinition, ResultNode
 from dbt.contracts.util import (
     BaseArtifactMetadata,
     ArtifactMixin,
     VersionedSchema,
     Replaceable,
@@ -157,14 +159,28 @@
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
 
     @property
     def skipped(self):
         return self.status == RunStatus.Skipped
 
+    @classmethod
+    def from_node(cls, node: ResultNode, status: RunStatus, message: Optional[str]):
+        thread_id = threading.current_thread().name
+        return RunResult(
+            status=status,
+            thread_id=thread_id,
+            execution_time=0,
+            timing=[],
+            message=message,
+            node=node,
+            adapter_response={},
+            failures=None,
+        )
+
 
 @dataclass
 class ExecutionResult(dbtClassMixin):
     results: Sequence[BaseResult]
     elapsed_time: float
 
     def __len__(self):
```

### Comparing `dbt-core-1.6.0b8/dbt/contracts/selection.py` & `dbt-core-1.6.0rc1/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/sql.py` & `dbt-core-1.6.0rc1/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/state.py` & `dbt-core-1.6.0rc1/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/contracts/util.py` & `dbt-core-1.6.0rc1/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/dataclass_schema.py` & `dbt-core-1.6.0rc1/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deprecations.py` & `dbt-core-1.6.0rc1/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deps/base.py` & `dbt-core-1.6.0rc1/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deps/git.py` & `dbt-core-1.6.0rc1/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deps/local.py` & `dbt-core-1.6.0rc1/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deps/registry.py` & `dbt-core-1.6.0rc1/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deps/resolver.py` & `dbt-core-1.6.0rc1/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/deps/tarball.py` & `dbt-core-1.6.0rc1/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.6.0rc1/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/docs/source/conf.py` & `dbt-core-1.6.0rc1/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/events/adapter_endpoint.py` & `dbt-core-1.6.0rc1/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/events/base_types.py` & `dbt-core-1.6.0rc1/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/events/contextvars.py` & `dbt-core-1.6.0rc1/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/events/eventmgr.py` & `dbt-core-1.6.0rc1/dbt/events/eventmgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
             self._python_logger = self._get_python_log_for_handler(file_handler)
 
     def _get_python_log_for_handler(self, handler: logging.Handler):
         log = logging.getLogger(self.name)
         log.setLevel(_log_level_map[self.level])
         handler.setFormatter(logging.Formatter(fmt="%(message)s"))
         log.handlers.clear()
+        log.propagate = False
         log.addHandler(handler)
         return log
 
     def create_line(self, msg: EventMsg) -> str:
         raise NotImplementedError()
 
     def write_line(self, msg: EventMsg):
```

### Comparing `dbt-core-1.6.0b8/dbt/events/format.py` & `dbt-core-1.6.0rc1/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/events/functions.py` & `dbt-core-1.6.0rc1/dbt/events/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,26 @@
             _get_logbook_log_config(
                 flags.DEBUG, flags.USE_COLORS, flags.LOG_CACHE_EVENTS, flags.QUIET
             )
         )
     else:
         if flags.LOG_LEVEL != "none":
             line_format = _line_format_from_str(flags.LOG_FORMAT, LineFormat.PlainText)
-            log_level = EventLevel.DEBUG if flags.DEBUG else EventLevel(flags.LOG_LEVEL)
+            log_level = (
+                EventLevel.ERROR
+                if flags.QUIET
+                else EventLevel.DEBUG
+                if flags.DEBUG
+                else EventLevel(flags.LOG_LEVEL)
+            )
             console_config = _get_stdout_config(
                 line_format,
-                flags.DEBUG,
                 flags.USE_COLORS,
                 log_level,
                 flags.LOG_CACHE_EVENTS,
-                flags.QUIET,
             )
             EVENT_MANAGER.add_logger(console_config)
 
             if _CAPTURE_STREAM:
                 # Create second stdout logger to support test which want to know what's
                 # being sent to stdout.
                 console_config.output_stream = _CAPTURE_STREAM
@@ -77,50 +81,41 @@
         return LineFormat.Json
 
     return default
 
 
 def _get_stdout_config(
     line_format: LineFormat,
-    debug: bool,
     use_colors: bool,
     level: EventLevel,
     log_cache_events: bool,
-    quiet: bool,
 ) -> LoggerConfig:
 
     return LoggerConfig(
         name="stdout_log",
         level=level,
         use_colors=use_colors,
         line_format=line_format,
         scrubber=env_scrubber,
         filter=partial(
             _stdout_filter,
             log_cache_events,
-            debug,
-            quiet,
             line_format,
         ),
         output_stream=sys.stdout,
     )
 
 
 def _stdout_filter(
     log_cache_events: bool,
-    debug_mode: bool,
-    quiet_mode: bool,
     line_format: LineFormat,
     msg: EventMsg,
 ) -> bool:
-    return (
-        (msg.info.name not in ["CacheAction", "CacheDumpGraph"] or log_cache_events)
-        and (EventLevel(msg.info.level) != EventLevel.DEBUG or debug_mode)
-        and (EventLevel(msg.info.level) == EventLevel.ERROR or not quiet_mode)
-        and not (line_format == LineFormat.Json and type(msg.data) == Formatting)
+    return (msg.info.name not in ["CacheAction", "CacheDumpGraph"] or log_cache_events) and not (
+        line_format == LineFormat.Json and type(msg.data) == Formatting
     )
 
 
 def _get_logfile_config(
     log_path: str, use_colors: bool, line_format: LineFormat, level: EventLevel
 ) -> LoggerConfig:
     return LoggerConfig(
@@ -143,19 +138,17 @@
 
 
 def _get_logbook_log_config(
     debug: bool, use_colors: bool, log_cache_events: bool, quiet: bool
 ) -> LoggerConfig:
     config = _get_stdout_config(
         LineFormat.PlainText,
-        debug,
         use_colors,
-        EventLevel.DEBUG if debug else EventLevel.INFO,
+        EventLevel.ERROR if quiet else EventLevel.DEBUG if debug else EventLevel.INFO,
         log_cache_events,
-        quiet,
     )
     config.name = "logbook_log"
     config.filter = (
         NoFilter
         if log_cache_events
         else lambda e: e.info.name not in ["CacheAction", "CacheDumpGraph"]
     )
@@ -179,15 +172,15 @@
 # Since dbt-rpc does not do its own log setup, and since some events can
 # currently fire before logs can be configured by setup_event_logger(), we
 # create a default configuration with default settings and no file output.
 EVENT_MANAGER: EventManager = EventManager()
 EVENT_MANAGER.add_logger(
     _get_logbook_log_config(False, True, False, False)  # type: ignore
     if ENABLE_LEGACY_LOGGER
-    else _get_stdout_config(LineFormat.PlainText, False, True, EventLevel.INFO, False, False)
+    else _get_stdout_config(LineFormat.PlainText, True, EventLevel.INFO, False)
 )
 
 # This global, and the following two functions for capturing stdout logs are
 # an unpleasant hack we intend to remove as part of API-ification. The GitHub
 # issue #6350 was opened for that work.
 _CAPTURE_STREAM: Optional[TextIO] = None
```

### Comparing `dbt-core-1.6.0b8/dbt/events/helpers.py` & `dbt-core-1.6.0rc1/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/events/types.py` & `dbt-core-1.6.0rc1/dbt/events/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1212,14 +1212,30 @@
             f"Constraint types are not supported for {self.materialized} materializations and will "
             "be ignored.  Set 'warn_unsupported: false' on this constraint to ignore this warning."
         )
 
         return line_wrap_message(warning_tag(msg))
 
 
+class ParseInlineNodeError(ErrorLevel):
+    def code(self):
+        return "I069"
+
+    def message(self) -> str:
+        return "Error while parsing node: " + self.node_info.node_name + "\n" + self.exc
+
+
+class SemanticValidationFailure(WarnLevel):
+    def code(self):
+        return "I070"
+
+    def message(self) -> str:
+        return self.msg
+
+
 # =======================================================
 # M - Deps generation
 # =======================================================
 
 
 class GitSparseCheckoutSubdirectory(DebugLevel):
     def code(self):
```

### Comparing `dbt-core-1.6.0b8/dbt/exceptions.py` & `dbt-core-1.6.0rc1/dbt/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2326,14 +2326,19 @@
                 row = [yaml_col["name"], "", yaml_col["data_type"], "missing in definition"]
                 mismatches += [dict(zip(column_names, row))]
 
         mismatches_sorted = sorted(mismatches, key=lambda d: d["column_name"])
         return table_from_data_flat(mismatches_sorted, column_names)
 
     def get_message(self) -> str:
+        if not self.yaml_columns:
+            return (
+                "This model has an enforced contract, and its 'columns' specification is missing"
+            )
+
         table: agate.Table = self.get_mismatches()
         # Hack to get Agate table output as string
         output = io.StringIO()
         table.print_table(output=output, max_rows=None, max_column_width=50)  # type: ignore
         mismatches = output.getvalue()
 
         msg = (
```

### Comparing `dbt-core-1.6.0b8/dbt/flags.py` & `dbt-core-1.6.0rc1/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/graph/cli.py` & `dbt-core-1.6.0rc1/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/graph/graph.py` & `dbt-core-1.6.0rc1/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/graph/queue.py` & `dbt-core-1.6.0rc1/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/graph/selector.py` & `dbt-core-1.6.0rc1/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/graph/selector_methods.py` & `dbt-core-1.6.0rc1/dbt/graph/selector_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,22 +433,26 @@
             raise DbtRuntimeError(f'Invalid resource_type selector "{selector}"') from exc
         for node, real_node in self.parsed_nodes(included_nodes):
             if real_node.resource_type == resource_type:
                 yield node
 
 
 class TestNameSelectorMethod(SelectorMethod):
+    __test__ = False
+
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         for node, real_node in self.parsed_nodes(included_nodes):
             if real_node.resource_type == NodeType.Test and hasattr(real_node, "test_metadata"):
                 if fnmatch(real_node.test_metadata.name, selector):  # type: ignore[union-attr]
                     yield node
 
 
 class TestTypeSelectorMethod(SelectorMethod):
+    __test__ = False
+
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         search_type: Type
         # continue supporting 'schema' + 'data' for backwards compatibility
         if selector in ("generic", "schema"):
             search_type = GenericTestNode
         elif selector in ("singular", "data"):
             search_type = SingularTestNode
```

### Comparing `dbt-core-1.6.0b8/dbt/graph/selector_spec.py` & `dbt-core-1.6.0rc1/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/helper_types.py` & `dbt-core-1.6.0rc1/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/README.md` & `dbt-core-1.6.0rc1/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/docs/overview.md` & `dbt-core-1.6.0rc1/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/drop_relation.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/drop_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/clone/clone.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/clone/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/alter_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/get_materialized_view_configuration_changes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/materialized_view/replace_materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files 15% similar despite different names*

```diff
@@ -29,18 +29,25 @@
 {%- endmacro %}
 
 {#
   Compares the column schema provided by a model's sql file to the column schema provided by a model's schema file.
   If any differences in name, data_type or number of columns exist between the two schemas, raises a compiler error
 #}
 {% macro assert_columns_equivalent(sql) %}
+
+  {#-- First ensure the user has defined 'columns' in yaml specification --#}
+  {%- set user_defined_columns = model['columns'] -%}
+  {%- if not user_defined_columns -%}
+      {{ exceptions.raise_contract_error([], []) }}
+  {%- endif -%}
+
   {#-- Obtain the column schema provided by sql file. #}
   {%- set sql_file_provided_columns = get_column_schema_from_query(sql, config.get('sql_header', none)) -%}
   {#--Obtain the column schema provided by the schema file by generating an 'empty schema' query from the model's columns. #}
-  {%- set schema_file_provided_columns = get_column_schema_from_query(get_empty_schema_sql(model['columns'])) -%}
+  {%- set schema_file_provided_columns = get_column_schema_from_query(get_empty_schema_sql(user_defined_columns)) -%}
 
   {#-- create dictionaries with name and formatted data type and strings for exception #}
   {%- set sql_columns = format_columns(sql_file_provided_columns) -%}
   {%- set yaml_columns = format_columns(schema_file_provided_columns)  -%}
 
   {%- if sql_columns|length != yaml_columns|length -%}
     {%- do exceptions.raise_contract_error(yaml_columns, sql_columns) -%}
```

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
     split_part(
         {{ string_text }},
         {{ delimiter_text }},
           length({{ string_text }})
           - length(
               replace({{ string_text }},  {{ delimiter_text }}, '')
-          ) + 2 {{ part_number }}
+          ) + 2 + {{ part_number }}
         )
 
 {% endmacro %}
```

### Comparing `dbt-core-1.6.0b8/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.6.0rc1/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/index.html` & `dbt-core-1.6.0rc1/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/starter_project/README.md` & `dbt-core-1.6.0rc1/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.6.0rc1/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/internal_deprecations.py` & `dbt-core-1.6.0rc1/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/logger.py` & `dbt-core-1.6.0rc1/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/node_types.py` & `dbt-core-1.6.0rc1/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/__init__.py` & `dbt-core-1.6.0rc1/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/analysis.py` & `dbt-core-1.6.0rc1/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/base.py` & `dbt-core-1.6.0rc1/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/common.py` & `dbt-core-1.6.0rc1/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/docs.py` & `dbt-core-1.6.0rc1/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/generic_test.py` & `dbt-core-1.6.0rc1/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/generic_test_builders.py` & `dbt-core-1.6.0rc1/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/hooks.py` & `dbt-core-1.6.0rc1/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/macros.py` & `dbt-core-1.6.0rc1/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/manifest.py` & `dbt-core-1.6.0rc1/dbt/parser/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     Type,
     Union,
     Tuple,
     Set,
 )
 from itertools import chain
 import time
+
+from dbt.contracts.graph.semantic_manifest import SemanticManifest
 from dbt.events.base_types import EventLevel
 import json
 import pprint
 import msgpack
 
 import dbt.exceptions
 import dbt.tracking
@@ -512,14 +514,18 @@
             self.process_sources(self.root_project.project_name)
             self.process_refs(self.root_project.project_name, self.root_project.dependencies)
             self.process_docs(self.root_project)
             self.process_metrics(self.root_project)
             self.check_valid_group_config()
             self.check_valid_access_property()
 
+            semantic_manifest = SemanticManifest(self.manifest)
+            if not semantic_manifest.validate():
+                raise dbt.exceptions.ParsingError("Semantic Manifest validation failed.")
+
             # update tracking data
             self._perf_info.process_manifest_elapsed = time.perf_counter() - start_process
             self._perf_info.static_analysis_parsed_path_count = (
                 self.manifest._parsing_info.static_analysis_parsed_path_count
             )
             self._perf_info.static_analysis_path_count = (
                 self.manifest._parsing_info.static_analysis_path_count
@@ -838,18 +844,21 @@
                     or macro.file_id in self.partial_parser.file_diff["added"]
                 ):
                     # The file with the macro in it has changed
                     return True
         return False
 
     def read_manifest_for_partial_parse(self) -> Optional[Manifest]:
-        if not get_flags().PARTIAL_PARSE:
+        flags = get_flags()
+        if not flags.PARTIAL_PARSE:
             fire_event(PartialParsingNotEnabled())
             return None
-        path = os.path.join(self.root_project.project_target_path, PARTIAL_PARSE_FILE_NAME)
+        path = flags.PARTIAL_PARSE_FILE_PATH or os.path.join(
+            self.root_project.project_target_path, PARTIAL_PARSE_FILE_NAME
+        )
 
         reparse_reason = None
 
         if os.path.exists(path):
             try:
                 with open(path, "rb") as fp:
                     manifest_mp = fp.read()
@@ -1441,28 +1450,40 @@
 
 
 def _process_metric_node(
     manifest: Manifest,
     current_project: str,
     metric: Metric,
 ) -> None:
-    """Sets a metric's input_measures"""
+    """Sets a metric's `input_measures` and `depends_on` properties"""
 
     # This ensures that if this metrics input_measures have already been set
     # we skip the work. This could happen either due to recursion or if multiple
     # metrics derive from another given metric.
     # NOTE: This does not protect against infinite loops
     if len(metric.type_params.input_measures) > 0:
         return
 
     if metric.type is MetricType.SIMPLE or metric.type is MetricType.CUMULATIVE:
         assert (
             metric.type_params.measure is not None
         ), f"{metric} should have a measure defined, but it does not."
         metric.type_params.input_measures.append(metric.type_params.measure)
+        target_semantic_model = manifest.resolve_semantic_model_for_measure(
+            target_measure_name=metric.type_params.measure.name,
+            current_project=current_project,
+            node_package=metric.package_name,
+        )
+        if target_semantic_model is None:
+            raise dbt.exceptions.ParsingError(
+                f"A semantic model having a measure `{metric.type_params.measure.name}` does not exist but was referenced.",
+                node=metric,
+            )
+
+        metric.depends_on.add_node(target_semantic_model.unique_id)
 
     elif metric.type is MetricType.DERIVED or metric.type is MetricType.RATIO:
         input_metrics = metric.input_metrics
         if metric.type is MetricType.RATIO:
             if metric.type_params.numerator is None or metric.type_params.denominator is None:
                 raise dbt.exceptions.ParsingError(
                     "Invalid ratio metric. Both a numerator and denominator must be specified",
@@ -1489,14 +1510,15 @@
                     node=metric,
                 )
 
             _process_metric_node(
                 manifest=manifest, current_project=current_project, metric=target_metric
             )
             metric.type_params.input_measures.extend(target_metric.type_params.input_measures)
+            metric.depends_on.add_node(target_metric.unique_id)
     else:
         assert_values_exhausted(metric.type)
 
 
 def _process_metrics_for_node(
     manifest: Manifest,
     current_project: str,
@@ -1647,15 +1669,16 @@
     _process_refs(manifest, config.project_name, node, config.dependencies)
     ctx = generate_runtime_docs_context(config, node, manifest, config.project_name)
     _process_docs_for_node(ctx, node)
 
 
 def write_semantic_manifest(manifest: Manifest, target_path: str) -> None:
     path = os.path.join(target_path, SEMANTIC_MANIFEST_FILE_NAME)
-    write_file(path, manifest.pydantic_semantic_manifest.json())
+    semantic_manifest = SemanticManifest(manifest)
+    semantic_manifest.write_json_to_file(path)
 
 
 def write_manifest(manifest: Manifest, target_path: str):
     path = os.path.join(target_path, MANIFEST_FILE_NAME)
     manifest.write(path)
 
     write_semantic_manifest(manifest=manifest, target_path=target_path)
```

### Comparing `dbt-core-1.6.0b8/dbt/parser/models.py` & `dbt-core-1.6.0rc1/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/partial.py` & `dbt-core-1.6.0rc1/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/read_files.py` & `dbt-core-1.6.0rc1/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/schema_generic_tests.py` & `dbt-core-1.6.0rc1/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/schema_renderer.py` & `dbt-core-1.6.0rc1/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/schema_yaml_readers.py` & `dbt-core-1.6.0rc1/dbt/parser/schema_yaml_readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,28 +482,27 @@
     def _get_non_additive_dimension(
         self, unparsed: Optional[UnparsedNonAdditiveDimension]
     ) -> Optional[NonAdditiveDimension]:
         if unparsed is not None:
             return NonAdditiveDimension(
                 name=unparsed.name,
                 window_choice=AggregationType(unparsed.window_choice),
-                window_grouples=unparsed.window_grouples,
+                window_groupings=unparsed.window_groupings,
             )
         else:
             return None
 
     def _get_measures(self, unparsed_measures: List[UnparsedMeasure]) -> List[Measure]:
         measures: List[Measure] = []
         for unparsed in unparsed_measures:
             measures.append(
                 Measure(
                     name=unparsed.name,
                     agg=AggregationType(unparsed.agg),
                     description=unparsed.description,
-                    create_metric=unparsed.create_metric,
                     expr=str(unparsed.expr) if unparsed.expr is not None else None,
                     agg_params=unparsed.agg_params,
                     non_additive_dimension=self._get_non_additive_dimension(
                         unparsed.non_additive_dimension
                     ),
                     agg_time_dimension=unparsed.agg_time_dimension,
                 )
```

### Comparing `dbt-core-1.6.0b8/dbt/parser/schemas.py` & `dbt-core-1.6.0rc1/dbt/parser/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,14 +647,16 @@
                             node_name=patch.name,
                         )
                     )
 
 
 # TestablePatchParser = seeds, snapshots
 class TestablePatchParser(NodePatchParser[UnparsedNodeUpdate]):
+    __test__ = False
+
     def get_block(self, node: UnparsedNodeUpdate) -> TestBlock:
         return TestBlock.from_yaml_block(self.yaml, node)
 
     def _target_type(self) -> Type[UnparsedNodeUpdate]:
         return UnparsedNodeUpdate
 
 
@@ -780,14 +782,17 @@
                 # Node patched before config because config patching depends on model name,
                 # which may have been updated in the version patch
                 # versioned_model_node.patch(versioned_model_patch)
                 self.patch_node_properties(versioned_model_node, versioned_model_patch)
 
                 # Includes alias recomputation
                 self.patch_node_config(versioned_model_node, versioned_model_patch)
+
+                # Need to reapply this here, in the case that 'contract: {enforced: true}' was during config-setting
+                versioned_model_node.build_contract_checksum()
                 source_file.append_patch(
                     versioned_model_patch.yaml_key, versioned_model_node.unique_id
                 )
             self.manifest.rebuild_ref_lookup()
             self.manifest.rebuild_disabled_lookup()
 
     def _target_type(self) -> Type[UnparsedModelUpdate]:
```

### Comparing `dbt-core-1.6.0b8/dbt/parser/search.py` & `dbt-core-1.6.0rc1/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/seeds.py` & `dbt-core-1.6.0rc1/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/singular_test.py` & `dbt-core-1.6.0rc1/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/snapshots.py` & `dbt-core-1.6.0rc1/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/sources.py` & `dbt-core-1.6.0rc1/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/parser/sql.py` & `dbt-core-1.6.0rc1/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/plugins/__init__.py` & `dbt-core-1.6.0rc1/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/plugins/manager.py` & `dbt-core-1.6.0rc1/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/plugins/manifest.py` & `dbt-core-1.6.0rc1/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/semver.py` & `dbt-core-1.6.0rc1/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/base.py` & `dbt-core-1.6.0rc1/dbt/task/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,27 +292,14 @@
             timing_info=timing_info,
             message=result.message,
             agate_table=result.agate_table,
             adapter_response=result.adapter_response,
             failures=result.failures,
         )
 
-    def skip_result(self, node, message):
-        thread_id = threading.current_thread().name
-        return RunResult(
-            status=RunStatus.Skipped,
-            thread_id=thread_id,
-            execution_time=0,
-            timing=[],
-            message=message,
-            node=node,
-            adapter_response={},
-            failures=None,
-        )
-
     def compile_and_execute(self, manifest, ctx):
         result = None
         with self.adapter.connection_for(self.node) if get_flags().INTROSPECT else nullcontext():
             ctx.node.update_event_status(node_status=RunningStatus.Compiling)
             fire_event(
                 NodeCompiling(
                     node_info=ctx.node.node_info,
@@ -479,13 +466,13 @@
                         node_name=node_name,
                         index=self.node_index,
                         total=self.num_nodes,
                         node_info=self.node.node_info,
                     )
                 )
 
-        node_result = self.skip_result(self.node, error_message)
+        node_result = RunResult.from_node(self.node, RunStatus.Skipped, error_message)
         return node_result
 
     def do_skip(self, cause=None):
         self.skip = True
         self.skip_cause = cause
```

### Comparing `dbt-core-1.6.0b8/dbt/task/build.py` & `dbt-core-1.6.0rc1/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/clean.py` & `dbt-core-1.6.0rc1/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/clone.py` & `dbt-core-1.6.0rc1/dbt/task/clone.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/compile.py` & `dbt-core-1.6.0rc1/dbt/task/compile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import threading
 from typing import AbstractSet, Optional
 
 from dbt.contracts.graph.manifest import WritableManifest
 from dbt.contracts.results import RunStatus, RunResult
 from dbt.events.base_types import EventLevel
 from dbt.events.functions import fire_event
-from dbt.events.types import CompiledNode, Note
-from dbt.exceptions import DbtInternalError
+from dbt.events.types import CompiledNode, Note, ParseInlineNodeError
+from dbt.exceptions import (
+    CompilationError,
+    DbtInternalError,
+    Exception as DbtException,
+)
+
 from dbt.graph import ResourceTypeSelector
 from dbt.node_types import NodeType
 from dbt.parser.manifest import write_manifest, process_node
 from dbt.parser.sql import SqlBlockParser
 from dbt.task.base import BaseRunner
 from dbt.task.runnable import GraphRunnableTask
 
@@ -114,22 +119,34 @@
             favor_state=bool(self.args.favor_state),
         )
         # TODO: is it wrong to write the manifest here? I think it's right...
         write_manifest(self.manifest, self.config.project_target_path)
 
     def _runtime_initialize(self):
         if getattr(self.args, "inline", None):
-            block_parser = SqlBlockParser(
-                project=self.config, manifest=self.manifest, root_project=self.config
-            )
-            sql_node = block_parser.parse_remote(self.args.inline, "inline_query")
-            process_node(self.config, self.manifest, sql_node)
-            # keep track of the node added to the manifest
-            self._inline_node_id = sql_node.unique_id
-
+            try:
+                block_parser = SqlBlockParser(
+                    project=self.config, manifest=self.manifest, root_project=self.config
+                )
+                sql_node = block_parser.parse_remote(self.args.inline, "inline_query")
+                process_node(self.config, self.manifest, sql_node)
+                # keep track of the node added to the manifest
+                self._inline_node_id = sql_node.unique_id
+            except CompilationError as exc:
+                fire_event(
+                    ParseInlineNodeError(
+                        exc=str(exc.msg),
+                        node_info={
+                            "node_path": "sql/inline_query",
+                            "node_name": "inline_query",
+                            "unique_id": "sqloperation.test.inline_query",
+                        },
+                    )
+                )
+                raise DbtException("Error parsing inline query")
         super()._runtime_initialize()
 
     def after_run(self, adapter, results):
         # remove inline node from manifest
         if self._inline_node_id:
             self.manifest.nodes.pop(self._inline_node_id)
             self._inline_node_id = None
```

### Comparing `dbt-core-1.6.0b8/dbt/task/debug.py` & `dbt-core-1.6.0rc1/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/deps.py` & `dbt-core-1.6.0rc1/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/freshness.py` & `dbt-core-1.6.0rc1/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/generate.py` & `dbt-core-1.6.0rc1/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/init.py` & `dbt-core-1.6.0rc1/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/list.py` & `dbt-core-1.6.0rc1/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/printer.py` & `dbt-core-1.6.0rc1/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/retry.py` & `dbt-core-1.6.0rc1/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/run.py` & `dbt-core-1.6.0rc1/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/run_operation.py` & `dbt-core-1.6.0rc1/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/runnable.py` & `dbt-core-1.6.0rc1/dbt/task/runnable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 import os
 import time
-from pathlib import Path
 from abc import abstractmethod
 from concurrent.futures import as_completed
 from datetime import datetime
 from multiprocessing.dummy import Pool as ThreadPool
+from pathlib import Path
 from typing import Optional, Dict, List, Set, Tuple, Iterable, AbstractSet
 
-from .printer import (
-    print_run_result_error,
-    print_run_end_messages,
-)
-
-from dbt.task.base import ConfiguredTask
+import dbt.exceptions
+import dbt.tracking
+import dbt.utils
 from dbt.adapters.base import BaseRelation
 from dbt.adapters.factory import get_adapter
-from dbt.logger import (
-    DbtProcessState,
-    TextOnly,
-    UniqueID,
-    TimestampNamed,
-    DbtModelState,
-    ModelMetadata,
-    NodeCount,
+from dbt.contracts.graph.manifest import WritableManifest
+from dbt.contracts.graph.nodes import ResultNode
+from dbt.contracts.results import (
+    NodeStatus,
+    RunExecutionResult,
+    RunningStatus,
+    RunResult,
+    RunStatus,
 )
+from dbt.contracts.state import PreviousState
+from dbt.events.contextvars import log_contextvars, task_contextvars
 from dbt.events.functions import fire_event, warn_or_error
 from dbt.events.types import (
     Formatting,
     LogCancelLine,
     DefaultSelector,
     NodeStart,
     NodeFinished,
     QueryCancelationUnsupported,
     ConcurrencyLine,
     EndRunResult,
     NothingToDo,
 )
-from dbt.events.contextvars import log_contextvars, task_contextvars
-from dbt.contracts.graph.nodes import ResultNode
-from dbt.contracts.results import NodeStatus, RunExecutionResult, RunningStatus
-from dbt.contracts.state import PreviousState
 from dbt.exceptions import (
     DbtInternalError,
     NotImplementedError,
     DbtRuntimeError,
     FailFastError,
 )
-
+from dbt.flags import get_flags
 from dbt.graph import GraphQueue, NodeSelector, SelectionSpec, parse_difference
+from dbt.logger import (
+    DbtProcessState,
+    TextOnly,
+    UniqueID,
+    TimestampNamed,
+    DbtModelState,
+    ModelMetadata,
+    NodeCount,
+)
 from dbt.parser.manifest import write_manifest
-import dbt.tracking
-
-import dbt.exceptions
-from dbt.flags import get_flags
-import dbt.utils
-from dbt.contracts.graph.manifest import WritableManifest
+from dbt.task.base import ConfiguredTask
+from .printer import (
+    print_run_result_error,
+    print_run_end_messages,
+)
 
 RESULT_FILE_NAME = "run_results.json"
 RUNNING_STATE = DbtProcessState("running")
 
 
 class GraphRunnableTask(ConfiguredTask):
     MARK_DEPENDENT_ERRORS_STATUSES = [NodeStatus.Error]
@@ -356,29 +359,35 @@
             )
         with TextOnly():
             fire_event(Formatting(""))
 
         pool = ThreadPool(num_threads)
         try:
             self.run_queue(pool)
-
         except FailFastError as failure:
             self._cancel_connections(pool)
+
+            executed_node_ids = [r.node.unique_id for r in self.node_results]
+
+            for r in self._flattened_nodes:
+                if r.unique_id not in executed_node_ids:
+                    self.node_results.append(
+                        RunResult.from_node(r, RunStatus.Skipped, "Skipping due to fail_fast")
+                    )
+
             print_run_result_error(failure.result)
             raise
-
         except KeyboardInterrupt:
             self._cancel_connections(pool)
             print_run_end_messages(self.node_results, keyboard_interrupt=True)
             raise
-
-        pool.close()
-        pool.join()
-
-        return self.node_results
+        finally:
+            pool.close()
+            pool.join()
+            return self.node_results
 
     def _mark_dependent_errors(self, node_id, result, cause):
         if self.graph is None:
             raise DbtInternalError("graph is None in _mark_dependent_errors")
         for dep_node_id in self.graph.get_dependent_nodes(node_id):
             self._skipped_children[dep_node_id] = cause
```

### Comparing `dbt-core-1.6.0b8/dbt/task/seed.py` & `dbt-core-1.6.0rc1/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/serve.py` & `dbt-core-1.6.0rc1/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/show.py` & `dbt-core-1.6.0rc1/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/snapshot.py` & `dbt-core-1.6.0rc1/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/sql.py` & `dbt-core-1.6.0rc1/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/task/test.py` & `dbt-core-1.6.0rc1/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/tests/fixtures/project.py` & `dbt-core-1.6.0rc1/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/tests/util.py` & `dbt-core-1.6.0rc1/dbt/tests/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     fire_event,
     capture_stdout_logs,
     stop_capture_stdout_logs,
     reset_metadata_vars,
 )
 from dbt.events.base_types import EventLevel
 from dbt.events.types import Note
-
+from dbt.adapters.base.relation import BaseRelation
 
 # =============================================================================
 # Test utilities
 #   run_dbt
 #   run_dbt_and_capture
 #   get_manifest
 #   copy_file
@@ -584,7 +584,36 @@
         if self.contains is None:
             return True
 
         return self.contains in other
 
     def __repr__(self):
         return "AnyStringWith<{!r}>".format(self.contains)
+
+
+def assert_message_in_logs(message: str, logs: str, expected_pass: bool = True):
+    # if the logs are json strings, then 'jsonify' the message because of things like escape quotes
+    if os.environ.get("DBT_LOG_FORMAT", "") == "json":
+        message = message.replace(r'"', r"\"")
+
+    if expected_pass:
+        assert message in logs
+    else:
+        assert message not in logs
+
+
+def get_project_config(project):
+    file_yaml = read_file(project.project_root, "dbt_project.yml")
+    return yaml.safe_load(file_yaml)
+
+
+def set_project_config(project, config):
+    config_yaml = yaml.safe_dump(config)
+    write_file(config_yaml, project.project_root, "dbt_project.yml")
+
+
+def get_model_file(project, relation: BaseRelation) -> str:
+    return read_file(project.project_root, "models", f"{relation.name}.sql")
+
+
+def set_model_file(project, relation: BaseRelation, model_sql: str):
+    write_file(model_sql, project.project_root, "models", f"{relation.name}.sql")
```

### Comparing `dbt-core-1.6.0b8/dbt/tracking.py` & `dbt-core-1.6.0rc1/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/ui.py` & `dbt-core-1.6.0rc1/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/utils.py` & `dbt-core-1.6.0rc1/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.6.0b8/dbt/version.py` & `dbt-core-1.6.0rc1/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.6.0b8"
+__version__ = "1.6.0rc1"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.6.0b8/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.6.0rc1/dbt_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.6.0b8
+Version: 1.6.0rc1
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0b8 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.6.0rc1 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `dbt-core-1.6.0b8/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.6.0rc1/dbt_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 dbt/contracts/graph/manifest.py
 dbt/contracts/graph/manifest_upgrade.py
 dbt/contracts/graph/metrics.py
 dbt/contracts/graph/model_config.py
 dbt/contracts/graph/node_args.py
 dbt/contracts/graph/nodes.py
 dbt/contracts/graph/searcher.py
+dbt/contracts/graph/semantic_manifest.py
 dbt/contracts/graph/semantic_models.py
 dbt/contracts/graph/unparsed.py
 dbt/contracts/graph/utils.py
 dbt/deps/__init__.py
 dbt/deps/base.py
 dbt/deps/git.py
 dbt/deps/local.py
@@ -139,14 +140,15 @@
 dbt/include/global_project/macros/adapters/freshness.sql
 dbt/include/global_project/macros/adapters/indexes.sql
 dbt/include/global_project/macros/adapters/metadata.sql
 dbt/include/global_project/macros/adapters/persist_docs.sql
 dbt/include/global_project/macros/adapters/relation.sql
 dbt/include/global_project/macros/adapters/schema.sql
 dbt/include/global_project/macros/adapters/timestamps.sql
+dbt/include/global_project/macros/adapters/validate_sql.sql
 dbt/include/global_project/macros/etc/datetime.sql
 dbt/include/global_project/macros/etc/statement.sql
 dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
 dbt/include/global_project/macros/generic_test_sql/not_null.sql
 dbt/include/global_project/macros/generic_test_sql/relationships.sql
 dbt/include/global_project/macros/generic_test_sql/unique.sql
 dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
```

### Comparing `dbt-core-1.6.0b8/setup.py` & `dbt-core-1.6.0rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.6.0b8"
+package_version = "1.6.0rc1"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -55,15 +55,16 @@
         # ----
         # Legacy: This package has not been updated since 2019, and it is unused in dbt's logging system (since v1.0)
         # The dependency here will be removed along with the removal of 'legacy logging', in a future release of dbt-core
         "logbook>=1.5,<1.6",
         # ----
         # dbt-core uses these packages in standard ways. Pin to the major version, and check compatibility
         # with major versions in each new minor version of dbt-core.
-        "click>=7.0,<9",
+        # temporarily pinning click for mypy failures: https://github.com/pallets/click/issues/2558
+        "click>=8.1.1,<8.1.4",
         "networkx>=2.3,<4",
         # ----
         # These packages are major-version-0. Keep upper bounds on upcoming minor versions (which could have breaking changes)
         # and check compatibility / bump in each new minor version of dbt-core.
         "colorama>=0.3.9,<0.5",
         "pathspec>=0.9,<0.12",
         "isodate>=0.6,<0.7",
@@ -73,15 +74,15 @@
         # ----
         # These are major-version-0 packages also maintained by dbt-labs. Accept patches.
         "dbt-extractor~=0.4.1",
         "hologram~=0.0.16",  # includes transitive dependencies on python-dateutil and jsonschema
         "minimal-snowplow-tracker~=0.0.2",
         # DSI is under active development, so we're pinning to specific dev versions for now.
         # TODO: Before RC/final release, update to use ~= pinning.
-        "dbt-semantic-interfaces==0.1.0.dev8",
+        "dbt-semantic-interfaces~=0.1.0rc1",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "packaging>20.9",
         "protobuf>=4.0.0",
         "pytz>=2015.7",
         "pyyaml>=6.0",
         "typing-extensions>=3.7.4",
```

