# Comparing `tmp/investing_algorithm_framework-1.0.tar.gz` & `tmp/investing_algorithm_framework-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-1.0.tar", last modified: Mon Apr 24 15:39:32 2023, max compression
+gzip compressed data, was "investing_algorithm_framework-1.1.tar", last modified: Mon Jul 17 20:48:36 2023, max compression
```

## Comparing `investing_algorithm_framework-1.0.tar` & `investing_algorithm_framework-1.1.tar`

### file list

```diff
@@ -1,127 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/run_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/dependency_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/asset_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.624396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/synchronized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/model_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/order/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/order/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.628396 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/market_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/investing_algorithm_framework/services/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/market_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/order_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/portfolio_configuration_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/portfolio_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/investing_algorithm_framework/setup_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.620396 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 15:39:32.000000 investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:39:32.632396 investing_algorithm_framework-1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-24 15:38:54.000000 investing_algorithm_framework-1.0/tests/test_create_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/run_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/dependency_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.154462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/asset_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/position/position_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/model_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.158462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position_cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/market_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/investing_algorithm_framework/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/market_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15968 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/order_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_configuration_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/position_cost_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/investing_algorithm_framework/setup_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.150462 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 20:48:36.000000 investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:48:36.162462 investing_algorithm_framework-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-17 20:47:58.000000 investing_algorithm_framework-1.1/tests/test_create_app.py
```

### Comparing `investing_algorithm_framework-1.0/LICENSE` & `investing_algorithm_framework-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/PKG-INFO` & `investing_algorithm_framework-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing_algorithm_framework
-Version: 1.0
+Version: 1.1
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
 Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
 Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
