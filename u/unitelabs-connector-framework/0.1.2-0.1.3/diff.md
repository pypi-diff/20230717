# Comparing `tmp/unitelabs_connector_framework-0.1.2.tar.gz` & `tmp/unitelabs_connector_framework-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitelabs_connector_framework-0.1.2.tar", max compression
+gzip compressed data, was "unitelabs_connector_framework-0.1.3.tar", max compression
```

## Comparing `unitelabs_connector_framework-0.1.2.tar` & `unitelabs_connector_framework-0.1.3.tar`

### file list

```diff
@@ -1,78 +1,80 @@
--rw-r--r--   0        0        0     1069 2023-06-11 17:51:12.165815 unitelabs_connector_framework-0.1.2/LICENSE
--rw-r--r--   0        0        0     3026 2023-06-18 10:34:53.733054 unitelabs_connector_framework-0.1.2/README.md
--rw-r--r--   0        0        0     2061 2023-06-27 06:23:35.106315 unitelabs_connector_framework-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-14 09:28:37.005175 unitelabs_connector_framework-0.1.2/src/unitelabs/__init__.py
--rw-r--r--   0        0        0     1235 2023-06-10 08:57:12.994027 unitelabs_connector_framework-0.1.2/src/unitelabs/cli.py
--rw-r--r--   0        0        0      454 2023-06-10 08:19:00.892129 unitelabs_connector_framework-0.1.2/src/unitelabs/config.py
--rw-r--r--   0        0        0     1751 2023-06-18 10:34:53.743165 unitelabs_connector_framework-0.1.2/src/unitelabs/connector.py
--rw-r--r--   0        0        0     4429 2023-06-08 12:21:47.568189 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto
--rw-r--r--   0        0        0     5518 2023-06-08 12:21:47.572050 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml
--rw-r--r--   0        0        0      321 2023-06-08 12:21:47.573953 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/__init__.py
--rw-r--r--   0        0        0     3755 2023-06-25 20:18:33.251237 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller.py
--rw-r--r--   0        0        0     3421 2023-06-27 06:15:54.669793 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller_base.py
--rw-r--r--   0        0        0     7109 2023-06-08 12:01:08.346706 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto
--rw-r--r--   0        0        0     7902 2023-06-08 11:43:41.586033 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml
--rw-r--r--   0        0        0      111 2023-06-08 12:01:41.537455 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/__init__.py
--rw-r--r--   0        0        0     5936 2023-06-18 10:26:38.076224 unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/sila_service.py
--rw-r--r--   0        0        0       93 2023-06-18 10:34:53.743616 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/greeting_provider/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-18 10:34:53.744341 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py
--rw-r--r--   0        0        0       84 2023-06-18 10:34:53.744719 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/timer_provider/__init__.py
--rw-r--r--   0        0        0     1838 2023-06-18 10:34:53.745303 unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/timer_provider/timer_provider_base.py
--rw-r--r--   0        0        0      750 2023-06-27 06:15:54.670076 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/GripController-v1_0.proto
--rw-r--r--   0        0        0      954 2023-06-27 06:15:54.670865 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/GripController-v1_0.sila.xml
--rw-r--r--   0        0        0       87 2023-06-27 06:15:54.671502 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/__init__.py
--rw-r--r--   0        0        0      637 2023-06-27 06:15:54.671777 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/grip_controller_base.py
--rw-r--r--   0        0        0    14833 2023-06-27 05:46:00.048776 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto
--rw-r--r--   0        0        0    15654 2023-06-08 18:31:02.343015 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml
--rw-r--r--   0        0        0      407 2023-06-14 09:34:31.175200 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/__init__.py
--rw-r--r--   0        0        0    11465 2023-06-27 06:05:53.910295 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py
--rw-r--r--   0        0        0     3371 2023-06-27 06:02:55.958059 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.proto
--rw-r--r--   0        0        0     3602 2023-06-27 06:02:55.959024 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.sila.xml
--rw-r--r--   0        0        0      165 2023-06-27 06:02:55.959301 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/__init__.py
--rw-r--r--   0        0        0     2046 2023-06-27 06:02:55.960189 unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/movement_controller_base.py
--rw-r--r--   0        0        0     8041 2023-06-08 15:58:40.585326 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto
--rw-r--r--   0        0        0     8279 2023-06-08 15:58:37.034762 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml
--rw-r--r--   0        0        0       88 2023-06-08 15:56:50.422431 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/__init__.py
--rw-r--r--   0        0        0     5190 2023-06-11 10:29:43.300577 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py
--rw-r--r--   0        0        0     2891 2023-06-03 08:08:38.591011 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto
--rw-r--r--   0        0        0     2846 2023-06-10 09:38:31.720888 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml
--rw-r--r--   0        0        0       96 2023-05-07 08:13:10.387701 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/__init__.py
--rw-r--r--   0        0        0     2383 2023-06-25 19:52:23.455657 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/observable_command_test.py
--rw-r--r--   0        0        0     2146 2023-06-10 08:52:51.902499 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto
--rw-r--r--   0        0        0     1820 2023-06-10 08:52:10.669356 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml
--rw-r--r--   0        0        0       99 2023-06-10 08:56:35.314045 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/__init__.py
--rw-r--r--   0        0        0     1625 2023-06-10 09:22:10.087811 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/observable_property_test.py
--rw-r--r--   0        0        0     3147 2023-06-08 15:10:15.841233 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto
--rw-r--r--   0        0        0     4090 2023-06-08 15:12:39.575863 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml
--rw-r--r--   0        0        0      102 2023-06-08 15:57:00.405056 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/__init__.py
--rw-r--r--   0        0        0     2006 2023-06-11 10:22:39.326761 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py
--rw-r--r--   0        0        0     1465 2023-06-08 14:12:11.083908 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto
--rw-r--r--   0        0        0     1250 2023-06-08 14:13:49.773291 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml
--rw-r--r--   0        0        0      105 2023-06-08 14:14:24.590503 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/__init__.py
--rw-r--r--   0        0        0      725 2023-06-10 08:57:12.994633 unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py
--rw-r--r--   0        0        0     4157 2023-06-03 08:14:35.038359 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto
--rw-r--r--   0        0        0     8446 2023-05-07 08:33:49.313366 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml
--rw-r--r--   0        0        0       85 2023-06-03 08:14:35.038563 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/__init__.py
--rw-r--r--   0        0        0     2839 2023-06-11 10:28:57.427186 unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/weighing_service.py
--rw-r--r--   0        0        0      541 2023-06-06 19:24:50.656991 unitelabs_connector_framework-0.1.2/src/unitelabs/logging.py
--rw-r--r--   0        0        0        0 2023-06-12 08:59:43.667279 unitelabs_connector_framework-0.1.2/src/unitelabs/py.typed
--rw-r--r--   0        0        0     1140 2023-06-27 06:02:55.961038 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 09:33:36.508770 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/__init__.py
--rw-r--r--   0        0        0      425 2023-06-11 09:59:16.304398 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/intermediate.py
--rw-r--r--   0        0        0     1188 2023-06-11 10:57:11.616229 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/intermediate_response.py
--rw-r--r--   0        0        0     1455 2023-06-11 10:57:13.280572 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/response.py
--rw-r--r--   0        0        0      776 2023-06-27 06:15:54.672163 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/status.py
--rw-r--r--   0        0        0      661 2023-06-27 06:02:55.962831 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/__init__.py
--rw-r--r--   0        0        0      701 2023-06-19 12:58:38.071860 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/custom_data_type.py
--rw-r--r--   0        0        0     1513 2023-06-19 12:58:38.072789 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/data_type_definition.py
--rw-r--r--   0        0        0     3795 2023-06-19 12:58:38.073840 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/parser.py
--rw-r--r--   0        0        0      651 2023-06-19 10:48:02.425135 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/defined_execution_error.py
--rw-r--r--   0        0        0     1249 2023-06-19 10:47:59.222382 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/feature.py
--rw-r--r--   0        0        0      675 2023-06-19 10:47:57.307171 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/metadata.py
--rw-r--r--   0        0        0     4852 2023-06-19 12:58:38.074888 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_command.py
--rw-r--r--   0        0        0     1539 2023-06-19 12:58:38.075687 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_property.py
--rw-r--r--   0        0        0     3765 2023-06-19 12:58:38.076635 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_command.py
--rw-r--r--   0        0        0     1400 2023-06-19 12:58:38.077493 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_property.py
--rw-r--r--   0        0        0     2314 2023-06-06 20:10:09.131560 unitelabs_connector_framework-0.1.2/src/unitelabs/sila/utils.py
--rw-r--r--   0        0        0      307 2023-04-04 16:41:46.514608 unitelabs_connector_framework-0.1.2/src/unitelabs/utils.py
--rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 unitelabs_connector_framework-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-11 17:51:12.165815 unitelabs_connector_framework-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3026 2023-06-18 10:34:53.733054 unitelabs_connector_framework-0.1.3/README.md
+-rw-r--r--   0        0        0     2082 2023-07-17 14:02:13.425911 unitelabs_connector_framework-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-07-17 13:59:05.154198 unitelabs_connector_framework-0.1.3/src/unitelabs/__init__.py
+-rw-r--r--   0        0        0      110 2023-07-17 13:59:05.155112 unitelabs_connector_framework-0.1.3/src/unitelabs/cli/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-17 13:59:05.156124 unitelabs_connector_framework-0.1.3/src/unitelabs/cli/certificate.py
+-rw-r--r--   0        0        0     1544 2023-07-17 13:59:05.156820 unitelabs_connector_framework-0.1.3/src/unitelabs/cli/connector.py
+-rw-r--r--   0        0        0      457 2023-07-17 13:59:05.158156 unitelabs_connector_framework-0.1.3/src/unitelabs/config.py
+-rw-r--r--   0        0        0     1671 2023-07-17 13:59:05.159122 unitelabs_connector_framework-0.1.3/src/unitelabs/connector.py
+-rw-r--r--   0        0        0     4429 2023-06-08 12:21:47.568189 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto
+-rw-r--r--   0        0        0     5518 2023-06-08 12:21:47.572050 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml
+-rw-r--r--   0        0        0      321 2023-06-08 12:21:47.573953 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/__init__.py
+-rw-r--r--   0        0        0     3755 2023-06-25 20:18:33.251237 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/lock_controller.py
+-rw-r--r--   0        0        0     3421 2023-06-27 06:15:54.669793 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/lock_controller_base.py
+-rw-r--r--   0        0        0     7109 2023-06-08 12:01:08.346706 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto
+-rw-r--r--   0        0        0     7902 2023-06-08 11:43:41.586033 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml
+-rw-r--r--   0        0        0      111 2023-06-08 12:01:41.537455 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/__init__.py
+-rw-r--r--   0        0        0     5936 2023-07-14 16:09:39.839935 unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/sila_service.py
+-rw-r--r--   0        0        0       93 2023-06-18 10:34:53.743616 unitelabs_connector_framework-0.1.3/src/unitelabs/features/examples/greeting_provider/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-18 10:34:53.744341 unitelabs_connector_framework-0.1.3/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py
+-rw-r--r--   0        0        0       84 2023-06-18 10:34:53.744719 unitelabs_connector_framework-0.1.3/src/unitelabs/features/examples/timer_provider/__init__.py
+-rw-r--r--   0        0        0     1838 2023-06-18 10:34:53.745303 unitelabs_connector_framework-0.1.3/src/unitelabs/features/examples/timer_provider/timer_provider_base.py
+-rw-r--r--   0        0        0      750 2023-06-27 06:15:54.670076 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/GripController-v1_0.proto
+-rw-r--r--   0        0        0      954 2023-06-27 06:15:54.670865 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/GripController-v1_0.sila.xml
+-rw-r--r--   0        0        0       87 2023-06-27 06:15:54.671502 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-27 06:15:54.671777 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/grip_controller_base.py
+-rw-r--r--   0        0        0    14833 2023-06-27 05:46:00.048776 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto
+-rw-r--r--   0        0        0    15654 2023-06-08 18:31:02.343015 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml
+-rw-r--r--   0        0        0      407 2023-06-14 09:34:31.175200 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/__init__.py
+-rw-r--r--   0        0        0    11465 2023-06-27 06:05:53.910295 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py
+-rw-r--r--   0        0        0     3371 2023-06-27 06:02:55.958059 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.proto
+-rw-r--r--   0        0        0     3602 2023-06-27 06:02:55.959024 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.sila.xml
+-rw-r--r--   0        0        0      165 2023-06-27 06:02:55.959301 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/__init__.py
+-rw-r--r--   0        0        0     2046 2023-06-27 06:02:55.960189 unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/movement_controller_base.py
+-rw-r--r--   0        0        0     8041 2023-07-03 09:42:04.334723 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto
+-rw-r--r--   0        0        0     8279 2023-06-08 15:58:37.034762 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       88 2023-06-08 15:56:50.422431 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/__init__.py
+-rw-r--r--   0        0        0     5190 2023-07-03 09:42:04.335881 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py
+-rw-r--r--   0        0        0     2891 2023-06-03 08:08:38.591011 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto
+-rw-r--r--   0        0        0     2846 2023-06-10 09:38:31.720888 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       96 2023-05-07 08:13:10.387701 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/__init__.py
+-rw-r--r--   0        0        0     2383 2023-07-03 09:42:37.132539 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/observable_command_test.py
+-rw-r--r--   0        0        0     2146 2023-06-10 08:52:51.902499 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto
+-rw-r--r--   0        0        0     1820 2023-06-10 08:52:10.669356 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml
+-rw-r--r--   0        0        0       99 2023-06-10 08:56:35.314045 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/__init__.py
+-rw-r--r--   0        0        0     1625 2023-07-03 09:42:04.338055 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/observable_property_test.py
+-rw-r--r--   0        0        0     3147 2023-06-08 15:10:15.841233 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto
+-rw-r--r--   0        0        0     4090 2023-06-08 15:12:39.575863 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml
+-rw-r--r--   0        0        0      102 2023-06-08 15:57:00.405056 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/__init__.py
+-rw-r--r--   0        0        0     2006 2023-07-03 09:42:04.339024 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py
+-rw-r--r--   0        0        0     1465 2023-06-08 14:12:11.083908 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto
+-rw-r--r--   0        0        0     1250 2023-06-08 14:13:49.773291 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml
+-rw-r--r--   0        0        0      105 2023-06-08 14:14:24.590503 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-03 09:42:04.339677 unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py
+-rw-r--r--   0        0        0     4157 2023-06-03 08:14:35.038359 unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto
+-rw-r--r--   0        0        0     8446 2023-05-07 08:33:49.313366 unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml
+-rw-r--r--   0        0        0       85 2023-06-03 08:14:35.038563 unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/__init__.py
+-rw-r--r--   0        0        0     2839 2023-06-11 10:28:57.427186 unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/weighing_service.py
+-rw-r--r--   0        0        0      669 2023-07-17 13:59:05.159962 unitelabs_connector_framework-0.1.3/src/unitelabs/logging.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:59:43.667279 unitelabs_connector_framework-0.1.3/src/unitelabs/py.typed
+-rw-r--r--   0        0        0     1140 2023-06-27 06:02:55.961038 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 09:33:36.508770 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-11 09:59:16.304398 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/intermediate.py
+-rw-r--r--   0        0        0     1188 2023-06-11 10:57:11.616229 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/intermediate_response.py
+-rw-r--r--   0        0        0     1455 2023-06-11 10:57:13.280572 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/response.py
+-rw-r--r--   0        0        0      776 2023-06-27 06:15:54.672163 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/status.py
+-rw-r--r--   0        0        0      661 2023-06-27 06:02:55.962831 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-19 12:58:38.071860 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/custom_data_type.py
+-rw-r--r--   0        0        0     1513 2023-06-19 12:58:38.072789 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/data_type_definition.py
+-rw-r--r--   0        0        0     3795 2023-06-19 12:58:38.073840 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/parser.py
+-rw-r--r--   0        0        0      651 2023-06-19 10:48:02.425135 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/defined_execution_error.py
+-rw-r--r--   0        0        0     1249 2023-06-19 10:47:59.222382 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/feature.py
+-rw-r--r--   0        0        0      675 2023-06-19 10:47:57.307171 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/metadata.py
+-rw-r--r--   0        0        0     4852 2023-06-19 12:58:38.074888 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/observable_command.py
+-rw-r--r--   0        0        0     1539 2023-06-19 12:58:38.075687 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/observable_property.py
+-rw-r--r--   0        0        0     3765 2023-06-19 12:58:38.076635 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/unobservable_command.py
+-rw-r--r--   0        0        0     1400 2023-06-19 12:58:38.077493 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/unobservable_property.py
+-rw-r--r--   0        0        0     2314 2023-06-06 20:10:09.131560 unitelabs_connector_framework-0.1.3/src/unitelabs/sila/utils.py
+-rw-r--r--   0        0        0      307 2023-07-14 07:41:52.979402 unitelabs_connector_framework-0.1.3/src/unitelabs/utils.py
+-rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 unitelabs_connector_framework-0.1.3/PKG-INFO
```

### Comparing `unitelabs_connector_framework-0.1.2/LICENSE` & `unitelabs_connector_framework-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/README.md` & `unitelabs_connector_framework-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/pyproject.toml` & `unitelabs_connector_framework-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitelabs-connector-framework"
-version = "0.1.2"
+version = "0.1.3"
 description = "A framework to build connectors based on the SiLA 2 standard specification."
 license = "MIT"
 authors = ["UniteLabs AG <developers+connector@unitelabs.ch>"]
 readme = "README.md"
 homepage = "https://unitelabs.ch"
 repository = "https://gitlab.com/unitelabs/connector-framework"
 documentation = "https://gitlab.com/unitelabs/connector-framework/-/tree/main/docs/"
