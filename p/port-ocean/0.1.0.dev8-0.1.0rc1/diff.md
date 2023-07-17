# Comparing `tmp/port_ocean-0.1.0.dev8.tar.gz` & `tmp/port_ocean-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev8.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0rc1.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev8.tar` & `port_ocean-0.1.0rc1.tar`

### file list

```diff
@@ -1,80 +1,89 @@
--rw-r--r--   0        0        0     4561 2023-07-09 15:01:27.476122 port_ocean-0.1.0.dev8/README.md
--rw-r--r--   0        0        0      537 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5122 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0      449 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1699 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      405 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       71 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1167 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1755 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      722 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2528 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2700 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     5995 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3051 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2319 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/config/base.py
--rw-r--r--   0        0        0     1066 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3991 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/context/event.py
--rw-r--r--   0        0        0     4038 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/base.py
--rw-r--r--   0        0        0      300 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0      946 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     2674 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      452 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1432 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      852 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/get_related_entities.py
--rw-r--r--   0        0        0      988 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     7761 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1375 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     1976 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2557 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     9891 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      389 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/base.py
--rw-r--r--   0        0        0     2864 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/factory.py
--rw-r--r--   0        0        0      898 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/http.py
--rw-r--r--   0        0        0     3238 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/kafka.py
--rw-r--r--   0        0        0      909 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/settings.py
--rw-r--r--   0        0        0      563 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/types.py
--rw-r--r--   0        0        0     1924 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      473 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      670 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4325 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/ocean.py
--rw-r--r--   0        0        0      770 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/utils.py
--rw-r--r--   0        0        0     2024 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     5646 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 09:45:56.503705 port_ocean-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     4585 2023-07-17 09:45:56.507705 port_ocean-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      614 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5081 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0      388 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      598 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1699 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      653 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog_fragments/.gitignore
+-rw-r--r--   0        0        0      778 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       71 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1267 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      722 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2664 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     5666 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3085 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2277 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1053 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0      966 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4058 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4044 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/base.py
+-rw-r--r--   0        0        0      593 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     3083 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/http/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/kafka/__init__.py
+-rw-r--r--   0        0        0     3123 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/event_listener/sample/utils.py
+-rw-r--r--   0        0        0      716 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      863 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7855 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1339 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      949 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2679 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1432 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1966 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2706 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    11343 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/models.py
+-rw-r--r--   0        0        0      563 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/types.py
+-rw-r--r--   0        0        0     1916 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      670 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4220 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/ocean.py
+-rw-r--r--   0        0        0     1007 2023-07-17 09:45:56.535705 port_ocean-0.1.0rc1/port_ocean/utils.py
+-rw-r--r--   0        0        0     2741 2023-07-17 09:45:56.539705 port_ocean-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6202 1970-01-01 00:00:00.000000 port_ocean-0.1.0rc1/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev8/README.md` & `port_ocean-0.1.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
-[![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
+[![Lint](https://github.com/port-labs/Port-Ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
 Ocean is an innovative solution developed by Port to seamlessly integrate various third-party systems with our developer portal product,
 empowering engineers to effortlessly prioritize key features and streamline the integration process.
 
 ## Prerequisites
 
 - Python 3.11
@@ -42,27 +42,27 @@
 
 ![image](./assets/ExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/RealTimeUpdatesArchitecture.svg)
 
 ## Folder Structure
-The Integration Framework follows a specific folder structure within the mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
+The Ocean Integration Framework follows a specific folder structure within this mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
 port-ocean/
 ├── port_ocean (framework)/
 │ ├── ocean.py
 │ ├── core/
 | └── ...
 └── integrations/
-│  ├───integration_name/
-│  ├──── main.py
-│  ├──── pyproject.toml
-│  └──── Dockerfile
+│  └─── integration_name/
+│     ├──── main.py
+│     ├──── pyproject.toml
+│     └──── Dockerfile
 ├── ...
 └── ...
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
@@ -80,16 +80,16 @@
 # This is an example configuration file for the integration service.
 # Please copy this file to config.yaml file in the integration folder and edit it to your needs.
 
 port:
   clientId: PORT_CLIENT_ID # Can be loaded via environment variable: PORT_CLIENT_ID
   clientSecret: PORT_CLIENT_SECRET # Can be loaded via environment variable: PORT_CLIENT_SECRET
   baseUrl: https://api.getport.io/v1
-# The trigger channel to use for the integration service.
-triggerChannel:
+# The event listener to use for the integration service.
+eventListener:
   type: KAFKA / WEBHOOK
 integration:
   # The name of the integration.
   identifier: "my_integration"
   # The type of the integration.
   type: "PagerDuty"
   config:
@@ -156,11 +156,11 @@
    Or
 
    ```sh
    ocean sail
    ```
 
 ## License
-The Integration Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the `LICENSE` file for more details.
+The Ocean Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the [LICENSE](./LICENSE) file for more information.
 
 ## Contact
 For any questions or inquiries, please reach out to our team at support@getport.io
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/__init__.py` & `port_ocean-0.1.0rc1/port_ocean/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import warnings
+from importlib.metadata import version
 from importlib.util import find_spec
 
+__version__ = version("port-ocean")
+
 warnings.filterwarnings("ignore", category=FutureWarning)
 
+
 try:
     find_spec("click")
     find_spec("cookiecutter")
     find_spec("rich")
     find_spec("toml")
 
     cli_included = True
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/commands.py` & `port_ocean-0.1.0rc1/port_ocean/cli/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # ruff: noqa: E501
 import os
 
 import click
-import toml
 from cookiecutter.main import cookiecutter  # type: ignore
 from rich.console import Console
 
+from port_ocean import __version__
 from port_ocean.cli.download_git_folder import download_github_folder
 from port_ocean.cli.list_integrations import list_git_folders
 from port_ocean.config.integration import LogLevelType
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 console = Console()
 
@@ -49,19 +49,18 @@
     required=False,
     help="Display only the short version number.",
 )
 def version(short: bool) -> None:
     """
     Displays the version of the Ocean package.
     """
-    app_version = toml.load("pyproject.toml")["tool"]["poetry"]["version"]
     if short:
-        console.print(f"{app_version}")
+        console.print(__version__)
     else:
-        console.print(f"🌊 Ocean version: {app_version}")
+        console.print(f"🌊 Ocean version: {__version__}")
 
 
 @cli_start.command()
 @click.argument("path", default=".", type=click.Path(exists=True))
 @click.option(
     "-l",
     "--log-level",
@@ -125,15 +124,15 @@
 
 @cli_start.command(name="list")
 def list_integrations() -> None:
     """
     List all available public integrations.
     """
     console.print("🌊 Here are the integrations available to you:", style="bold")
-    options = list_git_folders("port-labs", "pulumi", "examples")
+    options = list_git_folders("port-labs", "port-ocean", "integrations")
 
     for option in options:
         console.print(f"⚓️ [bold][blue]{option}[/blue][/bold]")
 
 
 @cli_start.command()
 @click.argument("name", type=str)
@@ -148,9 +147,9 @@
 def pull(name: str, path: str) -> None:
     """
     Pull an integration bt the NAME from the list of available public integrations.
 
     NAME: Name of the integration to pull.
     """
     download_github_folder(
-        "port-labs", "pulumi", f"examples/{name}", path or f"./{name}"
+        "port-labs", "Port-Ocean", f"integrations/{name}", path or f"./{name}"
     )
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0rc1/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 port_ocean = { version = "^0.1.0.dev3", extras = ["cli"] }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
+towncrier = "^23.6.0"
+
+[tool.towncrier]
+directory = "changelog_fragments"
+filename = "CHANGELOG.md"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy]
 plugins = [
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0rc1/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0rc1/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.0rc1/port_ocean/clients/port/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,37 +22,38 @@
     def full_token(self) -> str:
         return f"{self.token_type} {self.access_token}"
 
 
 class PortAuthentication:
     def __init__(
         self,
+        client: httpx.AsyncClient,
         client_id: str,
         client_secret: str,
         api_url: str,
         integration_identifier: str,
         integration_type: str,
     ):
+        self.client = client
         self.api_url = api_url
         self.client_id = client_id
         self.client_secret = client_secret
         self.integration_identifier = integration_identifier
         self.integration_type = integration_type
         self._last_token_object: TokenResponse | None = None
 
     async def _get_token(self, client_id: str, client_secret: str) -> TokenResponse:
-        async with httpx.AsyncClient() as client:
-            logger.info(f"Fetching access token for clientId: {client_id}")
+        logger.info(f"Fetching access token for clientId: {client_id}")
 
-            credentials = {"clientId": client_id, "clientSecret": client_secret}
-            token_response = await client.post(
-                f"{self.api_url}/auth/access_token", json=credentials
-            )
-            token_response.raise_for_status()
-            return TokenResponse(**token_response.json())
+        credentials = {"clientId": client_id, "clientSecret": client_secret}
+        token_response = await self.client.post(
+            f"{self.api_url}/auth/access_token", json=credentials
+        )
+        token_response.raise_for_status()
+        return TokenResponse(**token_response.json())
 
     def user_agent(self, user_agent_type: UserAgentType | None = None) -> str:
         user_agent = f"port-ocean/{self.integration_type}/{self.integration_identifier}"
         if user_agent_type:
             user_agent += f"/{user_agent_type.value or UserAgentType.exporter.value}"
 
         return user_agent
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/clients/port/client.py` & `port_ocean-0.1.0rc1/port_ocean/clients/port/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,56 +18,57 @@
         base_url: str,
         client_id: str,
         client_secret: str,
         integration_identifier: str,
         integration_type: str,
     ):
         self.api_url = f"{base_url}/v1"
+        self.client = httpx.AsyncClient()
         self.auth = PortAuthentication(
+            self.client,
             client_id,
             client_secret,
             self.api_url,
             integration_identifier,
             integration_type,
         )
-        EntityClientMixin.__init__(self, self.auth)
-        IntegrationClientMixin.__init__(self, self.auth)
+        EntityClientMixin.__init__(self, self.auth, self.client)
+        IntegrationClientMixin.__init__(
+            self, integration_identifier, self.auth, self.client
+        )
 
     async def get_kafka_creds(self, silent: bool = False) -> KafkaCreds:
         logger.info("Fetching organization kafka credentials")
-        async with httpx.AsyncClient() as client:
-            response = await client.get(
-                f"{self.api_url}/kafka-credentials", headers=await self.auth.headers()
-            )
+        response = await self.client.get(
+            f"{self.api_url}/kafka-credentials", headers=await self.auth.headers()
+        )
         if response.is_error:
             logger.error(f"Error getting kafka credentials, error: {response.text}")
         handle_status_code(silent, response)
 
         credentials = response.json().get("credentials")
 
         if credentials is None:
             raise KafkaCredentialsNotFound("No kafka credentials found")
 
         return credentials
 
     async def get_org_id(self) -> str:
         logger.info("Fetching organization id")
 
-        async with httpx.AsyncClient() as client:
-            response = await client.get(
-                f"{self.api_url}/organization", headers=await self.auth.headers()
-            )
+        response = await self.client.get(
+            f"{self.api_url}/organization", headers=await self.auth.headers()
+        )
         if response.is_error:
             logger.error(f"Error getting organization id, error: {response.text}")
             response.raise_for_status()
 
         return response.json()["organization"]["id"]
 
     async def get_blueprint(self, identifier: str) -> Blueprint:
         logger.info(f"Fetching blueprint with id: {identifier}")
-        async with httpx.AsyncClient() as client:
-            response = await client.get(
-                f"{self.api_url}/blueprints/{identifier}",
-                headers=await self.auth.headers(),
-            )
+        response = await self.client.get(
+            f"{self.api_url}/blueprints/{identifier}",
+            headers=await self.auth.headers(),
+        )
         response.raise_for_status()
         return Blueprint.parse_obj(response.json()["blueprint"])
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 from port_ocean.clients.port.authentication import PortAuthentication
 from port_ocean.clients.port.types import RequestOptions, UserAgentType
 from port_ocean.clients.port.utils import handle_status_code
 from port_ocean.core.models import Entity
 
 
 class EntityClientMixin:
-    def __init__(self, auth: PortAuthentication):
+    def __init__(self, auth: PortAuthentication, client: httpx.AsyncClient):
         self.auth = auth
+        self.client = client
 
     async def upsert_entity(
         self,
         entity: Entity,
         request_options: RequestOptions,
         user_agent_type: UserAgentType | None = None,
         silent: bool = False,
     ) -> None:
         validation_only = request_options.get("validation_only", False)
         logger.info(
             f"{'Validating' if validation_only else 'Upserting'} entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         headers = await self.auth.headers(user_agent_type)
 
-        async with httpx.AsyncClient() as client:
-            response = await client.post(
-                f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities",
-                json=entity.dict(exclude_unset=True),
-                headers=headers,
-                params={
-                    "upsert": "true",
-                    "merge": str(request_options.get("merge", False)).lower(),
-                    "create_missing_related_entities": str(
-                        request_options.get("create_missing_related_entities", False)
-                    ).lower(),
-                    "validation_only": str(validation_only).lower(),
-                },
-            )
+        response = await self.client.post(
+            f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities",
+            json=entity.dict(exclude_unset=True),
+            headers=headers,
+            params={
+                "upsert": "true",
+                "merge": str(request_options.get("merge", False)).lower(),
+                "create_missing_related_entities": str(
+                    request_options.get("create_missing_related_entities", False)
+                ).lower(),
+                "validation_only": str(validation_only).lower(),
+            },
+        )
 
         if response.is_error:
             logger.error(
                 f"Error {'Validating' if validation_only else 'Upserting'} "
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
                 f"error: {response.text}"
@@ -54,43 +54,41 @@
         request_options: RequestOptions,
         user_agent_type: UserAgentType | None = None,
         silent: bool = False,
     ) -> None:
         logger.info(
             f"Delete entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
-        async with httpx.AsyncClient() as client:
-            response = await client.delete(
-                f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities/{entity.identifier}",
-                headers=await self.auth.headers(user_agent_type),
-                params={
-                    "delete_dependents": str(
-                        request_options.get("delete_dependent_entities", False)
-                    ).lower()
-                },
-            )
+        response = await self.client.delete(
+            f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities/{entity.identifier}",
+            headers=await self.auth.headers(user_agent_type),
+            params={
+                "delete_dependents": str(
+                    request_options.get("delete_dependent_entities", False)
+                ).lower()
+            },
+        )
 
         if response.is_error:
             logger.error(
                 f"Error deleting "
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
                 f"error: {response.text}"
             )
 
         handle_status_code(silent, response)
 
     async def validate_entity_exist(self, identifier: str, blueprint: str) -> None:
         logger.info(f"Validating entity {identifier} of blueprint {blueprint} exists")
 
-        async with httpx.AsyncClient() as client:
-            response = await client.get(
-                f"{self.auth.api_url}/blueprints/{blueprint}/entities/{identifier}",
-                headers=await self.auth.headers(),
-            )
+        response = await self.client.get(
+            f"{self.auth.api_url}/blueprints/{blueprint}/entities/{identifier}",
+            headers=await self.auth.headers(),
+        )
         if response.is_error:
             logger.error(
                 f"Error validating "
                 f"entity: {identifier} of "
                 f"blueprint: {blueprint}, "
                 f"error: {response.text}"
             )
@@ -105,24 +103,23 @@
                     "operator": "=",
                     "value": self.auth.user_agent(user_agent_type),
                 },
             ],
         }
 
         logger.info(f"Searching entities with query {query}")
-        async with httpx.AsyncClient() as client:
-            response = await client.post(
-                f"{self.auth.api_url}/entities/search",
-                json=query,
-                headers=await self.auth.headers(user_agent_type),
-                params={
-                    "exclude_calculated_properties": "true",
-                    "include": ["blueprint", "identifier"],
-                },
-            )
+        response = await self.client.post(
+            f"{self.auth.api_url}/entities/search",
+            json=query,
+            headers=await self.auth.headers(user_agent_type),
+            params={
+                "exclude_calculated_properties": "true",
+                "include": ["blueprint", "identifier"],
+            },
+        )
         response.raise_for_status()
         return [Entity.parse_obj(result) for result in response.json()["entities"]]
 
     async def search_dependent_entities(self, entity: Entity) -> list[Entity]:
         body = {
             "combinator": "and",
             "rules": [
@@ -132,20 +129,19 @@
                     "value": entity.identifier,
                     "direction": "downstream",
                 }
             ],
         }
 
         logger.info(f"Searching dependent entity with body {body}")
-        async with httpx.AsyncClient() as client:
-            response = await client.post(
-                f"{self.auth.api_url}/entities/search",
-                headers=await self.auth.headers(),
-                json=body,
-            )
+        response = await self.client.post(
+            f"{self.auth.api_url}/entities/search",
+            headers=await self.auth.headers(),
+            json=body,
+        )
         response.raise_for_status()
 
         return [Entity.parse_obj(result) for result in response.json()["entities"]]
 
     async def validate_entity_payload(
         self, entity: Entity, options: RequestOptions
     ) -> None:
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.0rc1/port_ocean/clients/port/mixins/integrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,72 +4,76 @@
 from loguru import logger
 from starlette import status
 
 from port_ocean.clients.port.authentication import PortAuthentication
 
 
 class IntegrationClientMixin:
-    def __init__(self, auth: PortAuthentication):
+    def __init__(
+        self,
+        integration_identifier: str,
+        auth: PortAuthentication,
+        client: httpx.AsyncClient,
+    ):
+        self.integration_identifier = integration_identifier
         self.auth = auth
+        self.client = client
 
-    async def get_integration(self, identifier: str) -> dict[str, Any]:
-        logger.info(f"Fetching integration with id: {identifier}")
-        async with httpx.AsyncClient() as client:
-            response = await client.get(
-                f"{self.auth.api_url}/integration/{identifier}",
-                headers=await self.auth.headers(),
-            )
+    async def get_current_integration(self) -> dict[str, Any]:
+        logger.info(f"Fetching integration with id: {self.integration_identifier}")
+        response = await self.client.get(
+            f"{self.auth.api_url}/integration/{self.integration_identifier}",
+            headers=await self.auth.headers(),
+        )
         response.raise_for_status()
         return response.json()["integration"]
 
     async def create_integration(
         self, _id: str, _type: str, changelog_destination: dict[str, Any]
     ) -> None:
         logger.info(f"Creating integration with id: {_id}")
         headers = await self.auth.headers()
         json = {
             "installationId": _id,
             "installationAppType": _type,
             "changelogDestination": changelog_destination,
         }
-        async with httpx.AsyncClient() as client:
-            response = await client.post(
-                f"{self.auth.api_url}/integration", headers=headers, json=json
-            )
+        response = await self.client.post(
+            f"{self.auth.api_url}/integration", headers=headers, json=json
+        )
         response.raise_for_status()
 
     async def patch_integration(
         self, _id: str, _type: str, changelog_destination: dict[str, Any]
     ) -> None:
         logger.info(f"Updating integration with id: {_id}")
         headers = await self.auth.headers()
         json = {
             "installationId": _id,
             "installationAppType": _type,
             "changelogDestination": changelog_destination,
         }
-        async with httpx.AsyncClient() as client:
-            response = await client.patch(
-                f"{self.auth.api_url}/integration/{_id}",
-                headers=headers,
-                json=json,
-            )
+        response = await self.client.patch(
+            f"{self.auth.api_url}/integration/{_id}",
+            headers=headers,
+            json=json,
+        )
         response.raise_for_status()
 
     async def initiate_integration(
         self, identifier: str, _type: str, changelog_destination: dict[str, Any]
     ) -> None:
         logger.info(f"Initiating integration with id: {identifier}")
         try:
-            integration = await self.get_integration(identifier)
+            integration = await self.get_current_integration(identifier)
 
             logger.info("Checking for diff in integration configuration")
             if (
                 integration["changelogDestination"] != changelog_destination
-                and integration["installationAppType"] == _type
+                or integration["installationAppType"] != _type
             ):
                 await self.patch_integration(identifier, _type, changelog_destination)
         except httpx.HTTPStatusError as e:
             if e.response.status_code == status.HTTP_404_NOT_FOUND:
                 await self.create_integration(identifier, _type, changelog_destination)
                 return
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/clients/port/types.py` & `port_ocean-0.1.0rc1/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/config/base.py` & `port_ocean-0.1.0rc1/port_ocean/config/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 def parse_config_provider(value: str) -> tuple[str, str]:
     match = re.match(PROVIDER_CONFIG_PATTERN, value)
     if not match:
         raise ValueError(
             f"Invalid pattern: {value}. Pattern should match: {PROVIDER_CONFIG_PATTERN}"
         )
 
-    index = value.find(" ")
-    provider_type, provider_value = value[:index], value[index + 1 :]
+    provider_type, provider_value = value.split(" ", 1)
 
     return provider_type, provider_value
 
 
 def load_from_config_provider(provider_type: str, value: str) -> Any:
     if provider_type == "env":
         result = os.environ.get(value)
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/config/integration.py` & `port_ocean-0.1.0rc1/port_ocean/config/integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import Any, Literal
 
 from pydantic import BaseModel, Field, BaseSettings
 
 from port_ocean.config.base import BaseOceanSettings
-from port_ocean.core.trigger_channel.settings import (
-    HttpTriggerChannelSettings,
-    KafkaTriggerChannelSettings,
-)
+from port_ocean.core.event_listener import EventListenerSettingsType
 
 
 class PortSettings(BaseSettings):
     client_id: str = Field(alias="clientId")
     client_secret: str = Field(alias="clientSecret")
     base_url: str = Field(alias="baseUrl", default="https://api.getport.io")
 
@@ -19,17 +16,15 @@
     identifier: str
     type: str
     config: dict[str, Any]
 
 
 class IntegrationConfiguration(BaseOceanSettings):
     port: PortSettings
-    trigger_channel: KafkaTriggerChannelSettings | HttpTriggerChannelSettings = Field(
-        alias="triggerChannel"
-    )
+    event_listener: EventListenerSettingsType = Field(alias="eventListener")
     batch_work_size: int | None = Field(alias="batchWorkSize", default=None)
     integration: IntegrationSettings
 
 
 LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0rc1/port_ocean/consumers/kafka_consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,27 @@
     brokers: str
     username: str | None = None
     password: str | None = None
     group_name: str | None = None
     security_protocol: str
     authentication_mechanism: str
     kafka_security_enabled: bool
+    consumer_poll_timeout: int
 
 
 class KafkaConsumer(BaseConsumer):
     def __init__(
         self,
         msg_process: Callable[[dict[Any, Any], str], Awaitable[None]],
         config: KafkaConsumerConfig,
         org_id: str,
     ) -> None:
         self.running = False
         self.org_id = org_id
+        self.config = config
 
         signal.signal(signal.SIGINT, self.exit_gracefully)
         signal.signal(signal.SIGTERM, self.exit_gracefully)
 
         self.msg_process = msg_process
         if config.kafka_security_enabled:
             kafka_config = {
@@ -70,24 +72,24 @@
         asyncio.run(try_wrapper())
 
     def start(self) -> None:
         try:
             logger.info("Start consumer...")
 
             self.consumer.subscribe(
-                [f"{self.org_id}.runs", f"{self.org_id}.change.log"],
+                [f"{self.org_id}.change.log"],
                 on_assign=lambda _, partitions: logger.info(
                     f"Assignment: {partitions}"
                 ),
             )
             logger.info("Subscribed to topics")
             self.running = True
             while self.running:
                 try:
-                    msg = self.consumer.poll(timeout=1.0)
+                    msg = self.consumer.poll(timeout=self.config.consumer_poll_timeout)
                     if msg is None:
                         continue
                     if msg.error():
                         raise KafkaException(msg.error())
                     else:
                         try:
                             logger.info(
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/context/event.py` & `port_ocean-0.1.0rc1/port_ocean/context/event.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/context/ocean.py` & `port_ocean-0.1.0rc1/port_ocean/context/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from typing import Callable, TYPE_CHECKING, Any
 
 from fastapi import APIRouter
 from werkzeug.local import LocalProxy, LocalStack
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.clients.port.types import UserAgentType
-from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.core.models import Entity
 from port_ocean.core.types import (
     RESYNC_EVENT_LISTENER,
     START_EVENT_LISTENER,
     RawEntityDiff,
 )
 from port_ocean.exceptions.context import PortOceanContextNotFoundError
 
 if TYPE_CHECKING:
+    from port_ocean.config.integration import IntegrationConfiguration
     from port_ocean.core.integrations.base import BaseIntegration
     from port_ocean.ocean import Ocean
 
 
 @dataclass
 class PortOceanContext:
     app: "Ocean"
 
     @property
-    def config(self) -> IntegrationConfiguration:
+    def config(self) -> "IntegrationConfiguration":
         return self.app.config
 
     @property
     def router(self) -> APIRouter:
         return self.app.integration_router
 
     @property
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/base.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @dataclass
 class EntityPortDiff:
     deleted: list[Entity] = field(default_factory=list)
     modified: list[Entity] = field(default_factory=list)
     created: list[Entity] = field(default_factory=list)
 
 
-class BaseManipulation(BaseWithContext):
+class BaseEntityProcessor(BaseWithContext):
     @abstractmethod
     async def _parse_items(
         self, mapping: ResourceConfig, raw_data: RawEntityDiff
     ) -> EntityDiff:
         pass
 
     async def parse_items(
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/jq_manipulation.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from functools import lru_cache
 from typing import Any
 
 import pyjq as jq  # type: ignore
 
-from port_ocean.core.handlers.manipulation.base import BaseManipulation
+from port_ocean.core.handlers.entity_processor.base import BaseEntityProcessor
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff
-from port_ocean.exceptions.core import ManipulationHandlerException
+from port_ocean.exceptions.core import EntityProcessorException
 
 
-class JQManipulation(BaseManipulation):
+class JQEntityProcessor(BaseEntityProcessor):
     @lru_cache
     def _compile(self, pattern: str) -> Any:
         return jq.compile(pattern)
 
     def _search(self, data: dict[str, Any], pattern: str) -> Any:
         try:
             return self._compile(pattern).first(data) or None
@@ -23,15 +23,15 @@
 
     def _search_as_bool(self, data: dict[str, Any], pattern: str) -> bool:
         value = self._compile(pattern).first(data)
 
         if isinstance(value, bool):
             return value
 
-        raise ManipulationHandlerException(
+        raise EntityProcessorException(
             f"Expected boolean value, got {type(value)} instead"
         )
 
     def _search_as_object(
         self, data: dict[str, Any], obj: dict[str, Any]
     ) -> dict[str, Any | None]:
         result: dict[str, Any | None] = {}
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/get_related_entities.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/transport.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import asyncio
 from itertools import chain
 
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.context.event import event
-from port_ocean.core.handlers.manipulation.base import EntityPortDiff
-from port_ocean.core.handlers.transport.base import BaseTransport
-from port_ocean.core.handlers.transport.port.get_related_entities import (
+from port_ocean.core.handlers.entities_state_applier.base import (
+    BaseEntitiesStateApplier,
+)
+from port_ocean.core.handlers.entities_state_applier.port.get_related_entities import (
     get_related_entities,
 )
-from port_ocean.core.handlers.transport.port.order_by_entities_dependencies import (
+from port_ocean.core.handlers.entities_state_applier.port.order_by_entities_dependencies import (
     order_by_entities_dependencies,
 )
-from port_ocean.core.handlers.transport.port.validate_entity_relations import (
+from port_ocean.core.handlers.entities_state_applier.port.validate_entity_relations import (
     validate_entity_relations,
 )
+from port_ocean.core.handlers.entity_processor.base import EntityPortDiff
 from port_ocean.core.models import Entity
 from port_ocean.core.types import EntityDiff
 from port_ocean.core.utils import is_same_entity, get_unique, get_port_diff
 from port_ocean.exceptions.core import RelationValidationException
 
 
-class HttpPortTransport(BaseTransport):
+class HttpEntitiesStateApplier(BaseEntitiesStateApplier):
     async def _validate_delete_dependent_entities(self, entities: list[Entity]) -> None:
         logger.info("Validated deleted entities")
         if not event.port_app_config.delete_dependent_entities:
             dependent_entities = await asyncio.gather(
                 *(
                     self.context.port_client.search_dependent_entities(entity)
                     for entity in entities
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0rc1/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 
 from port_ocean.clients.port.client import PortClient
-from port_ocean.core.handlers.manipulation.base import EntityPortDiff
-from port_ocean.core.handlers.transport.port.get_related_entities import (
+from port_ocean.core.handlers.entities_state_applier.port.get_related_entities import (
     get_related_entities,
 )
+from port_ocean.core.handlers.entity_processor.base import EntityPortDiff
 from port_ocean.core.utils import is_same_entity
 from port_ocean.exceptions.core import RelationValidationException
 
 
 async def validate_entity_relations(
     diff: EntityPortDiff, port_client: PortClient
 ) -> None:
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0rc1/port_ocean/core/integrations/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from loguru import logger
 
 from port_ocean.context.event import (
     event_context,
     EventType,
 )
 from port_ocean.context.ocean import PortOceanContext
-from port_ocean.core.integrations.mixins.sync import SyncRawMixin, SyncMixin
-from port_ocean.core.trigger_channel.factory import (
-    TriggerChannelFactory,
+from port_ocean.core.event_listener.factory import (
+    EventListenerFactory,
 )
+from port_ocean.core.integrations.mixins.sync import SyncRawMixin, SyncMixin
 from port_ocean.exceptions.core import IntegrationAlreadyStartedException
 
 
 class BaseIntegration(SyncRawMixin, SyncMixin):
     def __init__(self, context: PortOceanContext):
         SyncRawMixin.__init__(self)
         SyncMixin.__init__(self)
         self.started = False
         self.context = context
-        self.trigger_channel_factory = TriggerChannelFactory(
+        self.event_listener_factory = EventListenerFactory(
             context,
             self.context.config.integration.identifier,
             {"on_resync": self.sync_raw_all},
         )
 
     async def start(self) -> None:
         logger.info("Starting integration")
@@ -39,20 +39,20 @@
 
         await self.initialize_handlers()
 
         logger.info("Initializing integration at port")
         await self.context.port_client.initiate_integration(
             self.context.config.integration.identifier,
             self.context.config.integration.type,
-            self.context.config.trigger_channel.to_request(),
+            self.context.config.event_listener.to_request(),
         )
 
         self.started = True
 
         async with event_context(EventType.START, trigger_type="machine"):
             await asyncio.gather(
                 *(listener() for listener in self.event_strategy["start"])
             )
 
-        logger.info("Initializing trigger channel")
-        trigger_channel = await self.trigger_channel_factory.create_trigger_channel()
-        await trigger_channel.start()
+        logger.info("Initializing event listener")
+        event_listener = await self.event_listener_factory.create_event_listener()
+        await event_listener.start()
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 from typing import Callable
 
 from loguru import logger
 
 from port_ocean.context.ocean import PortOceanContext, ocean
-from port_ocean.core.handlers import BaseManipulation, BasePortAppConfig, BaseTransport
-from port_ocean.core.handlers.manipulation.jq_manipulation import JQManipulation
-from port_ocean.core.handlers.port_app_config.api import APIPortAppConfig
-from port_ocean.core.handlers.transport.port.transport import HttpPortTransport
+from port_ocean.core.handlers import (
+    BaseEntityProcessor,
+    BasePortAppConfig,
+    BaseEntitiesStateApplier,
+    HttpEntitiesStateApplier,
+    JQEntityProcessor,
+    APIPortAppConfig,
+)
+
 from port_ocean.exceptions.core import IntegrationNotStartedException
 
 
 class HandlerMixin:
-    ManipulationHandlerClass: Callable[
-        [PortOceanContext], BaseManipulation
-    ] = JQManipulation
+    EntityProcessorClass: Callable[
+        [PortOceanContext], BaseEntityProcessor
+    ] = JQEntityProcessor
 
     AppConfigHandlerClass: Callable[
         [PortOceanContext], BasePortAppConfig
     ] = APIPortAppConfig
 
-    TransportHandlerClass: Callable[
-        [PortOceanContext], BaseTransport
-    ] = HttpPortTransport
+    EntitiesStateApplierClass: Callable[
+        [PortOceanContext], BaseEntitiesStateApplier
+    ] = HttpEntitiesStateApplier
 
     def __init__(self) -> None:
-        self._manipulation: BaseManipulation | None = None
+        self._entity_processor: BaseEntityProcessor | None = None
         self._port_app_config_handler: BasePortAppConfig | None = None
-        self._transport: BaseTransport | None = None
+        self._entities_state_applier: BaseEntitiesStateApplier | None = None
 
     @property
-    def manipulation(self) -> BaseManipulation:
-        if not self._manipulation:
-            raise IntegrationNotStartedException("Manipulation class not initialized")
-        return self._manipulation
+    def entity_processor(self) -> BaseEntityProcessor:
+        if not self._entity_processor:
+            raise IntegrationNotStartedException(
+                "Entity Processor class not initialized"
+            )
+        return self._entity_processor
 
     @property
     def port_app_config_handler(self) -> BasePortAppConfig:
         if self._port_app_config_handler is None:
             raise IntegrationNotStartedException("PortAppConfig class not initialized")
         return self._port_app_config_handler
 
     @property
-    def transport(self) -> BaseTransport:
-        if not self._transport:
-            raise IntegrationNotStartedException("Transport class not initialized")
-        return self._transport
-
-    async def _init_manipulation_instance(self) -> BaseManipulation:
-        self._manipulation = self.ManipulationHandlerClass(ocean)
-        return self._manipulation
+    def entities_state_applier(self) -> BaseEntitiesStateApplier:
+        if not self._entities_state_applier:
+            raise IntegrationNotStartedException(
+                "EntitiesStateApplier class not initialized"
+            )
+        return self._entities_state_applier
+
+    async def _init_entity_processor_instance(self) -> BaseEntityProcessor:
+        self._entity_processor = self.EntityProcessorClass(ocean)
+        return self._entity_processor
 
     async def _init_port_app_config_handler_instance(
         self,
     ) -> BasePortAppConfig:
         self._port_app_config_handler = self.AppConfigHandlerClass(ocean)
         return self._port_app_config_handler
 
-    async def _init_transport_instance(self) -> BaseTransport:
-        self._transport = self.TransportHandlerClass(ocean)
-        return self._transport
+    async def _init_entities_state_applier_instance(self) -> BaseEntitiesStateApplier:
+        self._entities_state_applier = self.EntitiesStateApplierClass(ocean)
+        return self._entities_state_applier
 
     async def initialize_handlers(self) -> None:
         logger.info("Initializing integration components")
-        await self._init_manipulation_instance()
+        await self._init_entity_processor_instance()
         await self._init_port_app_config_handler_instance()
-        await self._init_transport_instance()
+        await self._init_entities_state_applier_instance()
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0rc1/port_ocean/core/integrations/mixins/sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,46 +9,46 @@
 from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.events import EventsMixin
 from port_ocean.core.integrations.mixins.handler import HandlerMixin
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff, RESYNC_EVENT_LISTENER
 from port_ocean.core.utils import validate_result, zip_and_sum
-from port_ocean.exceptions.core import RawObjectValidationException
+from port_ocean.exceptions.core import RawObjectValidationException, OceanAbortException
 from port_ocean.utils import get_function_location
 
 
 class SyncMixin(HandlerMixin, EventsMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
         EventsMixin.__init__(self)
 
     async def register(
         self,
         entities: list[Entity],
         user_agent_type: UserAgentType,
     ) -> None:
-        await self.transport.upsert(entities, user_agent_type)
+        await self.entities_state_applier.upsert(entities, user_agent_type)
         logger.info("Finished registering change")
 
     async def unregister(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
-        await self.transport.delete(entities, user_agent_type)
+        await self.entities_state_applier.delete(entities, user_agent_type)
         logger.info("Finished unregistering change")
 
     async def sync(
         self,
         entities: list[Entity],
         user_agent_type: UserAgentType,
     ) -> None:
         entities_at_port = await ocean.port_client.search_entities(user_agent_type)
 
-        await self.transport.upsert(entities, user_agent_type)
-        await self.transport.delete_diff(
+        await self.entities_state_applier.upsert(entities, user_agent_type)
+        await self.entities_state_applier.delete_diff(
             {"before": entities_at_port, "after": entities}, user_agent_type
         )
 
         logger.info("Finished syncing change")
 
 
 class SyncRawMixin(HandlerMixin, EventsMixin):
@@ -61,33 +61,37 @@
 
     async def _calculate_raw(
         self, raw_diff: list[tuple[ResourceConfig, RawEntityDiff]]
     ) -> list[EntityDiff]:
         logger.info("Calculating diff in entities between states")
         return await asyncio.gather(
             *(
-                self.manipulation.parse_items(mapping, results)
+                self.entity_processor.parse_items(mapping, results)
                 for mapping, results in raw_diff
             )
         )
 
     async def _resync_function_wrapper(
         self, fn: RESYNC_EVENT_LISTENER, kind: str
     ) -> list[dict[str, Any]]:
-        results = await fn(kind)
         try:
+            results = await fn(kind)
             return validate_result(results)
         except RawObjectValidationException as error:
-            raise RawObjectValidationException(
+            raise OceanAbortException(
                 f"Failed to validate raw data for returned data from {get_function_location(fn)}, error: {error}"
             ) from error
+        except Exception as error:
+            raise OceanAbortException(
+                f"Failed to execute {get_function_location(fn)}, error: {error}"
+            ) from error
 
     async def _get_resource_raw_results(
         self, resource_config: ResourceConfig
-    ) -> list[dict[str, Any]]:
+    ) -> tuple[list[dict[str, Any]], list[Exception]]:
         logger.info(f"Fetching {resource_config.kind} resync results")
         tasks: list[Awaitable[list[dict[Any, Any]]]] = []
         with logger.contextualize(kind=resource_config.kind):
             if self.__class__._on_resync != SyncRawMixin._on_resync:
                 tasks.append(
                     self._resync_function_wrapper(self._on_resync, resource_config.kind)
                 )
@@ -102,20 +106,35 @@
                     self._resync_function_wrapper(resync_function, resource_config.kind)
                     for resync_function in fns
                 ]
             )
 
             logger.info(f"Found {len(tasks)} resync tasks for {resource_config.kind}")
 
+            results_with_error: list[
+                tuple[list[dict[Any, Any]], Exception]
+            ] = await asyncio.gather(*tasks, return_exceptions=True)
             results: list[dict[Any, Any]] = list(
-                chain.from_iterable(await asyncio.gather(*tasks))
+                chain.from_iterable(
+                    [
+                        result
+                        for result, _ in results_with_error
+                        if not isinstance(result, Exception)
+                    ]
+                )
             )
 
-            logger.info(f"Triggered {len(tasks)} tasks for {resource_config.kind}")
-            return results
+            errors = [
+                error for _, error in results_with_error if isinstance(error, Exception)
+            ]
+
+            logger.info(
+                f"Triggered {len(tasks)} tasks for {resource_config.kind}, failed: {len(errors)}"
+            )
+            return results, errors
 
     async def _register_resource_raw(
         self,
         resource: ResourceConfig,
         results: list[dict[Any, Any]],
         user_agent_type: UserAgentType,
     ) -> list[Entity]:
@@ -128,15 +147,15 @@
                         "after": results,
                     },
                 )
             ]
         )
 
         entities_after: list[Entity] = objects_diff[0]["after"]
-        await self.transport.upsert(entities_after, user_agent_type)
+        await self.entities_state_applier.upsert(entities_after, user_agent_type)
         return entities_after
 
     async def _unregister_resource_raw(
         self,
         resource: ResourceConfig,
         results: list[dict[Any, Any]],
         user_agent_type: UserAgentType,
@@ -150,25 +169,25 @@
                         "after": [],
                     },
                 )
             ]
         )
 
         entities_after: list[Entity] = objects_diff[0]["before"]
-        await self.transport.delete(entities_after, user_agent_type)
+        await self.entities_state_applier.delete(entities_after, user_agent_type)
         logger.info("Finished unregistering change")
         return entities_after
 
     async def _register_in_batches(
         self,
         resource_config: ResourceConfig,
         user_agent_type: UserAgentType,
         batch_work_size: int | None,
-    ) -> list[Entity]:
-        results = await self._get_resource_raw_results(resource_config)
+    ) -> tuple[list[Entity], list[Exception]]:
+        results, errors = await self._get_resource_raw_results(resource_config)
 
         tasks = []
 
         batch_size = batch_work_size or len(results) or 1
         batches = [
             results[i : i + batch_size] for i in range(0, len(results), batch_size)
         ]
@@ -179,15 +198,15 @@
             )
 
         registered_entities_results = await asyncio.gather(*tasks)
         entities: list[Entity] = sum(registered_entities_results, [])
         logger.info(
             f"Finished registering change for {len(results)} raw results for kind: {resource_config.kind}"
         )
-        return entities
+        return entities, errors
 
     async def register_raw(
         self,
         kind: str,
         results: list[dict[Any, Any]],
         user_agent_type: UserAgentType,
     ) -> list[Entity]:
@@ -245,37 +264,52 @@
             entities_before, entities_after = zip_and_sum(
                 (
                     (entities_change["before"], entities_change["after"])
                     for entities_change in objects_diff
                 )
             )
 
-            await self.transport.apply_diff(
+            await self.entities_state_applier.apply_diff(
                 {"before": entities_before, "after": entities_after}, user_agent_type
             )
 
     async def sync_raw_all(
         self,
         _: dict[Any, Any] | None = None,
         trigger_type: TriggerType = "machine",
         user_agent_type: UserAgentType = UserAgentType.exporter,
+        silent: bool = True,
     ) -> None:
         logger.info("Resync was triggered")
 
         async with event_context(EventType.RESYNC, trigger_type=trigger_type):
             app_config = await self.port_app_config_handler.get_port_app_config()
 
             entities_at_port = await ocean.port_client.search_entities(user_agent_type)
 
-            created_entities = await asyncio.gather(
+            creation_results: list[
+                tuple[list[Entity], list[Exception]]
+            ] = await asyncio.gather(
                 *(
                     self._register_in_batches(
                         resource, user_agent_type, ocean.config.batch_work_size
                     )
                     for resource in app_config.resources
                 )
             )
-            flat_created_entities: list[Entity] = sum(created_entities, [])
-            await self.transport.delete_diff(
-                {"before": entities_at_port, "after": flat_created_entities},
-                user_agent_type,
+            flat_created_entities, errors = zip_and_sum(creation_results)
+
+            if not errors:
+                await self.entities_state_applier.delete_diff(
+                    {"before": entities_at_port, "after": flat_created_entities},
+                    user_agent_type,
+                )
+
+            message = f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state"
+            error_group = ExceptionGroup(
+                f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state",
+                errors,
             )
+            if not silent:
+                raise error_group
+
+            logger.error(message, exc_info=error_group)
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/models.py` & `port_ocean-0.1.0rc1/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/types.py` & `port_ocean-0.1.0rc1/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/core/utils.py` & `port_ocean-0.1.0rc1/port_ocean/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Iterable, Any, TypeVar
 
 from pydantic import parse_obj_as, ValidationError
 
-from port_ocean.core.handlers.manipulation.base import EntityPortDiff
+from port_ocean.core.handlers.entity_processor.base import EntityPortDiff
 from port_ocean.core.models import Entity
 from port_ocean.exceptions.core import RawObjectValidationException
 
-T = TypeVar("T", bound=list[Any])
+T = TypeVar("T", bound=tuple[list[Any], ...])
 
 
-def zip_and_sum(collection: Iterable[tuple[T, ...]]) -> tuple[T, ...]:
+def zip_and_sum(collection: Iterable[T]) -> T:
     return tuple(sum(items, []) for items in zip(*collection))  # type: ignore
 
 
 def validate_result(result: Any) -> list[dict[str, Any]]:
     try:
         return parse_obj_as(list[dict[str, Any]], result)
     except ValidationError as e:
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/logger_setup.py` & `port_ocean-0.1.0rc1/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/middlewares.py` & `port_ocean-0.1.0rc1/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev8/port_ocean/ocean.py` & `port_ocean-0.1.0rc1/port_ocean/ocean.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from inspect import getmembers, isclass
 from types import ModuleType
 from typing import Type, Callable
 
 import uvicorn
 from fastapi import FastAPI, APIRouter
 from loguru import logger
-from pydantic import BaseSettings
+from pydantic import BaseModel
 from starlette.types import Scope, Receive, Send
 
 from port_ocean.clients.port.client import PortClient
+from port_ocean.config.dynamic import default_config_factory
 from port_ocean.config.integration import IntegrationConfiguration, LogLevelType
 from port_ocean.context.ocean import (
     PortOceanContext,
     ocean,
     initialize_port_ocean_context,
 )
 from port_ocean.core.integrations.base import BaseIntegration
 from port_ocean.logger_setup import setup_logger
 from port_ocean.middlewares import request_handler
+from port_ocean.utils import get_spec_file
 
 
 def _get_base_integration_class_from_module(
     module: ModuleType,
 ) -> Type[BaseIntegration]:
     for name, obj in getmembers(module):
         if (
@@ -44,39 +46,29 @@
 
     module = module_from_spec(spec)
     spec.loader.exec_module(module)
 
     return module
 
 
-def _include_target_channel_router(app: FastAPI, _ocean: PortOceanContext) -> None:
-    target_channel_router = APIRouter()
-
-    @target_channel_router.post("/resync")
-    async def resync() -> None:
-        await _ocean.integration.sync_raw_all()
-
-    app.include_router(target_channel_router)
-
-
 class Ocean:
     def __init__(
         self,
         app: FastAPI | None = None,
         integration_class: Callable[[PortOceanContext], BaseIntegration] | None = None,
         integration_router: APIRouter | None = None,
-        config_class: Type[BaseSettings] | None = None,
+        config_factory: Callable[..., BaseModel] | None = None,
     ):
         initialize_port_ocean_context(self)
         self.fast_api_app = app or FastAPI()
         self.fast_api_app.middleware("http")(request_handler)
 
         self.config = IntegrationConfiguration(base_path="./")
-        if config_class:
-            self.config.integration.config = config_class(
+        if config_factory:
+            self.config.integration.config = config_factory(
                 **self.config.integration.config
             ).dict()
         self.integration_router = integration_router or APIRouter()
 
         self.port_client = PortClient(
             base_url=self.config.port.base_url,
             client_id=self.config.port.client_id,
@@ -86,16 +78,14 @@
         )
         self.integration = (
             integration_class(ocean) if integration_class else BaseIntegration(ocean)
         )
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         self.fast_api_app.include_router(self.integration_router, prefix="/integration")
-        if self.config.trigger_channel.type == "http":
-            _include_target_channel_router(self.fast_api_app, ocean)
 
         @self.fast_api_app.on_event("startup")
         async def startup() -> None:
             try:
                 await self.integration.start()
             except Exception as e:
                 logger.error(f"Failed to start integration with error: {e}")
@@ -110,14 +100,20 @@
     try:
         integration_path = f"{path}/integration.py" if path else "integration.py"
         module = _load_module(integration_path)
         integration_class = _get_base_integration_class_from_module(module)
     except Exception:
         integration_class = None
 
-    default_app = Ocean(integration_class=integration_class)
+    spec = get_spec_file()
+    config_factory = None
+    if spec is not None:
+        config_factory = default_config_factory(spec.get("configurations", []))
+    default_app = Ocean(
+        integration_class=integration_class, config_factory=config_factory
+    )
 
     main_path = f"{path}/main.py" if path else "main.py"
     app_module = _load_module(main_path)
     app = {name: item for name, item in getmembers(app_module)}.get("app", default_app)
 
     uvicorn.run(app, host="0.0.0.0", port=8000)
```