```

### Comparing `investing_algorithm_framework-1.0/README.md` & `investing_algorithm_framework-1.1/README.md`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from .create_app import create_app
 from investing_algorithm_framework.domain import ApiException, \
     TradingDataType, OrderBook, Ticker, TradingTimeFrame, OHLCV, OrderType,\
     OrderStatus, OrderSide, Config, TimeUnit, TimeInterval, Order, Portfolio, \
     Position
 from investing_algorithm_framework.domain import PortfolioConfiguration, \
     RESOURCE_DIRECTORY
-from investing_algorithm_framework.app import TradingStrategy, StatelessAction
+from investing_algorithm_framework.app import TradingStrategy, \
+    StatelessAction, Task
 
 __all__ = [
     "RESOURCE_DIRECTORY",
     "App",
     "create_app",
     "ApiException",
     "TradingDataType",
@@ -25,9 +26,10 @@
     "PortfolioConfiguration",
     "TimeUnit",
     "TimeInterval",
     "TradingStrategy",
     "Order",
     "Portfolio",
     "Position",
-    "StatelessAction"
+    "StatelessAction",
+    "Task"
 ]
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import List
 
-from investing_algorithm_framework.domain import OrderStatus, \
+from investing_algorithm_framework.domain import OrderStatus, OrderFee, \
     Position, Order, Portfolio, OrderType, OrderSide, ApiException
 
 logger = logging.getLogger(__name__)
 
 
 class Algorithm:
 
@@ -44,98 +44,98 @@
     def config(self, config):
         self._config = config
 
     @property
     def running(self) -> bool:
         return self.strategy_orchestrator_service.running
 
-    def run_strategies(self):
-        self.strategy_orchestrator_service.run_pending_strategies()
+    def run_jobs(self):
+        self.strategy_orchestrator_service.run_pending_jobs()
 
     def create_order(
         self,
         target_symbol,
         price,
         type,
         side,
-        amount_target_symbol=None,
-        amount_trading_symbol=None,
+        amount,
         market=None,
-        execute=False,
-        validate=False
+        execute=True,
+        validate=True,
+        sync=True
     ):
         portfolio = self.portfolio_service.find({"market": market})
         return self.order_service.create(
             {
                 "target_symbol": target_symbol,
                 "price": price,
-                "amount_target_symbol": amount_target_symbol,
-                "amount_trading_symbol": amount_trading_symbol,
+                "amount": amount,
                 "type": type,
                 "side": side,
                 "portfolio_id": portfolio.id,
                 "status": OrderStatus.PENDING.value,
                 "trading_symbol": portfolio.trading_symbol,
             },
             execute=execute,
-            validate=validate
+            validate=validate,
+            sync=sync
         )
 
     def create_limit_order(
             self,
             target_symbol,
             price,
             side,
-            amount_target_symbol=None,
-            amount_trading_symbol=None,
+            amount,
             market=None,
             execute=True,
-            validate=True
+            validate=True,
+            sync=True
     ):
         portfolio = self.portfolio_service.find({"market": market})
         return self.order_service.create(
             {
                 "target_symbol": target_symbol,
                 "price": price,
-                "amount_target_symbol": amount_target_symbol,
-                "amount_trading_symbol": amount_trading_symbol,
+                "amount": amount,
                 "type": OrderType.LIMIT.value,
                 "side": OrderSide.from_value(side).value,
                 "portfolio_id": portfolio.id,
                 "status": OrderStatus.PENDING.value,
                 "trading_symbol": portfolio.trading_symbol,
             },
             execute=execute,
-            validate=validate
+            validate=validate,
+            sync=sync
         )
 
     def create_market_order(
         self,
         target_symbol,
         side,
-        amount_target_symbol=None,
-        amount_trading_symbol=None,
+        amount,
         market=None,
         execute=False,
-        validate=False
+        validate=False,
+        sync=True
     ):
         portfolio = self.portfolio_service.find({"market": market})
         return self.order_service.create(
             {
                 "target_symbol": target_symbol,
-                "amount_target_symbol": amount_target_symbol,
-                "amount_trading_symbol": amount_trading_symbol,
+                "amount": amount,
                 "type": OrderType.MARKET.value,
                 "side": OrderSide.from_value(side).value,
                 "portfolio_id": portfolio.id,
                 "status": OrderStatus.PENDING.value,
                 "trading_symbol": portfolio.trading_symbol,
             },
             execute=execute,
-            validate=validate
+            validate=validate,
+            sync=sync
         )
 
     def check_order_status(self, market=None, symbol=None, status=None):
         portfolio = self.portfolio_service.get({"market": market})
         orders = self.order_service \
             .get_all({"target_symbol": symbol, "status": status})
         self.order_service.check_order_status(portfolio, orders)
@@ -219,14 +219,17 @@
                 "target_symbol": target_symbol,
                 "status": status,
                 "type": type,
                 "side": side
             }
         )
 
+    def get_order_fee(self, order_id) -> OrderFee:
+        return self.order_service.get_order_fee(order_id)
+
     def get_positions(self, market=None, identifier=None) -> List[Position]:
         query_params = {}
 
         if market is not None:
             query_params["market"] = market
 
         if identifier is not None:
@@ -286,14 +289,18 @@
         )
         return (position.amount * ticker["bid"] /
                 self.get_allocated(identifier=portfolio.identifier)) * 100
 
     def add_strategies(self, strategies):
         self.strategy_orchestrator_service.add_strategies(strategies)
 
+    def add_tasks(self, tasks):
+        self.strategy_orchestrator_service.add_tasks(tasks)
+
+
     def get_allocated(self, market=None, identifier=None) -> float:
 
         if self.portfolio_configuration_service.count() > 1 \
                 and identifier is None and market is None:
             raise ApiException(
                 "Multiple portfolios found. Please specify a "
                 "portfolio identifier."
@@ -334,7 +341,10 @@
                 symbol = f"{position.symbol.upper()}/" \
                          f"{portfolio.trading_symbol.upper()}"
                 self.market_service.initialize(portfolio.configuration)
                 price = self.market_service.get_ticker(symbol)
                 allocated = allocated + (position.amount * price["bid"])
 
         return allocated
+
+    def get_portfolio_configurations(self):
+        return self.portfolio_configuration_service.get_all()
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from time import sleep
 
 from flask import Flask
 
 from investing_algorithm_framework.app.algorithm import Algorithm
 from investing_algorithm_framework.app.stateless import ActionHandler
 from investing_algorithm_framework.app.strategy import TradingStrategy
+from investing_algorithm_framework.app.task import Task
 from investing_algorithm_framework.app.web import create_flask_app
 from investing_algorithm_framework.domain import DATABASE_NAME, TimeUnit, \
     DATABASE_DIRECTORY_PATH, RESOURCE_DIRECTORY, ENVIRONMENT, Environment, \
     ImproperlyConfigured, SQLALCHEMY_DATABASE_URI, Config, \
     OperationalException
 from investing_algorithm_framework.infrastructure import setup_sqlalchemy, \
     create_all_tables
@@ -29,83 +30,24 @@
         self.container = None
         self.config = Config.from_dict(config)
         self._stateless = stateless
         self._web = web
         self.algorithm: Algorithm = None
         self._started = False
         self._strategies = []
+        self._tasks = []
 
     def initialize(self):
 
         if self._web:
-
-            if RESOURCE_DIRECTORY not in self._config \
-                    and RESOURCE_DIRECTORY.upper() not in self._config:
-                raise ImproperlyConfigured(
-                    "RESOURCE_DIRECTORY not set in configuration"
-                )
-            resource_dir = self._config.get(RESOURCE_DIRECTORY, None)
-
-            if not resource_dir:
-                resource_dir = self._config.get(
-                    RESOURCE_DIRECTORY.upper(), None
-                )
-
-            if not os.path.exists(resource_dir):
-                try:
-                    os.makedirs(resource_dir)
-                except OSError as e:
-                    logger.error(e)
-                    raise OperationalException(
-                        f"Could not create resource directory: {e}"
-                    )
-
-            self._config[DATABASE_DIRECTORY_PATH] = os.path.join(
-                resource_dir, "databases"
-            )
-            self._config[DATABASE_NAME] = "prod-database.sqlite3"
-            self._config[SQLALCHEMY_DATABASE_URI] = \
-                "sqlite:///" + os.path.join(
-                self._config[DATABASE_DIRECTORY_PATH],
-                self._config[DATABASE_NAME]
-            )
-            self._flask_app = create_flask_app(self._config)
+            self._initialize_web()
         elif self._stateless:
-            self._config[SQLALCHEMY_DATABASE_URI] = "sqlite://"
+            self._initialize_stateless()
         else:
-            if RESOURCE_DIRECTORY not in self._config \
-                    and RESOURCE_DIRECTORY.upper() not in self._config:
-                raise ImproperlyConfigured(
-                    "RESOURCE_DIRECTORY not set in configuration"
-                )
-            resource_dir = self._config.get(RESOURCE_DIRECTORY, None)
-
-            if not resource_dir:
-                resource_dir = self._config.get(
-                    RESOURCE_DIRECTORY.upper(), None
-                )
-
-            if not os.path.exists(resource_dir):
-                try:
-                    os.makedirs(resource_dir)
-                except OSError as e:
-                    logger.error(e)
-                    raise OperationalException(
-                        f"Could not create resource directory: {e}"
-                    )
-
-            self._config[DATABASE_DIRECTORY_PATH] = os.path.join(
-                resource_dir, "databases"
-            )
-            self._config[DATABASE_NAME] = "prod-database.sqlite3"
-            self._config[SQLALCHEMY_DATABASE_URI] = \
-                "sqlite:///" + os.path.join(
-                    self._config[DATABASE_DIRECTORY_PATH],
-                    self._config[DATABASE_NAME]
-                )
+            self._initialize_standard()
 
         setup_sqlalchemy(self)
         create_all_tables()
 
     def _initialize_management_commands(self):
 
         if not Environment.TEST.equals(self.config.get(ENVIRONMENT)):
@@ -126,14 +68,15 @@
         self,
         payload: dict = None,
         number_of_iterations: int = None,
         sync=True
     ):
         self.algorithm = self.container.algorithm()
         self.algorithm.add_strategies(self.strategies)
+        self.algorithm.add_tasks(self.tasks)
         portfolio_configuration_service = self.container\
             .portfolio_configuration_service()
         portfolio_service = self.container.portfolio_service()
 
         if portfolio_configuration_service.count() == 0:
             raise OperationalException("No portfolios configured")
 
@@ -165,15 +108,15 @@
 
         try:
             while self.algorithm.running:
                 if number_of_iterations_since_last_orders_check == 30:
                     order_service.check_pending_orders()
                     number_of_iterations_since_last_orders_check = 1
 
-                self.algorithm.run_strategies()
+                self.algorithm.run_jobs()
                 number_of_iterations_since_last_orders_check += 1
                 sleep(1)
         except KeyboardInterrupt:
             exit(0)
 
     def start_algorithm(self):
         self.algorithm.start()
@@ -214,14 +157,40 @@
     def web(self):
         return self._web
 
     @property
     def running(self):
         return self.algorithm.running
 
+    def task(
+        self,
+        function=None,
+        time_unit: TimeUnit = TimeUnit.MINUTE,
+        interval=10,
+    ):
+        if function:
+            task = Task(
+                decorated=function,
+                time_unit=time_unit,
+                interval=interval,
+            )
+            self.add_task(task)
+        else:
+            def wrapper(f):
+                self.add_task(
+                    Task(
+                        decorated=f,
+                        time_unit=time_unit,
+                        interval=interval
+                    )
+                )
+                return f
+
+            return wrapper
+
     def strategy(
         self,
         function=None,
         time_unit: TimeUnit = TimeUnit.MINUTE,
         interval=10,
         market=None,
         trading_data_type=None,
@@ -274,23 +243,38 @@
     def add_strategy(self, strategy):
 
         if inspect.isclass(strategy):
             strategy = strategy()
 
         assert isinstance(strategy, TradingStrategy), \
             OperationalException(
-                "Strategy is not an instance of a Strategy"
+                "Strategy object is not an instance of a Strategy"
             )
 
         self._strategies.append(strategy)
 
+    def add_task(self, task):
+        if inspect.isclass(task):
+            task = task()
+
+        assert isinstance(task, Task), \
+            OperationalException(
+                "Task object is not an instance of a Task"
+            )
+
+        self._tasks.append(task)
+
     @property
     def strategies(self):
         return self._strategies
 
+    @property
+    def tasks(self):
+        return self._tasks
+
     def sync_portfolios(self):
         portfolio_configuration_service = self.container\
             .portfolio_configuration_service()
         portfolio_configuration_service.create_portfolios()
         portfolio_service = self.container.portfolio_service()
         portfolio_service.sync_portfolios()
 
@@ -300,14 +284,15 @@
         market_service = self.container.market_service()
         portfolio_repository = self.container.portfolio_repository()
         position_repository = self.container.position_repository()
 
         for portfolio_configuration in \
                 portfolio_configuration_service.get_all():
             market_service.initialize(portfolio_configuration)
+
             if portfolio_repository.exists(
                 {"identifier": portfolio_configuration.identifier}
             ):
                 continue
 
             balances = market_service.get_balance()
             if portfolio_configuration.trading_symbol.upper() not in balances:
@@ -333,7 +318,99 @@
             position_repository.create(
                 {
                     "symbol": portfolio_configuration.trading_symbol,
                     "amount": unallocated,
                     "portfolio_id": portfolio.id
                 }
             )
+
+    def _initialize_web(self):
+        resource_dir = self._config[RESOURCE_DIRECTORY]
+
+        if resource_dir is None:
+            self._config[SQLALCHEMY_DATABASE_URI] = "sqlite://"
+        else:
+            resource_dir = self._create_resource_directory_if_not_exists()
+            self._config[DATABASE_DIRECTORY_PATH] = os.path.join(
+                resource_dir, "databases"
+            )
+            self._config[DATABASE_NAME] = "prod-database.sqlite3"
+            self._config[SQLALCHEMY_DATABASE_URI] = \
+                "sqlite:///" + os.path.join(
+                    self._config[DATABASE_DIRECTORY_PATH],
+                    self._config[DATABASE_NAME]
+                )
+            self._create_database_if_not_exists()
+
+        self._flask_app = create_flask_app(self._config)
+
+    def _initialize_stateless(self):
+        self._config[SQLALCHEMY_DATABASE_URI] = "sqlite://"
+
+    def _initialize_standard(self):
+        resource_dir = self._config[RESOURCE_DIRECTORY]
+
+        if resource_dir is None:
+            self._config[SQLALCHEMY_DATABASE_URI] = "sqlite://"
+        else:
+            resource_dir = self._create_resource_directory_if_not_exists()
+            self._config[DATABASE_DIRECTORY_PATH] = os.path.join(
+                resource_dir, "databases"
+            )
+            self._config[DATABASE_NAME] = "prod-database.sqlite3"
+            self._config[SQLALCHEMY_DATABASE_URI] = \
+                "sqlite:///" + os.path.join(
+                    self._config[DATABASE_DIRECTORY_PATH],
+                    self._config[DATABASE_NAME]
+                )
+            self._create_database_if_not_exists()
+
+    def _create_resource_directory_if_not_exists(self):
+        if self._stateless:
+            return
+
+        resource_dir = self._config.get(RESOURCE_DIRECTORY, None)
+
+        if resource_dir is None:
+            return
+
+        if not os.path.exists(resource_dir):
+            try:
+                os.makedirs(resource_dir)
+                open(resource_dir, 'w').close()
+            except OSError as e:
+                logger.error(e)
+                raise OperationalException(
+                    "Could not create resource directory"
+                )
+
+        return resource_dir
+
+    def _create_database_if_not_exists(self):
+        if self._stateless:
+            return
+
+        database_dir = self._config.get(DATABASE_DIRECTORY_PATH, None)
+
+        if database_dir is None:
+            return
+
+        database_name = self._config.get(DATABASE_NAME, None)
+
+        if database_name is None:
+            return
+
+        database_path = os.path.join(database_dir, database_name)
+
+        if not os.path.exists(database_dir):
+            try:
+                os.makedirs(database_dir)
+                open(database_path, 'w').close()
+            except OSError as e:
+                logger.error(e)
+                raise OperationalException(
+                    "Could not create database directory"
+                )
+ 
+    def get_portfolio_configurations(self):
+        return self.algorithm.get_portfolio_configurations()
+
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/dependency_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 from dependency_injector import containers, providers
 
 from investing_algorithm_framework.infrastructure import SQLOrderRepository, \
-    SQLPositionRepository, MarketService, SQLPortfolioRepository
+    SQLPositionRepository, MarketService, SQLPortfolioRepository, \
+    SQLPositionCostRepository, SQLOrderFeeRepository
 from investing_algorithm_framework.services import OrderService, \
     PositionService, PortfolioService, StrategyOrchestratorService, \
-    PortfolioConfigurationService, MarketDataService
+    PortfolioConfigurationService, MarketDataService, PositionCostService
 from investing_algorithm_framework.app.algorithm import Algorithm
 
 
 def setup_dependency_container(app, modules=None, packages=None):
     app.container = DependencyContainer()
     app.container.wire(modules=modules, packages=packages)
     return app
 
 
 class DependencyContainer(containers.DeclarativeContainer):
     config = providers.Configuration()
     wiring_config = containers.WiringConfiguration()
     order_repository = providers.Factory(SQLOrderRepository)
+    order_fee_repository = providers.Factory(SQLOrderFeeRepository)
     position_repository = providers.Factory(SQLPositionRepository)
+    position_cost_repository = providers.Factory(SQLPositionCostRepository)
     portfolio_repository = providers.Factory(SQLPortfolioRepository)
     market_service = providers.Factory(MarketService)
     market_data_service = providers.Factory(
         MarketDataService,
         market_service=market_service
     )
-    portfolio_configuration_service = providers.Singleton(
+    portfolio_configuration_service = providers.ThreadSafeSingleton(
         PortfolioConfigurationService,
         market_service=market_service,
         portfolio_repository=portfolio_repository,
         position_repository=position_repository,
     )
     order_service = providers.Factory(
         OrderService,
+        position_cost_repository=position_cost_repository,
         order_repository=order_repository,
+        order_fee_repository=order_fee_repository,
         portfolio_repository=portfolio_repository,
         position_repository=position_repository,
         market_service=market_service,
         portfolio_configuration_service=portfolio_configuration_service,
     )
+    position_cost_service = providers.Factory(
+        PositionCostService,
+        repository=position_cost_repository,
+    )
     position_service = providers.Factory(
         PositionService,
         repository=position_repository,
         market_service=market_service,
     )
     portfolio_service = providers.Factory(
         PortfolioService,
         market_service=market_service,
         position_repository=position_repository,
-        order_repository=order_repository,
+        order_service=order_service,
         portfolio_repository=portfolio_repository,
         portfolio_configuration_service=portfolio_configuration_service
     )
     strategy_orchestrator_service = providers.Factory(
         StrategyOrchestratorService,
         market_data_service=market_data_service
     )
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .config import Config, Environment
 from .models import OrderStatus, OrderSide, OrderType, TimeInterval, \
     TimeUnit, TimeFrame, TradingTimeFrame, TradingDataType, Ticker, \
     OHLCV, OrderBook, PortfolioConfiguration, AssetPrice, Portfolio, \
-    Position, Order
+    Position, Order, PositionCost, OrderFee
 from .exceptions import OperationalException, ApiException, \
     PermissionDeniedApiException, ImproperlyConfigured
 from .constants import ITEMIZE, ITEMIZED, PER_PAGE, PAGE, ENVIRONMENT, \
     DATABASE_DIRECTORY_PATH, DATABASE_NAME, DEFAULT_PER_PAGE_VALUE, \
     DEFAULT_PAGE_VALUE, SQLALCHEMY_DATABASE_URI, RESOURCE_DIRECTORY, \
     DATETIME_FORMAT
 from .singleton import Singleton
@@ -55,9 +55,11 @@
     'Environment',
     "StoppableThread",
     "Portfolio",
     "Position",
     "Order",
     "Strategy",
     "DATETIME_FORMAT",
-    "StatelessActions"
+    "StatelessActions",
+    "PositionCost",
+    "OrderFee"
 ]
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DATABASE_CONFIG = 'DATABASE_CONFIG'
 DATABASE_NAME = 'DATABASE_NAME'
 DATABASE_TYPE = 'DATABASE_TYPE'
 DATABASE_DIRECTORY_PATH = 'DATABASE_DIRECTORY_PATH'
 DATABASE_URL = 'DATABASE_URL'
 DEFAULT_DATABASE_NAME = "database"
 
-RESOURCE_DIRECTORY = "resource_directory"
+RESOURCE_DIRECTORY = "RESOURCE_DIRECTORY"
 LOG_LEVEL = 'LOG_LEVEL'
 BASE_DIR = 'BASE_DIR'
 SQLALCHEMY_DATABASE_URI = 'SQLALCHEMY_DATABASE_URI'
 SQLITE_INITIALIZED = "SQLITE_INITIALIZED"
 SQLALCHEMY_INITIALIZED = "SQLALCHEMY_INITIALIZED"
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .order import OrderStatus, OrderSide, OrderType, Order
+from .order import OrderStatus, OrderSide, OrderType, Order, OrderFee
 from .time_frame import TimeFrame
 from .time_interval import TimeInterval
 from .time_unit import TimeUnit
 from .market_data import OHLCV, OrderBook, Ticker, AssetPrice
 from .trading_data_types import TradingDataType
 from .trading_time_frame import TradingTimeFrame
 from .portfolio import PortfolioConfiguration, Portfolio
-from .position import Position
+from .position import Position, PositionCost
 
 __all__ = [
     "OrderStatus",
     "OrderSide",
     "OrderType",
     "Order",
     "TimeFrame",
@@ -20,9 +20,11 @@
     "OrderBook",
     "Ticker",
     "TradingTimeFrame",
     "TradingDataType",
     "PortfolioConfiguration",
     "AssetPrice",
     "Position",
-    "Portfolio"
+    "PositionCost",
+    "Portfolio",
+    "OrderFee"
 ]
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/asset_price.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/asset_price.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/ohlcv.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ohlcv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/order_book.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/order_book.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/market_data/ticker.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/market_data/ticker.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         identifier=None,
         max_unallocated=-1,
     ):
         self._market = market
         self._api_key = api_key
         self._secret_key = secret_key
         self._track_from = None
-        self._trading_symbol = trading_symbol
+        self._trading_symbol = trading_symbol.upper()
         self._identifier = identifier
         self._max_unallocated = max_unallocated
 
         if self.identifier is None:
             self._identifier = market.lower()
 
         if track_from:
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-from os import mkdir, path
 import logging
 
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, StaticPool
 from sqlalchemy.orm import DeclarativeBase, sessionmaker
 
 from investing_algorithm_framework.domain import SQLALCHEMY_DATABASE_URI, \
-    OperationalException, DATABASE_NAME, DATABASE_DIRECTORY_PATH
+    OperationalException
 
 Session = sessionmaker()
 logger = logging.getLogger(__name__)
 
 
 class SQLAlchemyAdapter:
 
     def __init__(self, app):
-
+        self._app = app
         if SQLALCHEMY_DATABASE_URI not in app.config \
                 or app.config[SQLALCHEMY_DATABASE_URI] is None:
             raise OperationalException("SQLALCHEMY_DATABASE_URI not set")
 
-        if not app.stateless:
-            database_dir = app.config[DATABASE_DIRECTORY_PATH]
-            database_name = app.config[DATABASE_NAME]
-            database_path = path.join(database_dir, database_name)
-
-            if not path.exists(database_dir):
-                try:
-                    mkdir(database_dir)
-                    open(database_path, 'w').close()
-                except OSError as e:
-                    logger.error(e)
-                    raise OperationalException(
-                        "Could not create database directory"
-                    )
-
         global Session
-        engine = create_engine(app.config[SQLALCHEMY_DATABASE_URI])
+
+        if app.config[SQLALCHEMY_DATABASE_URI] != "sqlite:///:memory:":
+            engine = create_engine(
+                app.config[SQLALCHEMY_DATABASE_URI],
+                connect_args={'check_same_thread': False},
+                poolclass=StaticPool
+            )
+        else:
+            engine = create_engine(
+                app.config[SQLALCHEMY_DATABASE_URI],
+            )
+
         Session.configure(bind=engine)
 
 
 def setup_sqlalchemy(app, throw_exception_if_not_set=True):
 
     try:
         SQLAlchemyAdapter(app)
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     __tablename__ = "portfolios"
     id = Column(Integer, primary_key=True)
     identifier = Column(String, nullable=False, unique=True)
     trading_symbol = Column(String, nullable=False)
     realized = Column(Float, nullable=False, default=0)
     total_revenue = Column(Float, nullable=False, default=0)
     total_cost = Column(Float, nullable=False, default=0)
+    total_net_gain = Column(Float, nullable=False, default=0)
+    unallocated = Column(Float, nullable=False, default=0)
     market = Column(String, nullable=False)
     positions = relationship(
         "SQLPosition",
         back_populates="portfolio",
         lazy="dynamic",
         cascade="all,delete",
     )
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     amount = Column(Float)
     orders = relationship(
         "SQLOrder",
         back_populates="position",
         lazy="dynamic",
         cascade="all, delete-orphan"
     )
+    position_costs = relationship(
+        "SQLPositionCost",
+        back_populates="position",
+        lazy="dynamic",
+        cascade="all, delete-orphan"
+    )
     portfolio_id = Column(Integer, ForeignKey('portfolios.id'))
     portfolio = relationship("SQLPortfolio", back_populates="positions")
     __table_args__ = (
         UniqueConstraint(
             'symbol', 'portfolio_id', name='_symbol_portfolio_uc'
         ),
     )
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,15 @@
         portfolio_query_param = self.get_query_param(
             "portfolio_id", query_params
         )
         side_query_param = self.get_query_param("side", query_params)
         type_query_param = self.get_query_param("type", query_params)
         status_query_param = self.get_query_param("status", query_params)
         price_query_param = self.get_query_param("price", query_params)
-        amount_target_symbol_query_param = \
-            self.get_query_param("amount_target_symbol", query_params)
-        amount_trading_symbol_query_param = \
-            self.get_query_param("amount_trading_symbol", query_params)
+        amount_query_param = self.get_query_param("amount", query_params)
         position_query_param = self.get_query_param(
             "position", query_params, many=True
         )
         target_symbol_query_param = self.get_query_param(
             "symbol", query_params
         )
         trading_symbol_query_param = self.get_query_param(
@@ -60,23 +57,16 @@
         if status_query_param:
             status = OrderStatus.from_value(status_query_param)
             query = query.filter_by(status=status.value)
 
         if price_query_param:
             query = query.filter(SQLOrder.price == price_query_param)
 
-        if amount_target_symbol_query_param:
-            query = query.filter_by(
-                amount_target_symbol=amount_target_symbol_query_param
-            )
-
-        if amount_trading_symbol_query_param:
-            query = query.filter_by(
-                amount_trading_symbol=amount_trading_symbol_query_param
-            )
+        if amount_query_param:
+            query = query.filter_by(amount=amount_query_param)
 
         if position_query_param:
             query = query.filter(SQLOrder.position_id.in_(
                 position_query_param)
             )
 
         if target_symbol_query_param:
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/infrastructure/services/market_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/infrastructure/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from .order_service import OrderService
 from .portfolio_service import PortfolioService
 from .position_service import PositionService
+from .position_cost_service import PositionCostService
 from .repository_service import RepositoryService
 from .strategy_orchestrator_service import StrategyOrchestratorService
 from .portfolio_configuration_service import PortfolioConfigurationService
 from .market_data_service import MarketDataService
 
 __all__ = [
     "StrategyOrchestratorService",
     "OrderService",
     "RepositoryService",
     "PortfolioService",
     "PositionService",
     "PortfolioConfigurationService",
-    "MarketDataService"
+    "MarketDataService",
+    "PositionCostService"
 ]
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/market_data_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/market_data_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     def get_data_for_strategy(self, strategy):
         data = {}
 
         if strategy.market and \
                 (strategy.trading_data_types or strategy.trading_data_type):
             self.market_service.market = strategy.market
 
+            if not strategy.trading_data_types:
+                strategy.trading_data_types = [strategy.trading_data_type]
+
             for trading_data_type in strategy.trading_data_types:
 
                 if TradingDataType.TICKER.equals(trading_data_type):
                     data["tickers"] = self.market_service.get_tickers(
                         symbols=strategy.symbols
                     )
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/portfolio_configuration_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_configuration_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,20 +11,24 @@
         self.market_service = market_service
         self.portfolio_configurations = []
 
     def add(self, portfolio_configuration):
         self.portfolio_configurations.append(portfolio_configuration)
 
     def get(self, identifier):
-        return next(
+        portfolio_configuration = next(
             (portfolio_configuration for portfolio_configuration in
                 self.portfolio_configurations if
                 portfolio_configuration.market == identifier.lower()),
             None
         )
+        if portfolio_configuration is None:
+            raise ApiException('Portfolio configuration not found', 404)
+
+        return portfolio_configuration
 
     def find(self, query_params):
         market = query_params.get("market", None)
         identifier = query_params.get("market", None)
 
         if market is not None:
             return next(
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/portfolio_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/portfolio_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 class PortfolioService(RepositoryService):
 
     def __init__(
         self,
         market_service,
         position_repository,
-        order_repository,
+        order_service,
         portfolio_repository,
         portfolio_configuration_service,
     ):
         self.market_service = market_service
         self.position_repository = position_repository
         self.portfolio_configuration_service = portfolio_configuration_service
-        self.order_repository = order_repository
+        self.order_service = order_service
         super(PortfolioService, self).__init__(portfolio_repository)
 
     def create(self, data):
         unallocated = data.get("unallocated", 0)
         del data["unallocated"]
         portfolio = super(PortfolioService, self).create(data)
         self.position_repository.create(
@@ -75,15 +75,24 @@
                 external_orders = self.market_service\
                     .get_orders(
                         f"{position.symbol}/{portfolio.trading_symbol}",
                         since=portfolio_configuration.track_from
                     )
 
                 for external_order in external_orders:
-                    if self.order_repository.exists(
+
+                    if self.order_service.exists(
                         {"external_id": external_order.external_id}
                     ):
-                        continue
-
-                    data = external_order.to_dict()
-                    data["position_id"] = position.id
-                    self.order_repository.create(data)
+                        order = self.order_service.find(
+                            {"external_id": external_order.external_id}
+                        )
+                        self.order_service.update(
+                            order.id, external_order.to_dict()
+                        )
+                    else:
+                        data = external_order.to_dict()
+                        data["position_id"] = position.id
+                        data["portfolio_id"] = portfolio.id
+                        self.order_service.create(
+                            data, execute=False, validate=False, sync=False
+                        )
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     OperationalException
 
 
 class StrategyOrchestratorService:
 
     def __init__(self, market_data_service):
         self.history = {}
-        self.strategies = []
+        self._strategies = []
+        self._tasks = []
         self.threads = []
         self.iterations = 0
         self.max_iterations = -1
         self.clear()
         self.market_data_service = market_data_service
 
     def cleanup_threads(self):
@@ -53,34 +54,66 @@
             )
             thread.name = strategy.worker_id
             thread.start()
             self.threads.append(thread)
 
         self.history[strategy.worker_id] = {"last_run": datetime.utcnow()}
 
+    def run_task(self, task, algorithm, sync=False):
+        self.cleanup_threads()
+
+        matching_thread = next(
+            (t for t in self.threads if t.name == task.worker_id),
+            None
+        )
+
+        # Don't run a strategy that is already running
+        if matching_thread:
+            return
+
+        if sync:
+            task.run(algorithm=algorithm)
+        else:
+            self.iterations += 1
+            thread = StoppableThread(
+                target=task.run,
+                kwargs={"algorithm": algorithm}
+            )
+            thread.name = task.worker_id
+            thread.start()
+            self.threads.append(thread)
+
+        self.history[task.worker_id] = {"last_run": datetime.utcnow()}
+
     def start(self, algorithm, number_of_iterations=None):
         self.max_iterations = number_of_iterations
 
         for strategy in self.strategies:
 
             if TimeUnit.SECOND.equals(strategy.time_unit):
                 schedule.every(strategy.interval)\
-                    .seconds.do(
-                        self.run_strategy, strategy, algorithm
-                    )
+                    .seconds.do(self.run_strategy, strategy, algorithm)
             elif TimeUnit.MINUTE.equals(strategy.time_unit):
                 schedule.every(strategy.interval)\
-                    .minutes.do(
-                        self.run_strategy, strategy, algorithm
-                    )
+                    .minutes.do(self.run_strategy, strategy, algorithm)
             elif TimeUnit.HOUR.equals(strategy.time_unit):
                 schedule.every(strategy.interval)\
-                    .hours.do(
-                        self.run_strategy, strategy, algorithm
-                    )
+                    .hours.do(self.run_strategy, strategy, algorithm)
+
+        for task in self.tasks:
+            
+            if TimeUnit.SECOND.equals(task.time_unit):
+                schedule.every(task.interval)\
+                    .seconds.do(self.run_task, task, algorithm)
+            elif TimeUnit.MINUTE.equals(task.time_unit):
+                schedule.every(task.interval)\
+                    .minutes.do(self.run_task, task, algorithm)
+            elif TimeUnit.HOUR.equals(task.time_unit):
+                schedule.every(task.interval)\
+                    .hours.do(self.run_task, task, algorithm)
 
     def stop(self):
         for thread in self.threads:
             thread.stop()
 
         schedule.clear()
 
@@ -95,15 +128,18 @@
         strategies = []
         for strategy in self.strategies:
             if strategy.worker_id in identifiers:
                 strategies.append(strategy)
 
         return strategies
 
-    def run_pending_strategies(self):
+    def get_jobs(self):
+        return schedule.jobs
+
+    def run_pending_jobs(self):
 
         if self.max_iterations is not None and \
                 self.max_iterations != -1 and \
                 self.iterations >= self.max_iterations:
             self.clear()
         else:
             schedule.run_pending()
@@ -129,25 +165,49 @@
         if has_duplicates:
             raise OperationalException(
                 "There are duplicate strategies with the same name"
             )
 
         self.strategies = strategies
 
+    def add_tasks(self, tasks):
+        has_duplicates = False
+
+        for i in range(len(tasks)):
+            for j in range(i + 1, len(tasks)):
+                if tasks[i].worker_id == tasks[j].worker_id:
+                    has_duplicates = True
+                    break
+
+        if has_duplicates:
+            raise OperationalException(
+                "There are duplicate tasks with the same name"
+            )
+
+        self.tasks = tasks
+
     @property
     def strategies(self):
         return self._strategies
 
     @strategies.setter
     def strategies(self, strategies):
         self._strategies = strategies
 
     @property
+    def tasks(self):
+        return self._tasks
+
+    @tasks.setter
+    def tasks(self, tasks):
+        self._tasks = tasks
+
+    @property
     def running(self):
-        if len(self.strategies) == 0:
+        if len(self.strategies) == 0 and len(self.tasks) == 0:
             return False
 
         if self.max_iterations == -1:
             return True
 
         return self.max_iterations is None \
             or self.iterations < self.max_iterations
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework/setup_logging.py` & `investing_algorithm_framework-1.1/investing_algorithm_framework/setup_logging.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/PKG-INFO` & `investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 1.0
+Version: 1.1
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
 Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
 Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
```