@@ -26,21 +26,22 @@
 ]
 packages = [{ include = "unitelabs", from = "src" }]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://gitlab.com/unitelabs/connector-framework/-/issues"
 
 [tool.poetry.scripts]
-connector = 'unitelabs.cli:cli'
+certificate = 'unitelabs.cli:certificate'
+connector = 'unitelabs.cli:connector'
 
 [tool.poetry.dependencies]
 python = "^3.9"
-click = "8.1.3"
-pydantic = { version = "1.10.9", extras = ["dotenv"] }
-unitelabs-sila = "0.1.1"
+click = "8.1.4"
+pydantic_settings = "2.0.1"
+unitelabs-sila = "0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 isort = "5.12.0"
 pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
```

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/connector.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,38 @@
 import typing
 
 from sila import cloud_connector, discovery, server
 
 from unitelabs.features.core.sila_service import SiLAService
 
 from .config import Config
-from .logging import create_logger
 
 
 class Connector:
     """Main app"""
 
     def __init__(self, config: typing.Optional[dict] = None):
         self.__config = Config.parse_obj(config or {})
 
         self._sila_server = server.Server(config=self.config.sila_server)
-        self.logger.info(self._sila_server)
+        self.logger.debug(self._sila_server)
         self._broadcaster = discovery.Broadcaster(self._sila_server)
         self._cloud_server_endpoint = cloud_connector.CloudServerEndpoint(
             self._sila_server, self.config.cloud_server_endpoint
         )
 
         self.register(SiLAService())
 
     def register(self, feature: server.Feature):
         """Register a new feature to this driver"""
         self.logger.debug("Added feature: %s", feature)
         self._sila_server.add_feature(feature)
 
     async def start(self):
         """Start running this driver"""
-        self.logger.info("Starting connector...")
-
         await asyncio.gather(
             asyncio.create_task(self._sila_server.start()),
             asyncio.create_task(self._broadcaster.start()),
             asyncio.create_task(self._cloud_server_endpoint.start()),
         )
 
     @property
@@ -47,13 +44,13 @@
     @property
     def sila_server(self) -> server.Server:
         return self._sila_server
 
     @property
     def logger(self) -> logging.Logger:
         """A standard Python :class:`~logging.Logger` for the app."""
-        return create_logger(self.debug)
+        return logging.getLogger(__package__)
 
     @property
     def debug(self) -> bool:
         """Whether debug mode is enabled."""
         return True
```

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/LockController-v2_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/LockController-v2_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/lock_controller.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/lock_controller/lock_controller_base.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/lock_controller/lock_controller_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/SiLAService-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/SiLAService-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/core/sila_service/sila_service.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/core/sila_service/sila_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     @sila.UnobservableProperty()
     def get_server_type(self) -> typing.Annotated[str, sila.constraints.Pattern(r"[A-Z][a-zA-Z0-9]*")]:
         """
         The type of this server. It, could be, e.g., in the case of a SiLA Device the model name.
         It is specified by the implementer of the SiLA Server and MAY not be unique.
         """
