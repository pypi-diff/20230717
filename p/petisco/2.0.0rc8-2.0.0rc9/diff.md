# Comparing `tmp/petisco-2.0.0rc8.tar.gz` & `tmp/petisco-2.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petisco-2.0.0rc8.tar", last modified: Thu Jun 29 18:43:06 2023, max compression
+gzip compressed data, was "petisco-2.0.0rc9.tar", last modified: Mon Jul  3 14:11:06 2023, max compression
```

## Comparing `petisco-2.0.0rc8.tar` & `petisco-2.0.0rc9.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.195644 petisco-2.0.0rc8/petisco/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/application_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/application_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco/base/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/chaos/chaos_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/chaos/check_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco/base/application/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/async_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/controller/meta_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco/base/application/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/dependency_injection/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/dependency_injection/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco/base/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/handlers/message_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.203644 petisco-2.0.0rc8/petisco/base/application/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/middleware/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/middleware/notifier_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/middleware/print_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.203644 petisco-2.0.0rc8/petisco/base/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/notifier/not_implemented_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/notifier/notifier_exception_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/notifier/notifier_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.203644 petisco-2.0.0rc8/petisco/base/application/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/patterns/app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/patterns/async_app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/patterns/crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/patterns/inmemory_crud_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/patterns/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.203644 petisco-2.0.0rc8/petisco/base/application/use_case/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/use_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/use_case/async_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/use_case/meta_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/use_case/use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/application/use_case/use_case_uncontrolled_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.203644 petisco-2.0.0rc8/petisco/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.203644 petisco-2.0.0rc8/petisco/base/domain/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/critical_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/default_http_error_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.207644 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/already_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/invalid_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/invalid_value_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/not_allowed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/defaults/not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/domain_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/errors/unknown_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.211644 petisco-2.0.0rc8/petisco/base/domain/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/all_message_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.211644 petisco-2.0.0rc8/petisco/base/domain/message/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/chaos/message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/chaos/message_chaos_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/command_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/consumer_derived_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 18:43:01.000000 petisco-2.0.0rc8/petisco/base/domain/message/domain_event_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message_handler_returns_none_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/message_subscriber_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_message_comsumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_message_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.211644 petisco-2.0.0rc8/petisco/base/domain/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/model/aggregate_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/model/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.211644 petisco-2.0.0rc8/petisco/base/domain/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/async_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/async_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/legacy_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/legacy_fake_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/domain/persistence/persistence_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/base/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/misc/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/base/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/base/testing/assert_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/cli/petisco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/cli/petisco_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/cli/petisco_rabbitmq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/extra/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/async_elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/elastic_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/elastic_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/elastic_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/is_elastic_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic/legacy_elastic_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/extra/elastic_apm/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic_apm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/elastic_apm/is_elastic_apm_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/extra/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.215644 petisco-2.0.0rc8/petisco/extra/fastapi/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/application/fastapi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.219644 petisco-2.0.0rc8/petisco/extra/fastapi/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/as_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_default_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_failure_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_result_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_success_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/is_fastapi_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.219644 petisco-2.0.0rc8/petisco/extra/fastapi/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/fastapi/testing/assert_http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.219644 petisco-2.0.0rc8/petisco/extra/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/logger/log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/logger/logging_based_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/logger/loguru_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/logger/not_implemented_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.219644 petisco-2.0.0rc8/petisco/extra/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.219644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/chaos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/chaos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18674 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/is_pika_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.223644 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/queue_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/specific_queue_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.227644 petisco-2.0.0rc8/petisco/extra/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.227644 petisco-2.0.0rc8/petisco/extra/redis/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.227644 petisco-2.0.0rc8/petisco/extra/redis/application/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/application/message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.231644 petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/redis_command_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/redis_message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/redis/is_redis_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.231644 petisco-2.0.0rc8/petisco/extra/slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.231644 petisco-2.0.0rc8/petisco/extra/slack/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.231644 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/create_text_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/slack/is_slack_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.235644 petisco-2.0.0rc8/petisco/extra/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.235644 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/async_sql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/base_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.235644 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/petisco/extra/sqlmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlmodel/is_sqlmodel_available.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/petisco/extra/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/extra/threading/pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/petisco/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.199644 petisco-2.0.0rc8/petisco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 18:43:06.000000 petisco-2.0.0rc8/petisco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:06.239644 petisco-2.0.0rc8/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:43:02.000000 petisco-2.0.0rc8/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.441987 petisco-2.0.0rc9/petisco/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 14:10:59.000000 petisco-2.0.0rc9/petisco/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/application_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/application_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/chaos/chaos_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/chaos/check_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/application/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/async_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/controller/meta_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/application/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/dependency_injection/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/dependency_injection/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/handlers/message_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco/base/application/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/middleware/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/middleware/notifier_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/middleware/print_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.449987 petisco-2.0.0rc9/petisco/base/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/notifier/not_implemented_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/notifier/notifier_exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/notifier/notifier_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.449987 petisco-2.0.0rc9/petisco/base/application/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/patterns/app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/patterns/async_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/patterns/crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/patterns/inmemory_crud_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/patterns/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.449987 petisco-2.0.0rc9/petisco/base/application/use_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/use_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/use_case/async_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/use_case/meta_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/use_case/use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/application/use_case/use_case_uncontrolled_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.449987 petisco-2.0.0rc9/petisco/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.449987 petisco-2.0.0rc9/petisco/base/domain/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/critical_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/default_http_error_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.449987 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/invalid_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/invalid_value_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/not_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/defaults/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/domain_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/errors/unknown_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.453987 petisco-2.0.0rc9/petisco/base/domain/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/all_message_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.453987 petisco-2.0.0rc9/petisco/base/domain/message/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/chaos/message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/chaos/message_chaos_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/chaos/not_implemented_message_chaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/command_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/consumer_derived_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/domain_event_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message_handler_returns_none_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/message_subscriber_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_message_comsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_message_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.453987 petisco-2.0.0rc9/petisco/base/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/model/aggregate_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/model/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.453987 petisco-2.0.0rc9/petisco/base/domain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/async_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/async_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/legacy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/legacy_fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/domain/persistence/persistence_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/base/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/misc/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/base/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/base/testing/assert_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/cli/petisco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/cli/petisco_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/cli/petisco_rabbitmq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/extra/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/async_elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/elastic_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/elastic_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/elastic_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/is_elastic_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic/legacy_elastic_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/extra/elastic_apm/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic_apm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/elastic_apm/is_elastic_apm_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/extra/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/extra/fastapi/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/application/fastapi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.457987 petisco-2.0.0rc9/petisco/extra/fastapi/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/as_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_default_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_failure_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_result_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_success_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/is_fastapi_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/fastapi/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/fastapi/testing/assert_http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/logger/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/logger/logging_based_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/logger/loguru_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/logger/not_implemented_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.461987 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_consumer_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18670 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/is_pika_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/queue_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/rabbitmq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/rabbitmq_exchange_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/rabbitmq_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/specific_queue_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/redis/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/redis/application/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/application/message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/redis_command_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/redis_message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/redis/is_redis_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/slack/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/create_text_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/slack/is_slack_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.465988 petisco-2.0.0rc9/petisco/extra/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/is_sqlalchemy_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/async_sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/base_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sqlite/sqlite_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/petisco/extra/sqlmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlmodel/is_sqlmodel_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/sqlmodel/sqlmodel_crud_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/petisco/extra/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/extra/threading/pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/petisco/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.445987 petisco-2.0.0rc9/petisco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 14:11:06.000000 petisco-2.0.0rc9/petisco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:06.469987 petisco-2.0.0rc9/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:58.000000 petisco-2.0.0rc9/tests/modules/__init__.py
```

### Comparing `petisco-2.0.0rc8/LICENSE` & `petisco-2.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/PKG-INFO` & `petisco-2.0.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc8 Summary: Petisco is a
+Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc9 Summary: Petisco is a
 framework for helping Python developers to build clean Applications Home-page:
 https://github.com/alice-biometrics/petisco Author: Alice Biometrics Author-
 email: support@alicebiometrics.com License: MIT Keywords: DDD,Use Case,Clean
 Architecture,REST,Applications Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `petisco-2.0.0rc8/README.md` & `petisco-2.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/application.py` & `petisco-2.0.0rc9/petisco/base/application/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class Application(BaseSettings):
     name: str
     version: str
     organization: str
     deployed_at: datetime
-    environment: str = Field(default="local", env="ENVIRONMENT")
+    environment: str = Field(default="local", validation_alias="ENVIRONMENT")
     dependencies_provider: Callable[..., List[Dependency]] = lambda: []
     configurers: List[ApplicationConfigurer] = []
     shared_error_map: Union[ErrorMap, None] = Field(default=dict())
 
     def __init__(self, **data: Any) -> None:
         info = ApplicationInfo(
             name=data["name"],
@@ -42,15 +42,14 @@
             f"Application: {info.name} {info.version} ({info.organization}) deployed at {deployed_at}"
         )
         super().__init__(**data)
 
     def configure(
         self, testing: bool = False, overwrite_dependencies: bool = False
     ) -> None:
-
         before_dependencies_configurers = [
             configurer
             for configurer in self.configurers
             if configurer.execute_after_dependencies is False
         ]
         name_configurers = [
             configurer.__class__.__name__
```