### Comparing `investing_algorithm_framework-1.0/investing_algorithm_framework.egg-info/SOURCES.txt` & `investing_algorithm_framework-1.1/investing_algorithm_framework.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 investing_algorithm_framework.egg-info/dependency_links.txt
 investing_algorithm_framework.egg-info/requires.txt
 investing_algorithm_framework.egg-info/top_level.txt
 investing_algorithm_framework/app/__init__.py
 investing_algorithm_framework/app/algorithm.py
 investing_algorithm_framework/app/app.py
 investing_algorithm_framework/app/strategy.py
+investing_algorithm_framework/app/task.py
 investing_algorithm_framework/app/stateless/__init__.py
 investing_algorithm_framework/app/stateless/exception_handler.py
 investing_algorithm_framework/app/stateless/action_handlers/__init__.py
 investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
 investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
 investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
 investing_algorithm_framework/app/web/__init__.py
@@ -53,48 +54,55 @@
 investing_algorithm_framework/domain/models/market_data/__init__.py
 investing_algorithm_framework/domain/models/market_data/asset_price.py
 investing_algorithm_framework/domain/models/market_data/ohlcv.py
 investing_algorithm_framework/domain/models/market_data/order_book.py
 investing_algorithm_framework/domain/models/market_data/ticker.py
 investing_algorithm_framework/domain/models/order/__init__.py
 investing_algorithm_framework/domain/models/order/order.py