### Comparing `port_ocean-0.1.0.dev8/port_ocean/utils.py` & `port_ocean-0.1.0rc1/port_ocean/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import inspect
+from pathlib import Path
 from time import time
 from typing import Callable, Any
 from uuid import uuid4
 
+import yaml
+
 
 def get_time(seconds_precision: bool = True) -> float:
     """Return current time as Unix/Epoch timestamp, in seconds.
     :param seconds_precision: if True, return with seconds precision as integer (default).
                               If False, return with milliseconds precision as floating point number of seconds.
     """
     return time() if not seconds_precision else int(time())
@@ -17,7 +20,14 @@
     return str(uuid4())
 
 
 def get_function_location(func: Callable[..., Any]) -> str:
     file_path = inspect.getsourcefile(func)
     line_number = inspect.getsourcelines(func)[1]
     return f"{file_path}:{line_number}"
+
+
+def get_spec_file(path: Path = Path(".")) -> dict[str, Any] | None:
+    try:
+        return yaml.safe_load((path / ".port/spec.yaml").read_text())
+    except FileNotFoundError:
+        return None
```

### Comparing `port_ocean-0.1.0.dev8/PKG-INFO` & `port_ocean-0.1.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev8
+Version: 0.1.0rc1
 Summary: Port Ocean is a CLI tool for managing your Port projects.
