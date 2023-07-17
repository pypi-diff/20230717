# Comparing `tmp/pytrinamic-0.2.6.tar.gz` & `tmp/pytrinamic-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrinamic-0.2.6.tar", last modified: Wed Jun 14 11:59:26 2023, max compression
+gzip compressed data, was "pytrinamic-0.2.7.tar", last modified: Mon Jul 17 11:53:20 2023, max compression
```

## Comparing `pytrinamic-0.2.6.tar` & `pytrinamic-0.2.7.tar`

### file list

```diff
@@ -1,170 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.999786 pytrinamic-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-14 11:59:25.999786 pytrinamic-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.955786 pytrinamic-0.2.6/pytrinamic/
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/RAMDebug.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.959786 pytrinamic-0.2.6/pytrinamic/connections/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.959786 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/can_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/dummy_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/serial_tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/tmcl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/uart_ic_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/connections/usb_tmcl_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.967786 pytrinamic-0.2.6/pytrinamic/evalboards/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/MAX22216_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2100_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2130_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2160_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2208_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2209_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2224_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2225_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2240_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2300_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2590_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC2660_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC4361_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC4671_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5031_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5041_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5062_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5072_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5130_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5160_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5160_shield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC5240_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC6100_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC6200_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC6300_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/TMC7300_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/evalboards/tmcl_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.975786 pytrinamic-0.2.6/pytrinamic/features/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/abn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/abn_encoder_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/absolute_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/absolute_encoder_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/coolstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/coolstep_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/current_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/current_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/digital_hall.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/digital_hall_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/drive_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/drive_setting_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/linear_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/linear_ramp_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/linear_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/motor_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/motor_control_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/motor_control_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/pid_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/ramp_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/ramp_settings_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/s_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/s_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/six_point_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/six_point_ramp_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/solenoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/solenoid_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/solenoid_control_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/solenoid_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/stallguard2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/stallguard2_ic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/features/stallguard2_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.987786 pytrinamic-0.2.6/pytrinamic/ic/
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/MAX22216.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2100.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2130.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2160.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2208.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2209.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2224.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2225.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2240.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2300.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2590.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC2660.py
--rw-r--r--   0 runner    (1001) docker     (123)    38190 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC4361.py
--rw-r--r--   0 runner    (1001) docker     (123)    49033 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC4671.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5031.py
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5041.py
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5062.py
--rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5072.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5130.py
--rw-r--r--   0 runner    (1001) docker     (123)    33995 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5160.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC5240.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC6100.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC6200.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC6300.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/TMC7300.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/ic/tmc_ic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.995786 pytrinamic-0.2.6/pytrinamic/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/Landungsbruecke.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCC160.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1140.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1141.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1160.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1161.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM123x_0_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1240.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1260.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1270.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1276.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1370.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1617.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1630.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1633.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1636.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1637.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1638.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1640.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM1670.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM3110.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM3312.py
--rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM3351.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM6110.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM6212.py
--rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM6214.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/TMCM_Python.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/canopen_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/tmc_eval_shield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/modules/tmcl_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.995786 pytrinamic-0.2.6/pytrinamic/referencedesigns/
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/referencedesigns/TMC4671_LEV_REF.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/referencedesigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/tmcl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.999786 pytrinamic-0.2.6/pytrinamic/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/tools/velocity_ramp_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/pytrinamic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.955786 pytrinamic-0.2.6/pytrinamic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-14 11:59:25.000000 pytrinamic-0.2.6/pytrinamic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-14 11:59:25.000000 pytrinamic-0.2.6/pytrinamic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:59:25.000000 pytrinamic-0.2.6/pytrinamic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:59:25.000000 pytrinamic-0.2.6/pytrinamic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 11:59:25.000000 pytrinamic-0.2.6/pytrinamic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 11:59:25.000000 pytrinamic-0.2.6/pytrinamic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-14 11:59:25.999786 pytrinamic-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:59:25.999786 pytrinamic-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/tests/test_can_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-14 11:59:11.000000 pytrinamic-0.2.6/tests/test_interface_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.359474 pytrinamic-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-17 11:53:20.359474 pytrinamic-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.323472 pytrinamic-0.2.7/pytrinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/RAMDebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.327473 pytrinamic-0.2.7/pytrinamic/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.331473 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/can_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/dummy_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/serial_tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/tmcl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/uart_ic_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/connections/usb_tmcl_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.343473 pytrinamic-0.2.7/pytrinamic/evalboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/MAX22216_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2100_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2130_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2160_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2208_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2209_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2224_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2225_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2240_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2590_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC2660_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC4361_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC4671_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5031_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5041_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5062_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5072_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5130_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5160_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5160_shield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC5240_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC6100_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC6200_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC6300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/TMC7300_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/evalboards/tmcl_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.351474 pytrinamic-0.2.7/pytrinamic/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/abn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/abn_encoder_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/absolute_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/absolute_encoder_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/coolstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/coolstep_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/current_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/current_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/digital_hall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/digital_hall_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/drive_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/drive_setting_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/linear_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/linear_ramp_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/linear_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/motor_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/motor_control_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/motor_control_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/pid_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/ramp_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/ramp_settings_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/s_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/s_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/six_point_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/six_point_ramp_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/solenoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/solenoid_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/solenoid_control_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/solenoid_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/stallguard2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/stallguard2_ic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/features/stallguard2_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.355474 pytrinamic-0.2.7/pytrinamic/ic/
+-rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/MAX22216.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2130.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2208.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2209.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2225.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2240.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2300.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2590.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC2660.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38190 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC4361.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49033 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC4671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5031.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5041.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5062.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25681 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5072.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5130.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33995 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5160.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC5240.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC6100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC6200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC6300.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/TMC7300.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/ic/tmc_ic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.359474 pytrinamic-0.2.7/pytrinamic/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/Landungsbruecke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCC160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1140.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1141.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1161.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM123x_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1240.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1260.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1270.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1276.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1370.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1630.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1633.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1636.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1637.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1638.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM1670.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM3110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM3312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM3351.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM6110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM6212.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM6214.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/TMCM_Python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/canopen_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/tmc_eval_shield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/modules/tmcl_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.359474 pytrinamic-0.2.7/pytrinamic/referencedesigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/referencedesigns/TMC4671_LEV_REF.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/referencedesigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/tmcl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.359474 pytrinamic-0.2.7/pytrinamic/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/tools/velocity_ramp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/pytrinamic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.327473 pytrinamic-0.2.7/pytrinamic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-17 11:53:20.000000 pytrinamic-0.2.7/pytrinamic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-07-17 11:53:20.000000 pytrinamic-0.2.7/pytrinamic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:53:20.000000 pytrinamic-0.2.7/pytrinamic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:53:20.000000 pytrinamic-0.2.7/pytrinamic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 11:53:20.000000 pytrinamic-0.2.7/pytrinamic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 11:53:20.000000 pytrinamic-0.2.7/pytrinamic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 11:53:20.363474 pytrinamic-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:53:20.359474 pytrinamic-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/tests/test_can_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-17 11:53:07.000000 pytrinamic-0.2.7/tests/test_interface_timeouts.py
```

### Comparing `pytrinamic-0.2.6/LICENSE` & `pytrinamic-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/MANIFEST.in` & `pytrinamic-0.2.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/PKG-INFO` & `pytrinamic-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrinamic
-Version: 0.2.6
+Version: 0.2.7
 Summary: TRINAMIC's Python Technology Access Package.
 Home-page: https://github.com/trinamic/PyTrinamic
 Author: Trinamic Software Team
 Author-email: tmc_info@trinamic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrinamic-0.2.6/README.md` & `pytrinamic-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/RAMDebug.py` & `pytrinamic-0.2.7/pytrinamic/RAMDebug.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/__init__.py` & `pytrinamic-0.2.7/pytrinamic/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/ixxat_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/kvaser_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/pcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/slcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/can_tmcl/socketcan_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/can_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/can_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/connection_manager.py` & `pytrinamic-0.2.7/pytrinamic/connections/connection_manager.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/dummy_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/dummy_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/serial_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/serial_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/uart_ic_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/uart_ic_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/connections/usb_tmcl_interface.py` & `pytrinamic-0.2.7/pytrinamic/connections/usb_tmcl_interface.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/MAX22216_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/MAX22216_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2100_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2100_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2130_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2130_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2160_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2160_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2208_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2208_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2209_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2209_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2224_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2224_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2225_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2225_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2240_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2240_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2300_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2590_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2590_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC2660_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC2660_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC4361_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC4361_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC4671_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC4671_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5031_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5031_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5041_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5041_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5062_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5062_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5072_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5072_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5130_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5130_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5160_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5160_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5160_shield.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5160_shield.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC5240_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC5240_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC6100_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC6100_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC6200_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC6200_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC6300_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC6300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/TMC7300_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/TMC7300_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/__init__.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/evalboards/tmcl_eval.py` & `pytrinamic-0.2.7/pytrinamic/evalboards/tmcl_eval.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/abn_encoder.py` & `pytrinamic-0.2.7/pytrinamic/features/abn_encoder.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/abn_encoder_module.py` & `pytrinamic-0.2.7/pytrinamic/features/abn_encoder_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/absolute_encoder.py` & `pytrinamic-0.2.7/pytrinamic/features/absolute_encoder.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/absolute_encoder_module.py` & `pytrinamic-0.2.7/pytrinamic/features/absolute_encoder_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/coolstep.py` & `pytrinamic-0.2.7/pytrinamic/features/coolstep.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/coolstep_module.py` & `pytrinamic-0.2.7/pytrinamic/features/coolstep_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/current.py` & `pytrinamic-0.2.7/pytrinamic/features/current.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/current_ic.py` & `pytrinamic-0.2.7/pytrinamic/features/current_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/current_module.py` & `pytrinamic-0.2.7/pytrinamic/features/current_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/digital_hall.py` & `pytrinamic-0.2.7/pytrinamic/features/digital_hall.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/digital_hall_module.py` & `pytrinamic-0.2.7/pytrinamic/features/digital_hall_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/drive_setting.py` & `pytrinamic-0.2.7/pytrinamic/features/drive_setting.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/drive_setting_module.py` & `pytrinamic-0.2.7/pytrinamic/features/drive_setting_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/linear_ramp.py` & `pytrinamic-0.2.7/pytrinamic/features/linear_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/linear_ramp_ic.py` & `pytrinamic-0.2.7/pytrinamic/features/linear_ramp_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/linear_ramp_module.py` & `pytrinamic-0.2.7/pytrinamic/features/linear_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/motor_control.py` & `pytrinamic-0.2.7/pytrinamic/features/motor_control.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/motor_control_ic.py` & `pytrinamic-0.2.7/pytrinamic/features/motor_control_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/motor_control_module.py` & `pytrinamic-0.2.7/pytrinamic/features/motor_control_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/pid.py` & `pytrinamic-0.2.7/pytrinamic/features/pid.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/pid_module.py` & `pytrinamic-0.2.7/pytrinamic/features/pid_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/ramp_settings.py` & `pytrinamic-0.2.7/pytrinamic/features/ramp_settings.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/ramp_settings_module.py` & `pytrinamic-0.2.7/pytrinamic/features/ramp_settings_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/s_ramp.py` & `pytrinamic-0.2.7/pytrinamic/features/s_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/s_ramp_module.py` & `pytrinamic-0.2.7/pytrinamic/features/s_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/six_point_ramp.py` & `pytrinamic-0.2.7/pytrinamic/features/six_point_ramp.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/six_point_ramp_module.py` & `pytrinamic-0.2.7/pytrinamic/features/six_point_ramp_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/solenoid.py` & `pytrinamic-0.2.7/pytrinamic/features/solenoid.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/solenoid_control_ic.py` & `pytrinamic-0.2.7/pytrinamic/features/solenoid_control_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/solenoid_ic.py` & `pytrinamic-0.2.7/pytrinamic/features/solenoid_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/stallguard2.py` & `pytrinamic-0.2.7/pytrinamic/features/stallguard2.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/stallguard2_ic.py` & `pytrinamic-0.2.7/pytrinamic/features/stallguard2_ic.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/features/stallguard2_module.py` & `pytrinamic-0.2.7/pytrinamic/features/stallguard2_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/helpers.py` & `pytrinamic-0.2.7/pytrinamic/helpers.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/MAX22216.py` & `pytrinamic-0.2.7/pytrinamic/ic/MAX22216.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2100.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2100.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2130.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2130.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2160.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2208.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2208.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2209.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2209.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2224.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2224.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2225.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2225.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2240.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2300.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2590.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2590.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC2660.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC2660.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC4361.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC4361.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC4671.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC4671.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5031.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5031.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5041.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5041.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5062.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5062.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5072.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5072.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5130.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5130.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5160.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC5240.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC5240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC6100.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC6100.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC6200.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC6200.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/TMC7300.py` & `pytrinamic-0.2.7/pytrinamic/ic/TMC7300.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/ic/__init__.py` & `pytrinamic-0.2.7/pytrinamic/ic/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/Landungsbruecke.py` & `pytrinamic-0.2.7/pytrinamic/modules/Landungsbruecke.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCC160.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCC160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1140.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1140.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1141.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1141.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1160.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1160.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1161.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1161.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM123x_0_1.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM123x_0_1.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1240.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1240.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1260.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1260.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1270.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1270.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1276.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1276.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1370.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1370.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1617.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1617.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1630.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1630.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1633.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1633.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1636.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1636.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1637.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1637.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1638.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1638.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1640.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1640.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM1670.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM1670.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM3110.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM3110.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM3312.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM3312.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM3351.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM3351.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM6110.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM6110.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM6212.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM6212.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM6214.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM6214.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/TMCM_Python.py` & `pytrinamic-0.2.7/pytrinamic/modules/TMCM_Python.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/__init__.py` & `pytrinamic-0.2.7/pytrinamic/modules/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .tmcl_module import TMCLModule
 from .TMCC160 import TMCC160