+investing_algorithm_framework/domain/models/order/order_fee.py
 investing_algorithm_framework/domain/models/order/order_side.py
 investing_algorithm_framework/domain/models/order/order_status.py
 investing_algorithm_framework/domain/models/order/order_type.py
 investing_algorithm_framework/domain/models/portfolio/__init__.py
 investing_algorithm_framework/domain/models/portfolio/portfolio.py
 investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
 investing_algorithm_framework/domain/models/position/__init__.py
 investing_algorithm_framework/domain/models/position/position.py
+investing_algorithm_framework/domain/models/position/position_cost.py
 investing_algorithm_framework/domain/utils/__init__.py
 investing_algorithm_framework/domain/utils/csv.py
 investing_algorithm_framework/domain/utils/random.py
 investing_algorithm_framework/domain/utils/signatures.py
 investing_algorithm_framework/domain/utils/stoppable_thread.py
 investing_algorithm_framework/domain/utils/synchronized.py
 investing_algorithm_framework/infrastructure/__init__.py
 investing_algorithm_framework/infrastructure/database/__init__.py
 investing_algorithm_framework/infrastructure/database/sql_alchemy.py
 investing_algorithm_framework/infrastructure/models/__init__.py
 investing_algorithm_framework/infrastructure/models/model_extension.py
 investing_algorithm_framework/infrastructure/models/order/__init__.py
 investing_algorithm_framework/infrastructure/models/order/order.py