-        return getattr(self.server, "name")
+        return getattr(self.server, "type")
 
     @sila.UnobservableProperty()
     def get_server_description(self) -> str:
         """
         Description of the SiLA Server. This should include the use and purpose of this SiLA Server.
         """
         return getattr(self.server, "description")
```

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/examples/greeting_provider/greeting_provider_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/examples/timer_provider/timer_provider_base.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/examples/timer_provider/timer_provider_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/GripController-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/GripController-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/GripController-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/GripController-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/grip_controller/grip_controller_base.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/grip_controller/grip_controller_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/LabwareTransferManipulatorController-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/labware_transfer_manipulator_controller/labware_transfer_manipulator_controller_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/MovementController-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/robot/movement_controller/movement_controller_base.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/robot/movement_controller/movement_controller_base.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/BasicDataTypesTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/basic_data_types_test/basic_data_types_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/ObservableCommandTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_command_test/observable_command_test.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_command_test/observable_command_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 
     @sila.ObservableCommand()
     @sila.Response(name="Received Value")
     async def echo_value_async(self, value: int, delay_in_ms: int, *, status: sila.Status) -> int:
         """
         Echo the given value asynchronously after the specified delay.
 
-        .. parameter:: The delay in milliseconds
         .. parameter:: The value to echo
+        .. parameter:: The delay in milliseconds
         .. return:: The Received Value
         """
         seconds, rest = divmod(delay_in_ms, 1000)
         for i in range(int(seconds)):
             status.update(
                 progress=i / (delay_in_ms / 1000),
                 remaining_time=sila.datetime.timedelta(microseconds=(delay_in_ms - i * 1000) * 1000),
```

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/ObservablePropertyTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/observable_property_test/observable_property_test.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/observable_property_test/observable_property_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/UnobservableCommandTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_command_test/unobservable_command_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/UnobservablePropertyTest-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/test/unobservable_property_test/unobservable_property_test.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.proto`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/WeighingService-v1_0.sila.xml`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/features/weighing/weighing_service/weighing_service.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/features/weighing/weighing_service/weighing_service.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/logging.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import logging
 