+from .TMCM1021 import TMCM1021
 from .TMCM1140 import TMCM1140
 from .TMCM1141 import TMCM1141
 from .TMCM1160 import TMCM1160
 from .TMCM1161 import TMCM1161
 from .TMCM1240 import TMCM1240
 from .TMCM1260 import TMCM1260
 from .TMCM1270 import TMCM1270
```

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/canopen_node.py` & `pytrinamic-0.2.7/pytrinamic/modules/canopen_node.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/tmc_eval_shield.py` & `pytrinamic-0.2.7/pytrinamic/modules/tmc_eval_shield.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/modules/tmcl_module.py` & `pytrinamic-0.2.7/pytrinamic/modules/tmcl_module.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/referencedesigns/TMC4671_LEV_REF.py` & `pytrinamic-0.2.7/pytrinamic/referencedesigns/TMC4671_LEV_REF.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/tmcl.py` & `pytrinamic-0.2.7/pytrinamic/tmcl.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic/tools/velocity_ramp_runner.py` & `pytrinamic-0.2.7/pytrinamic/tools/velocity_ramp_runner.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/pytrinamic.egg-info/PKG-INFO` & `pytrinamic-0.2.7/pytrinamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrinamic
-Version: 0.2.6
+Version: 0.2.7
 Summary: TRINAMIC's Python Technology Access Package.
 Home-page: https://github.com/trinamic/PyTrinamic
 Author: Trinamic Software Team
 Author-email: tmc_info@trinamic.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytrinamic-0.2.6/pytrinamic.egg-info/SOURCES.txt` & `pytrinamic-0.2.7/pytrinamic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 pytrinamic/ic/TMC6200.py
 pytrinamic/ic/TMC6300.py
 pytrinamic/ic/TMC7300.py
 pytrinamic/ic/__init__.py
 pytrinamic/ic/tmc_ic.py
 pytrinamic/modules/Landungsbruecke.py
 pytrinamic/modules/TMCC160.py
+pytrinamic/modules/TMCM1021.py
 pytrinamic/modules/TMCM1140.py
 pytrinamic/modules/TMCM1141.py
 pytrinamic/modules/TMCM1160.py
 pytrinamic/modules/TMCM1161.py
 pytrinamic/modules/TMCM123x_0_1.py
 pytrinamic/modules/TMCM1240.py
 pytrinamic/modules/TMCM1260.py
```

### Comparing `pytrinamic-0.2.6/setup.py` & `pytrinamic-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/tests/test_can_adapters.py` & `pytrinamic-0.2.7/tests/test_can_adapters.py`

 * *Files identical despite different names*

### Comparing `pytrinamic-0.2.6/tests/test_interface_timeouts.py` & `pytrinamic-0.2.7/tests/test_interface_timeouts.py`

 * *Files identical despite different names*