+investing_algorithm_framework/infrastructure/models/order/order_fee.py
 investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
 investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
 investing_algorithm_framework/infrastructure/models/position/__init__.py
 investing_algorithm_framework/infrastructure/models/position/position.py
+investing_algorithm_framework/infrastructure/models/position/position_cost.py
 investing_algorithm_framework/infrastructure/repositories/__init__.py
+investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
 investing_algorithm_framework/infrastructure/repositories/order_repository.py
 investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py
 investing_algorithm_framework/infrastructure/repositories/position_repository.py
 investing_algorithm_framework/infrastructure/repositories/repository.py
 investing_algorithm_framework/infrastructure/services/__init__.py
 investing_algorithm_framework/infrastructure/services/market_service.py
 investing_algorithm_framework/services/__init__.py
 investing_algorithm_framework/services/market_data_service.py
 investing_algorithm_framework/services/order_service.py
 investing_algorithm_framework/services/portfolio_configuration_service.py
 investing_algorithm_framework/services/portfolio_service.py
+investing_algorithm_framework/services/position_cost_service.py
 investing_algorithm_framework/services/position_service.py
 investing_algorithm_framework/services/repository_service.py
 investing_algorithm_framework/services/strategy_orchestrator_service.py
 tests/test_create_app.py
```

### Comparing `investing_algorithm_framework-1.0/setup.py` & `investing_algorithm_framework-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.0/tests/test_create_app.py` & `investing_algorithm_framework-1.1/tests/test_create_app.py`

 * *Files identical despite different names*