### Comparing `petisco-2.0.0rc8/petisco/base/application/application_info.py` & `petisco-2.0.0rc9/petisco/base/application/application_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/controller/async_controller.py` & `petisco-2.0.0rc9/petisco/base/application/controller/async_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/controller/controller.py` & `petisco-2.0.0rc9/petisco/base/application/controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,9 @@
         return ResultMapper(
             error_map=error_map,
             success_handler=getattr(config, "success_handler", lambda result: result),
             failure_handler=getattr(config, "failure_handler", default_failure_handler),
         )
 
     @abstractmethod
-    def execute(self, *args: tuple[str, ...], **kwargs: dict[str, Any]) -> AnyResult:
+    def execute(self, *args: Any, **kwargs: Any) -> AnyResult:
         return NotImplementedMethodError
```

### Comparing `petisco-2.0.0rc8/petisco/base/application/controller/http_error.py` & `petisco-2.0.0rc9/petisco/base/application/controller/http_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/controller/meta_controller.py` & `petisco-2.0.0rc9/petisco/base/application/controller/meta_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/dependency_injection/container.py` & `petisco-2.0.0rc9/petisco/base/application/dependency_injection/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
+from abc import ABC
 from collections import defaultdict
 from typing import Generic, TypeVar
 
 from petisco.base.application.dependency_injection.dependency import Dependency
 from petisco.base.misc.singleton import Singleton
 