-default_handler = logging.StreamHandler()
-default_handler.setFormatter(logging.Formatter("{asctime} [{levelname!s:<8}] {message!s}", style="{"))
 
-
-def create_logger(debug: bool = False) -> logging.Logger:
+def create_logger(name: str = __package__, level: logging._Level = logging.INFO) -> logging.Logger:
     """
     Get the app's logger and configure it if needed.
     """
-    logger = logging.getLogger(__package__)
 
-    if debug and not logger.level:
-        logger.setLevel(logging.DEBUG)
+    logger = logging.getLogger(name)
+    handlers = [handler for handler in logger.handlers if not isinstance(handler, logging.NullHandler)]
+
+    if not handlers:
+        formatter = logging.Formatter("{asctime} [{levelname!s:<8}] {message!s}", style="{")
+
+        stream_handler = logging.StreamHandler()
+        stream_handler.setFormatter(formatter)
 
-    if not logger.hasHandlers():
-        logger.addHandler(default_handler)
+        logger.setLevel(level)
+        logger.addHandler(stream_handler)
 
     return logger
```

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/__init__.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/intermediate_response.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/intermediate_response.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/response.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/response.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/commands/status.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/commands/status.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/__init__.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/custom_data_type.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/custom_data_type.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/data_type_definition.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/data_type_definition.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/data_types/parser.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/data_types/parser.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/defined_execution_error.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/feature.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/feature.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/metadata.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/metadata.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_command.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/observable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/observable_property.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/observable_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_command.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/unobservable_command.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/unobservable_property.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/unobservable_property.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/src/unitelabs/sila/utils.py` & `unitelabs_connector_framework-0.1.3/src/unitelabs/sila/utils.py`

 * *Files identical despite different names*

### Comparing `unitelabs_connector_framework-0.1.2/PKG-INFO` & `unitelabs_connector_framework-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitelabs-connector-framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: A framework to build connectors based on the SiLA 2 standard specification.
 Home-page: https://unitelabs.ch
 License: MIT
 Keywords: SiLA 2,laboratory,automation,connectivity
 Author: UniteLabs AG
 Author-email: developers+connector@unitelabs.ch
 Requires-Python: >=3.9,<4.0
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: click (==8.1.3)
-Requires-Dist: pydantic[dotenv] (==1.10.9)
-Requires-Dist: unitelabs-sila (==0.1.1)
+Requires-Dist: click (==8.1.4)
+Requires-Dist: pydantic_settings (==2.0.1)
+Requires-Dist: unitelabs-sila (==0.1.3)
 Project-URL: Bug Tracker, https://gitlab.com/unitelabs/connector-framework/-/issues
 Project-URL: Documentation, https://gitlab.com/unitelabs/connector-framework/-/tree/main/docs/
 Project-URL: Repository, https://gitlab.com/unitelabs/connector-framework
 Description-Content-Type: text/markdown
 
 # UniteLabs Connector Framework
```