+Home-page: https://app.getport.io
+Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
+Classifier: Framework :: FastAPI
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
 Provides-Extra: cli
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyjq (>=2.6.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0) ; extra == "cli"
 Requires-Dist: six (>=1.16.0,<2.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "cli"
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: werkzeug (>=2.3.4,<3.0.0)
+Project-URL: Repository, https://github.com/port-labs/Port-Ocean
 Description-Content-Type: text/markdown
 
 # Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
-[![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
+[![Lint](https://github.com/port-labs/Port-Ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
 Ocean is an innovative solution developed by Port to seamlessly integrate various third-party systems with our developer portal product,
 empowering engineers to effortlessly prioritize key features and streamline the integration process.
 
 ## Prerequisites
 
 - Python 3.11
@@ -70,27 +81,27 @@
 
 ![image](./assets/ExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/RealTimeUpdatesArchitecture.svg)
 
 ## Folder Structure
-The Integration Framework follows a specific folder structure within the mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
+The Ocean Integration Framework follows a specific folder structure within this mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
 port-ocean/
 ├── port_ocean (framework)/
 │ ├── ocean.py
 │ ├── core/
 | └── ...
 └── integrations/
-│  ├───integration_name/
-│  ├──── main.py
-│  ├──── pyproject.toml
-│  └──── Dockerfile
+│  └─── integration_name/
+│     ├──── main.py
+│     ├──── pyproject.toml
+│     └──── Dockerfile
 ├── ...
 └── ...
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
@@ -108,16 +119,16 @@
 # This is an example configuration file for the integration service.
 # Please copy this file to config.yaml file in the integration folder and edit it to your needs.
 
 port:
   clientId: PORT_CLIENT_ID # Can be loaded via environment variable: PORT_CLIENT_ID
   clientSecret: PORT_CLIENT_SECRET # Can be loaded via environment variable: PORT_CLIENT_SECRET
   baseUrl: https://api.getport.io/v1
-# The trigger channel to use for the integration service.
-triggerChannel:
+# The event listener to use for the integration service.
+eventListener:
   type: KAFKA / WEBHOOK
 integration:
   # The name of the integration.
   identifier: "my_integration"
   # The type of the integration.
   type: "PagerDuty"
   config:
@@ -184,11 +195,11 @@
    Or
 
    ```sh
    ocean sail
    ```
 
 ## License
-The Integration Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the `LICENSE` file for more details.
+The Ocean Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the [LICENSE](./LICENSE) file for more information.
 
 ## Contact
 For any questions or inquiries, please reach out to our team at support@getport.io
```