-T = TypeVar("T")
+T = TypeVar("T", bound=ABC)
 
 
 class Container(Generic[T], metaclass=Singleton):
     """
     Singleton which contains set dependencies (List[Dependency)) prepared to be instantiated in order to be injected
      in the UseCases of our application
     """
```

### Comparing `petisco-2.0.0rc8/petisco/base/application/dependency_injection/dependency.py` & `petisco-2.0.0rc9/petisco/base/application/dependency_injection/dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,30 +52,28 @@
         if self.builders is None or self.builders.get("default") is None:
             raise TypeError(
                 f"Dependency: Define at least one builder for {self.type.__name__} with `default` key. This is "
                 f"mandatory. Given builders={self.builders} "
             )
 
     def _set_envar_modifier(self, envar_modifier: str | None = None):
-
         if envar_modifier is None and self.type:
             return (
                 # "PETISCO_" + # TODO this will break compatibility (waiting for v2)
                 re.sub(r"(?<!^)(?=[A-Z])", "_", self.type.__name__).upper()
                 + "_TYPE"
             )
 
         return envar_modifier
 
     def _validate(self) -> None:
         if self.type and self.strict:
             if self.builders is None:
                 return
             for key, builder in self.builders.items():
-
                 klass = builder.klass
                 if hasattr(builder.klass, "__origin__"):
                     klass = builder.klass.__origin__
 
                 if not issubclass(klass, self.type):
                     raise TypeError(
                         f"Dependency: The class {builder.klass.__name__} from builders ({key}) is not a subclass from "
```

### Comparing `petisco-2.0.0rc8/petisco/base/application/handlers/message_handler.py` & `petisco-2.0.0rc9/petisco/base/application/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/middleware/middleware.py` & `petisco-2.0.0rc9/petisco/base/application/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/middleware/notifier_middleware.py` & `petisco-2.0.0rc9/petisco/base/application/middleware/notifier_middleware.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/notifier/notifier.py` & `petisco-2.0.0rc9/petisco/base/application/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/notifier/notifier_exception_message.py` & `petisco-2.0.0rc9/petisco/base/application/notifier/notifier_exception_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/patterns/crud_repository.py` & `petisco-2.0.0rc9/petisco/base/application/patterns/crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/patterns/inmemory_crud_repository.py` & `petisco-2.0.0rc9/petisco/base/application/patterns/inmemory_crud_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/application/use_case/meta_use_case.py` & `petisco-2.0.0rc9/petisco/base/application/use_case/meta_use_case.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/errors/default_http_error_map.py` & `petisco-2.0.0rc9/petisco/base/domain/errors/default_http_error_map.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/errors/defaults/already_exists.py` & `petisco-2.0.0rc9/petisco/base/domain/errors/defaults/already_exists.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/errors/defaults/not_found.py` & `petisco-2.0.0rc9/petisco/base/domain/errors/defaults/not_found.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/errors/domain_error.py` & `petisco-2.0.0rc9/petisco/base/domain/errors/domain_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/errors/unknown_error.py` & `petisco-2.0.0rc9/petisco/base/domain/errors/unknown_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/chaos/not_implemented_message_chaos.py` & `petisco-2.0.0rc9/petisco/base/domain/message/chaos/not_implemented_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/command.py` & `petisco-2.0.0rc9/petisco/base/domain/message/command.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/command_bus.py` & `petisco-2.0.0rc9/petisco/base/domain/message/command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/command_subscriber.py` & `petisco-2.0.0rc9/petisco/base/domain/message/command_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/domain_event.py` & `petisco-2.0.0rc9/petisco/base/domain/message/domain_event.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/domain_event_bus.py` & `petisco-2.0.0rc9/petisco/base/domain/message/domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/domain_event_subscriber.py` & `petisco-2.0.0rc9/petisco/base/domain/message/domain_event_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message_bus.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message_configurer.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message_consumer.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message_consumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message_handler_returns_none_error.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message_handler_returns_none_error.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message_subscriber.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message_subscriber.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/message_subscriber_info.py` & `petisco-2.0.0rc9/petisco/base/domain/message/message_subscriber_info.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_command_bus.py` & `petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_domain_event_bus.py` & `petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/message/not_implemented_message_comsumer.py` & `petisco-2.0.0rc9/petisco/base/domain/message/not_implemented_message_comsumer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/model/aggregate_root.py` & `petisco-2.0.0rc9/petisco/base/domain/model/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/model/uuid.py` & `petisco-2.0.0rc9/petisco/base/domain/model/uuid.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/model/value_object.py` & `petisco-2.0.0rc9/petisco/base/domain/model/value_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class ValueObject(BaseModel):
     """
     A base class to define ValueObject
 
     It is small object that represents a simple entity whose equality is not based on identity.
     """
 
-    value: Any
+    value: Any = None
 
     def __init__(self, value: Any, **data: Any) -> None:
         super().__init__(value=value, **data)
 
     def dict(self, **kwargs: Any) -> Any:
         return self.value
 
@@ -35,13 +35,13 @@
     @field_validator("value")
     def validate_value(cls, value: Any) -> Any:
         if value is None:
             raise InvalidValueObject()
         return value
 
     @staticmethod
-    def serializer(attribute_name: str):
-        def _serializer(value_object: ValueObject):
+    def serializer(attribute_name: str) -> Any:
+        def _serializer(value_object: ValueObject) -> Any:
             if value_object:
                 return value_object.value
 
         return field_serializer(attribute_name)(_serializer)
```

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/async_fake_database.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/async_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/database.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/databases.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/databases.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/legacy_database.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/legacy_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/legacy_fake_database.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/legacy_fake_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/persistence.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/persistence.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/domain/persistence/persistence_models.py` & `petisco-2.0.0rc9/petisco/base/domain/persistence/persistence_models.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/misc/async_wrapper.py` & `petisco-2.0.0rc9/petisco/base/misc/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/misc/builder.py` & `petisco-2.0.0rc9/petisco/base/misc/builder.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/misc/result_mapper.py` & `petisco-2.0.0rc9/petisco/base/misc/result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/misc/singleton.py` & `petisco-2.0.0rc9/petisco/base/misc/singleton.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/base/misc/wrapper.py` & `petisco-2.0.0rc9/petisco/base/misc/wrapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/cli/petisco.py` & `petisco-2.0.0rc9/petisco/cli/petisco.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     is_active = False
     for arg in vars(args):
         is_active = is_active or getattr(args, arg)
     return is_active
 
 
 def rename_template(original_name: str, replacement: str) -> None:
-
     for dname, _, _ in os.walk("."):
         if original_name in dname:
             os.rename(dname, dname.replace(original_name, replacement))
 
     blacklist = [".git/", ".idea"]
     for dname, dirs, files in os.walk("."):
         for fname in files:
```

### Comparing `petisco-2.0.0rc8/petisco/cli/petisco_dev.py` & `petisco-2.0.0rc9/petisco/cli/petisco_dev.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/cli/petisco_rabbitmq.py` & `petisco-2.0.0rc9/petisco/cli/petisco_rabbitmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 def main() -> None:
     args = get_args()
 
     if not args:
         return
 
     if args.requeue:
-
         if not args.consuming_queue:
             print(" ➜ Not consuming queue given")
             return
 
         if not args.retry_routing_key:
             print(" ➜ Not retry routing_key given")
             return
```

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic/__init__.py` & `petisco-2.0.0rc9/petisco/extra/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic/async_elastic_database.py` & `petisco-2.0.0rc9/petisco/extra/elastic/async_elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic/elastic_connection.py` & `petisco-2.0.0rc9/petisco/extra/elastic/elastic_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic/elastic_database.py` & `petisco-2.0.0rc9/petisco/extra/elastic/elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic/elastic_is_running_locally.py` & `petisco-2.0.0rc9/petisco/extra/elastic/elastic_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic/legacy_elastic_database.py` & `petisco-2.0.0rc9/petisco/extra/elastic/legacy_elastic_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py` & `petisco-2.0.0rc9/petisco/extra/elastic_apm/elastic_apm_monitoring_app_service.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/fastapi/__init__.py` & `petisco-2.0.0rc9/petisco/extra/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_controller.py` & `petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_controller.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_failure_handler.py` & `petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_failure_handler.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/fastapi/controller/fastapi_result_mapper.py` & `petisco-2.0.0rc9/petisco/extra/fastapi/controller/fastapi_result_mapper.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/fastapi/testing/assert_http_exception.py` & `petisco-2.0.0rc9/petisco/extra/fastapi/testing/assert_http_exception.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/logger/__init__.py` & `petisco-2.0.0rc9/petisco/extra/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/logger/log_message.py` & `petisco-2.0.0rc9/petisco/extra/logger/log_message.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/logger/logging_based_logger.py` & `petisco-2.0.0rc9/petisco/extra/logger/logging_based_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/logger/loguru_logger.py` & `petisco-2.0.0rc9/petisco/extra/logger/loguru_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/__init__.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from petisco.extra.rabbitmq.dependencies import get_default_message_dependencies
 from petisco.extra.rabbitmq.is_pika_available import is_pika_available
 
 __all__ = ["get_default_message_dependencies"]
 
 
 if is_pika_available():
-
     from petisco.extra.rabbitmq.application.chaos.rabbitmq_message_chaos import (
         RabbitMqMessageChaos,
     )
     from petisco.extra.rabbitmq.application.message.bus.rabbitmq_command_bus import (
         RabbitMqCommandBus,
     )
     from petisco.extra.rabbitmq.application.message.bus.rabbitmq_domain_event_bus import (
```

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/chaos/rabbitmq_message_chaos.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/bus/rabbitmq_message_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
     def execute(
         self,
         channel: BlockingChannel,
         message: Message,
         routing_key: Union[str, None] = None,
     ) -> None:
-
         if routing_key is None:
             routing_key = RabbitMqMessageQueueNameFormatter.format(
                 message, exchange_name=self._exchange_name
             )
 
         channel.confirm_delivery()
         channel.basic_publish(
```

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_store_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/configurer/rabbitmq_message_subscribers_configurer.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,18 +63,16 @@
     def _delete_exchange(self) -> None:
         self.rabbitmq.delete_exchange(self._exchange_name)
         self.rabbitmq.delete_exchange(self._retry_exchange_name)
         self.rabbitmq.delete_exchange(self._dead_letter_exchange_name)
 
     def _delete_queues(self) -> None:
         for SubscriberClass in self._configured_subscribers:
-
             subscriber = SubscriberClass()
             for subscriber_info in subscriber.get_message_subscribers_info():
-
                 if subscriber_info.message_type == "message":
                     # if subscriber_info is subscribed to message it will be consuming from store queue
                     break
 
                 queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(
                     subscriber_info, exchange_name=self._exchange_name
                 )
@@ -100,15 +98,14 @@
     def _declare_queues(
         self,
         exchange_name: str,
         retry_exchange_name: str,
         dead_letter_exchange_name: str,
         subscribers: List[Type[MessageSubscriber]],
     ) -> None:
-
         for SubscriberClass in subscribers:
             subscriber = SubscriberClass()
             for subscriber_info in subscriber.get_message_subscribers_info():
                 if subscriber_info.message_type == "message":
                     # if subscriber_info is subscribed to message it will be consuming from store queue
                     break
```

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_logger.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_event_consumer_printer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/consumer/rabbitmq_message_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,19 +142,17 @@
 
     def add_subscribers(self, subscribers: List[Type[MessageSubscriber]]) -> None:
         """
         Add defined subscribers to be connected with main queues.
         """
 
         for SubscriberClass in subscribers:
-
             subscriber: MessageSubscriber = SubscriberClass()
 
             for subscriber_info in subscriber.get_message_subscribers_info():
-
                 if subscriber_info.message_type == "message":
                     self._add_subscriber_instance_on_queue(
                         queue_name="store", subscriber=subscriber, is_store=True
                     )
                 else:
                     queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format(
                         subscriber_info, exchange_name=self.exchange_name
@@ -169,15 +167,14 @@
         self, subscriber: Type[MessageSubscriber]
     ) -> None:
         """
         Add defined subscribers to be connected with the correspondent dead letter.
         """
         instance_subscriber: MessageSubscriber = subscriber()
         for subscriber_info in instance_subscriber.get_message_subscribers_info():
-
             queue_name = RabbitMqMessageSubscriberQueueNameFormatter.format_dead_letter(
                 subscriber_info, exchange_name=self.exchange_name
             )
             self._add_subscriber_instance_on_queue(
                 queue_name=f"{queue_name}.{instance_subscriber.get_subscriber_name()}",
                 subscriber=instance_subscriber,
                 message_type_expected=subscriber_info.message_type,
@@ -313,15 +310,14 @@
         self,
         ch: BlockingChannel,
         method: Basic.Deliver,
         properties: BasicProperties,
         body: bytes,
         is_store: bool,
     ) -> ConsumerDerivedAction:
-
         if self.has_been_redelivered_too_much(properties):
             derived_action = self.send_to_dead_letter(ch, method, properties, body)
         else:
             derived_action = self.send_to_retry(ch, method, properties, body, is_store)
 
         ch.basic_ack(delivery_tag=method.delivery_tag)
```

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/application/message/formatter/rabbitmq_message_subscriber_queue_name_formatter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/dependencies.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from petisco.base.domain.message.not_implemented_message_configurer import (
     NotImplementedMessageConfigurer,
 )
 from petisco.base.misc.builder import Builder
 
 
 def get_default_message_dependencies() -> List[Dependency]:
-
     return [
         Dependency(
             DomainEventBus,
             builders={"default": Builder(NotImplementedDomainEventBus)},
             envar_modifier="PETISCO_DOMAIN_EVENT_BUS_TYPE",
         ),
         Dependency(
```

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/rabbitmq_message_application_configurer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/queue_config.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/rabbitmq_connector.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/rabbitmq_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         except ConnectionClosedByBroker:
             del self.open_connections[key_connection]
             connection = self.get_connection(key_connection)
             channel = connection.channel()
         return channel
 
     def _create_connection(self, key_connection: str) -> BlockingConnection:
-
         connection = self._create_blocking_connection(key_connection)
 
         self._wait_for_open_connection(connection, key_connection)
 
         if not connection.is_open:
             time_elapsed = round(
                 (self.wait_seconds_retry * self.num_max_retries_connection), 2
```

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/rabbitmq_declarer.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/rabbitmq/shared/specific_queue_config.py` & `petisco-2.0.0rc9/petisco/extra/rabbitmq/shared/specific_queue_config.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/redis_command_bus.py` & `petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/redis_command_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py` & `petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/redis_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/redis/application/message/bus/redis_message_bus.py` & `petisco-2.0.0rc9/petisco/extra/redis/application/message/bus/redis_message_bus.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/slack/__init__.py` & `petisco-2.0.0rc9/petisco/extra/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc9/petisco/extra/slack/application/notifier/blocks_slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py` & `petisco-2.0.0rc9/petisco/extra/slack/application/notifier/exception_blocks_slack_notifier_message_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
                     "type": "mrkdwn",
                     "text": text_error,
                 },
             }
         return error_block
 
     def convert(self, notifier_exception_message: NotifierExceptionMessage):
-
         blocks = []
         header_block = self._create_header_block(notifier_exception_message.title)
         message_block = self._create_message_block(notifier_exception_message)
         executor_block = self._create_executor_block(notifier_exception_message)
         error_block = self._create_error_block(notifier_exception_message)
 
         blocks.append(header_block)
```

### Comparing `petisco-2.0.0rc8/petisco/extra/slack/application/notifier/slack_notifier.py` & `petisco-2.0.0rc9/petisco/extra/slack/application/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py` & `petisco-2.0.0rc9/petisco/extra/slack/application/notifier/slack_notifier_message_converter.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/slack/dependencies.py` & `petisco-2.0.0rc9/petisco/extra/slack/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     NotImplementedNotifier,
 )
 from petisco.base.application.notifier.notifier import Notifier
 from petisco.base.misc.builder import Builder
 
 
 def get_default_notifier_dependencies() -> List[Dependency]:
-
     return [
         Dependency(
             Notifier,
             builders={"default": Builder(NotImplementedNotifier)},
             envar_modifier="PETISCO_NOTIFIER_TYPE",
         )
     ]
```

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/__init__.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/async_sql_database.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/async_sql_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 T = TypeVar("T")
 
 AsyncSqlSessionScope = Callable[..., AsyncContextManager[AsyncSession]]
 
 
 class AsyncSqlDatabase(SqlDatabase, AsyncDatabase[AsyncSession]):
-
     async_session_factory: async_sessionmaker | None = None
 
     async def initialize(self, base: DeclarativeBase = SqlBase) -> None:
         engine = create_async_engine(
             self.connection.url,
             json_serializer=lambda obj: obj,
             json_deserializer=lambda obj: obj,
```

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/async_sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/base_sql_repository.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/base_sql_repository.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql/legacy_mysql_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/mysql_is_running_locally.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_base.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_base.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_database.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 T = TypeVar("T")
 
 SqlSessionScope = Callable[..., ContextManager[Session]]
 
 
 class SqlDatabase(Database[Session]):
-
     session_factory: sessionmaker | None = None
 
     def __init__(
         self,
         connection: SqliteConnection | MySqlConnection,
         *,
         alias: str | None = None,
```

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_executor.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sql_session_scope_provider.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py` & `petisco-2.0.0rc9/petisco/extra/sqlalchemy/sql/sqlite/legacy_sqlite_database.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/extra/sqlmodel/sqlmodel_crud_repository.py` & `petisco-2.0.0rc9/petisco/extra/sqlmodel/sqlmodel_crud_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     @abstractmethod
     def get_sql_model_type(self) -> SQLModelType:
         return NotImplementedMethodError
 
     @meiga
     def save(self, aggregate_root: AggregateRootType) -> BoolResult:
-
         with Session(engine) as session:
             model = self.get_sql_model_type()
             statement = select(model).where(
                 model.aggregate_id == aggregate_root.aggregate_id.value
             )
             sql_model = session.exec(statement).first()
             if sql_model:
```

### Comparing `petisco-2.0.0rc8/petisco/extra/threading/pool_executor.py` & `petisco-2.0.0rc9/petisco/extra/threading/pool_executor.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco/public_api.py` & `petisco-2.0.0rc9/petisco/public_api.py`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/petisco.egg-info/PKG-INFO` & `petisco-2.0.0rc9/petisco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petisco
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: Petisco is a framework for helping Python developers to build clean Applications
 Home-page: https://github.com/alice-biometrics/petisco
 Author: Alice Biometrics
 Author-email: support@alicebiometrics.com
 License: MIT
 Keywords: DDD,Use Case,Clean Architecture,REST,Applications
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc8 Summary: Petisco is a
+Metadata-Version: 2.1 Name: petisco Version: 2.0.0rc9 Summary: Petisco is a
 framework for helping Python developers to build clean Applications Home-page:
 https://github.com/alice-biometrics/petisco Author: Alice Biometrics Author-
 email: support@alicebiometrics.com License: MIT Keywords: DDD,Use Case,Clean
 Architecture,REST,Applications Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `petisco-2.0.0rc8/petisco.egg-info/SOURCES.txt` & `petisco-2.0.0rc9/petisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/setup.cfg` & `petisco-2.0.0rc9/setup.cfg`

 * *Files identical despite different names*

### Comparing `petisco-2.0.0rc8/setup.py` & `petisco-2.0.0rc9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,11 +56,11 @@
         "rabbitmq": ["pika==1.3.2"],
         "slack": ["slack_sdk<4.0.0,>=3.20.2"],
         "elastic": [
             "elasticsearch[async]<8.0.0,>=7.13.1",
             "elastic-apm<7.0.0,>=6.15.1",
         ],
         "elastic-apm": ["elastic-apm<7.0.0,>=6.15.1"],
-        "fastapi": ["fastapi<1.0.0,>=0.100.0b1"],
+        "fastapi": ["fastapi<1.0.0,>=0.100.0b2"],
         "rich": ["rich"],
     },
 )
```

### Comparing `petisco-2.0.0rc8/tests/fixtures.py` & `petisco-2.0.0rc9/tests/fixtures.py`

 * *Files identical despite different names*

