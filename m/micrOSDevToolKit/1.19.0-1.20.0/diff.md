# Comparing `tmp/micrOSDevToolKit-1.19.0.tar.gz` & `tmp/micrOSDevToolKit-1.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.19.0.tar", last modified: Sat Jul 15 22:19:34 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.20.0.tar", last modified: Mon Jul 17 20:59:10 2023, max compression
```

## Comparing `micrOSDevToolKit-1.19.0.tar` & `micrOSDevToolKit-1.20.0.tar`

### file list

```diff
@@ -1,248 +1,249 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.821118 micrOSDevToolKit-1.19.0/
--rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.19.0/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-15 22:19:34.818263 micrOSDevToolKit-1.19.0/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.19.0/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.19.0/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.443977 micrOSDevToolKit-1.19.0/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.450500 micrOSDevToolKit-1.19.0/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.19.0/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.19.0/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.452857 micrOSDevToolKit-1.19.0/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.19.0/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.501919 micrOSDevToolKit-1.19.0/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.567354 micrOSDevToolKit-1.19.0/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.19.0/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6432 2023-07-15 19:59:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.19.0/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6346 2023-07-15 18:09:26.000000 micrOSDevToolKit-1.19.0/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2072 2023-07-15 18:08:04.000000 micrOSDevToolKit-1.19.0/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6950 2023-07-15 20:29:58.000000 micrOSDevToolKit-1.19.0/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11596 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.19.0/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.19.0/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.19.0/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.19.0/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.19.0/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.19.0/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-15 21:22:42.000000 micrOSDevToolKit-1.19.0/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.19.0/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2753 2023-07-15 18:06:40.000000 micrOSDevToolKit-1.19.0/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-06 11:13:33.000000 micrOSDevToolKit-1.19.0/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.19.0/micrOS/source/pycallgraph.png
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.19.0/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.19.0/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.570402 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8747 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-15 22:19:34.000000 micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-15 22:19:34.821301 micrOSDevToolKit-1.19.0/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-15 22:17:54.000000 micrOSDevToolKit-1.19.0/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.578247 micrOSDevToolKit-1.19.0/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.19.0/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.19.0/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.19.0/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.19.0/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.594991 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.598965 micrOSDevToolKit-1.19.0/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.19.0/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.19.0/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.19.0/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.19.0/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.624214 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.707354 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.19.0/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.711664 micrOSDevToolKit-1.19.0/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-15 22:19:34.814433 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1825 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3072 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1947 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      780 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2117 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4178 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2155 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3632 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3412 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5824 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1250 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1742 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-15 21:56:21.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1450 2023-07-15 21:56:20.000000 micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.301960 micrOSDevToolKit-1.20.0/
+-rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.20.0/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-17 20:59:10.301295 micrOSDevToolKit-1.20.0/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.0/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.0/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.020279 micrOSDevToolKit-1.20.0/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.034878 micrOSDevToolKit-1.20.0/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.0/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.0/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.040236 micrOSDevToolKit-1.20.0/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.0/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.081676 micrOSDevToolKit-1.20.0/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.153963 micrOSDevToolKit-1.20.0/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.0/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.0/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.0/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.0/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.0/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6889 2023-07-17 15:14:53.000000 micrOSDevToolKit-1.20.0/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-17 14:43:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7239 2023-07-17 17:38:40.000000 micrOSDevToolKit-1.20.0/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2870 2023-07-17 20:27:42.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.0/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.0/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.0/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.0/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.0/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-17 15:01:38.000000 micrOSDevToolKit-1.20.0/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.0/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.0/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.0/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.0/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.0/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.156912 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8792 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-17 20:59:10.302177 micrOSDevToolKit-1.20.0/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-17 19:37:44.000000 micrOSDevToolKit-1.20.0/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.165563 micrOSDevToolKit-1.20.0/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.0/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.0/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.0/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.0/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.184115 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.190248 micrOSDevToolKit-1.20.0/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.0/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.0/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.0/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.0/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.207990 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.244901 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.20.0/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.245909 micrOSDevToolKit-1.20.0/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.299912 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2111 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2141 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1453 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5760 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.19.0/PKG-INFO` & `micrOSDevToolKit-1.20.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.19.0
+Version: 1.20.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.19.0/README.md` & `micrOSDevToolKit-1.20.0/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/devToolKit.py` & `micrOSDevToolKit-1.20.0/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/media/dnd.png` & `micrOSDevToolKit-1.20.0/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/media/logo.png` & `micrOSDevToolKit-1.20.0/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/media/logo_mini.png` & `micrOSDevToolKit-1.20.0/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.20.0/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.0/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.20.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.20.0/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/Common.py` & `micrOSDevToolKit-1.20.0/micrOS/source/Common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 """
-Module is responsible for collect the additional
-feature definition dedicated to micrOS framework towards LoadModules
-
-socket_stream decorator
-- adds an extra msgobj to the wrapped function arg list
-- msgobj provides socket msg interface for the open connection
-
-Designed by Marcell Ban aka BxNxM
+micrOS Load Module programming API-s
+    Designed by Marcell Ban aka BxNxM
 """
 
 from SocketServer import SocketServer
 from machine import Pin, ADC
-from sys import platform
 from LogicalPins import physical_pin
 from Debug import logger, log_get
 try:
     from TaskManager import Task, Manager
 except Exception as e:
     print(f"Import ERROR, TaskManager: {e}")
     Task, Manager = None, None
 TELEGRAM = None
 
 
 def socket_stream(func):
     """
-    Provide socket message object as [msgobj]
-    (SocketServer singleton class)
+    [LM] Socket message streamer - adds msgobj to the decorated function arg list.
+    Use msgobj as print function: msgobj("hello")
+    (SocketServer singleton class - reply all bug/feature)
     """
     def wrapper(*args, **kwargs):
         return func(*args, **kwargs, msgobj=SocketServer.reply)
     return wrapper
 
 
 def transition(from_val, to_val, step_ms, interval_sec):
     """
-    transition v1 (core)
-    Generator for color transitions:
+    [LM] Single Generator for color/value transition:
     :param from_val: from value - start from
     :param to_val: to value - target value
     :param step_ms: step to reach to_val - timirq_seq
     :param interval_sec: full intervals
     """
     if interval_sec > 0:
         step_cnt = round((interval_sec*1000)/step_ms)
@@ -49,16 +42,15 @@
             yield round(from_val + (cnt * delta) * direc)
     else:
         yield round(to_val)
 
 
 def transition_gen(*args, interval_sec=1.0):
     """
-    transition v2
-    Create multiple transition generators
+    [LM] Multiple Generator for color/value transitions:
     - calculate minimum step count -> step_ms
     - autofill and use use transition(from_val, to_val, step_ms, interval_sec)
     :param args: ch1_from, ch1_to, ch2_from, ch2_to, etc...
     :param interval_sec: interval in sec to calculate optimal fade/transition effect
     return: gen, step_ms OR gen list, step_ms
     """
     step_ms_min = 5            # min calculated step is 5 ms - good enough
@@ -69,31 +61,31 @@
     if len(transitions) == 1:
         return transitions[0], step_ms
     return list(transitions), step_ms
 
 
 class SmartADC:
     """
+    [LM] General ADC implementation for auto scaled output: raw, percent, volt
     https://docs.micropython.org/en/latest/esp32/quickref.html#adc-analog-to-digital-conversion
-    ADC.ATTN_0DB: 0 dB attenuation, resulting in a full-scale voltage range of 0-1.1V
-    ADC.ATTN_2_5DB: 2.5 dB attenuation, resulting in a full-scale voltage range of 0-1.5V
-    ADC.ATTN_6DB: 6 dB attenuation, resulting in a full-scale voltage range of 0-2.2V
-    ADC.ATTN_11DB: 11 dB attenuation, resulting in a full-scale voltage range of 0-2450mV/
+        ADC.ATTN_0DB: 0 dB attenuation, resulting in a full-scale voltage range of 0-1.1V
+        ADC.ATTN_2_5DB: 2.5 dB ... of 0-1.5V
+        ADC.ATTN_6DB: 6 dB ... of 0-2.2V
+        ADC.ATTN_11DB: 11 dB ... of 0-2450mV/
     Note that the absolute maximum voltage rating for input pins is 3.6V. Going near to this boundary risks damage to the IC!
     """
     OBJS = {}
 
     def __init__(self, pin):
+        self.adp_prop = (65535, 2450)                               # 2450mV so 2,45V
         self.adc = None
-        self.adp_prop = ()
         if not isinstance(pin, int):
             pin = physical_pin(pin)
         self.adc = ADC(Pin(pin))
         self.adc.atten(ADC.ATTN_11DB)                               # 2450mV measure range
-        self.adp_prop = (65535, 2450)                               # 2450mV so 2,45V
 
     def get(self):
         raw = int((self.adc.read_u16() + self.adc.read_u16())/2)    # 16-bit ADC value (0-65535)
         percent = raw / self.adp_prop[0]
         volt = round(percent * self.adp_prop[1] / 1000, 2)          # devide with 1000 to get V from mV
         return {'raw': raw, 'percent': round(percent*100, 1), 'volt': volt}
 
@@ -103,15 +95,15 @@
             return SmartADC.OBJS[pin]
         SmartADC.OBJS[pin] = SmartADC(pin)
         return SmartADC.OBJS[pin]
 
 
 def micro_task(tag, task=None):
     """
-    Async task creation from Load Modules
+    [LM] Async task creation
     - Indirect interface
     tag:
         [1] tag=None: return task generator object
         [2] tag=taskID: return existing task object by tag
     task: coroutine to execute (built in overload protection and lcm)
     """
     # [0] Check dependencies
@@ -133,15 +125,15 @@
         state = Manager().create_task(callback=task, tag=tag)
         return state
 
 
 @socket_stream
 def data_logger(f_name, data=None, limit=12, msgobj=None):
     """
-    micrOS Common Data logger solution
+    [LM] micrOS Common Data logger solution
     - if data None => read mode
     - if data value => write mode
     :param f_name: log name (without extension, automatic: .dat)
     :param data: data to append
     :param limit: line limit (max.: 12 with short lines: limited disk speed!)
     :param msgobj: socket stream object (set automatically!)
     """
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.20.0/micrOS/source/ConfigHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from utime import sleep
 from json import load, dump
 from os import remove
 from Debug import DebugCfg, console_write, errlog_add
 try:
     from LogicalPins import set_pinmap
 except:
-    errlog_add("[ERR] LogicalPins import error: set_pinmap")
+    errlog_add("[ERR] LogicalPins import: set_pinmap")
     set_pinmap = None
 
 
 class Data:
     # micrOS config path
     CONFIG_PATH = "node_config.json"
     CONFIG_CACHE = {"version": "n/a",
@@ -75,53 +75,53 @@
         # SET dbg based on config settings (inject user conf)
         DebugCfg.DEBUG = cfgget('dbg')
         if Data.CONFIG_CACHE['dbg']:
             # if debug ON, set progress led
             DebugCfg.init_pled()
         else:
             # Show info message - dbg OFF
-            console_write("[micrOS] debug print was turned off")
+            console_write("[micrOS] debug print - turned off")
 
 
     @staticmethod
     def __inject_default_conf():
         # Load config and template
         liveconf = Data.read_cfg_file(nosafe=True)
         # Remove obsolete keys from conf
         try:
             remove('cleanup.pds')       # Try to remove cleanup.pds (cleanup indicator by micrOSloader)
-            console_write("[CONFIGHANDLER] Purge obsolete keys")
+            console_write("[CONF] Purge obsolete keys")
             for key in (key for key in liveconf.keys() if key not in Data.CONFIG_CACHE.keys()):
                 liveconf.pop(key, None)
+            # TODO: dynamic ... key in new config - re-store value in offloaded mode.
         except Exception:
-            console_write("[CONFIGHANDLER] SKIP obsolete keys check (no cleanup.pds)")
-        # Merge template to live conf
+            console_write("[CONF] SKIP obsolete keys check (no cleanup.pds)")
+        # Merge template to live conf (store active conf in Data.CONFIG_CACHE)
         Data.CONFIG_CACHE.update(liveconf)
-        # Run conf injection and store
-        console_write("[CONFIGHANDLER] Inject user config ...")  # Data.CONFIG_CACHE
+        console_write("[CONF] User config injection done")
         try:
             # [LOOP] Only returns True
             Data.write_cfg_file()
-            console_write("[CONFIGHANDLER] Save conf struct successful")
+            console_write("[CONF] Save conf struct successful")
         except Exception as e:
-            console_write(f"[CONFIGHANDLER] Save conf struct failed: {e}")
+            console_write(f"[CONF] Save conf struct failed: {e}")
             errlog_add(f"[ERR] __inject_default_conf error: {e}")
         finally:
             del liveconf
 
     @staticmethod
     def read_cfg_file(nosafe=False):
         conf = {}
         while True:
             try:
                 with open(Data.CONFIG_PATH, 'r') as f:
                     conf = load(f)
                 break
             except Exception as e:
-                console_write(f"[CONFIGHANDLER] read_cfg_file error {conf} (json): {e}")
+                console_write(f"[CONF] read_cfg_file error {conf} (json): {e}")
                 # Write out initial config, if no config exists.
                 if nosafe:
                     break
                 sleep(0.2)
                 errlog_add(f'[ERR] read_cfg_file error: {e}')
         # Return config cache
         return conf
@@ -131,15 +131,15 @@
         while True:
             try:
                 # WRITE JSON CONFIG
                 with open(Data.CONFIG_PATH, 'w') as f:
                     dump(Data.CONFIG_CACHE, f)
                 break
             except Exception as e:
-                console_write(f"[CONFIGHANDLER] __write_cfg_file error {Data.CONFIG_PATH} (json): {e}")
+                console_write(f"[CONF] __write_cfg_file error {Data.CONFIG_PATH} (json): {e}")
                 errlog_add(f'[ERR] write_cfg_file error: {e}')
             sleep(0.2)
         return True
 
     @staticmethod
     def type_handler(key, value):
         value_in_cfg = Data.CONFIG_CACHE[key]
@@ -198,15 +198,15 @@
     try:
         val = Data.CONFIG_CACHE.get(key, None)
         if val == '...':
             # Handle special "offloaded" keys
             return Data.disk_keys(key)
         return val
     except Exception as e:
-        console_write(f"[CONFIGHANDLER] Get config value error: {e}")
+        console_write(f"[CONF] Get config value error: {e}")
         errlog_add(f'[ERR] cfgget {key} error: {e}')
     return None
 
 
 def cfgput(key, value, type_check=False):
     # Handle special "offloaded" keys
     if str(Data.CONFIG_CACHE.get(key, None)) == '...':
@@ -228,9 +228,10 @@
         errlog_add(f'[ERR] cfgput {key} error: {e}')
         return False
 
 #################################################################
 #                       MODULE AUTO INIT                        #
 #################################################################
 
+
 # [!!!] Validate / update / create user config + sidecar functions
 Data.init()
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/Debug.py` & `micrOSDevToolKit-1.20.0/micrOS/source/Debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from LogicalPins import physical_pin, pinmap_dump, detect_platform
 except:
     detect_platform = None
 
 try:
     # TinyPICO progress led plugin
     import TinyPLed
-except Exception as e:
+except:
     TinyPLed = None
 
 
 #############################################
 #       DEBUG PRINT + PROGRESS LED          #
 #############################################
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.20.0/micrOS/source/InterConnect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uasyncio as asyncio
 from socket import getaddrinfo, SOCK_STREAM
-from re import match
+from re import compile
 from Debug import errlog_add
 from ConfigHandler import cfgget
 from SocketServer import SocketServer
 from TaskManager import Task
 
 
 class InterCon:
@@ -14,18 +14,16 @@
     def __init__(self):
         self.reader = None
         self.writer = None
         self.task = Task()
 
     @staticmethod
     def validate_ipv4(str_in):
-        pattern = r'^(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])$'
-        if bool(match(pattern, str_in)):
-            return True
-        return False
+        pattern = compile(r'^(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])\.(\d|[1-9]\d|1\d\d|2[0-4]\d|25[0-5])$')
+        return bool(pattern.match(str_in))
 
     async def send_cmd(self, host, cmd):
         """
         Async Main method to implement device-device communication with
         - dhcp host resolve and IP caching
         - async connection with prompt check and command query and result handling (via Task cache/output)
         :param host: hostname or IP address to connect with
@@ -128,47 +126,43 @@
     Async send command wrapper for further async task integration and sync send_cmd usage (main)
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     :param com_obj: InterCon object to utilize send_cmd method and task status updates
     """
     # Send command
     with com_obj.task:
-        out = await com_obj.send_cmd(host, cmd)
+        out = await com_obj.send_cmd(host, cmd)          # Send CMD
         if out is None:
             await asyncio.sleep_ms(150)
-            out = await com_obj.send_cmd(host, cmd)
+            out = await com_obj.send_cmd(host, cmd)      # Send CMD (retry)
             if out is None:
                 await asyncio.sleep_ms(150)
-                out = await com_obj.send_cmd(host, cmd)
+                out = await com_obj.send_cmd(host, cmd)  # Send CMD (retry)
         com_obj.task.out = '' if out is None else out
     return com_obj.task.out
 
 
 def send_cmd(host, cmd):
     """
-    Main wrapper of InterCon.send_cmd with
-    - Intercon object creation
-    - tag generation
-    - task creation
-    - task creation verdict generation
+    Sync wrapper of async _send_cmd (InterCon.send_cmd consumer with retry)
     :param host: hostname / IP address
     :param cmd: command string to server socket shell
     """
     def _tagify():
         nonlocal host, cmd
         _mod = cmd.split(' ')[0].strip()
         if InterCon.validate_ipv4(host):
             return f"{'.'.join(host.split('.')[-2:])}.{_mod}"
         return f"{host.replace('.local', '')}.{_mod}"
 
     com_obj = InterCon()
     tag = f"con.{_tagify()}"
     started = com_obj.task.create(callback=_send_cmd(host, cmd, com_obj), tag=tag)
     if started:
-        result = {"verdict": f"Task started {host}:{cmd} -> task show {tag}", "tag": tag}
+        result = {"verdict": f"Task started: task show {tag}", "tag": tag}
     else:
         result = {"verdict": "Task is Busy", "tag": tag}
     return result
 
 
 def dump_cache():
     """
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.20.0/micrOS/source/InterpreterShell.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 #                           IMPORTS                             #
 #################################################################
 from os import listdir
 from sys import modules
 from ConfigHandler import cfgget, cfgput
 from TaskManager import exec_lm_core
 from Debug import console_write, errlog_add
-from machine import reset as hard_reset
+from machine import reset as hard_reset, soft_reset
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.19.0-0'
+    MICROS_VERSION = '1.20.0-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
@@ -60,15 +60,14 @@
 
     def reboot(self, hard=False):
         """Reboot micropython VM"""
         self.msg(f"{'[HARD] ' if hard else ''}Reboot micrOS system.")
         self.msg("Bye!")
         if hard:
             hard_reset()
-        from machine import soft_reset
         soft_reset()
 
     def prompt(self):
         """Generate prompt"""
         auth = "[password] " if self.__auth_mode and not self.__auth_ok else ""
         mode = "[configure] " if self.__conf_mode else ""
         return f"{auth}{mode}{self.__devfid} $ "
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.20.0/micrOS/source/InterruptHandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,81 +94,80 @@
 # trigger=Pin.IRQ_RISING    signal LOW to HIGH
 #################################################################
 
 def initEventIRQs():
     """
     EVENT INTERRUPT CONFIGURATION - multiple
     """
+    # prell_last = {'Pin(1)': 'pin last call time', 'Pin(2)': 'pin last call time', ...}
+    prell_last = {}
+    prell_ms = cfgget("irq_prell_ms")
 
-    def __edge_exec(_pin_obj, resolver):
+    def __edge_exec(_pin_obj, _p_last, _cbf):
         """
         Prell filter / edge detection and execution
         :param _pin_obj: pin obj name
         :param resolver: callback resolver dict,  LM_cbf obj by pins {PinKey: [LM_cbf, prellTimer]}
         :return: None
         """
+        nonlocal prell_ms
         _pin = str(_pin_obj)
         # Get stored tick by pin - last successful trigger
-        last = resolver.get(_pin)[1]
+        last = _p_last.get(_pin)
         # Calculate trigger diff in ms (from now)
         diff = ticks_diff(ticks_ms(), last)
-        #console_write(f"[IRQ] Event {_pin} - tick diff: {diff}")
+        # console_write(f"[IRQ] Event {_pin} - tick diff: {diff}")
         # Threshold between ext. irq evens
-        if abs(diff) > resolver.get('prell_ms'):
+        if abs(diff) > prell_ms:
             # Save now tick - last trigger action
-            resolver[_pin][1] = ticks_ms()
+            _p_last[_pin] = ticks_ms()
             # [!] Execute User Load module by pin number (with micropython.schedule wrapper)
-            #console_write(f"---> action")
-            exec_lm_pipe_schedule(resolver.get(_pin)[0])
+            # console_write(f"---> action")
+            exec_lm_pipe_schedule(_cbf)
 
-    # Load External IRQ execution data set from node config
-    # ((irq, trig, lm_cbf), (irq, trig, lm_cbf), (irq, trig, lm_cbf), ...)
-    _irqdata = ((cfgget("irq1"), cfgget("irq1_trig"), cfgget("irq1_cbf")),
-                (cfgget("irq2"), cfgget("irq2_trig"), cfgget("irq2_cbf")),
-                (cfgget("irq3"), cfgget("irq3_trig"), cfgget("irq3_cbf")),
-                (cfgget("irq4"), cfgget("irq4_trig"), cfgget("irq4_cbf")))
-
-    # [*] hardcopy parameters to be able to resolve cbf-s
-    # cbf_resolver = {'Pin(1)': 'cbf;cbf', 'Pin(2)': 'cbf', ... + 'prell_ms': for example 300ms}
-    cbf_resolver = {'prell_ms': cfgget("irq_prell_ms")}
-    for i, data in enumerate(_irqdata):
-        irq, trig, lm_cbf = data
-        console_write("[IRQ] EXTIRQ SETUP - EXT IRQ{}: {} TRIG: {}".format(i+1, irq, trig))
-        console_write("|- [IRQ] EXTIRQ CBF: {}".format(lm_cbf))
-        if irq:
-            try:
-                pin = physical_pin('irq{}'.format(i + 1))  # irq1, irq2, etc.
-            except Exception as e:
-                msg = '[ERR] EVENT IRQ{} IO error: {}'.format(i+1, e)
-                pin = None
-                console_write("|-- [!] {}".format(msg))
-                errlog_add(msg)
-            if pin:
-                # [*] update resolver dict by pin number (available in irq callback):
-                # PinKey: [CallbackFunction, PrellTimer]  (prell: contact recurrence - fake event filtering... :D)
-                cbf_resolver['Pin({})'.format(pin)] = [lm_cbf, 0]
-                trig = trig.strip().lower()
-                # Init event irq with callback function wrapper
-                # pin_obj = Pin(pin, Pin.IN, Pin.PULL_UP)            #TODO: expose built in resistor parameter ?
-                pin_obj = Pin(pin, Pin.IN, Pin.PULL_DOWN)
-                # [IRQ] - event type setup
-                if trig == 'down':
-                    # pin_obj.irq(trigger=Pin.IRQ_FALLING, handler=lambda pin: print("[down] {}:{}".format(pin, cbf_resolver[str(pin)])))
-                    pin_obj.irq(trigger=Pin.IRQ_FALLING,
-                                handler=lambda pin: __edge_exec(pin, cbf_resolver))
-                    continue
-                if trig == 'both':
-                    # pin_obj.irq(trigger=Pin.IRQ_RISING | Pin.IRQ_FALLING, handler=lambda pin: print("[both] {}:{}".format(pin, cbf_resolver[str(pin)])))
-                    pin_obj.irq(trigger=Pin.IRQ_RISING | Pin.IRQ_FALLING,
-                                handler=lambda pin: __edge_exec(pin, cbf_resolver))
-                    continue
+    def __core(_pin, _trig, _lm_cbf):
+        nonlocal prell_last
+        if _pin and _lm_cbf != 'n/a':
+            # [*] update resolver dict by pin number (available in irq callback):
+            # PinKey: [CallbackFunction, PrellTimer]  (prell: contact recurrence - fake event filtering... :D)
+            prell_last['Pin({})'.format(_pin)] = 0
+            _trig = _trig.strip().lower()
+            # Init event irq with callback function wrapper
+            # pin_obj = Pin(pin, Pin.IN, Pin.PULL_UP) ?TODO?: expose built in resistor parameter ?
+            _pin_obj = Pin(_pin, Pin.IN, Pin.PULL_DOWN)
+            # [IRQ] - event type setup
+            if _trig == 'down':
+                _pin_obj.irq(trigger=Pin.IRQ_FALLING,
+                             handler=lambda pin: __edge_exec(pin, prell_last, _lm_cbf))
+            elif _trig == 'both':
+                _pin_obj.irq(trigger=Pin.IRQ_RISING | Pin.IRQ_FALLING,
+                             handler=lambda pin: __edge_exec(pin, prell_last, _lm_cbf))
+            else:
                 # Default - 'up'
-                # pin_obj.irq(trigger=Pin.IRQ_RISING, handler=lambda pin: print("[up] {}:{}".format(pin, cbf_resolver[str(pin)])))
-                pin_obj.irq(trigger=Pin.IRQ_RISING,
-                            handler=lambda pin: __edge_exec(pin, cbf_resolver))
+                _pin_obj.irq(trigger=Pin.IRQ_RISING,
+                             handler=lambda pin: __edge_exec(pin, prell_last, _lm_cbf))
+
+    def __get_pin(_p):
+        try:
+            return physical_pin(_p)
+        except Exception as e:
+            msg = f'[ERR] EVENT {_p} IO error: {e}'
+            console_write("|-- [!] {}".format(msg))
+            errlog_add(msg)
+        return None
+
+    # Load External IRQ execution data set from node config
+    if cfgget("irq1"):
+        __core(_pin=__get_pin('irq1'), _trig=cfgget("irq1_trig"), _lm_cbf=cfgget("irq1_cbf"))
+    if cfgget("irq2"):
+        __core(_pin=__get_pin('irq2'), _trig=cfgget("irq2_trig"), _lm_cbf=cfgget("irq2_cbf"))
+    if cfgget("irq3"):
+        __core(_pin=__get_pin('irq3'), _trig=cfgget("irq3_trig"), _lm_cbf=cfgget("irq3_cbf"))
+    if cfgget("irq4"):
+        __core(_pin=__get_pin('irq4'), _trig=cfgget("irq4_trig"), _lm_cbf=cfgget("irq4_cbf"))
 
 #################################################################
 #                         INIT MODULE                           #
 #################################################################
 
 
 emergency_mbuff()
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_system.py`

 * *Files 20% similar despite different names*

```diff
@@ -138,30 +138,14 @@
     :param sec
     :return: localtime
     """
     set_time(year, month, mday, hour, min, sec)
     return localtime()
 
 
-def module(unload=None):
-    """
-    List / unload Load Modules
-    :param unload str: module name to unload
-    :param unload None: list active modules
-    :return str: verdict
-    """
-    from sys import modules
-    if unload is None:
-        return list(modules.keys())
-    if unload in modules.keys():
-        del modules[unload]
-        return "Module unload {} done.".format(unload)
-    return "Module unload {} failed.".format(unload)
-
-
 @socket_stream
 def cachedump(cdel=None, msgobj=None):
     """
     Cache system persistent data storage files (.pds)
     """
     if cdel is None:
         # List pds files aka application cache
@@ -196,39 +180,14 @@
     if value > -80:
         return {'Okay': value}
     if value > -90:
         return {'NotGood': value}
     return {'Unusable': value}
 
 
-@socket_stream
-def lmpacman(lm_del=None, msgobj=None):
-    """
-    Load module package manager
-    :param lm_del str: LM_<loadmodulename.py/.mpy>
-    :param lm_del None: list available load modules
-    - Add name without LM_ but with extension!
-    """
-    from os import listdir, remove
-    if lm_del is not None and lm_del.endswith('py'):
-        # Check LM is in use
-        if 'system.' in lm_del:
-            return 'Load module {} is in use, skip delete.'.format(lm_del)
-        remove('LM_{}'.format(lm_del))
-        return 'Delete module: {}'.format(lm_del)
-    # Dump available LMs
-    msg_buf = []
-    for k in (res.replace('LM_', '') for res in listdir() if 'LM_' in res):
-        if msgobj is None:
-            msg_buf.append('   {}'.format(k))
-        else:
-            msgobj('   {}'.format(k))
-    return msg_buf if len(msg_buf) > 0 else ''
-
-
 def pinmap(key='builtin'):
     """
     Get Logical pin by key runtime
     :param key str: logical pin name to resolve
     :return dict: key map
     """
     from LogicalPins import pinmap_dump, get_pinmap
@@ -265,38 +224,22 @@
     """
     Show network ifconfig
     """
     from Network import ifconfig
     return ifconfig()
 
 
-@socket_stream
-def micros_checksum(msgobj=None):
-    from hashlib import sha1
-    from binascii import hexlify
-    from os import listdir
-    from ConfigHandler import cfgget
-
-    for f_name in (_pds for _pds in listdir() if _pds.endswith('py')):
-        with open(f_name, 'rb') as f:
-            cs = hexlify(sha1(f.read()).digest()).decode('utf-8')
-        msgobj("{} {}".format(cs, f_name))
-        gclean()
-    return "micrOS version: {}".format(cfgget('version'))
-
-
 #######################
 # LM helper functions #
 #######################
 
 def help():
     """
     [i] micrOS LM naming convention
     Load Module built-in help message
     :return tuple: list of functions implemented by this application
     """
     return 'info', 'gclean', 'heartbeat', 'clock',\
            'setclock year month mday hour min sec',\
-           'ntp', 'module unload="LM_rgb/None"', \
-           'rssi', 'cachedump cdel="rgb.pds/None"', 'lmpacman lm_del="LM_rgb.py/None"',\
+           'ntp', 'rssi', 'cachedump cdel="rgb.pds/None"',\
            'pinmap key="dhtpin"/None', 'ha_sta', 'alarms clean=False',\
-           'sun refresh=False', 'ifconfig', 'memory_usage', 'disk_usage', 'micros_checksum'
+           'sun refresh=False', 'ifconfig', 'memory_usage', 'disk_usage'
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.20.0/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/Network.py` & `micrOSDevToolKit-1.20.0/micrOS/source/Network.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
 #################################################################
 #              AUTOMATIC NETWORK CONFIGURATION                  #
 #              IF STA AVAILABLE, IF NOT AP MODE                 #
 #################################################################
 
 
-def auto_network_configuration():
+def auto_nw_config():
     # Retry mechanism - create some connection... prio.: STA > AP
     nwmd = cfgget('nwmd')
     for _ in range(0, 3):
         # nwmd: default or STA
         if nwmd is None or "AP" not in nwmd.upper():
             # SET WIFI (STA) MODE
             state = set_wifi(cfgget("staessid"), cfgget("stapwd"))
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/Notify.py` & `micrOSDevToolKit-1.20.0/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.20.0/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.20.0/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.20.0/micrOS/source/TaskManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 Designed by Marcell Ban aka BxNxM
 """
 
 #################################################################
 #                           IMPORTS                             #
 #################################################################
+import uasyncio as asyncio
+from micropython import schedule
 from sys import modules
 from json import dumps
-from micropython import schedule
-import uasyncio as asyncio
 from Debug import console_write, errlog_add
 from ConfigHandler import cfgget
 from utime import ticks_ms, ticks_diff
 
 try:
     from gc import collect
 except:
@@ -28,24 +28,24 @@
 
 #################################################################
 #                Implement custom task class                    #
 #################################################################
 
 
 class Task:
-    TASKS = {}                  # TASK OBJ list
+    TASKS = {}                       # TASK OBJ list
 
     def __init__(self):
+        self.task = None             # [TASK] Store created async task object
         self.__callback = None       # [LM] Task callback: list of strings (LM call)
         self.__inloop = False        # [LM] Task while loop for LM callback
         self.__sleep = 20            # [LM] Task while loop - async wait (proc feed) [ms]
-        self.task = None             # [LM] Store created async task object
-        self.done = asyncio.Event()  # [LM] Store task state
-        self.out = ""                # [LM] Store LM output
-        self.tag = None              # [LM] Task tag for identification
+        self.done = asyncio.Event()  # [TASK] Store done state
+        self.out = ""                # [TASK] Store output
+        self.tag = None              # [TASK] Task tag (identification)
 
     @staticmethod
     def is_busy(tag):
         """
         Check task is busy by tag in TASKS
         - exists + running = busy
         """
@@ -56,21 +56,20 @@
         # is NOT busy
         return False
 
     def __task_del(self, keep_cache=False):
         """
         Delete task from TASKS
         """
-        print(f"++++++ __task_del keep_cache={keep_cache} ++++++")
         self.done.set()
         if self.tag in Task.TASKS.keys():
-            if keep_cache:
+            if keep_cache:              # True - In case of destructor
                 del Task.TASKS[self.tag]
             del self.task
-        collect()           # GC collect
+        collect()                       # GC collect
 
     def __enter__(self):
         """
         START CONDITION
         Helper function for Task creation in Load Modules
         [HINT] Use python with feature to utilize this feature
         """
@@ -173,33 +172,33 @@
 
 #################################################################
 #                 Implement Task manager class                  #
 #################################################################
 
 
 class Manager:
-    __instance = None
+    OBJ = None                      # Manager object
     QUEUE_SIZE = cfgget('aioqueue')
     OLOAD = 0
 
     def __new__(cls):
         """
         Singleton design pattern
         __new__ - Customize the instance creation
         cls     - class
         """
-        if Manager.__instance is None:
+        if Manager.OBJ is None:
             # TaskManager singleton properties
-            Manager.__instance = super().__new__(cls)
+            Manager.OBJ = super().__new__(cls)
             # Set async event loop exception handler
             asyncio.get_event_loop().set_exception_handler(cls.axcept)
             # Start system idle task (IRQ(hack) + monitoring)
-            Manager.__instance.create_task(callback=Manager.idle_task(), tag="idle")
+            Manager.OBJ.create_task(callback=Manager.idle_task(), tag="idle")
             # ---         ----
-        return Manager.__instance
+        return Manager.OBJ
 
     @staticmethod
     def axcept(loop=None, context=None):
         """
         Set as async exception handler
         """
         errlog_add(f"[aio] exception: {loop}:{context}")
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/Time.py` & `micrOSDevToolKit-1.20.0/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.20.0/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.20.0/micrOS/source/micrOS.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,85 +5,86 @@
 Designed by Marcell Ban aka BxNxM
 """
 #################################################################
 #                           IMPORTS                             #
 #################################################################
 from TaskManager import Manager
 from SocketServer import SocketServer
-from Network import auto_network_configuration
-from Hooks import bootup_hook, profiling_info
+from Network import auto_nw_config
+from Hooks import bootup, profiling_info
 from InterruptHandler import enableInterrupt, enableCron
 from InterruptHandler import initEventIRQs
 from Debug import errlog_add
 from Time import ntp_time, suntime
 
 
 #################################################################
 #            INTERRUPT HANDLER INTERFACES / WRAPPERS            #
 #################################################################
 
 
-def safe_boot_hook():
+def safe_boot():
     try:
-        bootup_hook()
+        bootup()
     except Exception as e:
-        print(f"[micrOS main] Hooks.bootup_hook() error: {e}")
-        errlog_add(f"[ERR] safe_boot_hook error: {e}")
+        print(f"[micrOS main] Hooks.boot() error: {e}")
+        errlog_add(f"[ERR] safe_boot: {e}")
 
 
-def interrupt_handler():
+def irq_handler():
     try:
         enableInterrupt()
         enableCron()
     except Exception as e:
         print(f"[micrOS main] InterruptHandler.enableInterrupt/CronInterrupt error: {e}")
-        errlog_add(f"[ERR] interrupt_handler error: {e}")
+        errlog_add(f"[ERR] irq_handler error: {e}")
 
 
-def external_interrupt_handler():
+def external_irq_handler():
     try:
         initEventIRQs()
     except Exception as e:
         print(f"[micrOS main] InterruptHandler.initEventIRQs error: {e}")
-        errlog_add(f"[ERR] external_interrupt_handler error: {e}")
+        errlog_add(f"[ERR] external_irq_handler error: {e}")
 
 
 #################################################################
 #                      MAIN FUNCTION CALLS                      #
 #################################################################
 
 
 def micrOS():
     profiling_info(label='[memUsage] MAIN LOAD')
 
     # CREATE ASYNC TASK MANAGER
     aio = Manager()
 
-    # BOOT HOOK: Initial LM executions
-    safe_boot_hook()
+    # BOOT TASKS: Initial LM executions
+    safe_boot()
 
     # SET external interrupt with extirqcbf from nodeconfig
-    external_interrupt_handler()
+    external_irq_handler()
 
     # NETWORK setup
-    nwmd = auto_network_configuration()
+    nwmd = auto_nw_config()
     if nwmd == 'STA':
         # Set UTC + SUN TIMES FROM API ENDPOINTS
         suntime()
         # Set NTP - RTC + UTC shift + update uptime (boot time)
         ntp_time()
     else:
         # AP mode - no ntp sync set uptime anyway
         from Time import uptime
         uptime(update=True)
 
     # SET interrupt with timirqcbf from nodeconfig
-    interrupt_handler()
-    profiling_info(label='[memUsage] SYSTEM IS UP')
+    irq_handler()
 
     # [SocketServer] as async task
     aio.create_task(SocketServer().run_server(), tag='server')
+    profiling_info(label='[memUsage] SYSTEM IS UP')
+
     # [EVENT LOOP] Start async event loop
     aio.run_forever()
 
     # UNEXPECTED RESTART ???
     errlog_add("[ERR] !!! Unexpected micrOS restart")
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.20.0/micrOS/source/micrOSloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,20 @@
     print("[loader][if_mode:False] .if_mode:webrepl -> webrepl interface")
     print("[loader][recovery mode] - manually selected in .if_mode file")
     return False
 
 
 def __recovery_mode():
     # Recovery/Update mode (webrepl) - dependencies: Network, ConfigHandler
-    from Network import auto_network_configuration
+    from Network import auto_nw_config
     from ConfigHandler import cfgget
     pwd = cfgget('appwd')                       # Get pwd from config
     pwd = 'ADmin123' if pwd is None else pwd    # Default pwd if user pwd None
     # Set up network
-    auto_network_configuration()
+    auto_nw_config()
     # Start webrepl
     try:
         import webrepl
         webrepl.start(password=pwd)
     except Exception as e:
         print(f"Webrepl import error: {e}")
```

### Comparing `micrOSDevToolKit-1.19.0/micrOS/source/urequests.py` & `micrOSDevToolKit-1.20.0/micrOS/source/urequests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from usocket import socket, getaddrinfo
     from ussl import wrap_socket
 except ImportError as e:
     print(f"[Error] import u modules: {e}")
     from socket import socket, getaddrinfo
     from ssl import wrap_socket
-import json as ujson
+from json import loads, dumps
 
 
 #############################################
 #   Implement micropython request function  #
 #############################################
 def _chunked(data):
     decoded = bytearray()
@@ -78,15 +78,15 @@
         sock = wrap_socket(sock)
 
     # [3] BUILD REQUEST: body, headers
     if data is not None:
         body = data.encode('utf-8')
         headers['Content-Length'] = len(body)
     elif json is not None:
-        body = ujson.dumps(json).encode('utf-8')
+        body = dumps(json).encode('utf-8')
         headers['Content-Length'] = len(body)
         headers['Content-Type'] = 'application/json'
     else:
         body = None
     # [3.1] Create request lines list (body)
     lines = [f'{method} /{path} HTTP/1.1']
     for k, v in headers.items():
@@ -121,15 +121,15 @@
     status_code = int(headers.split(b' ')[1])
     headers = dict(h.split(b': ') for h in headers.split(b'\r\n')[1:])
     if headers.get(b'Transfer-Encoding', b'') == b'chunked':
         body = _chunked(body)
     else:
         body = body.decode('utf-8')
     # Return status code, headers and body (text or jsons)
-    return status_code, ujson.loads(body) if jsonify else body
+    return status_code, loads(body) if jsonify else body
 
 
 #############################################
 #      Implement http get/post functions    #
 #############################################
```

### Comparing `micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.19.0
+Version: 1.20.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.19.0/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 micrOS/source/LM_distance.py
 micrOS/source/LM_ds18.py
 micrOS/source/LM_esp32.py
 micrOS/source/LM_genIO.py
 micrOS/source/LM_i2c.py
 micrOS/source/LM_intercon.py
 micrOS/source/LM_light_sensor.py
+micrOS/source/LM_lmpacman.py
 micrOS/source/LM_neoeffects.py
 micrOS/source/LM_neopixel.py
 micrOS/source/LM_oled.py
 micrOS/source/LM_oled_sh1106.py
 micrOS/source/LM_oled_ui.py
 micrOS/source/LM_pet_feeder.py
 micrOS/source/LM_ph_sensor.py
@@ -71,15 +72,14 @@
 micrOS/source/SocketServer.py
 micrOS/source/TaskManager.py
 micrOS/source/Time.py
 micrOS/source/TinyPLed.py
 micrOS/source/main.py
 micrOS/source/micrOS.py
 micrOS/source/micrOSloader.py
-micrOS/source/pycallgraph.png
 micrOS/source/reset.py
 micrOS/source/urequests.py
 micrOSDevToolKit.egg-info/PKG-INFO
 micrOSDevToolKit.egg-info/SOURCES.txt
 micrOSDevToolKit.egg-info/dependency_links.txt
 micrOSDevToolKit.egg-info/requires.txt
 micrOSDevToolKit.egg-info/top_level.txt
@@ -190,14 +190,15 @@
 toolkit/workspace/precompiled/LM_distance.py
 toolkit/workspace/precompiled/LM_ds18.mpy
 toolkit/workspace/precompiled/LM_esp32.py
 toolkit/workspace/precompiled/LM_genIO.mpy
 toolkit/workspace/precompiled/LM_i2c.py
 toolkit/workspace/precompiled/LM_intercon.mpy
 toolkit/workspace/precompiled/LM_light_sensor.mpy
+toolkit/workspace/precompiled/LM_lmpacman.mpy
 toolkit/workspace/precompiled/LM_neoeffects.mpy
 toolkit/workspace/precompiled/LM_neopixel.mpy
 toolkit/workspace/precompiled/LM_oled.mpy
 toolkit/workspace/precompiled/LM_oled_sh1106.mpy
 toolkit/workspace/precompiled/LM_oled_ui.mpy
 toolkit/workspace/precompiled/LM_pet_feeder.py
 toolkit/workspace/precompiled/LM_ph_sensor.py
```

### Comparing `micrOSDevToolKit-1.19.0/setup.py` & `micrOSDevToolKit-1.20.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.19.0',
+    version='1.20.0',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.20.0/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.20.0/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.20.0/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/Gateway.py` & `micrOSDevToolKit-1.20.0/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.20.0/toolkit/MicrOSDevEnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,17 +124,18 @@
         [!] name dependency with micrOS internal manual provider
         """
         repo_version = self.get_micros_version_from_repo()
         static_help_json_path = os.path.join(self.sfuncman_output_path, 'sfuncman_{}.json'.format(repo_version))
         static_help_html_path = os.path.join(self.sfuncman_output_path, 'sfuncman.html')
 
         # [PARSING] Collect Load Module function structure buffer
+        modules_to_doc = (i.split('.')[0] for i in LocalMachine.FileHandler.list_dir(self.micrOS_dir_path) if
+                          i.startswith('LM_') and (i.endswith('.py')))
         module_function_dict = {}
-        for LM in (i.split('.')[0] for i in LocalMachine.FileHandler.list_dir(self.micrOS_dir_path) if
-                   i.startswith('LM_') and (i.endswith('.py'))):
+        for LM in modules_to_doc:
             LMpath = '{}/{}.py'.format(self.micrOS_dir_path, LM)
             try:
                 module_name = LM.replace('LM_', '')
                 module_function_dict[module_name] = {}
                 with open(LMpath, 'r') as f:
                     while True:
                         line = f.readline()
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.20.0/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.20.0/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.20.0/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.20.0/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.20.0/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.20.0/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/socketClient.py` & `micrOSDevToolKit-1.20.0/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Common.mpy`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,112 @@
-00000000: 4d06 001f 5306 1243 6f6d 6d6f 6e2e 7079  M...S..Common.py
+00000000: 4d06 001f 5106 1243 6f6d 6d6f 6e2e 7079  M...Q..Common.py
 00000010: 000f 1853 6f63 6b65 7453 6572 7665 7200  ...SocketServer.
 00000020: 0650 696e 0006 4144 4300 0e6d 6163 6869  .Pin..ADC..machi
-00000030: 6e65 0010 706c 6174 666f 726d 0006 7379  ne..platform..sy
-00000040: 7300 1870 6879 7369 6361 6c5f 7069 6e00  s..physical_pin.
-00000050: 164c 6f67 6963 616c 5069 6e73 000c 6c6f  .LogicalPins..lo
-00000060: 6767 6572 000e 6c6f 675f 6765 7400 0a44  gger..log_get..D
-00000070: 6562 7567 0008 5461 736b 000e 4d61 6e61  ebug..Task..Mana
-00000080: 6765 7200 1654 6173 6b4d 616e 6167 6572  ger..TaskManager
-00000090: 0081 2918 696e 7465 7276 616c 5f73 6563  ..).interval_sec
-000000a0: 0010 536d 6172 7441 4443 001a 736f 636b  ..SmartADC..sock
-000000b0: 6574 5f73 7472 6561 6d00 1474 7261 6e73  et_stream..trans
-000000c0: 6974 696f 6e00 1c74 7261 6e73 6974 696f  ition..transitio
-000000d0: 6e5f 6765 6e00 146d 6963 726f 5f74 6173  n_gen..micro_tas
-000000e0: 6b00 0a54 4153 4b53 0081 2d0e 6973 5f62  k..TASKS..-.is_b
-000000f0: 7573 7900 1663 7265 6174 655f 7461 736b  usy..create_task
-00000100: 0010 6361 6c6c 6261 636b 0006 7461 6700  ..callback..tag.
-00000110: 1664 6174 615f 6c6f 6767 6572 0008 2e64  .data_logger...d
-00000120: 6174 0081 1f08 7b7d 7b7d 000c 6d73 676f  at....{}{}..msgo
-00000130: 626a 000c 6e6f 7469 6679 0010 5465 6c65  bj..notify..Tele
-00000140: 6772 616d 000c 4e6f 7469 6679 0010 7365  gram..Notify..se
-00000150: 6e64 5f6d 7367 0008 5365 6e74 000e 7772  nd_msg..Sent..wr
-00000160: 6170 7065 7200 0a72 6570 6c79 0014 3c6c  apper..reply..<l
-00000170: 6973 7463 6f6d 703e 0023 0661 6463 0010  istcomp>.#.adc..
-00000180: 6164 705f 7072 6f70 000a 6174 7465 6e00  adp_prop..atten.
-00000190: 1241 5454 4e5f 3131 4442 0010 7265 6164  .ATTN_11DB..read
-000001a0: 5f75 3136 0006 7261 7700 0e70 6572 6365  _u16..raw..perce
-000001b0: 6e74 0008 766f 6c74 001a 6765 745f 7369  nt..volt..get_si
-000001c0: 6e67 6c65 746f 6e00 084f 424a 5300 8155  ngleton..OBJS..U
-000001d0: 4902 6500 8177 1054 454c 4547 5241 4d00  I.e..w.TELEGRAM.
-000001e0: 0866 756e 6300 1066 726f 6d5f 7661 6c00  .func..from_val.
-000001f0: 0c74 6f5f 7661 6c00 0e73 7465 705f 6d73  .to_val..step_ms
-00000200: 0082 0d73 066d 6178 0081 7981 5781 3d81  ...s.max..y.W.=.
-00000210: 592f 2d35 8229 0874 6173 6b00 0c66 5f6e  Y/-5.).task..f_n
-00000220: 616d 6500 0864 6174 6100 0a6c 696d 6974  ame..data..limit
-00000230: 0008 7465 7874 0082 2f0b 8213 0670 696e  ..text../....pin
-00000240: 0081 4305 1d49 6d70 6f72 7420 4552 524f  ..C..Import ERRO
-00000250: 522c 2054 6173 6b4d 616e 6167 6572 3a20  R, TaskManager: 
-00000260: 7b7d 000a 0201 0108 0331 2e30 0521 496d  {}.......1.0.!Im
-00000270: 706f 7274 2045 5252 4f52 2c20 4e6f 7469  port ERROR, Noti
-00000280: 6679 2e54 656c 6567 7261 6d3a 207b 7d00  fy.Telegram: {}.
-00000290: 0510 4e6f 7469 6679 2045 5252 4f52 3a20  ..Notify ERROR: 
-000002a0: 7b7d 000a 0207 0536 3535 3335 0704 3234  {}.....65535..24
-000002b0: 3530 8d7c b002 3201 800b 2c32 2c2c 3222  50.|..2...,2,,2"
-000002c0: 5e2d 3263 840a 8413 8c14 8922 881d 8e17  ^-2c......."....
-000002d0: 8010 022a 011b 021c 0216 0259 8010 0310  ...*.......Y....
-000002e0: 042a 021b 051c 0316 031c 0416 0459 8010  .*...........Y..
-000002f0: 062a 011b 071c 0616 0659 8010 082a 011b  .*.......Y...*..
-00000300: 091c 0816 0859 8010 0a10 0b2a 021b 0c1c  .....Y.....*....
-00000310: 0a16 0a1c 0b16 0b59 4814 8010 0d10 0e2a  .......YH......*
-00000320: 021b 0f1c 0d16 0d1c 0e16 0e59 4a29 5711  ...........YJ)W.
-00000330: 36df 4462 1637 4916 1138 2300 1410 1137  6.Db.7I..8#....7
-00000340: 3601 3401 5923 0130 0216 0d16 0e51 5116  6.4.Y#.0.....QQ.
-00000350: 3719 375d 4a01 5d51 1739 3200 1613 3201  7.7]J.]Q.92...2.
-00000360: 1614 532c 0023 0210 1162 3302 1615 5432  ..S,.#...b3...T2
-00000370: 0310 1234 0216 1251 2a01 5333 0416 1611  ...4...Q*.S3....
-00000380: 1351 8c51 2a03 5333 0534 0116 1d32 0616  .Q.Q*.S3.4...2..
-00000390: 2251 6307 810c 110f 133a 8019 6020 4500  "Qc......:..` E.
-000003a0: b020 0001 c1b1 6301 8148 c980 c040 0827  . ....c..H...@.'
-000003b0: 4f80 1e25 00b1 53b2 1021 1202 1328 8135  O..%..S..!...(.5
-000003c0: 8401 6386 08e8 441e 143b 3c3d 1180 2380  ..c...D..;<=..#.
-000003d0: 0826 2c2a 2a28 58b3 80d8 44c0 8012 3eb3  .&,**(X...D...>.
-000003e0: 2287 68f4 b2f7 3401 c412 3fb0 b1f3 b4f7  ".h...4...?.....
-000003f0: 3401 c5b0 b1d8 4443 7f42 4181 c6b4 81f2  4.....DC.BA.....
-00000400: 8042 5157 c712 3eb0 b7b5 f4b6 f4f2 3401  .BQW..>.......4.
-00000410: 6759 81e5 585a d743 2a59 5942 4712 3eb1  gY..XZ.C*YYBG.>.
-00000420: 3401 6759 5163 885c d888 80c0 409b 0115  4.gYQc.\....@...
-00000430: 1180 3680 0922 3936 2d3b 2928 0001 0585  ..6.."96-;)(....
-00000440: c212 40b1 2000 0112 4180 1242 2501 3401  ..@. ...A..B%.4.
-00000450: 81f3 8234 0334 0134 01c3 b380 d944 4380  ...4.4.4.....DC.
-00000460: 424c 1243 2500 2287 68f4 b3f7 3401 2705  BL.C%.".h...4.'.
-00000470: 2505 b2d7 4443 b242 4225 0527 0512 44b0  %...DC.BB%.'..D.
-00000480: b1b5 2001 0312 4180 1242 2501 3401 81f3  .. ...A..B%.4...
-00000490: 8234 0334 0134 01c4 1242 b434 0181 d944  .4.4.4...B.4...D
-000004a0: 48b4 8055 2505 2a02 6312 44b4 3401 2505  H..U%.*.c.D.4.%.
-000004b0: 2a02 6302 8210 620a 294f 4f80 402b 00b1  *.c...b.)OO.@+..
-000004c0: 5f4b 14c2 123f 2500 b255 2500 b281 f255  _K...?%..U%....U
-000004d0: f334 012f 1442 2a63 8240 f004 0e29 4f4f  .4./.B*c.@...)OO
-000004e0: 4f4f 8043 2b00 b35f 4b17 c412 1425 01b4  OO.C+.._K....%..
-000004f0: 5525 01b4 81f2 5525 0225 0034 042f 1442  U%....U%.%.4./.B
-00000500: 2763 8254 0814 1288 4a80 0844 8409 6460  'c.T....J..D..d`
-00000510: 1145 1646 1012 1647 2c00 1634 3200 162a  .E.F...G,..42..*
-00000520: 3201 1618 1148 3202 3401 1633 5163 0384  2....H2.4..3Qc..
-00000530: 2022 162a 5051 8055 2425 2926 2c2c 51b0   ".*PQ.U$%)&,,Q.
-00000540: 182b 2a00 b018 2c12 52b1 1243 3402 4346  .+*...,.R..C4.CF
-00000550: 1208 b134 01c1 1204 1203 b134 0134 01b0  ...4.......4.4..
-00000560: 182b b013 2b14 2d12 0413 2e36 0159 2305  .+..+.-....6.Y#.
-00000570: b018 2c51 6385 0039 0e18 5080 5e36 2831  ..,Qc..9..P.^6(1
-00000580: 1243 b013 2b14 2f36 00b0 132b 142f 3600  .C..+./6...+./6.
-00000590: f282 f734 01c1 b1b0 132c 8055 f7c2 123e  ...4.....,.U...>
-000005a0: b2b0 132c 8155 f422 8768 f782 3402 c32c  ...,.U.".h..4..,
-000005b0: 03b1 1030 6212 3eb2 2280 64f4 8134 0210  ...0b.>.".d..4..
-000005c0: 3162 b310 3262 6382 7019 0e33 5180 652c  1b..2bc.p..3Q.e,
-000005d0: 272b b012 1213 3414 3536 00dd 4447 1212  '+....4.56..DG..
-000005e0: 1334 b055 6312 12b0 3401 1212 1334 b056  .4.Uc...4....4.V
-000005f0: 1212 1334 b055 6385 10ca 0120 161c 4980  ...4.Uc.... ..I.
-00000600: 6c80 094c 2265 2b22 6962 2030 120d 51de  l..L"e+"ib 0..Q.
-00000610: 4346 120e 51de 4442 5163 b151 de44 4d12  CF..Q.DBQc.Q.DM.
-00000620: 0d13 1714 18b0 5136 02c2 b263 120d 1419  ......Q6...c....
-00000630: b036 0144 4251 6312 0e34 0014 1a10 1bb1  .6.DBQc..4......
-00000640: 101c b036 8400 c3b3 6351 6384 10c0 8501  ...6....cQc.....
-00000650: 1c1d 4a4b 4c21 808a 800a 2354 452a 4210  ..JKL!....#TE*B.
-00000660: 1ec4 b014 1fb4 3601 4443 b042 4810 2014  ......6.DC.BH. .
-00000670: 10b0 b436 02c0 b151 de44 4c12 0bb0 1021  ...6...Q.DL....!
-00000680: b334 8201 5952 6312 0ab1 b0b2 3403 6389  .4..YRc.....4.c.
-00000690: 00d1 0226 224d 80a0 6040 2026 222b 4e2c  ...&"M..`@ &"+N,
-000006a0: 2b22 552c 2f2c 2212 3951 de44 7248 1080  +"U,/,".9Q.DrH..
-000006b0: 1023 2a01 1b24 1c23 c159 b117 394a 2057  .#*..$.#.Y..9J W
-000006c0: 1236 df44 59c2 490f 1238 2303 1410 b236  .6.DY.I..8#....6
-000006d0: 0134 0159 5063 5151 c228 025d 4a01 5d48  .4.YPcQQ.(.]J.]H
-000006e0: 0c12 3934 0014 25b0 3601 c34a 2457 1236  ..94..%.6..J$W.6
-000006f0: df44 5dc2 4913 1238 2304 1410 b236 0134  .D].I..8#....6.4
-00000700: 0159 124e b234 01c3 5151 c228 025d 4a01  .Y.N.4..QQ.(.]J.
-00000710: 5db3 51de d344 48b3 1026 d944 4252 6350  ].Q..DH..&.DBRcP
-00000720: 63                                       c
+00000030: 6e65 0018 7068 7973 6963 616c 5f70 696e  ne..physical_pin
+00000040: 0016 4c6f 6769 6361 6c50 696e 7300 0c6c  ..LogicalPins..l
+00000050: 6f67 6765 7200 0e6c 6f67 5f67 6574 000a  ogger..log_get..
+00000060: 4465 6275 6700 0854 6173 6b00 0e4d 616e  Debug..Task..Man
+00000070: 6167 6572 0016 5461 736b 4d61 6e61 6765  ager..TaskManage
+00000080: 7200 8129 1869 6e74 6572 7661 6c5f 7365  r..).interval_se
+00000090: 6300 1053 6d61 7274 4144 4300 1a73 6f63  c..SmartADC..soc
+000000a0: 6b65 745f 7374 7265 616d 0014 7472 616e  ket_stream..tran
+000000b0: 7369 7469 6f6e 001c 7472 616e 7369 7469  sition..transiti
+000000c0: 6f6e 5f67 656e 0014 6d69 6372 6f5f 7461  on_gen..micro_ta
+000000d0: 736b 000a 5441 534b 5300 812d 0e69 735f  sk..TASKS..-.is_
+000000e0: 6275 7379 0016 6372 6561 7465 5f74 6173  busy..create_tas
+000000f0: 6b00 1063 616c 6c62 6163 6b00 0674 6167  k..callback..tag
+00000100: 0016 6461 7461 5f6c 6f67 6765 7200 082e  ..data_logger...
+00000110: 6461 7400 811f 087b 7d7b 7d00 0c6d 7367  dat....{}{}..msg
+00000120: 6f62 6a00 0c6e 6f74 6966 7900 1054 656c  obj..notify..Tel
+00000130: 6567 7261 6d00 0c4e 6f74 6966 7900 1073  egram..Notify..s
+00000140: 656e 645f 6d73 6700 0853 656e 7400 0e77  end_msg..Sent..w
+00000150: 7261 7070 6572 000a 7265 706c 7900 143c  rapper..reply..<
+00000160: 6c69 7374 636f 6d70 3e00 2310 6164 705f  listcomp>.#.adp_
+00000170: 7072 6f70 0006 6164 6300 0a61 7474 656e  prop..adc..atten
+00000180: 0012 4154 544e 5f31 3144 4200 1072 6561  ..ATTN_11DB..rea
+00000190: 645f 7531 3600 0672 6177 000e 7065 7263  d_u16..raw..perc
+000001a0: 656e 7400 0876 6f6c 7400 1a67 6574 5f73  ent..volt..get_s
+000001b0: 696e 676c 6574 6f6e 0008 4f42 4a53 0081  ingleton..OBJS..
+000001c0: 5549 0265 0081 7710 5445 4c45 4752 414d  UI.e..w.TELEGRAM
+000001d0: 0008 6675 6e63 0010 6672 6f6d 5f76 616c  ..func..from_val
+000001e0: 000c 746f 5f76 616c 000e 7374 6570 5f6d  ..to_val..step_m
+000001f0: 7300 820d 7306 6d61 7800 8179 8157 813d  s...s.max..y.W.=
+00000200: 8159 2f2d 3582 2908 7461 736b 000c 665f  .Y/-5.).task..f_
+00000210: 6e61 6d65 0008 6461 7461 000a 6c69 6d69  name..data..limi
+00000220: 7400 0874 6578 7400 822f 0b82 1306 7069  t..text../....pi
+00000230: 6e00 8143 051d 496d 706f 7274 2045 5252  n..C..Import ERR
+00000240: 4f52 2c20 5461 736b 4d61 6e61 6765 723a  OR, TaskManager:
+00000250: 207b 7d00 0a02 0101 0803 312e 3005 2149   {}.......1.0.!I
+00000260: 6d70 6f72 7420 4552 524f 522c 204e 6f74  mport ERROR, Not
+00000270: 6966 792e 5465 6c65 6772 616d 3a20 7b7d  ify.Telegram: {}
+00000280: 0005 104e 6f74 6966 7920 4552 524f 523a  ...Notify ERROR:
+00000290: 207b 7d00 0a02 0705 3635 3533 3507 0432   {}.....65535..2
+000002a0: 3435 308d 14b0 0230 0160 402c 322c 3222  450....0.`@,2,2"
+000002b0: 5e2d 3263 840b 8412 8c13 8922 881d 8e17  ^-2c......."....
+000002c0: 8010 022a 011b 021c 0216 0259 8010 0310  ...*.......Y....
+000002d0: 042a 021b 051c 0316 031c 0416 0459 8010  .*...........Y..
+000002e0: 062a 011b 071c 0616 0659 8010 0810 092a  .*.......Y.....*
+000002f0: 021b 0a1c 0816 081c 0916 0959 4814 8010  ...........YH...
+00000300: 0b10 0c2a 021b 0d1c 0b16 0b1c 0c16 0c59  ...*...........Y
+00000310: 4a29 5711 34df 4462 1635 4916 1136 2300  J)W.4.Db.5I..6#.
+00000320: 140e 1135 3601 3401 5923 0130 0216 0b16  ...56.4.Y#.0....
+00000330: 0c51 5116 3519 355d 4a01 5d51 1737 3200  .QQ.5.5]J.]Q.72.
+00000340: 1611 3201 1612 532c 0023 0210 0f62 3302  ..2...S,.#...b3.
+00000350: 1613 5432 0310 1034 0216 1051 2a01 5333  ..T2...4...Q*.S3
+00000360: 0416 1411 1151 8c51 2a03 5333 0534 0116  .....Q.Q*.S3.4..
+00000370: 1b32 0616 2051 6307 810c 110f 1138 8012  .2.. Qc......8..
+00000380: 6040 4500 b020 0001 c1b1 6301 8148 c980  `@E.. ....c..H..
+00000390: c040 0825 4d80 1825 00b1 53b2 101f 1202  .@.%M..%..S.....
+000003a0: 1326 8135 8401 6386 08e8 441e 1239 3a3b  .&.5..c...D..9:;
+000003b0: 0f80 1d80 0726 2c2a 2a28 58b3 80d8 44c0  .....&,**(X...D.
+000003c0: 8012 3cb3 2287 68f4 b2f7 3401 c412 3db0  ..<.".h...4...=.
+000003d0: b1f3 b4f7 3401 c5b0 b1d8 4443 7f42 4181  ....4.....DC.BA.
+000003e0: c6b4 81f2 8042 5157 c712 3cb0 b7b5 f4b6  .....BQW..<.....
+000003f0: f4f2 3401 6759 81e5 585a d743 2a59 5942  ..4.gY..XZ.C*YYB
+00000400: 4712 3cb1 3401 6759 5163 885c d888 80c0  G.<.4.gYQc.\....
+00000410: 409b 0113 0f80 2f80 0822 3936 2d3b 2928  @...../.."96-;)(
+00000420: 0001 0585 c212 3eb1 2000 0112 3f80 1240  ......>. ...?..@
+00000430: 2501 3401 81f3 8234 0334 0134 01c3 b380  %.4....4.4.4....
+00000440: d944 4380 424c 1241 2500 2287 68f4 b3f7  .DC.BL.A%.".h...
+00000450: 3401 2705 2505 b2d7 4443 b242 4225 0527  4.'.%...DC.BB%.'
+00000460: 0512 42b0 b1b5 2001 0312 3f80 1240 2501  ..B... ...?..@%.
+00000470: 3401 81f3 8234 0334 0134 01c4 1240 b434  4....4.4.4...@.4
+00000480: 0181 d944 48b4 8055 2505 2a02 6312 42b4  ...DH..U%.*.c.B.
+00000490: 3401 2505 2a02 6302 8210 620a 274d 4d80  4.%.*.c...b.'MM.
+000004a0: 382b 00b1 5f4b 14c2 123d 2500 b255 2500  8+.._K...=%..U%.
+000004b0: b281 f255 f334 012f 1442 2a63 8240 f004  ...U.4./.B*c.@..
+000004c0: 0e27 4d4d 4d4d 803b 2b00 b35f 4b17 c412  .'MMMM.;+.._K...
+000004d0: 1225 01b4 5525 01b4 81f2 5525 0225 0034  .%..U%....U%.%.4
+000004e0: 042f 1442 2763 8254 0814 1088 4280 0944  ./.B'c.T....B..D
+000004f0: 8408 6460 1143 1644 1010 1645 2c00 1632  ..d`.C.D...E,..2
+00000500: 3200 1628 3201 1616 1146 3202 3401 1631  2..(2....F2.4..1
+00000510: 5163 0383 7022 1428 4e4f 804e 2524 2926  Qc..p".(NO.N%$)&
+00000520: 2c23 05b0 1829 51b0 182a 1250 b112 4134  ,#...)Q..*.P..A4
+00000530: 0243 4612 06b1 3401 c112 0412 03b1 3401  .CF...4.......4.
+00000540: 3401 b018 2ab0 132a 142b 1204 132c 3601  4...*..*.+...,6.
+00000550: 5951 6385 0039 0e16 4e80 5636 2831 1241  YQc..9..N.V6(1.A
+00000560: b013 2a14 2d36 00b0 132a 142d 3600 f282  ..*.-6...*.-6...
+00000570: f734 01c1 b1b0 1329 8055 f7c2 123c b2b0  .4.....).U...<..
+00000580: 1329 8155 f422 8768 f782 3402 c32c 03b1  .).U.".h..4..,..
+00000590: 102e 6212 3cb2 2280 64f4 8134 0210 2f62  ..b.<.".d..4../b
+000005a0: b310 3062 6382 7019 0e31 4f80 5d2c 272b  ..0bc.p..1O.],'+
+000005b0: b012 1013 3214 3336 00dd 4447 1210 1332  ....2.36..DG...2
+000005c0: b055 6312 10b0 3401 1210 1332 b056 1210  .Uc...4....2.V..
+000005d0: 1332 b055 6385 10ca 0120 141a 4780 6480  .2.Uc.... ..G.d.
+000005e0: 094c 2265 2b22 6962 2030 120b 51de 4346  .L"e+"ib 0..Q.CF
+000005f0: 120c 51de 4442 5163 b151 de44 4d12 0b13  ..Q.DBQc.Q.DM...
+00000600: 1514 16b0 5136 02c2 b263 120b 1417 b036  ....Q6...c.....6
+00000610: 0144 4251 6312 0c34 0014 1810 19b1 101a  .DBQc..4........
+00000620: b036 8400 c3b3 6351 6384 10c0 8501 1c1b  .6....cQc.......
+00000630: 4849 4a1f 8082 800a 2354 452a 4210 1cc4  HIJ.....#TE*B...
+00000640: b014 1db4 3601 4443 b042 4810 1e14 0eb0  ....6.DC.BH.....
+00000650: b436 02c0 b151 de44 4c12 09b0 101f b334  .6...Q.DL......4
+00000660: 8201 5952 6312 08b1 b0b2 3403 6389 00d1  ..YRc.....4.c...
+00000670: 0226 204b 8098 6040 2026 222b 4e2c 2b22  .& K..`@ &"+N,+"
+00000680: 552c 2f2c 2212 3751 de44 7248 1080 1021  U,/,".7Q.DrH...!
+00000690: 2a01 1b22 1c21 c159 b117 374a 2057 1234  *..".!.Y..7J W.4
+000006a0: df44 59c2 490f 1236 2303 140e b236 0134  .DY.I..6#....6.4
+000006b0: 0159 5063 5151 c228 025d 4a01 5d48 0c12  .YPcQQ.(.]J.]H..
+000006c0: 3734 0014 23b0 3601 c34a 2457 1234 df44  74..#.6..J$W.4.D
+000006d0: 5dc2 4913 1236 2304 140e b236 0134 0159  ].I..6#....6.4.Y
+000006e0: 124c b234 01c3 5151 c228 025d 4a01 5db3  .L.4..QQ.(.]J.].
+000006f0: 51de d344 48b3 1024 d944 4252 6350 63    Q..DH..$.DBRcPc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files 12% similar despite different names*

```diff
@@ -39,154 +39,150 @@
 00000260: 6366 675f 6669 6c65 000c 6e6f 7361 6665  cfg_file..nosafe
 00000270: 0081 5581 7182 3f16 434f 4e46 4947 5f50  ..U.q.?.CONFIG_P
 00000280: 4154 4800 0272 0002 7700 815f 0874 7275  ATH..r..w.._.tru
 00000290: 6500 0a66 616c 7365 000e 2e7b 7d2e 6b65  e..false...{}.ke
 000002a0: 7900 8249 817b 8231 123c 6765 6e65 7870  y..I.{.1.<genexp
 000002b0: 723e 002f 2d35 8229 8153 4982 4514 7479  r>./-5.).SI.E.ty
 000002c0: 7065 5f63 6865 636b 0082 2f81 6d81 437d  pe_check../.m.C}
-000002d0: 813d 0a66 6c6f 6174 000b 052a 5b45 5252  .=.float...*[ERR
+000002d0: 813d 0a66 6c6f 6174 000b 0524 5b45 5252  .=.float...$[ERR
 000002e0: 5d20 4c6f 6769 6361 6c50 696e 7320 696d  ] LogicalPins im
-000002f0: 706f 7274 2065 7272 6f72 3a20 7365 745f  port error: set_
-00000300: 7069 6e6d 6170 0005 106e 6f64 655f 636f  pinmap...node_co
-00000310: 6e66 6967 2e6a 736f 6e00 050e 796f 7572  nfig.json...your
-00000320: 5f77 6966 695f 6e61 6d65 0005 1079 6f75  _wifi_name...you
-00000330: 725f 7769 6669 5f70 6173 7377 6400 050c  r_wifi_passwd...
-00000340: 6972 715f 7072 656c 6c5f 6d73 0005 2a5b  irq_prell_ms..*[
-00000350: 434f 4e46 4947 4841 4e44 4c45 525d 2047  CONFIGHANDLER] G
-00000360: 6574 2063 6f6e 6669 6720 7661 6c75 6520  et config value 
-00000370: 6572 726f 723a 207b 7d00 0519 5b45 5252  error: {}...[ERR
-00000380: 5d20 6366 6767 6574 207b 7d20 6572 726f  ] cfgget {} erro
-00000390: 723a 207b 7d00 0519 5b45 5252 5d20 6366  r: {}...[ERR] cf
-000003a0: 6770 7574 207b 7d20 6572 726f 723a 207b  gput {} error: {
-000003b0: 7d00 050c 5b50 494e 204d 4150 5d20 7b7d  }...[PIN MAP] {}
-000003c0: 0005 235b 6d69 6372 4f53 5d20 6465 6275  ..#[micrOS] debu
-000003d0: 6720 7072 696e 7420 7761 7320 7475 726e  g print was turn
-000003e0: 6564 206f 6666 0005 0b63 6c65 616e 7570  ed off...cleanup
-000003f0: 2e70 6473 0005 235b 434f 4e46 4947 4841  .pds..#[CONFIGHA
-00000400: 4e44 4c45 525d 2050 7572 6765 206f 6273  NDLER] Purge obs
-00000410: 6f6c 6574 6520 6b65 7973 0005 395b 434f  olete keys..9[CO
-00000420: 4e46 4947 4841 4e44 4c45 525d 2053 4b49  NFIGHANDLER] SKI
-00000430: 5020 6f62 736f 6c65 7465 206b 6579 7320  P obsolete keys 
-00000440: 6368 6563 6b20 286e 6f20 636c 6561 6e75  check (no cleanu
-00000450: 702e 7064 7329 0005 265b 434f 4e46 4947  p.pds)..&[CONFIG
-00000460: 4841 4e44 4c45 525d 2049 6e6a 6563 7420  HANDLER] Inject 
-00000470: 7573 6572 2063 6f6e 6669 6720 2e2e 2e00  user config ....
-00000480: 052b 5b43 4f4e 4649 4748 414e 444c 4552  .+[CONFIGHANDLER
-00000490: 5d20 5361 7665 2063 6f6e 6620 7374 7275  ] Save conf stru
-000004a0: 6374 2073 7563 6365 7373 6675 6c00 052b  ct successful..+
-000004b0: 5b43 4f4e 4649 4748 414e 444c 4552 5d20  [CONFIGHANDLER] 
-000004c0: 5361 7665 2063 6f6e 6620 7374 7275 6374  Save conf struct
-000004d0: 2066 6169 6c65 643a 207b 7d00 0525 5b45   failed: {}..%[E
-000004e0: 5252 5d20 5f5f 696e 6a65 6374 5f64 6566  RR] __inject_def
-000004f0: 6175 6c74 5f63 6f6e 6620 6572 726f 723a  ault_conf error:
-00000500: 207b 7d00 0531 5b43 4f4e 4649 4748 414e   {}..1[CONFIGHAN
-00000510: 444c 4552 5d20 7265 6164 5f63 6667 5f66  DLER] read_cfg_f
-00000520: 696c 6520 6572 726f 7220 7b7d 2028 6a73  ile error {} (js
-00000530: 6f6e 293a 207b 7d00 0803 302e 3205 1d5b  on): {}...0.2..[
-00000540: 4552 525d 2072 6561 645f 6366 675f 6669  ERR] read_cfg_fi
-00000550: 6c65 2065 7272 6f72 3a20 7b7d 0005 345b  le error: {}..4[
-00000560: 434f 4e46 4947 4841 4e44 4c45 525d 205f  CONFIGHANDLER] _
-00000570: 5f77 7269 7465 5f63 6667 5f66 696c 6520  _write_cfg_file 
-00000580: 6572 726f 7220 7b7d 2028 6a73 6f6e 293a  error {} (json):
-00000590: 207b 7d00 051e 5b45 5252 5d20 7772 6974   {}...[ERR] writ
-000005a0: 655f 6366 675f 6669 6c65 2065 7272 6f72  e_cfg_file error
-000005b0: 3a20 7b7d 0005 2074 7970 655f 6861 6e64  : {}.. type_hand
-000005c0: 6c65 7220 7479 7065 2068 616e 646c 696e  ler type handlin
-000005d0: 6720 6572 726f 7200 051a 496e 7075 7420  g error...Input 
-000005e0: 7661 6c75 6520 7479 7065 2065 7272 6f72  value type error
-000005f0: 2120 7b7d 0089 2c24 2201 800e 2c32 2c38  ! {}..,$"...,2,8
-00000600: 224f 2766 89a9 880f 881a 8010 022a 011b  "O'f.........*..
-00000610: 031c 0216 0259 8010 0410 052a 021b 061c  .....Y.....*....
-00000620: 0416 041c 0516 0559 8010 072a 011b 081c  .......Y...*....
-00000630: 0716 0759 8010 0910 0a10 0b2a 031b 0c1c  ...Y.......*....
-00000640: 0916 091c 0a16 0a1c 0b16 0b59 480e 8010  ...........YH...
-00000650: 0d2a 011b 0e1c 0d16 0d59 4a0e 5911 0b23  .*.......YJ.Y..#
-00000660: 0034 0159 5116 0d4a 015d 5432 0010 0f34  .4.YQ..J.]T2...4
-00000670: 0216 0f51 2a01 5333 0116 3a50 2a01 5333  ...Q*.S3..:P*.S3
-00000680: 0216 3f11 0f14 1036 0059 5163 0393 1c10  ..?....6.YQc....
-00000690: 660f 881b 2427 2425 2525 2524 2525 2627  f...$'$%%%%$%%&'
-000006a0: 2524 2524 2526 2425 2524 2525 2425 2524  %$%$%&$%%$%%$%%$
-000006b0: 2525 2625 2425 2425 2547 8812 881a 8c12  %%&%$%$%%G......
-000006c0: 880e 8818 1155 1656 100f 1657 2301 164a  .....U.V...W#..J
-000006d0: 2c25 1011 1012 6250 1013 6223 0210 1462  ,%....bP..b#...b
-000006e0: 2303 1015 6210 1610 1762 1018 1019 6252  #...b....b....bR
-000006f0: 101a 6210 1b10 1c62 1011 101d 6222 8064  ..b....b....b".d
-00000700: 101e 6222 80c6 3010 1f62 1011 1020 6250  ..b"..0..b... bP
-00000710: 1021 6210 1110 2262 5010 2362 1011 1024  .!b..."bP.#b...$
-00000720: 6222 8768 1025 6250 1026 6210 1110 2762  b".h.%bP.&b...'b
-00000730: 1011 1028 6250 1029 6210 1110 2a62 1011  ...(bP.)b...*b..
-00000740: 102b 6250 102c 6210 1110 2d62 1011 102e  .+bP.,b...-b....
-00000750: 6250 102f 6210 1110 3062 1011 1031 6222  bP./b...0b...1b"
-00000760: 822c 2304 6210 1110 3262 8310 3362 223c  .,#.b...2b..3b"<
-00000770: 1034 6252 1035 6210 3610 3762 1011 1038  .4bR.5b.6.7b...8
-00000780: 6210 1110 3962 163b 1158 3200 3401 1610  b...9b.;.X2.4...
-00000790: 1158 3201 3401 1642 1158 502a 0153 3302  .X2.4..B.XP*.S3.
-000007a0: 3401 1645 1158 3203 3401 1641 1158 3204  4..E.X2.4..A.X2.
-000007b0: 3401 1640 1158 512a 0153 3305 3401 163d  4..@.XQ*.S3.4..=
-000007c0: 5163 0685 3820 1410 8045 4727 2c4c 2a49  Qc..8 ...EG',L*I
-000007d0: 6912 0f14 4236 0059 120d 51de d344 5812  i...B6.Y..Q..DX.
-000007e0: 0d12 0f13 3b10 3855 3401 c012 0a23 0814  ....;.8U4....#..
-000007f0: 3eb0 3601 3401 5912 3a10 1a34 0112 0918  >.6.4.Y.:..4....
-00000800: 4312 0f13 3b10 1a55 4449 1209 1444 3600  C...;..UDI...D6.
-00000810: 5942 4712 0a23 0934 0159 5163 8a7c d402  YBG..#.4.YQc.|..
-00000820: 2242 8057 4b22 2727 2e53 4a4a 2744 2752  "B.WK"''.SJJ'D'R
-00000830: 2c56 120f 1445 1046 5236 8200 c048 2812  ,V...E.FR6...H(.
-00000840: 0723 0a34 0159 120a 230b 3401 5932 00b0  .#.4.Y..#.4.Y2..
-00000850: 1447 3600 5e34 015f 4b0b c1b0 1448 b151  .G6.^4._K....H.Q
-00000860: 3602 5942 334a 1157 125a df44 4a59 120a  6.YB3J.W.Z.DJY..
-00000870: 230c 3401 594a 015d 120f 133b 1449 b036  #.4.YJ.]...;.I.6
-00000880: 0159 120a 230d 3401 5949 3d48 1012 0f14  .Y..#.4.YI=H....
-00000890: 4136 0059 120a 230e 3401 594a 2a57 125a  A6.Y..#.4.YJ*W.Z
-000008a0: df44 63c2 4919 120a 230f 143e b236 0134  .Dc.I...#..>.6.4
-000008b0: 0159 120b 2310 143e b236 0134 0159 5151  .Y..#..>.6.4.YQQ
-000008c0: c228 025d 4a01 5d51 2800 5d51 6301 8210  .(.]J.]Q(.]Qc...
-000008d0: c140 0854 6380 5c53 b053 534b 13c1 b112  .@.Tc.\S.SSK....
-000008e0: 0f13 3b14 4736 00dd d344 30b1 6759 422b  ..;.G6...D0.gYB+
-000008f0: 5163 8678 d903 1e45 4680 7023 2022 2d29  Qc.x...EF.p# "-)
-00000900: 4e4d 2323 2758 2c00 c148 1b12 5e12 0f13  NM##'X,..H..^...
-00000910: 4a10 4b34 0247 08c2 1204 b234 01c1 515c  J.K4.G.....4..Q\
-00000920: 5d40 7e01 4a38 5712 5adf 4471 c349 2712  ]@~.J8W.Z.Dq.I'.
-00000930: 0a23 1114 3eb1 b336 0234 0159 b044 4340  .#..>..6.4.Y.DC@
-00000940: 6002 1202 2312 3401 5912 0b23 1314 3eb3  `...#.4.Y..#..>.
-00000950: 3601 3401 5951 51c3 2803 5d4a 015d 42a8  6.4.YQQ.(.]J.]B.
-00000960: 7fb1 6386 48c8 0216 4180 8220 422d 2d4e  ..c.H...A.. B--N
-00000970: 3035 2a48 1f12 5e12 0f13 4a10 4c34 0247  05*H..^...J.L4.G
-00000980: 0cc0 1205 120f 133b b034 0259 515c 5d40  .......;.4.YQ\]@
-00000990: 7b01 4a2e 5712 5adf 4467 c149 1d12 0a23  {.J.W.Z.Dg.I...#
-000009a0: 1414 3e12 0f13 4ab1 3602 3401 5912 0b23  ..>...J.6.4.Y..#
-000009b0: 1514 3eb1 3601 3401 5951 51c1 2801 5d4a  ..>.6.4.YQQ.(.]J
-000009c0: 015d 1202 2312 3401 5942 a77f 5263 8a58  .]..#.4.YB..Rc.X
-000009d0: d202 3040 595b 8090 2722 2922 2e22 2e22  ..0@Y[..'")"."."
-000009e0: 2729 2226 2922 2629 2251 3512 0f13 3bb0  ')"&)"&)"Q5...;.
-000009f0: 55c2 4867 125f b212 6034 0244 6928 0212  U.Hg._..`4.Di(..
-00000a00: 5db1 3401 144d 3600 104e d944 4252 6312  ].4..M6..N.DBRc.
-00000a10: 5db1 3401 144d 3600 104f d944 4250 6312  ].4..M6..O.DBPc.
-00000a20: 5a23 1634 0165 125f b212 5d34 0244 4828  Z#.4.e._..]4.DH(
-00000a30: 0212 5db1 3401 6312 5fb2 1261 3402 4448  ..].4.c._..a4.DH
-00000a40: 2802 1261 b134 0163 125f b212 6234 0244  (..a.4.c._..b4.D
-00000a50: 4828 0212 62b1 3401 634a 1e57 125a df44  H(..b.4.cJ.W.Z.D
-00000a60: 57c3 490d 120a 2317 143e b336 0134 0159  W.I...#..>.6.4.Y
-00000a70: 5151 c328 035d 4a01 5d51 6388 20c2 0320  QQ.(.]J.]Qc. .. 
-00000a80: 3d59 5b80 a860 4035 2230 2a4b 4522 3076  =Y[..`@5"0*KE"0v
-00000a90: 125f b112 5d34 0244 78b0 120f 133b 1447  ._..]4.Dx....;.G
-00000aa0: 3600 dd44 6c48 1e12 5e10 5014 3eb0 3601  6..DlH..^.P.>.6.
-00000ab0: 104c 3402 4709 c2b2 1451 b136 0159 515c  .L4.G....Q.6.YQ\
-00000ac0: 5d52 634a 0c57 125a df44 4559 5063 4a01  ]RcJ.W.Z.DEYPcJ.
-00000ad0: 5d48 1f12 5e10 5014 3eb0 3601 104b 3402  ]H..^.P.>.6..K4.
-00000ae0: 470c c2b2 1452 3600 1453 3600 6351 5c5d  G....R6..S6.cQ\]
-00000af0: 4a0d 5712 5adf 4446 5910 1163 4a01 5d51  J.W.Z.DFY..cJ.]Q
-00000b00: 6386 30d1 031a 3a59 80c3 2525 222b 4628  c.0...:Y..%%"+F(
-00000b10: 4d2c 36b0 51de 4445 120f 133b 6348 1d12  M,6.Q.DE...;cH..
-00000b20: 0f13 3b14 3cb0 5136 02c1 b110 36d9 4448  ..;.<.Q6....6.DH
-00000b30: 120f 143d b036 0163 b163 4a2b 5712 5adf  ...=.6.c.cJ+W.Z.
-00000b40: 4464 c249 1a12 0a23 0514 3eb2 3601 3401  Dd.I...#..>.6.4.
-00000b50: 5912 0b23 0614 3eb0 b236 0234 0159 5151  Y..#..>..6.4.YQQ
-00000b60: c228 025d 4a01 5d51 6389 28db 0328 3f59  .(.]J.]Qc.(..(?Y
-00000b70: 5b5c 80d3 3349 2a22 2223 492f 2227 2722  [\..3I*""#I/"''"
-00000b80: 4d2d 125d 120f 133b 143c b051 3602 3401  M-.]...;.<.Q6.4.
-00000b90: 1036 d944 4912 0f14 3db0 b136 0263 120f  .6.DI...=..6.c..
-00000ba0: 133b b055 b1d9 4442 5263 4831 b244 4912  .;.U..DBRcH1.DI.
-00000bb0: 0f14 40b0 b136 02c1 b151 de43 4a12 5db1  ..@..6...Q.CJ.].
-00000bc0: 3401 1036 d944 4250 63b1 120f 133b b056  4..6.DBPc....;.V
-00000bd0: 120f 1441 3600 5928 0152 634a 2157 125a  ...A6.Y(.RcJ!W.Z
-00000be0: df44 5ac3 4910 120b 2307 143e b0b3 3602  .DZ.I...#..>..6.
-00000bf0: 3401 5950 6351 51c3 2803 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
+000002f0: 706f 7274 3a20 7365 745f 7069 6e6d 6170  port: set_pinmap
+00000300: 0005 106e 6f64 655f 636f 6e66 6967 2e6a  ...node_config.j
+00000310: 736f 6e00 050e 796f 7572 5f77 6966 695f  son...your_wifi_
+00000320: 6e61 6d65 0005 1079 6f75 725f 7769 6669  name...your_wifi
+00000330: 5f70 6173 7377 6400 050c 6972 715f 7072  _passwd...irq_pr
+00000340: 656c 6c5f 6d73 0005 215b 434f 4e46 5d20  ell_ms..![CONF] 
+00000350: 4765 7420 636f 6e66 6967 2076 616c 7565  Get config value
+00000360: 2065 7272 6f72 3a20 7b7d 0005 195b 4552   error: {}...[ER
+00000370: 525d 2063 6667 6765 7420 7b7d 2065 7272  R] cfgget {} err
+00000380: 6f72 3a20 7b7d 0005 195b 4552 525d 2063  or: {}...[ERR] c
+00000390: 6667 7075 7420 7b7d 2065 7272 6f72 3a20  fgput {} error: 
+000003a0: 7b7d 0005 0c5b 5049 4e20 4d41 505d 207b  {}...[PIN MAP] {
+000003b0: 7d00 0521 5b6d 6963 724f 535d 2064 6562  }..![micrOS] deb
+000003c0: 7567 2070 7269 6e74 202d 2074 7572 6e65  ug print - turne
+000003d0: 6420 6f66 6600 050b 636c 6561 6e75 702e  d off...cleanup.
+000003e0: 7064 7300 051a 5b43 4f4e 465d 2050 7572  pds...[CONF] Pur
+000003f0: 6765 206f 6273 6f6c 6574 6520 6b65 7973  ge obsolete keys
+00000400: 0005 305b 434f 4e46 5d20 534b 4950 206f  ..0[CONF] SKIP o
+00000410: 6273 6f6c 6574 6520 6b65 7973 2063 6865  bsolete keys che
+00000420: 636b 2028 6e6f 2063 6c65 616e 7570 2e70  ck (no cleanup.p
+00000430: 6473 2900 0521 5b43 4f4e 465d 2055 7365  ds)..![CONF] Use
+00000440: 7220 636f 6e66 6967 2069 6e6a 6563 7469  r config injecti
+00000450: 6f6e 2064 6f6e 6500 0522 5b43 4f4e 465d  on done.."[CONF]
+00000460: 2053 6176 6520 636f 6e66 2073 7472 7563   Save conf struc
+00000470: 7420 7375 6363 6573 7366 756c 0005 225b  t successful.."[
+00000480: 434f 4e46 5d20 5361 7665 2063 6f6e 6620  CONF] Save conf 
+00000490: 7374 7275 6374 2066 6169 6c65 643a 207b  struct failed: {
+000004a0: 7d00 0525 5b45 5252 5d20 5f5f 696e 6a65  }..%[ERR] __inje
+000004b0: 6374 5f64 6566 6175 6c74 5f63 6f6e 6620  ct_default_conf 
+000004c0: 6572 726f 723a 207b 7d00 0528 5b43 4f4e  error: {}..([CON
+000004d0: 465d 2072 6561 645f 6366 675f 6669 6c65  F] read_cfg_file
+000004e0: 2065 7272 6f72 207b 7d20 286a 736f 6e29   error {} (json)
+000004f0: 3a20 7b7d 0008 0330 2e32 051d 5b45 5252  : {}...0.2..[ERR
+00000500: 5d20 7265 6164 5f63 6667 5f66 696c 6520  ] read_cfg_file 
+00000510: 6572 726f 723a 207b 7d00 052b 5b43 4f4e  error: {}..+[CON
+00000520: 465d 205f 5f77 7269 7465 5f63 6667 5f66  F] __write_cfg_f
+00000530: 696c 6520 6572 726f 7220 7b7d 2028 6a73  ile error {} (js
+00000540: 6f6e 293a 207b 7d00 051e 5b45 5252 5d20  on): {}...[ERR] 
+00000550: 7772 6974 655f 6366 675f 6669 6c65 2065  write_cfg_file e
+00000560: 7272 6f72 3a20 7b7d 0005 2074 7970 655f  rror: {}.. type_
+00000570: 6861 6e64 6c65 7220 7479 7065 2068 616e  handler type han
+00000580: 646c 696e 6720 6572 726f 7200 051a 496e  dling error...In
+00000590: 7075 7420 7661 6c75 6520 7479 7065 2065  put value type e
+000005a0: 7272 6f72 2120 7b7d 0089 2c24 2201 800e  rror! {}..,$"...
+000005b0: 2c32 2c38 224f 2766 89a9 880f 881b 8010  ,2,8"O'f........
+000005c0: 022a 011b 031c 0216 0259 8010 0410 052a  .*.......Y.....*
+000005d0: 021b 061c 0416 041c 0516 0559 8010 072a  ...........Y...*
+000005e0: 011b 081c 0716 0759 8010 0910 0a10 0b2a  .......Y.......*
+000005f0: 031b 0c1c 0916 091c 0a16 0a1c 0b16 0b59  ...............Y
+00000600: 480e 8010 0d2a 011b 0e1c 0d16 0d59 4a0e  H....*.......YJ.
+00000610: 5911 0b23 0034 0159 5116 0d4a 015d 5432  Y..#.4.YQ..J.]T2
+00000620: 0010 0f34 0216 0f51 2a01 5333 0116 3a50  ...4...Q*.S3..:P
+00000630: 2a01 5333 0216 3f11 0f14 1036 0059 5163  *.S3..?....6.YQc
+00000640: 0393 1c10 660f 881b 2427 2425 2525 2524  ....f...$'$%%%%$
+00000650: 2525 2627 2524 2524 2526 2425 2524 2525  %%&'%$%$%&$%%$%%
+00000660: 2425 2524 2525 2625 2425 2425 2547 8812  $%%$%%&%$%$%%G..
+00000670: 881a 8c12 880e 8818 1155 1656 100f 1657  .........U.V...W
+00000680: 2301 164a 2c25 1011 1012 6250 1013 6223  #..J,%....bP..b#
+00000690: 0210 1462 2303 1015 6210 1610 1762 1018  ...b#...b....b..
+000006a0: 1019 6252 101a 6210 1b10 1c62 1011 101d  ..bR..b....b....
+000006b0: 6222 8064 101e 6222 80c6 3010 1f62 1011  b".d..b"..0..b..
+000006c0: 1020 6250 1021 6210 1110 2262 5010 2362  . bP.!b..."bP.#b
+000006d0: 1011 1024 6222 8768 1025 6250 1026 6210  ...$b".h.%bP.&b.
+000006e0: 1110 2762 1011 1028 6250 1029 6210 1110  ..'b...(bP.)b...
+000006f0: 2a62 1011 102b 6250 102c 6210 1110 2d62  *b...+bP.,b...-b
+00000700: 1011 102e 6250 102f 6210 1110 3062 1011  ....bP./b...0b..
+00000710: 1031 6222 822c 2304 6210 1110 3262 8310  .1b".,#.b...2b..
+00000720: 3362 223c 1034 6252 1035 6210 3610 3762  3b"<.4bR.5b.6.7b
+00000730: 1011 1038 6210 1110 3962 163b 1158 3200  ...8b...9b.;.X2.
+00000740: 3401 1610 1158 3201 3401 1642 1158 502a  4....X2.4..B.XP*
+00000750: 0153 3302 3401 1645 1158 3203 3401 1641  .S3.4..E.X2.4..A
+00000760: 1158 3204 3401 1640 1158 512a 0153 3305  .X2.4..@.XQ*.S3.
+00000770: 3401 163d 5163 0685 3820 1410 8045 4727  4..=Qc..8 ...EG'
+00000780: 2c4c 2a49 6912 0f14 4236 0059 120d 51de  ,L*Ii...B6.Y..Q.
+00000790: d344 5812 0d12 0f13 3b10 3855 3401 c012  .DX.....;.8U4...
+000007a0: 0a23 0814 3eb0 3601 3401 5912 3a10 1a34  .#..>.6.4.Y.:..4
+000007b0: 0112 0918 4312 0f13 3b10 1a55 4449 1209  ....C...;..UDI..
+000007c0: 1444 3600 5942 4712 0a23 0934 0159 5163  .D6.YBG..#.4.YQc
+000007d0: 8a7c d402 2242 8057 4b22 2727 2e73 4a2a  .|.."B.WK"''.sJ*
+000007e0: 2744 2752 2c56 120f 1445 1046 5236 8200  'D'R,V...E.FR6..
+000007f0: c048 2812 0723 0a34 0159 120a 230b 3401  .H(..#.4.Y..#.4.
+00000800: 5932 00b0 1447 3600 5e34 015f 4b0b c1b0  Y2...G6.^4._K...
+00000810: 1448 b151 3602 5942 334a 1157 125a df44  .H.Q6.YB3J.W.Z.D
+00000820: 4a59 120a 230c 3401 594a 015d 120f 133b  JY..#.4.YJ.]...;
+00000830: 1449 b036 0159 120a 230d 3401 5949 3d48  .I.6.Y..#.4.YI=H
+00000840: 1012 0f14 4136 0059 120a 230e 3401 594a  ....A6.Y..#.4.YJ
+00000850: 2a57 125a df44 63c2 4919 120a 230f 143e  *W.Z.Dc.I...#..>
+00000860: b236 0134 0159 120b 2310 143e b236 0134  .6.4.Y..#..>.6.4
+00000870: 0159 5151 c228 025d 4a01 5d51 2800 5d51  .YQQ.(.]J.]Q(.]Q
+00000880: 6301 8210 c140 0854 6380 5c53 b053 534b  c....@.Tc.\S.SSK
+00000890: 13c1 b112 0f13 3b14 4736 00dd d344 30b1  ......;.G6...D0.
+000008a0: 6759 422b 5163 8678 d903 1e45 4680 7023  gYB+Qc.x...EF.p#
+000008b0: 2022 2d29 4e4d 2323 2758 2c00 c148 1b12   "-)NM##'X,..H..
+000008c0: 5e12 0f13 4a10 4b34 0247 08c2 1204 b234  ^...J.K4.G.....4
+000008d0: 01c1 515c 5d40 7e01 4a38 5712 5adf 4471  ..Q\]@~.J8W.Z.Dq
+000008e0: c349 2712 0a23 1114 3eb1 b336 0234 0159  .I'..#..>..6.4.Y
+000008f0: b044 4340 6002 1202 2312 3401 5912 0b23  .DC@`...#.4.Y..#
+00000900: 1314 3eb3 3601 3401 5951 51c3 2803 5d4a  ..>.6.4.YQQ.(.]J
+00000910: 015d 42a8 7fb1 6386 48c8 0216 4180 8220  .]B...c.H...A.. 
+00000920: 422d 2d4e 3035 2a48 1f12 5e12 0f13 4a10  B--N05*H..^...J.
+00000930: 4c34 0247 0cc0 1205 120f 133b b034 0259  L4.G.......;.4.Y
+00000940: 515c 5d40 7b01 4a2e 5712 5adf 4467 c149  Q\]@{.J.W.Z.Dg.I
+00000950: 1d12 0a23 1414 3e12 0f13 4ab1 3602 3401  ...#..>...J.6.4.
+00000960: 5912 0b23 1514 3eb1 3601 3401 5951 51c1  Y..#..>.6.4.YQQ.
+00000970: 2801 5d4a 015d 1202 2312 3401 5942 a77f  (.]J.]..#.4.YB..
+00000980: 5263 8a58 d202 3040 595b 8090 2722 2922  Rc.X..0@Y[..'")"
+00000990: 2e22 2e22 2729 2226 2922 2629 2251 3512  ."."')"&)"&)"Q5.
+000009a0: 0f13 3bb0 55c2 4867 125f b212 6034 0244  ..;.U.Hg._..`4.D
+000009b0: 6928 0212 5db1 3401 144d 3600 104e d944  i(..].4..M6..N.D
+000009c0: 4252 6312 5db1 3401 144d 3600 104f d944  BRc.].4..M6..O.D
+000009d0: 4250 6312 5a23 1634 0165 125f b212 5d34  BPc.Z#.4.e._..]4
+000009e0: 0244 4828 0212 5db1 3401 6312 5fb2 1261  .DH(..].4.c._..a
+000009f0: 3402 4448 2802 1261 b134 0163 125f b212  4.DH(..a.4.c._..
+00000a00: 6234 0244 4828 0212 62b1 3401 634a 1e57  b4.DH(..b.4.cJ.W
+00000a10: 125a df44 57c3 490d 120a 2317 143e b336  .Z.DW.I...#..>.6
+00000a20: 0134 0159 5151 c328 035d 4a01 5d51 6388  .4.YQQ.(.]J.]Qc.
+00000a30: 20c2 0320 3d59 5b80 a860 4035 2230 2a4b   .. =Y[..`@5"0*K
+00000a40: 4522 3076 125f b112 5d34 0244 78b0 120f  E"0v._..]4.Dx...
+00000a50: 133b 1447 3600 dd44 6c48 1e12 5e10 5014  .;.G6..DlH..^.P.
+00000a60: 3eb0 3601 104c 3402 4709 c2b2 1451 b136  >.6..L4.G....Q.6
+00000a70: 0159 515c 5d52 634a 0c57 125a df44 4559  .YQ\]RcJ.W.Z.DEY
+00000a80: 5063 4a01 5d48 1f12 5e10 5014 3eb0 3601  PcJ.]H..^.P.>.6.
+00000a90: 104b 3402 470c c2b2 1452 3600 1453 3600  .K4.G....R6..S6.
+00000aa0: 6351 5c5d 4a0d 5712 5adf 4446 5910 1163  cQ\]J.W.Z.DFY..c
+00000ab0: 4a01 5d51 6386 30d1 031a 3a59 80c3 2525  J.]Qc.0...:Y..%%
+00000ac0: 222b 4628 4d2c 36b0 51de 4445 120f 133b  "+F(M,6.Q.DE...;
+00000ad0: 6348 1d12 0f13 3b14 3cb0 5136 02c1 b110  cH....;.<.Q6....
+00000ae0: 36d9 4448 120f 143d b036 0163 b163 4a2b  6.DH...=.6.c.cJ+
+00000af0: 5712 5adf 4464 c249 1a12 0a23 0514 3eb2  W.Z.Dd.I...#..>.
+00000b00: 3601 3401 5912 0b23 0614 3eb0 b236 0234  6.4.Y..#..>..6.4
+00000b10: 0159 5151 c228 025d 4a01 5d51 6389 28db  .YQQ.(.]J.]Qc.(.
+00000b20: 0328 3f59 5b5c 80d3 3349 2a22 2223 492f  .(?Y[\..3I*""#I/
+00000b30: 2227 2722 4d2d 125d 120f 133b 143c b051  "''"M-.]...;.<.Q
+00000b40: 3602 3401 1036 d944 4912 0f14 3db0 b136  6.4..6.DI...=..6
+00000b50: 0263 120f 133b b055 b1d9 4442 5263 4831  .c...;.U..DBRcH1
+00000b60: b244 4912 0f14 40b0 b136 02c1 b151 de43  .DI...@..6...Q.C
+00000b70: 4a12 5db1 3401 1036 d944 4250 63b1 120f  J.].4..6.DBPc...
+00000b80: 133b b056 120f 1441 3600 5928 0152 634a  .;.V...A6.Y(.RcJ
+00000b90: 2157 125a df44 5ac3 4910 120b 2307 143e  !W.Z.DZ.I...#..>
+00000ba0: b0b3 3602 3401 5950 6351 51c3 2803 5d4a  ..6.4.YPcQQ.(.]J
+00000bb0: 015d 5163                                .]Qc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Debug.mpy`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 4d06 001f 5308 1044 6562 7567 2e70 7900  M...S..Debug.py.
+00000000: 4d06 001f 5208 1044 6562 7567 2e70 7900  M...R..Debug.py.
 00000010: 0f04 6f73 0012 6c6f 6361 6c74 696d 6500  ..os..localtime.
 00000020: 0874 696d 6500 0650 696e 000e 6d61 6368  .time..Pin..mach
 00000030: 696e 6500 104e 656f 5069 7865 6c00 106e  ine..NeoPixel..n
 00000040: 656f 7069 7865 6c00 1870 6879 7369 6361  eopixel..physica
 00000050: 6c5f 7069 6e00 1670 696e 6d61 705f 6475  l_pin..pinmap_du
 00000060: 6d70 001e 6465 7465 6374 5f70 6c61 7466  mp..detect_platf
 00000070: 6f72 6d00 164c 6f67 6963 616c 5069 6e73  orm..LogicalPins
@@ -25,98 +25,97 @@
 00000180: 3130 3200 185f 7374 6570 5f77 7332 3831  102.._step_ws281
 00000190: 3200 124e 454f 5f57 4845 454c 0033 8249  2..NEO_WHEEL.3.I
 000001a0: 8245 0e5f 6c6f 6767 6572 0002 2e00 8151  .E._logger.....Q
 000001b0: 022d 0002 3a00 0c7b 7d20 7b7d 0a00 1272  .-..:..{} {}...r
 000001c0: 6561 646c 696e 6573 0079 0873 6565 6b00  eadlines.y.seek.
 000001d0: 0314 3c6c 6973 7463 6f6d 703e 0081 1f08  ..<listcomp>....
 000001e0: 2e6c 6f67 001a 5f5f 636f 6c6f 725f 7768  .log..__color_wh
-000001f0: 6565 6c00 4902 6500 2f2d 3582 2906 6d73  eel.I.e./-5.).ms
-00000200: 6700 8177 0864 6174 6100 0c66 5f6e 616d  g..w.data..f_nam
-00000210: 6500 0c6d 7367 6f62 6a00 816d 8143 0a5f  e..msgobj..m.C._
-00000220: 6461 7461 000e 5f66 5f6e 616d 6500 0c5f  data.._f_name.._
-00000230: 6c69 6d69 7400 0c66 5f6d 6f64 6500 8157  limit..f_mode..W
-00000240: 0b82 2f05 0b20 4465 6c65 7465 3a20 7b7d  ../.. Delete: {}
-00000250: 0005 1864 6562 7567 206c 6564 2073 7465  ...debug led ste
-00000260: 7020 6572 726f 723a 207b 7d00 0a03 0702  p error: {}.....
-00000270: 3130 0701 3007 0130 0a03 0701 3507 0135  10..0..0....5..5
-00000280: 0701 300a 0307 0130 0702 3130 0701 300a  ..0....0..10..0.
-00000290: 0307 0130 0701 3507 0135 0a03 0701 3007  ...0..5..5....0.
-000002a0: 0130 0702 3130 0a03 0701 3507 0130 0701  .0..10....5..0..
-000002b0: 358b 44a8 0230 0126 2c2c 4c22 5b46 4252  5.D..0.&,,L"[FBR
-000002c0: 8d08 894e 840c 842f 881c 8409 8807 8051  ...N.../.......Q
-000002d0: 1b02 1602 8010 032a 011b 041c 0316 0359  .......*.......Y
-000002e0: 8010 052a 011b 061c 0516 0559 8010 072a  ...*.......Y...*
-000002f0: 011b 081c 0716 0759 481a 8010 0910 0a10  .......YH.......
-00000300: 0b2a 031b 0c1c 0916 091c 0a16 0a1c 0b16  .*..............
-00000310: 0b59 4a07 5951 160b 4a01 5d48 0880 511b  .YJ.YQ..J.]H..Q.
-00000320: 0d16 0d4a 1757 113f df44 5016 4049 0451  ...J.W.?.DP.@I.Q
-00000330: 160d 5151 1640 1940 5d4a 015d 5432 0010  ..QQ.@.@]J.]T2..
-00000340: 0e34 0216 0e32 0116 0f32 0216 1251 2a01  .4...2...2...Q*.
-00000350: 5333 0316 1532 0416 1a51 2a01 5333 0516  S3...2...Q*.S3..
-00000360: 1d51 2a01 5333 0616 1e51 6307 852c 0820  .Q*.S3...Qc..,. 
-00000370: 0e88 1723 2343 8812 6840 6840 6840 880f  ...##C..h@h@h@..
-00000380: 1141 1642 100e 1643 5216 1051 162a 5116  .A.B...CR..Q.*Q.
-00000390: 2d11 4432 0034 0116 2211 4432 0134 0116  -.D2.4..".D2.4..
-000003a0: 2811 4432 0234 0116 2411 4432 0334 0116  (.D2.4..$.D2.4..
-000003b0: 2711 4432 0434 0116 2c11 4432 0534 0116  '.D2.4..,.D2.4..
-000003c0: 1151 6306 8540 1016 2280 1e46 2225 4d29  .Qc..@.."..F"%M)
-000003d0: 2e46 6912 0b51 de44 4251 6312 0b34 00c0  .Fi..Q.DBQc..4..
-000003e0: b010 23d9 4450 120d 51de d344 4912 0e14  ..#.DP..Q..DI...
-000003f0: 2436 0059 4266 120a 1025 3401 1025 5551  $6.YBf...%4..%UQ
-00000400: ded3 4458 b010 26d9 4449 120e 1427 3600  ..DX..&.DI...'6.
-00000410: 5942 4712 0e14 2836 0059 4240 5163 8148  YBG...(6.YB@Qc.H
-00000420: 1006 2880 3012 0512 0910 2534 0112 0513  ..(.0.....%4....
-00000430: 2934 0212 0e18 2a51 6381 0808 0624 8035  )4....*Qc....$.5
-00000440: 120d 142b 3600 120e 182a 5163 8168 1808  ...+6....*Qc.h..
-00000450: 2780 392b 1205 1209 1025 3401 3401 c012  '.9+.....%4.4...
-00000460: 07b0 8134 0212 0e18 2a51 6383 2c18 102c  ...4....*Qc.,..,
-00000470: 803e 8308 2827 2e32 00c0 120e 132d 51de  .>..('.2.....-Q.
-00000480: 4447 b034 0012 0e18 2d12 0e13 2d14 2e36  DG.4....-...-..6
-00000490: 0012 0e13 2a80 5612 0e13 2a14 2f36 0059  ....*.V...*./6.Y
-000004a0: 5163 0182 4080 4012 3e80 3f20 2424 2424  Qc..@.@.>.? $$$$
-000004b0: 2423 0267 5923 0367 5923 0467 5923 0567  $#.gY#.gY#.gY#.g
-000004c0: 5923 0667 5923 0767 5942 2651 6388 28b8  Y#.gY#.gYB&Qc.(.
-000004d0: 0220 1180 4d60 4022 4c32 224c 2722 4e27  . ..M`@"L2"L'"N'
-000004e0: 4d2c 484e 124b 120e 132a 1205 3402 4454  M,HN.K...*..4.DT
-000004f0: 120e 132a 1430 120e 132a 1430 3600 d336  ...*.0...*.06..6
-00000500: 0159 5263 124b 120e 132a 1207 3402 4449  .YRc.K...*..4.DI
-00000510: 120e 142c 3600 5950 6312 0d51 de43 5112  ...,6.YPc..Q.CQ.
-00000520: 0e13 2a51 de43 4912 0d14 1136 0059 5063  ..*Q.CI....6.YPc
-00000530: 4a20 5712 3fdf 4459 c049 0f12 1a23 0114  J W.?.DY.I...#..
-00000540: 20b0 3601 3401 5950 6351 51c0 2800 5d4a   .6.4.YPcQQ.(.]J
-00000550: 015d 5163 8248 1910 0f45 8065 2627 2623  .]Qc.H...E.e&'&#
-00000560: 120e 1310 4457 120e 1411 3600 c112 46b0  ....DW....6...F.
-00000570: 3401 59b1 4447 120e 1411 3600 5951 6383  4.Y.DG....6.YQc.
-00000580: 74db 021e 1247 481c 8071 800a 8818 424a  t....GH..q....BJ
-00000590: 424c 2810 132a 0153 3300 c348 09b3 b0b1  BL(..*.S3..H....
-000005a0: b234 0359 4a17 5948 0bb3 b0b1 b210 1434  .4.YJ.YH.......4
-000005b0: 0459 4a06 5950 634a 015d 4a01 5d52 6301  .YJ.YPcJ.]J.]Rc.
-000005c0: 8a14 fc05 2831 4c4d 4e4f 807c 4a29 5d29  ....(1LMNO.|J)])
-000005d0: 494a 2627 4725 284a 48b2 9ed8 4443 9e42  IJ&'G%(JH...DC.B
-000005e0: 41b2 c232 0012 0334 0034 01c4 1032 1433  A..2...4.4...2.3
-000005f0: b480 832e 0255 3601 1034 f210 3514 33b4  .....U6..4..5.3.
-00000600: 8386 2e02 5536 01f2 c512 4ab1 b334 0247  ....U6....J..4.G
-00000610: 4fc6 1036 1420 b5b0 3602 c032 01b6 1437  O..6. ..6..2...7
-00000620: 3600 3401 c712 50b7 3401 c8b7 1438 b036  6.4...P.4....8.6
-00000630: 0159 b614 3980 3601 59b8 b2db 4452 b7b2  .Y..9.6.Y...DR..
-00000640: d151 2e02 55c7 103a 1433 b736 01c9 4248  .Q..U..:.3.6..BH
-00000650: 103a 1433 b736 01c9 b614 2fb9 3601 5951  .:.3.6..../.6.YQ
-00000660: 5c5d 5163 0281 3841 083b 5180 7e2b 00b0  \]Qc..8A.;Q.~+..
-00000670: 5f4b 0ac1 1252 b134 012f 1442 3463 8178  _K...R.4./.B4c.x
-00000680: 4108 3b51 8084 2b00 b05f 4b12 c110 34b1  A.;Q..+.._K...4.
-00000690: dd44 3710 32b1 dd44 31b1 2f14 422c 6386  .D7.2..D1./.B,c.
-000006a0: 30ca 0324 1548 4980 a060 2022 222a 2a42  0..$.HI..` ""**B
-000006b0: 4d25 4825 5323 80c2 4847 124a b010 1634  M%H%S#..HG.J...4
-000006c0: 0247 3ac3 b314 1736 0014 1836 00c4 4269  .G:....6...6..Bi
-000006d0: b210 19b4 dd44 4381 4241 80e5 c2b1 51de  .....DC.BA....Q.
-000006e0: 4448 120f b434 0159 4245 b1b4 3401 59b3  DH...4.YBE..4.Y.
-000006f0: 1417 3600 1418 3600 c4b4 4314 515c 5d4a  ..6...6...C.Q\]J
-00000700: 0459 4a01 5db2 6381 3831 0e1a 4780 bc60  .YJ.].c.81..G..`
-00000710: 2023 101b c112 12b0 b110 1c85 3482 0263   #..........4..c
-00000720: 8128 a901 0c1d 4980 c523 4710 1bc1 1215  .(....I..#G.....
-00000730: b1b0 3402 c2b2 6384 1cd1 0114 1e49 80cc  ..4...c......I..
-00000740: 2b25 2825 4825 3200 1202 141f 3600 3401  +%(%H%2.....6.4.
-00000750: c1b1 5f4b 25c2 2300 1420 b236 01c3 b051  .._K%.#.. .6...Q
-00000760: de44 4812 0fb3 3401 5942 45b0 b334 0159  .DH...4.YBE..4.Y
-00000770: 1202 1421 b236 0159 4219 5163 0181 6049  ...!.6.YB.Qc..`I
-00000780: 083b 5180 cc2b 00b0 5f4b 0fc1 b114 3c10  .;Q..+.._K....<.
-00000790: 3d36 0144 34b1 2f14 422f 63              =6.D4./.B/c
+000001f0: 6565 6c00 2f2d 3582 2906 6d73 6700 8177  eel./-5.).msg..w
+00000200: 0864 6174 6100 0c66 5f6e 616d 6500 0c6d  .data..f_name..m
+00000210: 7367 6f62 6a00 816d 8143 490a 5f64 6174  sgobj..m.CI._dat
+00000220: 6100 0e5f 665f 6e61 6d65 000c 5f6c 696d  a.._f_name.._lim
+00000230: 6974 000c 665f 6d6f 6465 0081 570b 822f  it..f_mode..W../
+00000240: 050b 2044 656c 6574 653a 207b 7d00 0518  .. Delete: {}...
+00000250: 6465 6275 6720 6c65 6420 7374 6570 2065  debug led step e
+00000260: 7272 6f72 3a20 7b7d 000a 0307 0231 3007  rror: {}.....10.
+00000270: 0130 0701 300a 0307 0135 0701 3507 0130  .0..0....5..5..0
+00000280: 0a03 0701 3007 0231 3007 0130 0a03 0701  ....0..10..0....
+00000290: 3007 0135 0701 350a 0307 0130 0701 3007  0..5..5....0..0.
+000002a0: 0231 300a 0307 0135 0701 3007 0135 8a3c  .10....5..0..5.<
+000002b0: 1c30 0126 2c2c 4c22 5b46 4249 8608 894e  .0.&,,L"[FBI...N
+000002c0: 840c 842f 881c 8409 8807 8051 1b02 1602  .../.......Q....
+000002d0: 8010 032a 011b 041c 0316 0359 8010 052a  ...*.......Y...*
+000002e0: 011b 061c 0516 0559 8010 072a 011b 081c  .......Y...*....
+000002f0: 0716 0759 481a 8010 0910 0a10 0b2a 031b  ...YH........*..
+00000300: 0c1c 0916 091c 0a16 0a1c 0b16 0b59 4a07  .............YJ.
+00000310: 5951 160b 4a01 5d48 0880 511b 0d16 0d4a  YQ..J.]H..Q....J
+00000320: 0759 5116 0d4a 015d 5432 0010 0e34 0216  .YQ..J.]T2...4..
+00000330: 0e32 0116 0f32 0216 1251 2a01 5333 0316  .2...2...Q*.S3..
+00000340: 1532 0416 1a51 2a01 5333 0516 1d51 2a01  .2...Q*.S3...Q*.
+00000350: 5333 0616 1e51 6307 852c 0820 0e88 1723  S3...Qc..,. ...#
+00000360: 2343 8812 6840 6840 6840 880f 113f 1640  #C..h@h@h@...?.@
+00000370: 100e 1641 5216 1051 162a 5116 2d11 4232  ...AR..Q.*Q.-.B2
+00000380: 0034 0116 2211 4232 0134 0116 2811 4232  .4..".B2.4..(.B2
+00000390: 0234 0116 2411 4232 0334 0116 2711 4232  .4..$.B2.4..'.B2
+000003a0: 0434 0116 2c11 4232 0534 0116 1151 6306  .4..,.B2.4...Qc.
+000003b0: 8540 1016 2280 1e46 2225 4d29 2e46 6912  .@.."..F"%M).Fi.
+000003c0: 0b51 de44 4251 6312 0b34 00c0 b010 23d9  .Q.DBQc..4....#.
+000003d0: 4450 120d 51de d344 4912 0e14 2436 0059  DP..Q..DI...$6.Y
+000003e0: 4266 120a 1025 3401 1025 5551 ded3 4458  Bf...%4..%UQ..DX
+000003f0: b010 26d9 4449 120e 1427 3600 5942 4712  ..&.DI...'6.YBG.
+00000400: 0e14 2836 0059 4240 5163 8148 1006 2880  ..(6.YB@Qc.H..(.
+00000410: 3012 0512 0910 2534 0112 0513 2934 0212  0.....%4....)4..
+00000420: 0e18 2a51 6381 0808 0624 8035 120d 142b  ..*Qc....$.5...+
+00000430: 3600 120e 182a 5163 8168 1808 2780 392b  6....*Qc.h..'.9+
+00000440: 1205 1209 1025 3401 3401 c012 07b0 8134  .....%4.4......4
+00000450: 0212 0e18 2a51 6383 2c18 102c 803e 8308  ....*Qc.,..,.>..
+00000460: 2827 2e32 00c0 120e 132d 51de 4447 b034  ('.2.....-Q.DG.4
+00000470: 0012 0e18 2d12 0e13 2d14 2e36 0012 0e13  ....-...-..6....
+00000480: 2a80 5612 0e13 2a14 2f36 0059 5163 0182  *.V...*./6.YQc..
+00000490: 4080 4012 3e80 3f20 2424 2424 2423 0267  @.@.>.? $$$$$#.g
+000004a0: 5923 0367 5923 0467 5923 0567 5923 0667  Y#.gY#.gY#.gY#.g
+000004b0: 5923 0767 5942 2651 6388 28b8 0220 1180  Y#.gYB&Qc.(.. ..
+000004c0: 4d60 4022 4c32 224c 2722 4e27 4d2c 484e  M`@"L2"L'"N'M,HN
+000004d0: 1249 120e 132a 1205 3402 4454 120e 132a  .I...*..4.DT...*
+000004e0: 1430 120e 132a 1430 3600 d336 0159 5263  .0...*.06..6.YRc
+000004f0: 1249 120e 132a 1207 3402 4449 120e 142c  .I...*..4.DI...,
+00000500: 3600 5950 6312 0d51 de43 5112 0e13 2a51  6.YPc..Q.CQ...*Q
+00000510: de43 4912 0d14 1136 0059 5063 4a20 5712  .CI....6.YPcJ W.
+00000520: 4adf 4459 c049 0f12 1a23 0114 20b0 3601  J.DY.I...#.. .6.
+00000530: 3401 5950 6351 51c0 2800 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
+00000540: 8248 1910 0f43 8065 2627 2623 120e 1310  .H...C.e&'&#....
+00000550: 4457 120e 1411 3600 c112 44b0 3401 59b1  DW....6...D.4.Y.
+00000560: 4447 120e 1411 3600 5951 6383 74db 021e  DG....6.YQc.t...
+00000570: 1245 461c 8071 800a 8818 424a 424c 2810  .EF..q....BJBL(.
+00000580: 132a 0153 3300 c348 09b3 b0b1 b234 0359  .*.S3..H.....4.Y
+00000590: 4a17 5948 0bb3 b0b1 b210 1434 0459 4a06  J.YH.......4.YJ.
+000005a0: 5950 634a 015d 4a01 5d52 6301 8a14 fc05  YPcJ.]J.]Rc.....
+000005b0: 2831 4b4c 4d4e 807c 4a29 5d29 494a 2627  (1KLMN.|J)])IJ&'
+000005c0: 4725 284a 48b2 9ed8 4443 9e42 41b2 c232  G%(JH...DC.BA..2
+000005d0: 0012 0334 0034 01c4 1032 1433 b480 832e  ...4.4...2.3....
+000005e0: 0255 3601 1034 f210 3514 33b4 8386 2e02  .U6..4..5.3.....
+000005f0: 5536 01f2 c512 48b1 b334 0247 4fc6 1036  U6....H..4.GO..6
+00000600: 1420 b5b0 3602 c032 01b6 1437 3600 3401  . ..6..2...76.4.
+00000610: c712 4fb7 3401 c8b7 1438 b036 0159 b614  ..O.4....8.6.Y..
+00000620: 3980 3601 59b8 b2db 4452 b7b2 d151 2e02  9.6.Y...DR...Q..
+00000630: 55c7 103a 1433 b736 01c9 4248 103a 1433  U..:.3.6..BH.:.3
+00000640: b736 01c9 b614 2fb9 3601 5951 5c5d 5163  .6..../.6.YQ\]Qc
+00000650: 0281 3841 083b 5080 7e2b 00b0 5f4b 0ac1  ..8A.;P.~+.._K..
+00000660: 1251 b134 012f 1442 3463 8178 4108 3b50  .Q.4./.B4c.xA.;P
+00000670: 8084 2b00 b05f 4b12 c110 34b1 dd44 3710  ..+.._K...4..D7.
+00000680: 32b1 dd44 31b1 2f14 422c 6386 30ca 0324  2..D1./.B,c.0..$
+00000690: 1546 4780 a060 2022 222a 2a42 4d25 4825  .FG..` ""**BM%H%
+000006a0: 5323 80c2 4847 1248 b010 1634 0247 3ac3  S#..HG.H...4.G:.
+000006b0: b314 1736 0014 1836 00c4 4269 b210 19b4  ...6...6..Bi....
+000006c0: dd44 4381 4241 80e5 c2b1 51de 4448 120f  .DC.BA....Q.DH..
+000006d0: b434 0159 4245 b1b4 3401 59b3 1417 3600  .4.YBE..4.Y...6.
+000006e0: 1418 3600 c4b4 4314 515c 5d4a 0459 4a01  ..6...C.Q\]J.YJ.
+000006f0: 5db2 6381 3831 0e1a 4580 bc60 2023 101b  ].c.81..E..` #..
+00000700: c112 12b0 b110 1c85 3482 0263 8128 a901  ........4..c.(..
+00000710: 0c1d 4780 c523 4710 1bc1 1215 b1b0 3402  ..G..#G.......4.
+00000720: c2b2 6384 1cd1 0114 1e47 80cc 2b25 2825  ..c......G..+%(%
+00000730: 4825 3200 1202 141f 3600 3401 c1b1 5f4b  H%2.....6.4..._K
+00000740: 25c2 2300 1420 b236 01c3 b051 de44 4812  %.#.. .6...Q.DH.
+00000750: 0fb3 3401 5942 45b0 b334 0159 1202 1421  ..4.YBE..4.Y...!
+00000760: b236 0159 4219 5163 0181 6049 083b 5080  .6.YB.Qc..`I.;P.
+00000770: cc2b 00b0 5f4b 0fc1 b114 3c10 3d36 0144  .+.._K....<.=6.D
+00000780: 34b1 2f14 422f 63                        4./.B/c
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files 23% similar despite different names*

```diff
@@ -3,47 +3,46 @@
 00000020: 6d00 164c 6f67 6963 616c 5069 6e73 000c  m..LogicalPins..
 00000030: 6366 6767 6574 001a 436f 6e66 6967 4861  cfgget..ConfigHa
 00000040: 6e64 6c65 7200 1a63 6f6e 736f 6c65 5f77  ndler..console_w
 00000050: 7269 7465 000a 4465 6275 6700 1865 7865  rite..Debug..exe
 00000060: 635f 6c6d 5f70 6970 6500 1654 6173 6b4d  c_lm_pipe..TaskM
 00000070: 616e 6167 6572 0010 6d65 6d5f 696e 666f  anager..mem_info
 00000080: 0081 6708 6672 6571 000e 6d61 6368 696e  ..g.freq..machin
-00000090: 6500 0316 626f 6f74 7570 5f68 6f6f 6b00  e...bootup_hook.
-000000a0: 1062 6f6f 7468 6f6f 6b00 815f 066e 2f61  .boothook.._.n/a
-000000b0: 0081 290e 626f 6f73 746d 6400 0a65 7370  ..).boostmd..esp
-000000c0: 3332 001c 7072 6f66 696c 696e 675f 696e  32..profiling_in
-000000d0: 666f 0006 6462 6700 027e 000a 6c61 6265  fo..dbg..~..labe
-000000e0: 6c00 0518 5b42 4f4f 5448 4f4f 4b5d 2045  l...[BOOTHOOK] E
-000000f0: 5845 4355 5449 4f4e 202e 2e2e 0005 167c  XECUTION ......|
-00000100: 2d5b 424f 4f54 484f 4f4b 5d20 5441 534b  -[BOOTHOOK] TASK
-00000110: 533a 207b 7d00 0511 7c2d 5b42 4f4f 5448  S: {}...|-[BOOTH
-00000120: 4f4f 4b5d 2044 4f4e 4500 0512 7c2d 5b42  OOK] DONE...|-[B
-00000130: 4f4f 5448 4f4f 4b5d 2045 5252 4f52 0005  OOTHOOK] ERROR..
-00000140: 2d5b 424f 4f54 2048 4f4f 4b53 5d20 5365  -[BOOT HOOKS] Se
-00000150: 7420 7570 2043 5055 2068 6967 6820 487a  t up CPU high Hz
-00000160: 202d 2062 6f6f 7374 6d64 3a20 7b7d 0005   - boostmd: {}..
-00000170: 2c5b 424f 4f54 2048 4f4f 4b53 5d20 5365  ,[BOOT HOOKS] Se
-00000180: 7420 7570 2043 5055 206c 6f77 2048 7a20  t up CPU low Hz 
-00000190: 2d20 626f 6f73 746d 643a 207b 7d00 051b  - boostmd: {}...
-000001a0: 7b7d 205b 5052 4f46 494c 494e 4720 494e  {} [PROFILING IN
-000001b0: 464f 5d20 2d20 7b7d 207b 7d00 862c 0818  FO] - {} {}..,..
-000001c0: 0180 132c 2c2c 2c2c 8c07 8419 8010 022a  ...,,,,,.......*
-000001d0: 011b 031c 0216 0259 8010 042a 011b 051c  .......Y...*....
-000001e0: 0416 0459 8010 062a 011b 071c 0616 0659  ...Y...*.......Y
-000001f0: 8010 082a 011b 091c 0816 0859 8010 0a2a  ...*.......Y...*
-00000200: 011b 0b1c 0a16 0a59 8010 0c2a 011b 0d1c  .......Y...*....
-00000210: 0c16 0c59 3200 160f 100e 2a01 5333 0116  ...Y2.....*.S3..
-00000220: 1651 6302 8a68 2824 0f80 2060 2027 2730  .Qc..h($.. ` ''0
-00000230: 2c27 4967 2a31 294d 3129 1206 2300 3401  ,'Ig*1)M1)..#.4.
-00000240: 5912 0410 1034 01c0 b051 ded3 446d b014  Y....4...Q..Dm..
-00000250: 1136 0010 12dc 4463 1206 2301 1413 b036  .6....Dc..#....6
-00000260: 0134 0159 1208 b034 0144 4912 0623 0234  .4.Y...4.DI..#.4
-00000270: 0159 4247 1206 2303 3401 5912 0410 1434  .YBG..#.4.Y....4
-00000280: 0152 de44 6712 0623 0414 1312 0410 1434  .R.Dg..#.......4
-00000290: 0136 0134 0159 1015 1202 3400 dd44 4b12  .6.4.Y....4..DK.
-000002a0: 0c22 80f2 b8b8 0034 0159 4265 1206 2305  .".....4.YBe..#.
-000002b0: 1413 1204 1014 3401 3601 3401 5910 1512  ......4.6.4.Y...
-000002c0: 0234 00dd 444b 120c 2280 cca5 d000 3401  .4..DK..".....4.
-000002d0: 5951 6383 38b9 0110 1619 8039 6028 3425  YQc.8......9`(4%
-000002e0: 1204 1017 3401 4462 1206 2306 1413 1018  ....4.Db..#.....
-000002f0: 85f4 b010 1885 f436 0334 0159 120a 3400  .......6.4.Y..4.
-00000300: 5912 0610 189e f434 0159 5163            Y......4.YQc
+00000090: 6500 030c 626f 6f74 7570 0010 626f 6f74  e...bootup..boot
+000000a0: 686f 6f6b 0081 5f06 6e2f 6100 8129 0e62  hook.._.n/a..).b
+000000b0: 6f6f 7374 6d64 000a 6573 7033 3200 1c70  oostmd..esp32..p
+000000c0: 726f 6669 6c69 6e67 5f69 6e66 6f00 0664  rofiling_info..d
+000000d0: 6267 0002 7e00 0a6c 6162 656c 0005 145b  bg..~..label...[
+000000e0: 424f 4f54 5d20 4558 4543 5554 494f 4e20  BOOT] EXECUTION 
+000000f0: 2e2e 2e00 0512 7c2d 5b42 4f4f 545d 2054  ......|-[BOOT] T
+00000100: 4153 4b53 3a20 7b7d 0005 0d7c 2d5b 424f  ASKS: {}...|-[BO
+00000110: 4f54 5d20 444f 4e45 0005 0e7c 2d5b 424f  OT] DONE...|-[BO
+00000120: 4f54 5d20 4552 524f 5200 052d 5b42 4f4f  OT] ERROR..-[BOO
+00000130: 5420 484f 4f4b 535d 2053 6574 2075 7020  T HOOKS] Set up 
+00000140: 4350 5520 6869 6768 2048 7a20 2d20 626f  CPU high Hz - bo
+00000150: 6f73 746d 643a 207b 7d00 052c 5b42 4f4f  ostmd: {}..,[BOO
+00000160: 5420 484f 4f4b 535d 2053 6574 2075 7020  T HOOKS] Set up 
+00000170: 4350 5520 6c6f 7720 487a 202d 2062 6f6f  CPU low Hz - boo
+00000180: 7374 6d64 3a20 7b7d 0005 1b7b 7d20 5b50  stmd: {}...{} [P
+00000190: 524f 4649 4c49 4e47 2049 4e46 4f5d 202d  ROFILING INFO] -
+000001a0: 207b 7d20 7b7d 0086 2c08 1801 8013 2c2c   {} {}..,.....,,
+000001b0: 2c2c 2c8c 0784 1980 1002 2a01 1b03 1c02  ,,,.......*.....
+000001c0: 1602 5980 1004 2a01 1b05 1c04 1604 5980  ..Y...*.......Y.
+000001d0: 1006 2a01 1b07 1c06 1606 5980 1008 2a01  ..*.......Y...*.
+000001e0: 1b09 1c08 1608 5980 100a 2a01 1b0b 1c0a  ......Y...*.....
+000001f0: 160a 5980 100c 2a01 1b0d 1c0c 160c 5932  ..Y...*.......Y2
+00000200: 0016 0f10 0e2a 0153 3301 1616 5163 028a  .....*.S3...Qc..
+00000210: 6828 240f 8020 6020 2727 302c 2749 672a  h($.. ` ''0,'Ig*
+00000220: 3129 4d31 2912 0623 0034 0159 1204 1010  1)M1)..#.4.Y....
+00000230: 3401 c0b0 51de d344 6db0 1411 3600 1012  4...Q..Dm...6...
+00000240: dc44 6312 0623 0114 13b0 3601 3401 5912  .Dc..#....6.4.Y.
+00000250: 08b0 3401 4449 1206 2302 3401 5942 4712  ..4.DI..#.4.YBG.
+00000260: 0623 0334 0159 1204 1014 3401 52de 4467  .#.4.Y....4.R.Dg
+00000270: 1206 2304 1413 1204 1014 3401 3601 3401  ..#.......4.6.4.
+00000280: 5910 1512 0234 00dd 444b 120c 2280 f2b8  Y....4..DK.."...
+00000290: b800 3401 5942 6512 0623 0514 1312 0410  ..4.YBe..#......
+000002a0: 1434 0136 0134 0159 1015 1202 3400 dd44  .4.6.4.Y....4..D
+000002b0: 4b12 0c22 80cc a5d0 0034 0159 5163 8338  K..".....4.YQc.8
+000002c0: b901 1016 1980 3960 2834 2512 0410 1734  ......9`(4%....4
+000002d0: 0144 6212 0623 0614 1310 1885 f4b0 1018  .Db..#..........
+000002e0: 85f4 3603 3401 5912 0a34 0059 1206 1018  ..6.4.Y..4.Y....
+000002f0: 9ef4 3401 5951 63                        ..4.YQc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,132 @@
-00000000: 4d06 001f 4e09 1e49 6e74 6572 436f 6e6e  M...N..InterConn
+00000000: 4d06 001f 4f09 1e49 6e74 6572 436f 6e6e  M...O..InterConn
 00000010: 6563 742e 7079 000f 1075 6173 796e 6369  ect.py...uasynci
 00000020: 6f00 1667 6574 6164 6472 696e 666f 0016  o..getaddrinfo..
 00000030: 534f 434b 5f53 5452 4541 4d00 0c73 6f63  SOCK_STREAM..soc
-00000040: 6b65 7400 0a6d 6174 6368 0004 7265 0014  ket..match..re..
-00000050: 6572 726c 6f67 5f61 6464 000a 4465 6275  errlog_add..Debu
-00000060: 6700 0c63 6667 6765 7400 1a43 6f6e 6669  g..cfgget..Confi
-00000070: 6748 616e 646c 6572 0018 536f 636b 6574  gHandler..Socket
-00000080: 5365 7276 6572 0008 5461 736b 0016 5461  Server..Task..Ta
-00000090: 736b 4d61 6e61 6765 7200 1049 6e74 6572  skManager..Inter
-000000a0: 436f 6e00 0e73 6f63 706f 7274 0012 5f73  Con..socport.._s
-000000b0: 656e 645f 636d 6400 0874 6173 6b00 1073  end_cmd..task..s
-000000c0: 656e 645f 636d 6400 1073 6c65 6570 5f6d  end_cmd..sleep_m
-000000d0: 7300 0306 6f75 7400 0c63 6f6e 2e7b 7d00  s...out..con.{}.
-000000e0: 8129 0c63 7265 6174 6500 1063 616c 6c62  .).create..callb
-000000f0: 6163 6b00 0674 6167 000e 7665 7264 6963  ack..tag..verdic
-00000100: 7400 1464 756d 705f 6361 6368 6500 1043  t..dump_cache..C
-00000110: 4f4e 4e5f 4d41 5000 230c 7265 6164 6572  ONN_MAP.#.reader
-00000120: 000c 7772 6974 6572 001a 7661 6c69 6461  ..writer..valida
-00000130: 7465 5f69 7076 3400 812d 0850 4f52 5400  te_ipv4..-.PORT.
-00000140: 0a72 6570 6c79 001e 6f70 656e 5f63 6f6e  .reply..open_con
-00000150: 6e65 6374 696f 6e00 1a5f 5f72 756e 5f63  nection..__run_c
-00000160: 6f6d 6d61 6e64 0081 0f16 7761 6974 5f63  ommand....wait_c
-00000170: 6c6f 7365 6400 0c65 6e63 6f64 6500 1c5f  losed..encode.._
-00000180: 5f72 6563 6569 7665 5f64 6174 6100 8203  _receive_data...
-00000190: 0224 0082 3182 2302 2e00 8249 0a64 7261  .$..1.#....I.dra
-000001a0: 696e 000c 7072 6f6d 7074 0002 0000 817b  in..prompt.....{
-000001b0: 0c64 6563 6f64 6500 8243 0842 7965 2100  .decode..C.Bye!.
-000001c0: 0709 0e5f 7461 6769 6679 000a 7b7d 2e7b  ..._tagify..{}.{
-000001d0: 7d00 8151 0c2e 6c6f 6361 6c00 0e61 7379  }..Q..local..asy
-000001e0: 6e63 696f 002f 2d35 8229 0868 6f73 7400  ncio./-5.).host.
-000001f0: 0663 6d64 000e 636f 6d5f 6f62 6a00 8213  .cmd..com_obj...
-00000200: 0c73 7472 5f69 6e00 7d61 1068 6f73 746e  .str_in.}a.hostn
-00000210: 616d 6500 822f 0b05 2254 6173 6b20 7374  ame../.."Task st
-00000220: 6172 7465 6420 7b7d 3a7b 7d20 2d3e 2074  arted {}:{} -> t
-00000230: 6173 6b20 7368 6f77 207b 7d00 050c 5461  ask show {}...Ta
-00000240: 736b 2069 7320 4275 7379 0005 8114 5e28  sk is Busy....^(
-00000250: 5c64 7c5b 312d 395d 5c64 7c31 5c64 5c64  \d|[1-9]\d|1\d\d
-00000260: 7c32 5b30 2d34 5d5c 647c 3235 5b30 2d35  |2[0-4]\d|25[0-5
-00000270: 5d29 5c2e 285c 647c 5b31 2d39 5d5c 647c  ])\.(\d|[1-9]\d|
-00000280: 315c 645c 647c 325b 302d 345d 5c64 7c32  1\d\d|2[0-4]\d|2
-00000290: 355b 302d 355d 295c 2e28 5c64 7c5b 312d  5[0-5])\.(\d|[1-
-000002a0: 395d 5c64 7c31 5c64 5c64 7c32 5b30 2d34  9]\d|1\d\d|2[0-4
-000002b0: 5d5c 647c 3235 5b30 2d35 5d29 5c2e 285c  ]\d|25[0-5])\.(\
-000002c0: 647c 5b31 2d39 5d5c 647c 315c 645c 647c  d|[1-9]\d|1\d\d|
-000002d0: 325b 302d 345d 5c64 7c32 355b 302d 355d  2[0-4]\d|25[0-5]
-000002e0: 2924 0005 155b 696e 7465 7263 6f6e 5d20  )$...[intercon] 
-000002f0: 4e6f 486f 7374 3a20 7b7d 0005 205b 696e  NoHost: {}.. [in
-00000300: 7465 7263 6f6e 5d20 7365 6e64 5f63 6d64  tercon] send_cmd
-00000310: 207b 7d20 6f73 6572 723a 207b 7d00 0520   {} oserr: {}.. 
-00000320: 5b69 6e74 6572 636f 6e5d 5b45 5252 5d20  [intercon][ERR] 
-00000330: 496e 7661 6c69 6420 686f 7374 3a20 7b7d  Invalid host: {}
-00000340: 0005 1843 6f6e 6e65 6374 696f 6e20 6973  ...Connection is
-00000350: 2062 7573 792e 2042 7965 2100 0534 5b69   busy. Bye!..4[i
-00000360: 6e74 6572 636f 6e5d 2070 726f 6d70 7420  ntercon] prompt 
-00000370: 6d69 736d 6174 6368 2c20 686f 7374 6e61  mismatch, hostna
-00000380: 6d65 3a20 7b7d 2070 726f 6d70 743a 207b  me: {} prompt: {
-00000390: 7d20 0005 0b5b 636f 6e66 6967 7572 655d  } ...[configure]
-000003a0: 0087 5c10 1c01 2632 2c2c 2c2c 6c89 7484  ..\...&2,,,,l.t.
-000003b0: 1484 1b80 511b 0216 3f80 1003 1004 2a02  ....Q...?.....*.
-000003c0: 1b05 1c03 1603 1c04 1604 5980 1006 2a01  ..........Y...*.
-000003d0: 1b07 1c06 1606 5980 1008 2a01 1b09 1c08  ......Y...*.....
-000003e0: 1608 5980 100a 2a01 1b0b 1c0a 160a 5980  ..Y...*.......Y.
-000003f0: 100c 2a01 1b0c 1c0c 160c 5980 100d 2a01  ..*.......Y...*.
-00000400: 1b0e 1c0d 160d 5954 3200 100f 3402 160f  ......YT2...4...
-00000410: 3201 1611 3202 1613 3203 161d 5163 0484  2...2...2...Qc..
-00000420: 0c08 1a0f 880a 2448 6440 8807 8432 8419  ......$Hd@...2..
-00000430: 1140 1641 100f 1642 2c00 161e 110a 1010  .@.A...B,.......
-00000440: 3401 1624 3200 161f 1143 3201 3401 1622  4..$2....C2.4.."
-00000450: 3202 1613 3203 1627 512a 0153 3304 162b  2...2..'Q*.S3..+
-00000460: 5163 0581 4811 0c1f 4780 0e24 2451 b018  Qc..H...G..$$Q..
-00000470: 2051 b018 2112 0d34 00b0 1812 5163 8160   Q..!..4....Qc.`
-00000480: 290e 2248 8014 232c 2223 02c1 1249 1206  )."H..#,"#...I..
-00000490: b1b0 3402 3401 4442 5263 5063 9318 f742  ..4.4.DBRcPc...B
-000004a0: 4213 4744 4580 1a80 0742 2a42 2f22 2d53  B.GDE....B*B/"-S
-000004b0: 2e2d 6e47 2a44 5656 2e2d 4c25 286c 464f  .-nG*DVV.-L%(lFO
-000004c0: 422c 51c3 120f 1422 b136 0143 e380 b1c3  B,Q....".6.C....
-000004d0: 120f 131e 1423 b351 3602 51de 44cb 8048  .....#.Q6.Q.D..H
-000004e0: 1712 03b1 120f 1324 8012 0434 04c4 b47f  .......$...4....
-000004f0: 5584 5580 55c1 4a30 5712 4adf 4469 c549  U.U.U.J0W.J.Di.I
-00000500: 1f12 0c14 2523 0314 18b5 3601 3601 5912  ....%#....6.6.Y.
-00000510: 0823 0414 18b1 b536 0234 0159 1015 6351  .#.....6.4.Y..cQ
-00000520: 51c5 2805 5d4a 015d 4247 120f 131e b355  Q.(.]J.]BG.....U
-00000530: c112 0f14 22b1 3601 4487 8149 5548 2312  ....".6.D..IUH#.
-00000540: 3f14 26b1 120f 1324 3602 5e51 6830 02b0  ?.&....$6.^Qh0..
-00000550: 1820 b018 21b0 1427 b2b3 3602 5e51 68c6  . ..!..'..6.^Qh.
-00000560: 4a2f 5712 4adf 4468 c549 1e12 0c14 2523  J/W.J.Dh.I....%#
-00000570: 0314 18b5 3601 3601 5912 0823 0414 18b1  ....6.6.Y..#....
-00000580: b536 0234 0159 51c6 5151 c528 055d 4a01  .6.4.YQ.QQ.(.]J.
-00000590: 5d51 b013 2144 53b0 1321 1428 3600 59b0  ]Q..!DS..!.(6.Y.
-000005a0: 1321 1429 3600 5e51 6859 5db3 51de d344  .!.)6.^QhY].Q..D
-000005b0: 4fb6 51de 4443 5142 41b1 120f 131e b356  O.Q.DCQBA......V
-000005c0: b663 1208 2305 1418 b136 0134 0159 1015  .c..#....6.4.Y..
-000005d0: 6389 70db 402a 2747 454b 804c 6060 282c  c.p.@*'GEK.L``(,
-000005e0: 2642 1f4c 292b 3026 4242 2f12 4c14 2ab1  &B.L)+0&BB/.L.*.
-000005f0: 3601 c1b0 142b 3600 5e51 6830 02c3 c423  6....+6.^Qh0...#
-00000600: 06b4 dd44 4251 63b2 51de 4366 b451 de43  ...DBQc.Q.Cf.Q.C
-00000610: 6112 4cb4 3401 142c 102d 1015 3602 142e  a.L.4..,.-..6...
-00000620: 3600 124c b234 0114 2f10 3036 0180 55d9  6..L.4../.06..U.
-00000630: 446e b013 2114 31b1 3601 59b0 1321 1432  Dn..!.1.6.Y..!.2
-00000640: 3600 5e51 6859 b014 2b10 33b4 3682 005e  6.^QhY..+.3.6..^
-00000650: 5168 3002 c3c5 b310 34d9 4442 5163 b363  Qh0.....4.DBQc.c
-00000660: 120c 1425 2307 1418 b2b4 3602 3601 5951  ...%#.....6.6.YQ
-00000670: 6388 78ce 4128 2b47 3380 6560 2043 2022  c.x.A(+G3.e` C "
-00000680: 2e23 244c 2e44 354c 2931 1015 c248 4db0  .#$L.D5L)1...HM.
-00000690: 1320 1435 2281 0036 015e 5168 c3b3 4344  . .5"..6.^Qh..CD
-000006a0: 40c9 8001 b314 3610 3736 0114 2e36 00c3  @.....6.76...6..
-000006b0: b151 de44 47b3 142e 3600 4241 b1c1 b2b3  .Q.DG...6.BA....
-000006c0: e5c2 b1b2 142e 3600 dd43 4c23 08b2 dd43  ......6..CL#...C
-000006d0: 4610 38b3 dd44 4340 5301 4a0d 5712 4adf  F.8..DC@S.J.W.J.
-000006e0: 4446 5940 4701 4a01 5d42 a17f b214 2cb1  DFY@G.J.]B....,.
-000006f0: 1015 3602 142c 1039 103a 3602 c2b2 b12a  ..6..,.9.:6....*
-00000700: 0263 8738 cf40 2211 4445 4680 7e80 0726  .c.8.@".DEF.~..&
-00000710: 2b25 2d2b 252d 2b32 b213 1247 5659 b214  +%-+%-+2...GVY..
-00000720: 13b0 b136 025e 5168 c3b3 51de 4475 123f  ...6.^Qh..Q.Du.?
-00000730: 1414 2281 1636 015e 5168 59b2 1413 b0b1  .."..6.^QhY.....
-00000740: 3602 5e51 68c3 b351 de44 5812 3f14 1422  6.^Qh..Q.DX.?.."
-00000750: 8116 3601 5e51 6859 b214 13b0 b136 025e  ..6.^QhY.....6.^
-00000760: 5168 c3b3 51de 4444 1015 4241 b3b2 1312  Qh..Q.DD..BA....
-00000770: 1816 515c 5db2 1312 1316 6386 446a 9e01  ..Q\].....c.Dj..
-00000780: 1344 4580 9280 0986 0725 2a37 2357 2c00  .DE......%*7#W,.
-00000790: 01b0 b120 0002 c212 0f34 00c3 1017 1418  ... .....4......
-000007a0: b234 0036 01c4 b313 1214 1910 1a12 1125  .4.6...........%
-000007b0: 0025 01b3 3403 101b b436 8400 c5b5 4457  .%..4....6....DW
-000007c0: 2c02 2300 1418 2500 2501 b436 0310 1c62  ,.#...%.%..6...b
-000007d0: b410 1b62 c642 4c2c 0223 0110 1c62 b410  ...b.BL,.#...b..
-000007e0: 1b62 c6b6 6301 8508 4a12 3b4d 4d80 9c20  .b..c...J.;MM.. 
-000007f0: 2f2a 3b25 0114 2f10 3a36 0180 5514 2e36  /*;%../.:6..U..6
-00000800: 00c2 120f 1422 2500 3601 445b 103c 1418  ....."%.6.D[.<..
-00000810: 1030 143d 2500 142f 1030 3601 7e51 2e02  .0.=%../.06.~Q..
-00000820: 5536 01b2 3602 6310 3c14 1825 0014 2c10  U6..6.c.<..%..,.
-00000830: 3e10 1536 02b2 3602 6358 0008 1d80 ad60  >..6..6.cX.....`
-00000840: 120f 131e 63                             ....c
+00000040: 6b65 7400 0e63 6f6d 7069 6c65 0004 7265  ket..compile..re
+00000050: 0014 6572 726c 6f67 5f61 6464 000a 4465  ..errlog_add..De
+00000060: 6275 6700 0c63 6667 6765 7400 1a43 6f6e  bug..cfgget..Con
+00000070: 6669 6748 616e 646c 6572 0018 536f 636b  figHandler..Sock
+00000080: 6574 5365 7276 6572 0008 5461 736b 0016  etServer..Task..
+00000090: 5461 736b 4d61 6e61 6765 7200 1049 6e74  TaskManager..Int
+000000a0: 6572 436f 6e00 0e73 6f63 706f 7274 0012  erCon..socport..
+000000b0: 5f73 656e 645f 636d 6400 0874 6173 6b00  _send_cmd..task.
+000000c0: 1073 656e 645f 636d 6400 1073 6c65 6570  .send_cmd..sleep
+000000d0: 5f6d 7300 0306 6f75 7400 0c63 6f6e 2e7b  _ms...out..con.{
+000000e0: 7d00 8129 0c63 7265 6174 6500 1063 616c  }..).create..cal
+000000f0: 6c62 6163 6b00 0674 6167 000e 7665 7264  lback..tag..verd
+00000100: 6963 7400 1464 756d 705f 6361 6368 6500  ict..dump_cache.
+00000110: 1043 4f4e 4e5f 4d41 5000 230c 7265 6164  .CONN_MAP.#.read
+00000120: 6572 000c 7772 6974 6572 001a 7661 6c69  er..writer..vali
+00000130: 6461 7465 5f69 7076 3400 0a6d 6174 6368  date_ipv4..match
+00000140: 0081 2d08 504f 5254 000a 7265 706c 7900  ..-.PORT..reply.
+00000150: 1e6f 7065 6e5f 636f 6e6e 6563 7469 6f6e  .open_connection
+00000160: 001a 5f5f 7275 6e5f 636f 6d6d 616e 6400  ..__run_command.
+00000170: 810f 1677 6169 745f 636c 6f73 6564 000c  ...wait_closed..
+00000180: 656e 636f 6465 001c 5f5f 7265 6365 6976  encode..__receiv
+00000190: 655f 6461 7461 0082 0302 2400 8231 8223  e_data....$..1.#
+000001a0: 022e 0082 490a 6472 6169 6e00 0c70 726f  ....I.drain..pro
+000001b0: 6d70 7400 0200 0081 7b0c 6465 636f 6465  mpt.....{.decode
+000001c0: 0082 4308 4279 6521 0007 090e 5f74 6167  ..C.Bye!...._tag
+000001d0: 6966 7900 0a7b 7d2e 7b7d 0081 510c 2e6c  ify..{}.{}..Q..l
+000001e0: 6f63 616c 000e 6173 796e 6369 6f00 2f2d  ocal..asyncio./-
+000001f0: 3582 2908 686f 7374 0006 636d 6400 0e63  5.).host..cmd..c
+00000200: 6f6d 5f6f 626a 0082 130c 7374 725f 696e  om_obj....str_in
+00000210: 007d 6110 686f 7374 6e61 6d65 0082 2f0b  .}a.hostname../.
+00000220: 051a 5461 736b 2073 7461 7274 6564 3a20  ..Task started: 
+00000230: 7461 736b 2073 686f 7720 7b7d 0005 0c54  task show {}...T
+00000240: 6173 6b20 6973 2042 7573 7900 0581 145e  ask is Busy....^
+00000250: 285c 647c 5b31 2d39 5d5c 647c 315c 645c  (\d|[1-9]\d|1\d\
+00000260: 647c 325b 302d 345d 5c64 7c32 355b 302d  d|2[0-4]\d|25[0-
+00000270: 355d 295c 2e28 5c64 7c5b 312d 395d 5c64  5])\.(\d|[1-9]\d
+00000280: 7c31 5c64 5c64 7c32 5b30 2d34 5d5c 647c  |1\d\d|2[0-4]\d|
+00000290: 3235 5b30 2d35 5d29 5c2e 285c 647c 5b31  25[0-5])\.(\d|[1
+000002a0: 2d39 5d5c 647c 315c 645c 647c 325b 302d  -9]\d|1\d\d|2[0-
+000002b0: 345d 5c64 7c32 355b 302d 355d 295c 2e28  4]\d|25[0-5])\.(
+000002c0: 5c64 7c5b 312d 395d 5c64 7c31 5c64 5c64  \d|[1-9]\d|1\d\d
+000002d0: 7c32 5b30 2d34 5d5c 647c 3235 5b30 2d35  |2[0-4]\d|25[0-5
+000002e0: 5d29 2400 0515 5b69 6e74 6572 636f 6e5d  ])$...[intercon]
+000002f0: 204e 6f48 6f73 743a 207b 7d00 0520 5b69   NoHost: {}.. [i
+00000300: 6e74 6572 636f 6e5d 2073 656e 645f 636d  ntercon] send_cm
+00000310: 6420 7b7d 206f 7365 7272 3a20 7b7d 0005  d {} oserr: {}..
+00000320: 205b 696e 7465 7263 6f6e 5d5b 4552 525d   [intercon][ERR]
+00000330: 2049 6e76 616c 6964 2068 6f73 743a 207b   Invalid host: {
+00000340: 7d00 0518 436f 6e6e 6563 7469 6f6e 2069  }...Connection i
+00000350: 7320 6275 7379 2e20 4279 6521 0005 345b  s busy. Bye!..4[
+00000360: 696e 7465 7263 6f6e 5d20 7072 6f6d 7074  intercon] prompt
+00000370: 206d 6973 6d61 7463 682c 2068 6f73 746e   mismatch, hostn
+00000380: 616d 653a 207b 7d20 7072 6f6d 7074 3a20  ame: {} prompt: 
+00000390: 7b7d 2000 050b 5b63 6f6e 6669 6775 7265  {} ...[configure
+000003a0: 5d00 875c 101c 0126 322c 2c2c 2c6c 8972  ]..\...&2,,,,l.r
+000003b0: 8414 8417 8051 1b02 1640 8010 0310 042a  .....Q...@.....*
+000003c0: 021b 051c 0316 031c 0416 0459 8010 062a  ...........Y...*
+000003d0: 011b 071c 0616 0659 8010 082a 011b 091c  .......Y...*....
+000003e0: 0816 0859 8010 0a2a 011b 0b1c 0a16 0a59  ...Y...*.......Y
+000003f0: 8010 0c2a 011b 0c1c 0c16 0c59 8010 0d2a  ...*.......Y...*
+00000400: 011b 0e1c 0d16 0d59 5432 0010 0f34 0216  .......YT2...4..
+00000410: 0f32 0116 1132 0216 1332 0316 1d51 6304  .2...2...2...Qc.
+00000420: 840c 081a 0f88 0a24 4864 4068 4084 3284  .......$Hd@h@.2.
+00000430: 1911 4116 4210 0f16 432c 0016 1e11 0a10  ..A.B...C,......
+00000440: 1034 0116 2532 0016 1f11 4432 0134 0116  .4..%2....D2.4..
+00000450: 2232 0216 1332 0316 2851 2a01 5333 0416  "2...2..(Q*.S3..
+00000460: 2c51 6305 8148 110c 1f48 800e 2424 51b0  ,Qc..H...H..$$Q.
+00000470: 1820 51b0 1821 120d 3400 b018 1251 6381  . Q..!..4....Qc.
+00000480: 4829 0a22 4980 1427 1206 2302 3401 c112  H)."I..'..#.4...
+00000490: 4ab1 1423 b036 0134 0163 9318 f742 4213  J..#.6.4.c...BB.
+000004a0: 4845 4680 1880 0742 2a42 2f22 2d53 2e2d  HEF....B*B/"-S.-
+000004b0: 6e47 2a44 5656 2e2d 4c25 286c 464f 422c  nG*DVV.-L%(lFOB,
+000004c0: 51c3 120f 1422 b136 0143 e380 b1c3 120f  Q....".6.C......
+000004d0: 131e 1424 b351 3602 51de 44cb 8048 1712  ...$.Q6.Q.D..H..
+000004e0: 03b1 120f 1325 8012 0434 04c4 b47f 5584  .....%...4....U.
+000004f0: 5580 55c1 4a30 5712 4bdf 4469 c549 1f12  U.U.J0W.K.Di.I..
+00000500: 0c14 2623 0314 18b5 3601 3601 5912 0823  ..&#....6.6.Y..#
+00000510: 0414 18b1 b536 0234 0159 1015 6351 51c5  .....6.4.Y..cQQ.
+00000520: 2805 5d4a 015d 4247 120f 131e b355 c112  (.]J.]BG.....U..
+00000530: 0f14 22b1 3601 4487 8149 5548 2312 4014  ..".6.D..IUH#.@.
+00000540: 27b1 120f 1325 3602 5e51 6830 02b0 1820  '....%6.^Qh0... 
+00000550: b018 21b0 1428 b2b3 3602 5e51 68c6 4a2f  ..!..(..6.^Qh.J/
+00000560: 5712 4bdf 4468 c549 1e12 0c14 2623 0314  W.K.Dh.I....&#..
+00000570: 18b5 3601 3601 5912 0823 0414 18b1 b536  ..6.6.Y..#.....6
+00000580: 0234 0159 51c6 5151 c528 055d 4a01 5d51  .4.YQ.QQ.(.]J.]Q
+00000590: b013 2144 53b0 1321 1429 3600 59b0 1321  ..!DS..!.)6.Y..!
+000005a0: 142a 3600 5e51 6859 5db3 51de d344 4fb6  .*6.^QhY].Q..DO.
+000005b0: 51de 4443 5142 41b1 120f 131e b356 b663  Q.DCQBA......V.c
+000005c0: 1208 2305 1418 b136 0134 0159 1015 6389  ..#....6.4.Y..c.
+000005d0: 70db 402a 2848 464c 804a 6060 282c 2642  p.@*(HFL.J``(,&B
+000005e0: 1f4c 292b 3026 4242 2f12 4d14 2bb1 3601  .L)+0&BB/.M.+.6.
+000005f0: c1b0 142c 3600 5e51 6830 02c3 c423 06b4  ...,6.^Qh0...#..
+00000600: dd44 4251 63b2 51de 4366 b451 de43 6112  .DBQc.Q.Cf.Q.Ca.
+00000610: 4db4 3401 142d 102e 1015 3602 142f 3600  M.4..-....6../6.
+00000620: 124d b234 0114 3010 3136 0180 55d9 446e  .M.4..0.16..U.Dn
+00000630: b013 2114 32b1 3601 59b0 1321 1433 3600  ..!.2.6.Y..!.36.
+00000640: 5e51 6859 b014 2c10 34b4 3682 005e 5168  ^QhY..,.4.6..^Qh
+00000650: 3002 c3c5 b310 35d9 4442 5163 b363 120c  0.....5.DBQc.c..
+00000660: 1426 2307 1418 b2b4 3602 3601 5951 6388  .&#.....6.6.YQc.
+00000670: 78ce 4128 2c48 3480 6360 2043 2022 2e23  x.A(,H4.c` C ".#
+00000680: 244c 2e44 354c 2931 1015 c248 4db0 1320  $L.D5L)1...HM.. 
+00000690: 1436 2281 0036 015e 5168 c3b3 4344 40c9  .6"..6.^Qh..CD@.
+000006a0: 8001 b314 3710 3836 0114 2f36 00c3 b151  ....7.86../6...Q
+000006b0: de44 47b3 142f 3600 4241 b1c1 b2b3 e5c2  .DG../6.BA......
+000006c0: b1b2 142f 3600 dd43 4c23 08b2 dd43 4610  .../6..CL#...CF.
+000006d0: 39b3 dd44 4340 5301 4a0d 5712 4bdf 4446  9..DC@S.J.W.K.DF
+000006e0: 5940 4701 4a01 5d42 a17f b214 2db1 1015  Y@G.J.]B....-...
+000006f0: 3602 142d 103a 103b 3602 c2b2 b12a 0263  6..-.:.;6....*.c
+00000700: 8738 cf40 2211 4546 4780 7c80 0726 2b25  .8.@".EFG.|..&+%
+00000710: 2d2b 252d 2b32 b213 1247 5659 b214 13b0  -+%-+2...GVY....
+00000720: b136 025e 5168 c3b3 51de 4475 1240 1414  .6.^Qh..Q.Du.@..
+00000730: 2281 1636 015e 5168 59b2 1413 b0b1 3602  "..6.^QhY.....6.
+00000740: 5e51 68c3 b351 de44 5812 4014 1422 8116  ^Qh..Q.DX.@.."..
+00000750: 3601 5e51 6859 b214 13b0 b136 025e 5168  6.^QhY.....6.^Qh
+00000760: c3b3 51de 4444 1015 4241 b3b2 1312 1816  ..Q.DD..BA......
+00000770: 515c 5db2 1312 1316 6386 246a 9e01 1345  Q\].....c.$j...E
+00000780: 4680 9060 4086 0725 2a37 2353 2c00 01b0  F..`@..%*7#S,...
+00000790: b120 0002 c212 0f34 00c3 1017 1418 b234  . .....4.......4
+000007a0: 0036 01c4 b313 1214 1910 1a12 1125 0025  .6...........%.%
+000007b0: 01b3 3403 101b b436 8400 c5b5 4453 2c02  ..4....6....DS,.
+000007c0: 2300 1418 b436 0110 1c62 b410 1b62 c642  #....6...b...b.B
+000007d0: 4c2c 0223 0110 1c62 b410 1b62 c6b6 6301  L,.#...b...b..c.
+000007e0: 8508 4a12 3c4e 4e80 9620 2f2a 3b25 0114  ..J.<NN.. /*;%..
+000007f0: 3010 3b36 0180 5514 2f36 00c2 120f 1422  0.;6..U./6....."
+00000800: 2500 3601 445b 103d 1418 1031 143e 2500  %.6.D[.=...1.>%.
+00000810: 1430 1031 3601 7e51 2e02 5536 01b2 3602  .0.16.~Q..U6..6.
+00000820: 6310 3d14 1825 0014 2d10 3f10 1536 02b2  c.=..%..-.?..6..
+00000830: 3602 6358 0008 1d80 a760 120f 131e 63    6.cX.....`....c
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 00000020: 7464 6972 0004 6f73 000e 6d6f 6475 6c65  tdir..os..module
 00000030: 7300 0673 7973 000c 6366 6767 6574 000c  s..sys..cfgget..
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
-00000090: 7567 000a 7265 7365 7400 0e6d 6163 6869  ug..reset..machi
-000000a0: 6e65 000a 5368 656c 6c00 1031 2e31 392e  ne..Shell..1.19.
-000000b0: 302d 3000 230e 6d73 675f 6f62 6a00 0c64  0-0.#.msg_obj..d
-000000c0: 6576 6669 6400 105f 5f64 6576 6669 6400  evfid..__devfid.
-000000d0: 0861 7574 6800 165f 5f61 7574 685f 6d6f  .auth..__auth_mo
-000000e0: 6465 000a 6877 7569 6400 0e5f 5f68 7775  de..hwuid..__hwu
-000000f0: 6964 0012 5f5f 6175 7468 5f6f 6b00 165f  id..__auth_ok.._
-00000100: 5f63 6f6e 665f 6d6f 6465 000e 7665 7273  _conf_mode..vers
-00000110: 696f 6e00 1c4d 4943 524f 535f 5645 5253  ion..MICROS_VERS
-00000120: 494f 4e00 8129 066d 7367 000c 7265 626f  ION..).msg..rebo
-00000130: 6f74 000e 5b48 4152 445d 2000 0308 4279  ot..[HARD] ...By
-00000140: 6521 0014 736f 6674 5f72 6573 6574 000c  e!..soft_reset..
+00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
+000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
+000000b0: 5368 656c 6c00 1031 2e32 302e 302d 3000  Shell..1.20.0-0.
+000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
+000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
+000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
+000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
+00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
+00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
+00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
+00000130: 8129 066d 7367 000c 7265 626f 6f74 000e  .).msg..reboot..
+00000140: 5b48 4152 445d 2000 0308 4279 6521 000c  [HARD] ...Bye!..
 00000150: 7072 6f6d 7074 0012 7b7d 7b7d 7b7d 2024  prompt..{}{}{} $
 00000160: 2000 205f 5f61 7574 6865 6e74 6963 6174   . __authenticat
 00000170: 696f 6e00 0a61 7070 7764 0082 310c 4175  ion..appwd..1.Au
 00000180: 7468 4f6b 000a 7368 656c 6c00 0e5f 5f73  thOk..shell..__s
 00000190: 6865 6c6c 0082 230a 6865 6c6c 6f00 042d  hell..#.hello..-
 000001a0: 6800 8227 0e77 6562 7265 706c 0004 2d75  h..'.webrepl..-u
 000001b0: 0082 3f08 636f 6e66 000c 6e6f 636f 6e66  ..?.conf..noconf
@@ -129,134 +129,133 @@
 00000800: 7274 206e 6f64 6520 7468 656e 2073 7461  rt node then sta
 00000810: 7274 2077 6562 7265 706c 2e2e 2e00 0520  rt webrepl..... 
 00000820: 5b45 5252 5d20 7768 696c 6520 7374 6172  [ERR] while star
 00000830: 7469 6e67 2077 6562 7265 706c 3a20 7b7d  ting webrepl: {}
 00000840: 0005 0f6d 6963 724f 5369 7354 6865 4265  ...micrOSisTheBe
 00000850: 7374 0005 1f5b 7b7d 5d20 5348 4f57 204c  st...[{}] SHOW L
 00000860: 4d20 5041 5253 4552 2057 4152 4e49 4e47  M PARSER WARNING
-00000870: 3a20 7b7d 0086 5c10 1401 800d 2c2c 322c  : {}..\.....,,2,
-00000880: 328c 0780 1002 2a01 1b03 1c02 1602 5980  2.....*.......Y.
-00000890: 1004 2a01 1b05 1c04 1604 5980 1006 1007  ..*.......Y.....
-000008a0: 2a02 1b08 1c06 1606 1c07 1607 5980 1009  *...........Y...
-000008b0: 2a01 1b0a 1c09 1609 5980 100b 100c 2a02  *.......Y.....*.
-000008c0: 1b0d 1c0b 160b 1c0c 160c 5980 100e 2a01  ..........Y...*.
-000008d0: 1b0f 1c0e 165e 5954 3200 1010 3402 1610  .....^YT2...4...
-000008e0: 5163 0187 0410 3010 881a 4488 1484 0764  Qc....0...D....d
-000008f0: 4088 0964 6084 0e84 0984 6a88 258c 2111  @..d`.....j.%.!.
-00000900: 5f16 6010 1016 6110 1116 1d51 2a01 5333  _.`...a....Q*.S3
-00000910: 0016 1232 0116 1f32 0216 0e50 2a01 5333  ...2...2...P*.S3
-00000920: 0316 2032 0416 2532 0516 2732 0616 2b32  .. 2..%2..'2..+2
-00000930: 0716 2c11 6232 0834 0116 3a11 6250 2a01  ..,.b2.4..:.bP*.
-00000940: 5333 0934 0116 3811 6250 2a01 5333 0a34  S3.4..8.bP*.S3.4
-00000950: 0116 3151 630b 8728 ca03 2012 5813 801d  ..1Qc..(.. .X...
-00000960: 6020 4429 2949 2444 2256 2cb1 b018 1312  ` D))I$D"V,.....
-00000970: 0610 1434 01b0 1815 1206 1016 3401 b018  ...4........4...
-00000980: 1712 0610 1834 01b0 1819 50b0 181a 50b0  .....4....P...P.
-00000990: 181b 480d 1207 101c 1210 131d 3402 594a  ..H.........4.YJ
-000009a0: 2a57 1263 df44 63c2 4919 120b 2300 141e  *W.c.Dc.I...#...
-000009b0: b236 0134 0159 120c 2301 141e b236 0134  .6.4.Y..#....6.4
-000009c0: 0159 5151 c228 025d 4a01 5d51 6382 0836  .YQQ.(.]J.]Qc..6
-000009d0: 101f 581f 8031 2022 4a48 09b0 1413 b136  ..X..1 "JH.....6
-000009e0: 0159 4a0a 5912 64b1 3401 594a 015d 5163  .YJ.Y.d.4.YJ.]Qc
-000009f0: 8110 110c 0e58 8038 2024 50b0 181a 50b0  .....X.8 $P...P.
-00000a00: 181b 5163 8420 ba01 1620 5865 803d 2035  ..Qc. ... Xe.= 5
-00000a10: 2823 252b b014 1f23 0214 1eb1 4444 1021  (#%+...#....DD.!
-00000a20: 4242 1022 3601 3601 59b0 141f 1023 3601  BB."6.6.Y....#6.
-00000a30: 59b1 4445 125e 3400 5980 1024 2a01 1b0f  Y.DE.^4.Y..$*...
-00000a40: 1c24 c259 b234 0059 5163 8310 390e 2558  .$.Y.4.YQc..9.%X
-00000a50: 8046 2031 2cb0 1317 4449 b013 1a43 4423  .F 1,...DI...CD#
-00000a60: 0342 4210 22c1 b013 1b44 4423 0442 4210  .BB."....DD#.BB.
-00000a70: 22c2 1026 141e b1b2 b013 1536 0363 8508  "..&.......6.c..
-00000a80: 2a1c 2758 6680 4c40 4a27 2b24 2826 2826  *.'Xf.L@J'+$(&(&
-00000a90: b013 1744 77b0 131a 4372 1206 1028 3401  ...Dw...Cr...(4.
-00000aa0: c2b2 b180 5514 2936 00d9 4452 52b0 181a  ....U.)6..DRR...
-00000ab0: b014 1f10 2a36 0159 522b 002a 0263 b014  ....*6.YR+.*.c..
-00000ac0: 1f23 0536 0159 502b 002a 0263 52b1 2a02  .#.6.YP+.*.cR.*.
-00000ad0: 6381 7832 122b 581f 805a 6020 272b b014  c.x2.+X..Z` '+..
-00000ae0: 2cb1 3601 c2b0 141f b014 2536 0036 0159  ,.6.......%6.6.Y
-00000af0: b263 a400 ea02 8602 2c58 1f80 6380 0b52  .c......,X..c..R
-00000b00: 228a 0848 3242 2a23 2229 6248 2e62 2822  "..H2B*#")bH.b("
-00000b10: 5122 472b 3130 6d2b 2422 2b24 6229 2828  Q"G+10m+$"+$b)((
-00000b20: 2828 2828 2828 2828 2828 2828 2828 2828  ((((((((((((((((
-00000b30: 2a2d 7020 4e4b 6040 4259 2db1 51de 434d  *-p NK`@BY-.Q.CM
-00000b40: 1267 b114 2936 0034 0180 d944 4252 63b1  .g..)6.4...DBRc.
-00000b50: 1429 3600 142d 3600 c2b2 8055 102e d944  .)6..-6....U...D
-00000b60: 54b0 141f 2306 141e b013 15b0 1319 3602  T...#.........6.
-00000b70: 3601 5952 63b0 1427 b236 0130 02c3 c2b3  6.YRc..'.6.0....
-00000b80: 4342 5063 1267 b234 0180 d944 4252 63b2  CBPc.g.4...DBRc.
-00000b90: 8055 101c d944 50b0 141f 1268 1210 131d  .U...DP....h....
-00000ba0: 3401 3601 5952 63b2 8055 1020 d944 5c50  4.6.YRc..U. .D\P
-00000bb0: c412 67b2 3401 82db 444a 102f b281 55dd  ..g.4...DJ./..U.
-00000bc0: 4442 52c4 b014 20b4 3601 59b2 8055 1430  DBR... .6.Y..U.0
-00000bd0: 1031 3601 446e 1267 b234 0182 d944 5810  .16.Dn.g.4...DX.
-00000be0: 32b2 8155 dd44 5012 1014 3110 13b0 131f  2..U.DP...1.....
-00000bf0: 1033 5236 8400 5912 1014 3110 13b0 131f  .3R6..Y...1.....
-00000c00: 3682 0059 b280 5514 3010 3436 0144 4652  6..Y..U.0.46.DFR
-00000c10: b018 1b52 63b2 8055 1430 1035 3601 4446  ...Rc..U.0.56.DF
-00000c20: 50b0 181b 5263 b280 5510 36d9 44b7 81b0  P...Rc..U.6.D...
-00000c30: 141f 2307 3601 59b0 141f 2308 3601 59b0  ..#.6.Y...#.6.Y.
-00000c40: 141f 2309 3601 59b0 141f 230a 3601 59b0  ..#.6.Y...#.6.Y.
-00000c50: 141f 230b 3601 59b0 141f 230c 3601 59b0  ..#.6.Y...#.6.Y.
-00000c60: 141f 230d 3601 59b0 141f 230e 3601 59b0  ..#.6.Y...#.6.Y.
-00000c70: 141f 230f 3601 59b0 141f 2310 3601 59b0  ..#.6.Y...#.6.Y.
-00000c80: 141f 2311 3601 59b0 141f 2312 3601 59b0  ..#.6.Y...#.6.Y.
-00000c90: 141f 2313 3601 59b0 141f 2314 3601 59b0  ..#.6.Y...#.6.Y.
-00000ca0: 141f 2315 3601 59b0 141f 2316 3601 59b0  ..#.6.Y...#.6.Y.
-00000cb0: 141f 2317 3601 59b0 141f 2318 3601 5910  ..#.6.Y...#.6.Y.
-00000cc0: 3712 68b2 3401 dd44 4d12 1014 3810 13b0  7.h.4..DM...8...
-00000cd0: 131f 3682 0063 1210 1438 1013 b013 1f10  ..6..c...8......
-00000ce0: 3952 3684 0063 b013 1b44 5412 67b2 3401  9R6..c...DT.g.4.
-00000cf0: 80d8 444b 1210 143a b013 1fb2 3602 6348  ..DK...:....6.cH
-00000d00: 1012 0910 3bb2 103c b013 1f34 8400 634a  ....;..<...4..cJ
-00000d10: 2157 1263 df44 5ac5 4910 b014 1f23 1914  !W.c.DZ.I....#..
-00000d20: 1eb5 3601 3601 5950 6351 51c5 2805 5d4a  ..6.6.YPcQQ.(.]J
-00000d30: 015d 5163 8d00 9212 303a 1369 80ce 6060  .]Qc....0:.i..``
-00000d40: 2a48 2f28 3642 2b42 4a24 4d22 562b 4b30  *H/(6B+BJ$M"V+K0
-00000d50: 2c12 67b1 3401 81d9 44c4 80b1 8055 103d  ,.g.4...D....U.=
-00000d60: d944 6f12 0634 0014 3e36 005f 4b22 3002  .Do..4..>6._K"0.
-00000d70: c2c3 8a12 67b2 3401 f3c4 b023 1a14 1eb2  ....g.4....#....
-00000d80: 103f b4f4 103f 87f4 b336 0434 0159 421c  .?...?...6.4.YB.
-00000d90: 5263 b012 06b1 8055 3401 3401 5952 6312  Rc.....U4.4.YRc.
-00000da0: 67b1 3401 82db 44db 80b1 8055 c210 3f14  g.4...D....U..?.
-00000db0: 40b1 8151 2e02 5536 01c3 480d 1207 b2b3  @..Q..U6..H.....
-00000dc0: 1041 5234 8202 c54a 1f57 1263 df44 58c6  .AR4...J.W.c.DX.
-00000dd0: 490e b023 1b14 1eb6 3601 3401 5950 c551  I..#....6.4.YP.Q
-00000de0: 51c6 2806 5d4a 015d 1206 b234 0151 de44  Q.(.]J.]...4.Q.D
-00000df0: 4423 1c42 4223 1dc7 b0b5 4444 1042 4241  D#.BB#....DD.BBA
-00000e00: b734 0159 5263 8364 b201 9a01 3813 3980  .4.YRc.d....8.9.
-00000e10: f360 2085 1423 282c 4500 04b0 2000 01c2  .` ..#(,E... ...
-00000e20: b144 5912 0414 4336 0027 04b4 2001 0112  .DY...C6.'.. ...
-00000e30: 0234 005e 3401 c3b2 b334 0163 b212 0234  .4.^4....4.c...4
-00000e40: 0034 0163 028f 4ca2 122c 4c6b 6c80 f82b  .4.c..L..,Lkl..+
-00000e50: 3223 2c29 1f24 242a 2323 263b 1f57 2d2e  2#,).$$*##&;.W-.
-00000e60: 3200 b15e 3401 5f4b d401 c2b2 144d 104e  2..^4._K.....M.N
-00000e70: 1022 3602 142d 104f 3601 8055 c348 9a01  ."6..-.O6..U.H..
-00000e80: 2500 1050 141e b336 0134 0159 b214 5110  %..P...6.4.Y..Q.
-00000e90: 5236 0144 6725 0010 5314 1e10 3f12 67b2  R6.Dg%..S...?.g.
-00000ea0: 144d 104e 1022 3602 142d 104f 3601 8055  .M.N."6..-.O6..U
-00000eb0: 3401 f436 0134 0159 40ac 7f01 126a b210  4..6.4.Y@....j..
-00000ec0: 5434 0247 51c4 2324 c542 c580 b414 5536  T4.GQ.#$.B....U6
-00000ed0: 00c5 b514 2936 0014 3010 5636 0144 7210  ....)6..0.V6.Dr.
-00000ee0: 57b5 ddd3 446b 1058 b5dd d344 6425 0010  W...Dk.X...Dd%..
-00000ef0: 5914 1e10 3f12 67b3 3401 f4b5 144d 105a  Y...?.g.4....M.Z
-00000f00: 1022 3602 142d 105b 3601 8055 3602 3401  ."6..-.[6..U6.4.
-00000f10: 59b5 43b7 7f51 5c5d 4a21 5712 63df 445a  Y.C..Q\]J!W.c.DZ
-00000f20: c649 1025 0023 2514 1eb2 b636 0234 0159  .I.%.#%....6.4.Y
-00000f30: 5063 5151 c628 065d 4a01 5d42 a97e 5263  PcQQ.(.]J.]B.~Rc
-00000f40: 0182 38c1 4008 5c6b 80f8 53b0 5353 4b18  ..8.@.\k..S.SSK.
-00000f50: c1b1 1430 104e 3601 4434 b114 5110 5d36  ...0.N6.D4..Q.]6
-00000f60: 0144 2bb1 6759 4226 5163 8220 ca40 0a5c  .D+.gYB&Qc. .@.\
-00000f70: 6b6b 900d 53b1 5353 4b14 c2b2 142d 104f  kk..S.SSK....-.O
-00000f80: 3601 8055 2500 dd44 2fb2 6759 422a 5163  6..U%..D/.gYB*Qc
-00000f90: 8c00 e203 2c31 1333 9014 4b26 2631 3023  ....,1.3..K&&10#
-00000fa0: 2626 432b 2b25 2225 5d28 2580 1044 2a01  &&C++%"%](%..D*.
-00000fb0: 1b45 1c44 c259 b023 1e34 0159 b023 1f34  .E.D.Y.#.4.Y.#.4
-00000fc0: 0159 b023 2014 1eb2 3400 8155 8055 3601  .Y.# ...4..U.U6.
-00000fd0: 3401 59b0 2321 141e 1206 1028 3401 3601  4.Y.#!.....(4.6.
-00000fe0: 3401 59b1 4446 b023 2234 0159 b010 4634  4.Y.DF.#"4.Y..F4
-00000ff0: 0159 b144 5b12 6a10 4710 4834 0247 0ac3  .Y.D[.j.G.H4.G..
-00001000: b314 4910 3136 0159 515c 5d12 5e34 0059  ..I.16.YQ\].^4.Y
-00001010: 4819 8051 1b31 c4b0 b414 4a10 4b12 0610  H..Q.1....J.K...
-00001020: 2834 0136 8200 3401 594a 2557 1263 df44  (4.6..4.YJ%W.c.D
-00001030: 5ec5 4914 2323 141e b536 01c6 b0b6 3401  ^.I.##...6....4.
-00001040: 5912 0cb6 3401 5951 51c5 2805 5d4a 015d  Y...4.YQQ.(.]J.]
-00001050: 5163                                     Qc
+00000870: 3a20 7b7d 0087 1410 1601 800d 2c2c 322c  : {}........,,2,
+00000880: 3272 6020 8010 022a 011b 031c 0216 0259  2r` ...*.......Y
+00000890: 8010 042a 011b 051c 0416 0459 8010 0610  ...*.......Y....
+000008a0: 072a 021b 081c 0616 061c 0716 0759 8010  .*...........Y..
+000008b0: 092a 011b 0a1c 0916 0959 8010 0b10 0c2a  .*.......Y.....*
+000008c0: 021b 0d1c 0b16 0b1c 0c16 0c59 8010 0e10  ...........Y....
+000008d0: 0f2a 021b 101c 0e16 5e1c 0f16 0f59 5432  .*......^....YT2
+000008e0: 0010 1134 0216 1151 6301 8704 1030 1188  ...4...Qc....0..
+000008f0: 1a44 8814 8407 6440 8808 6460 840e 8409  .D....d@..d`....
+00000900: 846a 8825 8c21 115f 1660 1011 1661 1012  .j.%.!._.`...a..
+00000910: 161e 512a 0153 3300 1613 3201 1620 3202  ..Q*.S3...2.. 2.
+00000920: 160e 502a 0153 3303 1621 3204 1625 3205  ..P*.S3..!2..%2.
+00000930: 1627 3206 162b 3207 162c 1162 3208 3401  .'2..+2..,.b2.4.
+00000940: 163a 1162 502a 0153 3309 3401 1638 1162  .:.bP*.S3.4..8.b
+00000950: 502a 0153 330a 3401 1631 5163 0b87 28ca  P*.S3.4..1Qc..(.
+00000960: 0320 1358 1480 1d60 2044 2929 4924 4422  . .X...` D))I$D"
+00000970: 562c b1b0 1814 1206 1015 3401 b018 1612  V,........4.....
+00000980: 0610 1734 01b0 1818 1206 1019 3401 b018  ...4........4...
+00000990: 1a50 b018 1b50 b018 1c48 0d12 0710 1d12  .P...P...H......
+000009a0: 1113 1e34 0259 4a2a 5712 63df 4463 c249  ...4.YJ*W.c.Dc.I
+000009b0: 1912 0b23 0014 1fb2 3601 3401 5912 0c23  ...#....6.4.Y..#
+000009c0: 0114 1fb2 3601 3401 5951 51c2 2802 5d4a  ....6.4.YQQ.(.]J
+000009d0: 015d 5163 8208 3610 2058 2080 3120 224a  .]Qc..6. X .1 "J
+000009e0: 4809 b014 14b1 3601 594a 0a59 1264 b134  H.....6.YJ.Y.d.4
+000009f0: 0159 4a01 5d51 6381 1011 0c0e 5880 3820  .YJ.]Qc.....X.8 
+00000a00: 2450 b018 1b50 b018 1c51 6383 48b2 0114  $P...P...Qc.H...
+00000a10: 2158 6580 3d20 3528 2325 b014 2023 0214  !Xe.= 5(#%.. #..
+00000a20: 1fb1 4444 1022 4242 1023 3601 3601 59b0  ..DD."BB.#6.6.Y.
+00000a30: 1420 1024 3601 59b1 4445 125e 3400 5912  . .$6.Y.DE.^4.Y.
+00000a40: 0f34 0059 5163 8310 390e 2558 8045 2031  .4.YQc..9.%X.E 1
+00000a50: 2cb0 1318 4449 b013 1b43 4423 0342 4210  ,...DI...CD#.BB.
+00000a60: 23c1 b013 1c44 4423 0442 4210 23c2 1026  #....DD#.BB.#..&
+00000a70: 141f b1b2 b013 1636 0363 8508 2a1c 2758  .......6.c..*.'X
+00000a80: 6680 4b40 4a27 2b24 2826 2826 b013 1844  f.K@J'+$(&(&...D
+00000a90: 77b0 131b 4372 1206 1028 3401 c2b2 b180  w...Cr...(4.....
+00000aa0: 5514 2936 00d9 4452 52b0 181b b014 2010  U.)6..DRR..... .
+00000ab0: 2a36 0159 522b 002a 0263 b014 2023 0536  *6.YR+.*.c.. #.6
+00000ac0: 0159 502b 002a 0263 52b1 2a02 6381 7832  .YP+.*.cR.*.c.x2
+00000ad0: 122b 5820 8059 6020 272b b014 2cb1 3601  .+X .Y` '+..,.6.
+00000ae0: c2b0 1420 b014 2536 0036 0159 b263 a400  ... ..%6.6.Y.c..
+00000af0: ea02 8602 2c58 2080 6280 0b52 228a 0848  ....,X .b..R"..H
+00000b00: 3242 2a23 2229 6248 2e62 2822 5122 472b  2B*#")bH.b("Q"G+
+00000b10: 3130 6d2b 2422 2b24 6229 2828 2828 2828  10m+$"+$b)((((((
+00000b20: 2828 2828 2828 2828 2828 2828 2a2d 7020  ((((((((((((*-p 
+00000b30: 4e4b 6040 4259 2db1 51de 434d 1267 b114  NK`@BY-.Q.CM.g..
+00000b40: 2936 0034 0180 d944 4252 63b1 1429 3600  )6.4...DBRc..)6.
+00000b50: 142d 3600 c2b2 8055 102e d944 54b0 1420  .-6....U...DT.. 
+00000b60: 2306 141f b013 16b0 131a 3602 3601 5952  #.........6.6.YR
+00000b70: 63b0 1427 b236 0130 02c3 c2b3 4342 5063  c..'.6.0....CBPc
+00000b80: 1267 b234 0180 d944 4252 63b2 8055 101d  .g.4...DBRc..U..
+00000b90: d944 50b0 1420 1268 1211 131e 3401 3601  .DP.. .h....4.6.
+00000ba0: 5952 63b2 8055 1021 d944 5c50 c412 67b2  YRc..U.!.D\P..g.
+00000bb0: 3401 82db 444a 102f b281 55dd 4442 52c4  4...DJ./..U.DBR.
+00000bc0: b014 21b4 3601 59b2 8055 1430 1031 3601  ..!.6.Y..U.0.16.
+00000bd0: 446e 1267 b234 0182 d944 5810 32b2 8155  Dn.g.4...DX.2..U
+00000be0: dd44 5012 1114 3110 14b0 1320 1033 5236  .DP...1.... .3R6
+00000bf0: 8400 5912 1114 3110 14b0 1320 3682 0059  ..Y...1.... 6..Y
+00000c00: b280 5514 3010 3436 0144 4652 b018 1c52  ..U.0.46.DFR...R
+00000c10: 63b2 8055 1430 1035 3601 4446 50b0 181c  c..U.0.56.DFP...
+00000c20: 5263 b280 5510 36d9 44b7 81b0 1420 2307  Rc..U.6.D.... #.
+00000c30: 3601 59b0 1420 2308 3601 59b0 1420 2309  6.Y.. #.6.Y.. #.
+00000c40: 3601 59b0 1420 230a 3601 59b0 1420 230b  6.Y.. #.6.Y.. #.
+00000c50: 3601 59b0 1420 230c 3601 59b0 1420 230d  6.Y.. #.6.Y.. #.
+00000c60: 3601 59b0 1420 230e 3601 59b0 1420 230f  6.Y.. #.6.Y.. #.
+00000c70: 3601 59b0 1420 2310 3601 59b0 1420 2311  6.Y.. #.6.Y.. #.
+00000c80: 3601 59b0 1420 2312 3601 59b0 1420 2313  6.Y.. #.6.Y.. #.
+00000c90: 3601 59b0 1420 2314 3601 59b0 1420 2315  6.Y.. #.6.Y.. #.
+00000ca0: 3601 59b0 1420 2316 3601 59b0 1420 2317  6.Y.. #.6.Y.. #.
+00000cb0: 3601 59b0 1420 2318 3601 5910 3712 68b2  6.Y.. #.6.Y.7.h.
+00000cc0: 3401 dd44 4d12 1114 3810 14b0 1320 3682  4..DM...8.... 6.
+00000cd0: 0063 1211 1438 1014 b013 2010 3952 3684  .c...8.... .9R6.
+00000ce0: 0063 b013 1c44 5412 67b2 3401 80d8 444b  .c...DT.g.4...DK
+00000cf0: 1211 143a b013 20b2 3602 6348 1012 0910  ...:.. .6.cH....
+00000d00: 3bb2 103c b013 2034 8400 634a 2157 1263  ;..<.. 4..cJ!W.c
+00000d10: df44 5ac5 4910 b014 2023 1914 1fb5 3601  .DZ.I... #....6.
+00000d20: 3601 5950 6351 51c5 2805 5d4a 015d 5163  6.YPcQQ.(.]J.]Qc
+00000d30: 8d00 9212 303a 1469 80cd 6060 2a48 2f28  ....0:.i..``*H/(
+00000d40: 3642 2b42 4a24 4d22 562b 4b30 2c12 67b1  6B+BJ$M"V+K0,.g.
+00000d50: 3401 81d9 44c4 80b1 8055 103d d944 6f12  4...D....U.=.Do.
+00000d60: 0634 0014 3e36 005f 4b22 3002 c2c3 8a12  .4..>6._K"0.....
+00000d70: 67b2 3401 f3c4 b023 1a14 1fb2 103f b4f4  g.4....#.....?..
+00000d80: 103f 87f4 b336 0434 0159 421c 5263 b012  .?...6.4.YB.Rc..
+00000d90: 06b1 8055 3401 3401 5952 6312 67b1 3401  ...U4.4.YRc.g.4.
+00000da0: 82db 44db 80b1 8055 c210 3f14 40b1 8151  ..D....U..?.@..Q
+00000db0: 2e02 5536 01c3 480d 1207 b2b3 1041 5234  ..U6..H......AR4
+00000dc0: 8202 c54a 1f57 1263 df44 58c6 490e b023  ...J.W.c.DX.I..#
+00000dd0: 1b14 1fb6 3601 3401 5950 c551 51c6 2806  ....6.4.YP.QQ.(.
+00000de0: 5d4a 015d 1206 b234 0151 de44 4423 1c42  ]J.]...4.Q.DD#.B
+00000df0: 4223 1dc7 b0b5 4444 1042 4241 b734 0159  B#....DD.BBA.4.Y
+00000e00: 5263 8364 b201 9a01 3814 3980 f260 2085  Rc.d....8.9..` .
+00000e10: 1423 282c 4500 04b0 2000 01c2 b144 5912  .#(,E... ....DY.
+00000e20: 0414 4336 0027 04b4 2001 0112 0234 005e  ..C6.'.. ....4.^
+00000e30: 3401 c3b2 b334 0163 b212 0234 0034 0163  4....4.c...4.4.c
+00000e40: 028f 4ca2 122c 4c6b 6c80 f72b 3223 2c29  ..L..,Lkl..+2#,)
+00000e50: 1f24 242a 2323 263b 1f57 2d2e 3200 b15e  .$$*##&;.W-.2..^
+00000e60: 3401 5f4b d401 c2b2 144d 104e 1023 3602  4._K.....M.N.#6.
+00000e70: 142d 104f 3601 8055 c348 9a01 2500 1050  .-.O6..U.H..%..P
+00000e80: 141f b336 0134 0159 b214 5110 5236 0144  ...6.4.Y..Q.R6.D
+00000e90: 6725 0010 5314 1f10 3f12 67b2 144d 104e  g%..S...?.g..M.N
+00000ea0: 1023 3602 142d 104f 3601 8055 3401 f436  .#6..-.O6..U4..6
+00000eb0: 0134 0159 40ac 7f01 126a b210 5434 0247  .4.Y@....j..T4.G
+00000ec0: 51c4 2324 c542 c580 b414 5536 00c5 b514  Q.#$.B....U6....
+00000ed0: 2936 0014 3010 5636 0144 7210 57b5 ddd3  )6..0.V6.Dr.W...
+00000ee0: 446b 1058 b5dd d344 6425 0010 5914 1f10  Dk.X...Dd%..Y...
+00000ef0: 3f12 67b3 3401 f4b5 144d 105a 1023 3602  ?.g.4....M.Z.#6.
+00000f00: 142d 105b 3601 8055 3602 3401 59b5 43b7  .-.[6..U6.4.Y.C.
+00000f10: 7f51 5c5d 4a21 5712 63df 445a c649 1025  .Q\]J!W.c.DZ.I.%
+00000f20: 0023 2514 1fb2 b636 0234 0159 5063 5151  .#%....6.4.YPcQQ
+00000f30: c628 065d 4a01 5d42 a97e 5263 0182 38c1  .(.]J.]B.~Rc..8.
+00000f40: 4008 5c6b 80f7 53b0 5353 4b18 c1b1 1430  @.\k..S.SSK....0
+00000f50: 104e 3601 4434 b114 5110 5d36 0144 2bb1  .N6.D4..Q.]6.D+.
+00000f60: 6759 4226 5163 8220 ca40 0a5c 6b6b 900c  gYB&Qc. .@.\kk..
+00000f70: 53b1 5353 4b14 c2b2 142d 104f 3601 8055  S.SSK....-.O6..U
+00000f80: 2500 dd44 2fb2 6759 422a 5163 8c00 e203  %..D/.gYB*Qc....
+00000f90: 2c31 1433 9013 4b26 2631 3023 2626 432b  ,1.3..K&&10#&&C+
+00000fa0: 2b25 2225 5d28 2580 1044 2a01 1b45 1c44  +%"%](%..D*..E.D
+00000fb0: c259 b023 1e34 0159 b023 1f34 0159 b023  .Y.#.4.Y.#.4.Y.#
+00000fc0: 2014 1fb2 3400 8155 8055 3601 3401 59b0   ...4..U.U6.4.Y.
+00000fd0: 2321 141f 1206 1028 3401 3601 3401 59b1  #!.....(4.6.4.Y.
+00000fe0: 4446 b023 2234 0159 b010 4634 0159 b144  DF.#"4.Y..F4.Y.D
+00000ff0: 5b12 6a10 4710 4834 0247 0ac3 b314 4910  [.j.G.H4.G....I.
+00001000: 3136 0159 515c 5d12 5e34 0059 4819 8051  16.YQ\].^4.YH..Q
+00001010: 1b31 c4b0 b414 4a10 4b12 0610 2834 0136  .1....J.K...(4.6
+00001020: 8200 3401 594a 2557 1263 df44 5ec5 4914  ..4.YJ%W.c.D^.I.
+00001030: 2323 141f b536 01c6 b0b6 3401 5912 0cb6  ##...6....4.Y...
+00001040: 3401 5951 51c5 2805 5d4a 015d 5163       4.YQQ.(.]J.]Qc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files 21% similar despite different names*

```diff
@@ -1,227 +1,173 @@
-00000000: 4d06 001f 8107 1218 4c4d 5f73 7973 7465  M.......LM_syste
-00000010: 6d2e 7079 000f 126c 6f63 616c 7469 6d65  m.py...localtime
-00000020: 000a 7574 696d 6500 1a73 6f63 6b65 745f  ..utime..socket_
-00000030: 7374 7265 616d 000c 436f 6d6d 6f6e 000e  stream..Common..
-00000040: 6765 745f 6d61 6300 1c73 7461 5f68 6967  get_mac..sta_hig
-00000050: 685f 6176 6169 6c00 0e4e 6574 776f 726b  h_avail..Network
-00000060: 0010 6e74 705f 7469 6d65 0010 7365 745f  ..ntp_time..set_
-00000070: 7469 6d65 000c 7570 7469 6d65 0008 5469  time..uptime..Ti
-00000080: 6d65 000e 6275 696c 7469 6e00 186d 656d  me..builtin..mem
-00000090: 6f72 795f 7573 6167 6500 106d 656d 5f66  ory_usage..mem_f
-000000a0: 7265 6500 126d 656d 5f61 6c6c 6f63 000e  ree..mem_alloc..
-000000b0: 636f 6c6c 6563 7400 0467 6300 0a73 696d  collect..gc..sim
-000000c0: 6763 000e 7065 7263 656e 7400 106d 656d  gc..percent..mem
-000000d0: 5f75 7365 6400 1464 6973 6b5f 7573 6167  _used..disk_usag
-000000e0: 6500 0e73 7461 7476 6673 000c 6765 7463  e..statvfs..getc
-000000f0: 7764 0004 6f73 000e 6673 5f75 7365 6400  wd..os..fs_used.
-00000100: 0869 6e66 6f00 0866 7265 7100 0e6d 6163  .info..freq..mac
-00000110: 6869 6e65 000a 756e 616d 6500 8129 1262  hine..uname..).b
-00000120: 6f61 7264 3a20 7b7d 000e 6d61 633a 207b  oard: {}..mac: {
-00000130: 7d00 106d 6163 3a20 6e2f 6100 1475 7074  }..mac: n/a..upt
-00000140: 696d 653a 207b 7d00 0781 510c 6763 6c65  ime: {}...Q.gcle
-00000150: 616e 0012 6865 6172 7462 6561 7400 0a63  an..heartbeat..c
-00000160: 6c6f 636b 0002 2e00 023a 0006 6e74 7000  lock.....:..ntp.
-00000170: 0c63 6667 6765 7400 1a43 6f6e 6669 6748  .cfgget..ConfigH
-00000180: 616e 646c 6572 0006 7375 6e00 0e73 756e  andler..sun..sun
-00000190: 7469 6d65 0006 5375 6e00 0854 494d 4500  time..Sun..TIME.
-000001a0: 1073 6574 636c 6f63 6b00 0c6d 6f64 756c  .setclock..modul
-000001b0: 6500 0e6d 6f64 756c 6573 0006 7379 7300  e..modules..sys.
-000001c0: 8155 1263 6163 6865 6475 6d70 000e 6c69  .U.cachedump..li
-000001d0: 7374 6469 7200 0272 0079 0c7b 7d3a 207b  stdir..r.y.{}: {
-000001e0: 7d00 817b 0382 010c 7b7d 2e70 6473 0008  }..{....{}.pds..
-000001f0: 7273 7369 0008 574c 414e 000c 5354 415f  rssi..WLAN..STA_
-00000200: 4946 000e 6e65 7477 6f72 6b00 0c73 7461  IF..network..sta
-00000210: 7475 7300 0e41 6d61 7a69 6e67 0010 5665  tus..Amazing..Ve
-00000220: 7279 476f 6f64 0008 4f6b 6179 000e 4e6f  ryGood..Okay..No
-00000230: 7447 6f6f 6400 1055 6e75 7361 626c 6500  tGood..Unusable.
-00000240: 106c 6d70 6163 6d61 6e00 811f 0470 7900  .lmpacman....py.
-00000250: 0e73 7973 7465 6d2e 000a 4c4d 5f7b 7d00  .system...LM_{}.
-00000260: 0a20 2020 7b7d 000c 7069 6e6d 6170 0016  .   {}..pinmap..
-00000270: 7069 6e6d 6170 5f64 756d 7000 1467 6574  pinmap_dump..get
-00000280: 5f70 696e 6d61 7000 164c 6f67 6963 616c  _pinmap..Logical
-00000290: 5069 6e73 000c 6861 5f73 7461 000c 616c  Pins..ha_sta..al
-000002a0: 6172 6d73 0014 6572 726c 6f67 5f67 6574  arms..errlog_get
-000002b0: 0014 6572 726c 6f67 5f61 6464 0018 6572  ..errlog_add..er
-000002c0: 726c 6f67 5f63 6c65 616e 000a 4465 6275  rlog_clean..Debu
-000002d0: 6700 0c6d 7367 6f62 6a00 124e 4f4b 2061  g..msgobj..NOK a
-000002e0: 6c61 726d 0010 4f4b 2061 6c61 726d 0010  larm..OK alarm..
-000002f0: 6966 636f 6e66 6967 001e 6d69 6372 6f73  ifconfig..micros
-00000300: 5f63 6865 636b 7375 6d00 0873 6861 3100  _checksum..sha1.
-00000310: 0e68 6173 686c 6962 000e 6865 786c 6966  .hashlib..hexlif
-00000320: 7900 1062 696e 6173 6369 6900 0472 6200  y..binascii..rb.
-00000330: 0c64 6967 6573 7400 0c64 6563 6f64 6500  .digest..decode.
-00000340: 8243 0a7b 7d20 7b7d 000e 7665 7273 696f  .C.{} {}..versio
-00000350: 6e00 0868 656c 7000 0c5f 7265 706c 7900  n..help.._reply.
-00000360: 0e7b 7d20 287b 7d29 0014 3c6c 6973 7463  .{} ({})..<listc
-00000370: 6f6d 703e 0012 3c67 656e 6578 7072 3e00  omp>..<genexpr>.
-00000380: 082e 7064 7300 064c 4d5f 0082 0382 0d81  ..pds..LM_......
-00000390: 3d49 0e72 6566 7265 7368 0008 7965 6172  =I.refresh..year
-000003a0: 000a 6d6f 6e74 6800 086d 6461 7900 0868  ..month..mday..h
-000003b0: 6f75 7200 066d 696e 0006 7365 6300 0c75  our..min..sec..u
-000003c0: 6e6c 6f61 6400 8159 0863 6465 6c00 816d  nload..Y.cdel..m
-000003d0: 8157 0c6c 6d5f 6465 6c00 8153 0a63 6c65  .W.lm_del..S.cle
-000003e0: 616e 0008 7465 7374 000b 066d 7367 0082  an..test...msg..
-000003f0: 2f05 1343 5055 2063 6c6f 636b 3a20 7b7d  /..CPU clock: {}
-00000400: 205b 4d48 7a5d 0008 0531 652d 3037 050f   [MHz]...1e-07..
-00000410: 4d65 6d20 7573 6167 653a 207b 7d20 2500  Mem usage: {} %.
-00000420: 050e 4653 2075 7361 6765 3a20 7b7d 2025  ..FS usage: {} %
-00000430: 0005 0b75 7079 7468 6f6e 3a20 7b7d 0005  ...upython: {}..
-00000440: 1047 4320 4d65 6d46 7265 655b 6279 7465  .GC MemFree[byte
-00000450: 5d00 050f 3c33 2068 6561 7274 6265 6174  ]...<3 heartbeat
-00000460: 203c 3300 0514 7b7d 2020 7b7d 0a57 443a   <3...{}  {}.WD:
-00000470: 207b 7d20 5944 3a20 7b7d 0005 0c6e 7470   {} YD: {}...ntp
-00000480: 2065 7272 6f72 3a7b 7d00 0516 4d6f 6475   error:{}...Modu
-00000490: 6c65 2075 6e6c 6f61 6420 7b7d 2064 6f6e  le unload {} don
-000004a0: 652e 0005 184d 6f64 756c 6520 756e 6c6f  e....Module unlo
-000004b0: 6164 207b 7d20 6661 696c 6564 2e00 0513  ad {} failed....
-000004c0: 7b7d 2e70 6473 2064 656c 6574 6520 646f  {}.pds delete do
-000004d0: 6e65 2e00 0511 7b7d 2e70 6473 206e 6f74  ne....{}.pds not
-000004e0: 2065 7869 7374 7300 0526 4c6f 6164 206d   exists..&Load m
-000004f0: 6f64 756c 6520 7b7d 2069 7320 696e 2075  odule {} is in u
-00000500: 7365 2c20 736b 6970 2064 656c 6574 652e  se, skip delete.
-00000510: 0005 1144 656c 6574 6520 6d6f 6475 6c65  ...Delete module
-00000520: 3a20 7b7d 0005 105b 4552 525d 2054 6553  : {}...[ERR] TeS
-00000530: 7420 4572 526f 5200 0512 6d69 6372 4f53  t ErRoR...micrOS
-00000540: 2076 6572 7369 6f6e 3a20 7b7d 000a 1205   version: {}....
-00000550: 0469 6e66 6f00 0506 6763 6c65 616e 0005  .info...gclean..
-00000560: 0968 6561 7274 6265 6174 0005 0563 6c6f  .heartbeat...clo
-00000570: 636b 0005 2573 6574 636c 6f63 6b20 7965  ck..%setclock ye
-00000580: 6172 206d 6f6e 7468 206d 6461 7920 686f  ar month mday ho
-00000590: 7572 206d 696e 2073 6563 0005 036e 7470  ur min sec...ntp
-000005a0: 0005 1b6d 6f64 756c 6520 756e 6c6f 6164  ...module unload
-000005b0: 3d22 4c4d 5f72 6762 2f4e 6f6e 6522 0005  ="LM_rgb/None"..
-000005c0: 0472 7373 6900 051d 6361 6368 6564 756d  .rssi...cachedum
-000005d0: 7020 6364 656c 3d22 7267 622e 7064 732f  p cdel="rgb.pds/
-000005e0: 4e6f 6e65 2200 0520 6c6d 7061 636d 616e  None".. lmpacman
-000005f0: 206c 6d5f 6465 6c3d 224c 4d5f 7267 622e   lm_del="LM_rgb.
-00000600: 7079 2f4e 6f6e 6522 0005 1870 696e 6d61  py/None"...pinma
-00000610: 7020 6b65 793d 2264 6874 7069 6e22 2f4e  p key="dhtpin"/N
-00000620: 6f6e 6500 0506 6861 5f73 7461 0005 1261  one...ha_sta...a
-00000630: 6c61 726d 7320 636c 6561 6e3d 4661 6c73  larms clean=Fals
-00000640: 6500 0511 7375 6e20 7265 6672 6573 683d  e...sun refresh=
-00000650: 4661 6c73 6500 0508 6966 636f 6e66 6967  False...ifconfig
-00000660: 0005 0c6d 656d 6f72 795f 7573 6167 6500  ...memory_usage.
-00000670: 050a 6469 736b 5f75 7361 6765 0005 0f6d  ..disk_usage...m
-00000680: 6963 726f 735f 6368 6563 6b73 756d 008f  icros_checksum..
-00000690: 2418 5201 2c2c 3278 8410 840e 8c24 840c  $.R.,,2x.....$..
-000006a0: 8407 840b 840d 880e 840f 8810 8d19 8411  ................
-000006b0: 8d19 890c 8407 8e11 8408 8c13 8010 022a  ...............*
-000006c0: 011b 031c 0216 0259 8010 042a 011b 051c  .......Y...*....
-000006d0: 0416 0459 8010 0610 072a 021b 081c 0616  ...Y.....*......
-000006e0: 061c 0716 0759 8010 0910 0a10 0b2a 031b  .....Y.......*..
-000006f0: 0c1c 0916 091c 0a16 0a1c 0b16 0b59 3200  .............Y2.
-00000700: 160e 3201 1616 1104 512a 0153 3302 3401  ..2.....Q*.S3.4.
-00000710: 161b 3203 1626 3204 1627 3205 1628 3206  ..2..&2..'2..(2.
-00000720: 162b 502a 0153 3307 162e 3208 1632 512a  .+P*.S3...2..2Q*
-00000730: 0153 3309 1633 1104 5151 2a02 5333 0a34  .S3..3..QQ*.S3.4
-00000740: 0116 3732 0b16 4011 0451 512a 0253 330c  ..72..@..QQ*.S3.
-00000750: 3401 164a 100d 2a01 5333 0d16 5032 0e16  4..J..*.S3..P2..
-00000760: 5411 0450 5051 2a03 5333 0f34 0116 5532  T..PPQ*.S3.4..U2
-00000770: 1016 5d11 0451 2a01 5333 1134 0116 5e32  ..]..Q*.S3.4..^2
-00000780: 1216 6951 6313 8640 6418 0e80 0760 2022  ..iQc..@d....` "
-00000790: 5838 2428 242d 4817 8010 0f10 1010 112a  X8$($-H........*
-000007a0: 031b 121c 0fc0 1c10 c11c 11c2 594a 1959  ............YJ.Y
-000007b0: 8010 0f10 1010 112a 031b 131c 0fc0 1c10  .......*........
-000007c0: c11c 11c2 594a 015d b234 0059 b034 00b1  ....YJ.].4.Y.4..
-000007d0: 3400 f2c3 b134 00c4 1271 b4b3 f722 8064  4....4...q...".d
-000007e0: f481 3402 c52c 02b5 1014 62b4 1015 6263  ..4..,....b...bc
-000007f0: 8500 4816 1680 1760 2030 2728 2824 2d80  ..H....` 0'(($-.
-00000800: 1017 1018 2a02 1b19 1c17 c01c 18c1 59b0  ....*.........Y.
-00000810: b134 0034 01c2 b280 55b2 8255 f4c3 b280  .4.4....U..U....
-00000820: 55b2 8355 f4c4 b3b4 f3c5 1271 b5b3 f722  U..U.......q..."
-00000830: 8064 f481 3402 c62c 02b6 1014 62b5 101a  .d..4..,....b...
-00000840: 6263 8c0c d501 a801 1b5a 8026 6020 2b2b  bc.......Z.&` ++
-00000850: 4486 0d34 3131 2f2f 2251 292e 0004 8010  D..411//"Q).....
-00000860: 1c2a 011b 1d1c 1cc1 5980 101e 2a01 1b19  .*......Y...*...
-00000870: 1c1e c259 2b00 2704 b0b4 2000 02c3 b323  ...Y+.'... ....#
-00000880: 0014 1f12 72b1 3400 2301 f434 0136 0134  ....r.4.#..4.6.4
-00000890: 0159 b323 0214 1f12 0e34 0010 1455 3601  .Y.#.....4...U6.
-000008a0: 3401 59b3 2303 141f 1216 3400 1014 5536  4.Y.#.....4...U6
-000008b0: 0134 0159 b323 0414 1fb2 3400 8355 3601  .4.Y.#....4..U6.
-000008c0: 3401 59b3 1020 141f b234 0084 5536 0134  4.Y.. ...4..U6.4
-000008d0: 0159 4810 b310 2114 1f12 0634 0036 0134  .YH...!....4.6.4
-000008e0: 0159 4a0a 59b3 1022 3401 594a 015d b310  .YJ.Y.."4.YJ.]..
-000008f0: 2314 1f12 0b34 0036 0134 0159 1024 1425  #....4.6.4.Y.$.%
-00000900: 2504 3601 6301 8470 e302 1c6a 8104 8104  %.6.c..p...j....
-00000910: 8105 802f 2022 466a 7148 1825 0051 de44  .../ "FjqH.%.Q.D
-00000920: 4a25 0114 3ab2 3601 5942 4625 00b2 3401  J%..:.6.YBF%..4.
-00000930: 594a 2157 1273 df44 5ac3 4910 2501 143a  YJ!W.s.DZ.I.%..:
-00000940: 106b 141f b2b3 3602 3601 5951 51c3 2803  .k....6.6.YQQ.(.
-00000950: 5d4a 015d 5163 8378 3c10 2680 4960 2253  ]J.]Qc.x<.&.I`"S
-00000960: 3324 4812 8010 1110 0f2a 021b 121c 11c0  3$H......*......
-00000970: 1c0f c159 4a14 5980 1011 100f 2a02 1b13  ...YJ.Y.....*...
-00000980: 1c11 c01c 0fc1 594a 015d b034 0059 2c01  ......YJ.].4.Y,.
-00000990: b134 0023 0562 6348 0008 2780 5560 2306  .4.#.bcH..'.U`#.
-000009a0: 6383 3440 0c28 805c 6060 2932 0012 0234  c.4@.(.\``)2...4
-000009b0: 0034 01c0 2307 141f 1029 1425 b080 832e  .4..#....).%....
-000009c0: 0255 3601 102a 1425 b083 862e 0255 3601  .U6..*.%.....U6.
-000009d0: b086 55b0 8755 3604 6301 8148 410a 6c81  ..U..U6.c..HA.l.
-000009e0: 0480 622b 00b0 5f4b 0bc1 1281 06b1 3401  ..b+.._K......4.
-000009f0: 2f14 4233 6384 30c8 0210 2b80 6760 2b42  /.B3c.0...+.g`+B
-00000a00: 2553 8010 2c2a 011b 2d1c 2cc0 5948 0f12  %S..,*..-.,.YH..
-00000a10: 0934 00c1 b112 0234 002a 0263 4a1d 5712  .4.....4.*.cJ.W.
-00000a20: 73df 4456 c249 0c50 2308 141f b236 012a  s.DV.I.P#....6.*
-00000a30: 0263 5151 c228 025d 4a01 5d51 6382 38a9  .cQQ.(.]J.]Qc.8.
-00000a40: 0112 2e74 8074 8007 3023 2480 102f 1030  ...t.t..0#$../.0
-00000a50: 2a02 1b0c 1c2f c11c 30c2 59b0 4444 b134  *..../..0.Y.DD.4
-00000a60: 0063 b213 3163 8178 e204 1832 7576 7778  .c..1c.x...2uvwx
-00000a70: 797a 8082 800a 2b12 0ab0 b1b2 b3b4 b534  yz....+........4
-00000a80: 0659 1202 3400 6384 38a1 0118 337b 8091  .Y..4.c.8...3{..
-00000a90: 6060 2b25 2a29 2528 8010 342a 011b 351c  ``+%*)%(..4*..5.
-00000aa0: 34c1 59b0 51de 444a 127c b114 3636 0034  4.Y.Q.DJ.|..66.4
-00000ab0: 0163 b0b1 1436 3600 dd44 4db1 b053 5b56  .c...66..DM..S[V
-00000ac0: 2309 141f b036 0163 230a 141f b036 0163  #....6.c#....6.c
-00000ad0: 8a6c 9e90 0126 377d 5a80 a260 462b 232c  .l...&7}Z..`F+#,
-00000ae0: 2a25 5435 4e2b 222b 4bb0 51de 44e0 8080  *%T5N+"+K.Q.D...
-00000af0: 1038 2a01 1b19 1c38 c259 2b00 c332 00b2  .8*....8.Y+..2..
-00000b00: 3400 5e34 015f 4b39 c412 7eb4 1039 3402  4.^4._K9..~..94.
-00000b10: 472b c5b1 51de 4454 b314 3a10 3b14 1fb4  G+..Q.DT..:.;...
-00000b20: b514 3c36 0036 0236 0159 4250 b110 3b14  ..<6.6.6.YBP..;.
-00000b30: 1fb4 b514 3c36 0036 0234 0159 515c 5d42  ....<6.6.4.YQ\]B
-00000b40: 0512 7fb3 3401 80d8 4442 b363 103d 6380  ....4...DB.c.=c.
-00000b50: 103e 2a01 1b19 1c3e c659 4815 b610 3f14  .>*....>.YH...?.
-00000b60: 1fb0 3601 3401 5923 0b14 1fb0 3601 634a  ..6.4.Y#....6.cJ
-00000b70: 0c59 230c 141f b036 0163 4a01 5d51 6301  .Y#....6.cJ.]Qc.
-00000b80: 8178 c140 0a6d 8104 80a9 53b0 5353 4b0f  .x.@.m....S.SSK.
-00000b90: c1b1 144b 106e 3601 4434 b167 5942 2f51  ...K.n6.D4.gYB/Q
-00000ba0: 6386 5028 1c40 80ba 6030 2b27 2727 2727  c.P(.@..`0+'''''
-00000bb0: 2727 2780 1041 1042 2a02 1b43 1c41 c01c  '''..A.B*..C.A..
-00000bc0: 42c1 59b0 b134 0114 4410 4036 01c2 b222  B.Y..4..D.@6..."
-00000bd0: ff3d d844 472c 01b2 1045 6263 b222 ff3a  .=.DG,...Ebc.".:
-00000be0: d844 472c 01b2 1046 6263 b222 ff30 d844  .DG,...Fbc.".0.D
-00000bf0: 472c 01b2 1047 6263 b222 ff26 d844 472c  G,...Gbc.".&.DG,
-00000c00: 01b2 1048 6263 2c01 b210 4962 6389 2cf2  ...Hbc,...Ibc.,.
-00000c10: 8001 264a 8100 5a80 cc60 6030 4f26 282b  ..&J..Z..``0O&(+
-00000c20: 4823 2c25 4f2d 8010 3810 3e2a 021b 191c  H#,%O-..8.>*....
-00000c30: 38c2 1c3e c359 b051 ded3 446a b014 4b10  8..>.Y.Q..Dj..K.
-00000c40: 4c36 0144 6110 4db0 dd44 4823 0d14 1fb0  L6.Da.M..DH#....
-00000c50: 3601 63b3 104e 141f b036 0134 0159 230e  6.c..N...6.4.Y#.
-00000c60: 141f b036 0163 2b00 c432 00b2 3400 5e34  ...6.c+..2..4.^4
-00000c70: 015f 4b22 c5b1 51de 444f b414 3a10 4f14  ._K"..Q.DO..:.O.
-00000c80: 1fb5 3601 3601 5942 4bb1 104f 141f b536  ..6.6.YBK..O...6
-00000c90: 0134 0159 421c 127f b434 0180 d844 42b4  .4.YB....4...DB.
-00000ca0: 6310 3d63 0182 20c9 400a 6d81 0480 db53  c.=c.. .@.m....S
-00000cb0: b053 534b 14c1 106f b1dd 4437 b114 7010  .SSK...o..D7..p.
-00000cc0: 6f10 3d36 0267 5942 2a51 6382 60b1 0114  o.=6.gYB*Qc.`...
-00000cd0: 5081 0180 e460 4030 2429 8010 5110 522a  P....`@0$)..Q.R*
-00000ce0: 021b 531c 51c1 1c52 c259 b234 00c3 b1b0  ..S.Q..R.Y.4....
-00000cf0: 3401 b055 b3b0 56b3 6358 0008 5480 f060  4..U..V.cX..T..`
-00000d00: 1207 3400 6385 40d3 8101 2055 8102 8103  ..4.c.@... U....
-00000d10: 5a80 f860 6035 2326 2328 2880 1056 1057  Z..``5#&#((..V.W
-00000d20: 1058 2a03 1b59 1c56 c31c 57c4 1c58 c559  .X*..Y.V..W..X.Y
-00000d30: b144 46b4 230f 3401 59b0 4448 b510 5ab2  .DF.#.4.Y.DH..Z.
-00000d40: 3482 0059 b310 5ab2 3482 00c6 b680 d844  4..Y..Z.4......D
-00000d50: 472c 01b6 105b 6263 2c01 b610 5c62 6381  G,...[bc,...\bc.
-00000d60: 3010 0a5d 9008 602b 8010 5d2a 011b 081c  0..]..`+..]*....
-00000d70: 5dc0 59b0 3400 6388 548d 111a 5e5a 9011  ].Y.4.c.T...^Z..
-00000d80: 2b2b 2b4b 2c2a 392c 2780 105f 2a01 1b60  +++K,*9,'.._*..`
-00000d90: 1c5f c159 8010 612a 011b 621c 61c2 5980  ._.Y..a*..b.a.Y.
-00000da0: 1038 2a01 1b19 1c38 c359 8010 2c2a 011b  .8*....8.Y..,*..
-00000db0: 2d1c 2cc4 5932 00b3 3400 5e34 015f 4b37  -.,.Y2..4.^4._K7
-00000dc0: c512 7eb5 1063 3402 4718 c6b2 b1b6 143c  ..~..c4.G......<
-00000dd0: 3600 3401 1464 3600 3401 1465 1066 3601  6.4..d6.4..e.f6.
-00000de0: c751 5c5d b010 6714 1fb7 b536 0234 0159  .Q\]..g....6.4.Y
-00000df0: 1226 3400 5942 0723 1014 1fb4 1068 3401  .&4.YB.#.....h4.
-00000e00: 3601 6301 8178 c140 0a6d 8104 9016 53b0  6.c..x.@.m....S.
-00000e10: 5353 4b0f c1b1 144b 104c 3601 4434 b167  SSK....K.L6.D4.g
-00000e20: 5942 2f51 6350 000a 6990 2360 4023 1163  YB/QcP..i.#`@#.c
+00000000: 4d06 001f 6e0d 184c 4d5f 7379 7374 656d  M...n..LM_system
+00000010: 2e70 7900 0f12 6c6f 6361 6c74 696d 6500  .py...localtime.
+00000020: 0a75 7469 6d65 001a 736f 636b 6574 5f73  .utime..socket_s
+00000030: 7472 6561 6d00 0c43 6f6d 6d6f 6e00 0e67  tream..Common..g
+00000040: 6574 5f6d 6163 001c 7374 615f 6869 6768  et_mac..sta_high
+00000050: 5f61 7661 696c 000e 4e65 7477 6f72 6b00  _avail..Network.
+00000060: 106e 7470 5f74 696d 6500 1073 6574 5f74  .ntp_time..set_t
+00000070: 696d 6500 0c75 7074 696d 6500 0854 696d  ime..uptime..Tim
+00000080: 6500 0e62 7569 6c74 696e 0018 6d65 6d6f  e..builtin..memo
+00000090: 7279 5f75 7361 6765 0010 6d65 6d5f 6672  ry_usage..mem_fr
+000000a0: 6565 0012 6d65 6d5f 616c 6c6f 6300 0e63  ee..mem_alloc..c
+000000b0: 6f6c 6c65 6374 0004 6763 000a 7369 6d67  ollect..gc..simg
+000000c0: 6300 0e70 6572 6365 6e74 0010 6d65 6d5f  c..percent..mem_
+000000d0: 7573 6564 0014 6469 736b 5f75 7361 6765  used..disk_usage
+000000e0: 000e 7374 6174 7666 7300 0c67 6574 6377  ..statvfs..getcw
+000000f0: 6400 046f 7300 0e66 735f 7573 6564 0008  d..os..fs_used..
+00000100: 696e 666f 0008 6672 6571 000e 6d61 6368  info..freq..mach
+00000110: 696e 6500 0a75 6e61 6d65 0081 2912 626f  ine..uname..).bo
+00000120: 6172 643a 207b 7d00 0e6d 6163 3a20 7b7d  ard: {}..mac: {}
+00000130: 0010 6d61 633a 206e 2f61 0014 7570 7469  ..mac: n/a..upti
+00000140: 6d65 3a20 7b7d 0007 8151 0c67 636c 6561  me: {}...Q.gclea
+00000150: 6e00 1268 6561 7274 6265 6174 000a 636c  n..heartbeat..cl
+00000160: 6f63 6b00 022e 0002 3a00 066e 7470 000c  ock.....:..ntp..
+00000170: 6366 6767 6574 001a 436f 6e66 6967 4861  cfgget..ConfigHa
+00000180: 6e64 6c65 7200 0673 756e 000e 7375 6e74  ndler..sun..sunt
+00000190: 696d 6500 0653 756e 0008 5449 4d45 0010  ime..Sun..TIME..
+000001a0: 7365 7463 6c6f 636b 0012 6361 6368 6564  setclock..cached
+000001b0: 756d 7000 0e6c 6973 7464 6972 0002 7200  ump..listdir..r.
+000001c0: 790c 7b7d 3a20 7b7d 0081 7b03 8201 0c7b  y.{}: {}..{....{
+000001d0: 7d2e 7064 7300 0872 7373 6900 0857 4c41  }.pds..rssi..WLA
+000001e0: 4e00 0c53 5441 5f49 4600 0e6e 6574 776f  N..STA_IF..netwo
+000001f0: 726b 000c 7374 6174 7573 000e 416d 617a  rk..status..Amaz
+00000200: 696e 6700 1056 6572 7947 6f6f 6400 084f  ing..VeryGood..O
+00000210: 6b61 7900 0e4e 6f74 476f 6f64 0010 556e  kay..NotGood..Un
+00000220: 7573 6162 6c65 000c 7069 6e6d 6170 0016  usable..pinmap..
+00000230: 7069 6e6d 6170 5f64 756d 7000 1467 6574  pinmap_dump..get
+00000240: 5f70 696e 6d61 7000 164c 6f67 6963 616c  _pinmap..Logical
+00000250: 5069 6e73 000c 6861 5f73 7461 000c 616c  Pins..ha_sta..al
+00000260: 6172 6d73 0014 6572 726c 6f67 5f67 6574  arms..errlog_get
+00000270: 0014 6572 726c 6f67 5f61 6464 0018 6572  ..errlog_add..er
+00000280: 726c 6f67 5f63 6c65 616e 000a 4465 6275  rlog_clean..Debu
+00000290: 6700 0c6d 7367 6f62 6a00 124e 4f4b 2061  g..msgobj..NOK a
+000002a0: 6c61 726d 0010 4f4b 2061 6c61 726d 0010  larm..OK alarm..
+000002b0: 6966 636f 6e66 6967 0008 6865 6c70 000c  ifconfig..help..
+000002c0: 5f72 6570 6c79 000e 7b7d 2028 7b7d 2900  _reply..{} ({}).
+000002d0: 143c 6c69 7374 636f 6d70 3e00 123c 6765  .<listcomp>..<ge
+000002e0: 6e65 7870 723e 0081 1f08 2e70 6473 0082  nexpr>.....pds..
+000002f0: 0d81 3d49 0e72 6566 7265 7368 0008 7965  ..=I.refresh..ye
+00000300: 6172 000a 6d6f 6e74 6800 086d 6461 7900  ar..month..mday.
+00000310: 0868 6f75 7200 066d 696e 0006 7365 6300  .hour..min..sec.
+00000320: 0863 6465 6c00 816d 8157 8153 0a63 6c65  .cdel..m.W.S.cle
+00000330: 616e 0008 7465 7374 000b 066d 7367 0082  an..test...msg..
+00000340: 2f05 1343 5055 2063 6c6f 636b 3a20 7b7d  /..CPU clock: {}
+00000350: 205b 4d48 7a5d 0008 0531 652d 3037 050f   [MHz]...1e-07..
+00000360: 4d65 6d20 7573 6167 653a 207b 7d20 2500  Mem usage: {} %.
+00000370: 050e 4653 2075 7361 6765 3a20 7b7d 2025  ..FS usage: {} %
+00000380: 0005 0b75 7079 7468 6f6e 3a20 7b7d 0005  ...upython: {}..
+00000390: 1047 4320 4d65 6d46 7265 655b 6279 7465  .GC MemFree[byte
+000003a0: 5d00 050f 3c33 2068 6561 7274 6265 6174  ]...<3 heartbeat
+000003b0: 203c 3300 0514 7b7d 2020 7b7d 0a57 443a   <3...{}  {}.WD:
+000003c0: 207b 7d20 5944 3a20 7b7d 0005 0c6e 7470   {} YD: {}...ntp
+000003d0: 2065 7272 6f72 3a7b 7d00 0513 7b7d 2e70   error:{}...{}.p
+000003e0: 6473 2064 656c 6574 6520 646f 6e65 2e00  ds delete done..
+000003f0: 0511 7b7d 2e70 6473 206e 6f74 2065 7869  ..{}.pds not exi
+00000400: 7374 7300 0510 5b45 5252 5d20 5465 5374  sts...[ERR] TeSt
+00000410: 2045 7252 6f52 000a 0f05 0469 6e66 6f00   ErRoR.....info.
+00000420: 0506 6763 6c65 616e 0005 0968 6561 7274  ..gclean...heart
+00000430: 6265 6174 0005 0563 6c6f 636b 0005 2573  beat...clock..%s
+00000440: 6574 636c 6f63 6b20 7965 6172 206d 6f6e  etclock year mon
+00000450: 7468 206d 6461 7920 686f 7572 206d 696e  th mday hour min
+00000460: 2073 6563 0005 036e 7470 0005 0472 7373   sec...ntp...rss
+00000470: 6900 051d 6361 6368 6564 756d 7020 6364  i...cachedump cd
+00000480: 656c 3d22 7267 622e 7064 732f 4e6f 6e65  el="rgb.pds/None
+00000490: 2200 0518 7069 6e6d 6170 206b 6579 3d22  "...pinmap key="
+000004a0: 6468 7470 696e 222f 4e6f 6e65 0005 0668  dhtpin"/None...h
+000004b0: 615f 7374 6100 0512 616c 6172 6d73 2063  a_sta...alarms c
+000004c0: 6c65 616e 3d46 616c 7365 0005 1173 756e  lean=False...sun
+000004d0: 2072 6566 7265 7368 3d46 616c 7365 0005   refresh=False..
+000004e0: 0869 6663 6f6e 6669 6700 050c 6d65 6d6f  .ifconfig...memo
+000004f0: 7279 5f75 7361 6765 0005 0a64 6973 6b5f  ry_usage...disk_
+00000500: 7573 6167 6500 8c6c 1846 012c 2c32 7884  usage..l.F.,,2x.
+00000510: 1084 0e8c 2484 0c84 0784 0b84 0d88 0e84  ....$...........
+00000520: 0f8d 1984 1189 0c84 078e 1184 0c80 1002  ................
+00000530: 2a01 1b03 1c02 1602 5980 1004 2a01 1b05  *.......Y...*...
+00000540: 1c04 1604 5980 1006 1007 2a02 1b08 1c06  ....Y.....*.....
+00000550: 1606 1c07 1607 5980 1009 100a 100b 2a03  ......Y.......*.
+00000560: 1b0c 1c09 1609 1c0a 160a 1c0b 160b 5932  ..............Y2
+00000570: 0016 0e32 0116 1611 0451 2a01 5333 0234  ...2.....Q*.S3.4
+00000580: 0116 1b32 0316 2632 0416 2732 0516 2832  ...2..&2..'2..(2
+00000590: 0616 2b50 2a01 5333 0716 2e32 0816 3211  ..+P*.S3...2..2.
+000005a0: 0451 512a 0253 3309 3401 1633 320a 163c  .QQ*.S3.4..32..<
+000005b0: 100d 2a01 5333 0b16 4632 0c16 4a11 0450  ..*.S3..F2..J..P
+000005c0: 5051 2a03 5333 0d34 0116 4b32 0e16 5332  PQ*.S3.4..K2..S2
+000005d0: 0f16 5451 6310 8640 6418 0e80 0760 2022  ..TQc..@d....` "
+000005e0: 5838 2428 242d 4817 8010 0f10 1010 112a  X8$($-H........*
+000005f0: 031b 121c 0fc0 1c10 c11c 11c2 594a 1959  ............YJ.Y
+00000600: 8010 0f10 1010 112a 031b 131c 0fc0 1c10  .......*........
+00000610: c11c 11c2 594a 015d b234 0059 b034 00b1  ....YJ.].4.Y.4..
+00000620: 3400 f2c3 b134 00c4 125b b4b3 f722 8064  4....4...[...".d
+00000630: f481 3402 c52c 02b5 1014 62b4 1015 6263  ..4..,....b...bc
+00000640: 8500 4816 1680 1760 2030 2728 2824 2d80  ..H....` 0'(($-.
+00000650: 1017 1018 2a02 1b19 1c17 c01c 18c1 59b0  ....*.........Y.
+00000660: b134 0034 01c2 b280 55b2 8255 f4c3 b280  .4.4....U..U....
+00000670: 55b2 8355 f4c4 b3b4 f3c5 125b b5b3 f722  U..U.......[..."
+00000680: 8064 f481 3402 c62c 02b6 1014 62b5 101a  .d..4..,....b...
+00000690: 6263 8c0c d501 a801 1b50 8026 6020 2b2b  bc.......P.&` ++
+000006a0: 4486 0d34 3131 2f2f 2251 292e 0004 8010  D..411//"Q).....
+000006b0: 1c2a 011b 1d1c 1cc1 5980 101e 2a01 1b19  .*......Y...*...
+000006c0: 1c1e c259 2b00 2704 b0b4 2000 02c3 b323  ...Y+.'... ....#
+000006d0: 0014 1f12 5cb1 3400 2301 f434 0136 0134  ....\.4.#..4.6.4
+000006e0: 0159 b323 0214 1f12 0e34 0010 1455 3601  .Y.#.....4...U6.
+000006f0: 3401 59b3 2303 141f 1216 3400 1014 5536  4.Y.#.....4...U6
+00000700: 0134 0159 b323 0414 1fb2 3400 8355 3601  .4.Y.#....4..U6.
+00000710: 3401 59b3 1020 141f b234 0084 5536 0134  4.Y.. ...4..U6.4
+00000720: 0159 4810 b310 2114 1f12 0634 0036 0134  .YH...!....4.6.4
+00000730: 0159 4a0a 59b3 1022 3401 594a 015d b310  .YJ.Y.."4.YJ.]..
+00000740: 2314 1f12 0b34 0036 0134 0159 1024 1425  #....4.6.4.Y.$.%
+00000750: 2504 3601 6301 8458 e302 1655 6b6b 6c80  %.6.c..X...Ukkl.
+00000760: 2f20 2246 6a71 4818 2500 51de 444a 2501  / "FjqH.%.Q.DJ%.
+00000770: 1436 b236 0159 4246 2500 b234 0159 4a21  .6.6.YBF%..4.YJ!
+00000780: 5712 5ddf 445a c349 1025 0114 3610 5614  W.].DZ.I.%..6.V.
+00000790: 1fb2 b336 0236 0159 5151 c328 035d 4a01  ...6.6.YQQ.(.]J.
+000007a0: 5d51 6383 783c 1026 8049 6022 5333 2448  ]Qc.x<.&.I`"S3$H
+000007b0: 1280 1011 100f 2a02 1b12 1c11 c01c 0fc1  ......*.........
+000007c0: 594a 1459 8010 1110 0f2a 021b 131c 11c0  YJ.Y.....*......
+000007d0: 1c0f c159 4a01 5db0 3400 592c 01b1 3400  ...YJ.].4.Y,..4.
+000007e0: 2305 6263 4800 0827 8055 6023 0663 8334  #.bcH..'.U`#.c.4
+000007f0: 400c 2880 5c60 6029 3200 1202 3400 3401  @.(.\``)2...4.4.
+00000800: c023 0714 1f10 2914 25b0 8083 2e02 5536  .#....).%.....U6
+00000810: 0110 2a14 25b0 8386 2e02 5536 01b0 8655  ..*.%.....U6...U
+00000820: b087 5536 0463 0181 3841 0857 6b80 622b  ..U6.c..8A.Wk.b+
+00000830: 00b0 5f4b 0ac1 126d b134 012f 1442 3463  .._K...m.4./.B4c
+00000840: 8430 c802 102b 8067 602b 4225 5380 102c  .0...+.g`+B%S..,
+00000850: 2a01 1b2d 1c2c c059 480f 1209 3400 c1b1  *..-.,.YH...4...
+00000860: 1202 3400 2a02 634a 1d57 125d df44 56c2  ..4.*.cJ.W.].DV.
+00000870: 490c 5023 0814 1fb2 3601 2a02 6351 51c2  I.P#....6.*.cQQ.
+00000880: 2802 5d4a 015d 5163 8238 a901 122e 5e80  (.]J.]Qc.8....^.
+00000890: 7480 0730 2324 8010 2f10 302a 021b 0c1c  t..0#$../.0*....
+000008a0: 2fc1 1c30 c259 b044 44b1 3400 63b2 1331  /..0.Y.DD.4.c..1
+000008b0: 6381 78e2 0418 325f 6061 6263 6480 8280  c.x...2_`abcd...
+000008c0: 0a2b 120a b0b1 b2b3 b4b5 3406 5912 0234  .+........4.Y..4
+000008d0: 0063 8a6c 9e90 0126 3365 5080 9260 462b  .c.l...&3eP..`F+
+000008e0: 232c 2a25 5435 4e2b 222b 4bb0 51de 44e0  #,*%T5N+"+K.Q.D.
+000008f0: 8080 1034 2a01 1b19 1c34 c259 2b00 c332  ...4*....4.Y+..2
+00000900: 00b2 3400 5e34 015f 4b39 c412 66b4 1035  ..4.^4._K9..f..5
+00000910: 3402 472b c5b1 51de 4454 b314 3610 3714  4.G+..Q.DT..6.7.
+00000920: 1fb4 b514 3836 0036 0236 0159 4250 b110  ....86.6.6.YBP..
+00000930: 3714 1fb4 b514 3836 0036 0234 0159 515c  7.....86.6.4.YQ\
+00000940: 5d42 0512 67b3 3401 80d8 4442 b363 1039  ]B..g.4...DB.c.9
+00000950: 6380 103a 2a01 1b19 1c3a c659 4815 b610  c..:*....:.YH...
+00000960: 3b14 1fb0 3601 3401 5923 0914 1fb0 3601  ;...6.4.Y#....6.
+00000970: 634a 0c59 230a 141f b036 0163 4a01 5d51  cJ.Y#....6.cJ.]Q
+00000980: 6301 8170 c140 0858 6b80 9953 b053 534b  c..p.@.Xk..S.SSK
+00000990: 0fc1 b114 5910 5a36 0144 34b1 6759 422f  ....Y.Z6.D4.gYB/
+000009a0: 5163 8650 281c 3c80 aa60 302b 2727 2727  Qc.P(.<..`0+''''
+000009b0: 2727 2727 8010 3d10 3e2a 021b 3f1c 3dc0  ''''..=.>*..?.=.
+000009c0: 1c3e c159 b0b1 3401 1440 103c 3601 c2b2  .>.Y..4..@.<6...
+000009d0: 22ff 3dd8 4447 2c01 b210 4162 63b2 22ff  ".=.DG,...Abc.".
+000009e0: 3ad8 4447 2c01 b210 4262 63b2 22ff 30d8  :.DG,...Bbc.".0.
+000009f0: 4447 2c01 b210 4362 63b2 22ff 26d8 4447  DG,...Cbc.".&.DG
+00000a00: 2c01 b210 4462 632c 01b2 1045 6263 8258  ,...Dbc,...Ebc.X
+00000a10: b101 1246 6880 bb60 4030 2429 8010 4710  ...Fh..`@0$)..G.
+00000a20: 482a 021b 491c 47c1 1c48 c259 b234 00c3  H*..I.G..H.Y.4..
+00000a30: b1b0 3401 b055 b3b0 56b3 6358 0008 4a80  ..4..U..V.cX..J.
+00000a40: c760 1207 3400 6385 30d3 8101 1c4b 696a  .`..4.c.0....Kij
+00000a50: 5080 cf60 6035 2326 2328 2880 104c 104d  P..``5#&#((..L.M
+00000a60: 104e 2a03 1b4f 1c4c c31c 4dc4 1c4e c559  .N*..O.L..M..N.Y
+00000a70: b144 46b4 230b 3401 59b0 4448 b510 50b2  .DF.#.4.Y.DH..P.
+00000a80: 3482 0059 b310 50b2 3482 00c6 b680 d844  4..Y..P.4......D
+00000a90: 472c 01b6 1051 6263 2c01 b610 5262 6381  G,...Qbc,...Rbc.
+00000aa0: 3010 0a53 80df 602b 8010 532a 011b 081c  0..S..`+..S*....
+00000ab0: 53c0 59b0 3400 6350 000a 5480 eb60 4023  S.Y.4.cP..T..`@#
+00000ac0: 0c63                                     .c
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Network.mpy`

 * *Files 2% similar despite different names*

```diff
@@ -23,192 +23,191 @@
 00000160: 636f 6e6e 6563 7400 1464 6973 636f 6e6e  connect..disconn
 00000170: 6563 7400 0a64 6576 6970 0030 5f5f 7365  ect..devip.0__se
 00000180: 745f 7769 6669 5f64 6576 5f73 7461 7469  t_wifi_dev_stati
 00000190: 635f 6970 0006 6e2f 6100 815f 022e 0020  c_ip..n/a.._... 
 000001a0: 7365 745f 6163 6365 7373 5f70 6f69 6e74  set_access_point
 000001b0: 000a 6573 7369 6400 1070 6173 7377 6f72  ..essid..passwor
 000001c0: 6400 1061 7574 686d 6f64 6500 166d 6178  d..authmode..max
-000001d0: 5f63 6c69 656e 7473 0034 6175 746f 5f6e  _clients.4auto_n
-000001e0: 6574 776f 726b 5f63 6f6e 6669 6775 7261  etwork_configura
-000001f0: 7469 6f6e 0008 6e77 6d64 0082 4110 7374  tion..nwmd..A.st
-00000200: 6165 7373 6964 000c 7374 6170 7764 000a  aessid..stapwd..
-00000210: 6170 7077 6400 0e55 6e6b 6e6f 776e 001c  appwd..Unknown..
-00000220: 7374 615f 6869 6768 5f61 7661 696c 000a  sta_high_avail..
-00000230: 7265 7365 7400 123c 6765 6e65 7870 723e  reset..<genexpr>
-00000240: 000a 4e57 5f49 4600 490c 7374 615f 6966  ..NW_IF.I.sta_if
-00000250: 0012 7261 775f 6573 7369 6400 0e72 6177  ..raw_essid..raw
-00000260: 5f70 7764 0012 656e 756d 6572 6174 6500  _pwd..enumerate.
-00000270: 822f 0670 7764 000e 7469 6d65 6f75 7400  ./.pwd..timeout.
-00000280: 8159 823b 0c5f 6573 7369 6400 085f 7077  .Y.;._essid.._pw
-00000290: 6400 125f 6175 7468 6d6f 6465 000b 0a02  d.._authmode....
-000002a0: 0500 000a 0405 0730 2e30 2e30 2e30 0005  .......0.0.0.0..
-000002b0: 0730 2e30 2e30 2e30 0005 0730 2e30 2e30  .0.0.0.0...0.0.0
-000002c0: 2e30 0005 0730 2e30 2e30 2e30 0005 1b5b  .0...0.0.0.0...[
-000002d0: 4552 525d 2073 6574 5f64 6576 5f75 6964  ERR] set_dev_uid
-000002e0: 2065 7272 6f72 3a20 7b7d 0005 2209 7c20   error: {}..".| 
-000002f0: 2d20 5b4e 573a 2053 5441 5d20 4553 5349  - [NW: STA] ESSI
-00000300: 4420 5741 5320 464f 554e 443a 207b 7d00  D WAS FOUND: {}.
-00000310: 052b 097c 202d 205b 4e57 3a20 5354 415d  .+.| - [NW: STA]
-00000320: 2077 6966 6920 7374 6170 7764 2063 6f6e   wifi stapwd con
-00000330: 6669 6720 6572 726f 723a 207b 7d00 0526  fig error: {}..&
-00000340: 5b45 5252 5d5b 5345 5420 5354 415d 2073  [ERR][SET STA] s
-00000350: 7461 7077 6420 636f 6e66 6967 2065 7272  tapwd config err
-00000360: 6f72 3a20 7b7d 000a 0201 0500 0005 1c5b  or: {}.........[
-00000370: 4e57 3a20 5354 415d 2053 4554 2057 4946  NW: STA] SET WIF
-00000380: 4920 5354 4120 4e57 207b 7d00 051c 6468  I STA NW {}...dh
-00000390: 6370 5f68 6f73 746e 616d 6520 636f 6e66  cp_hostname conf
-000003a0: 2065 7272 6f72 3a20 7b7d 0005 2409 7c20   error: {}..$.| 
-000003b0: 5b4e 573a 2053 5441 5d20 414c 5245 4144  [NW: STA] ALREAD
-000003c0: 5920 434f 4e4e 4543 5445 4420 544f 207b  Y CONNECTED TO {
-000003d0: 7d00 0522 097c 205b 4e57 3a20 5354 415d  }..".| [NW: STA]
-000003e0: 2043 4f4e 4e45 4354 2054 4f20 4e45 5457   CONNECT TO NETW
-000003f0: 4f52 4b20 7b7d 0005 2d09 7c20 5b4e 573a  ORK {}..-.| [NW:
-00000400: 2053 5441 5d20 5761 6974 696e 6720 666f   STA] Waiting fo
-00000410: 7220 636f 6e6e 6563 7469 6f6e 2e2e 2e20  r connection... 
-00000420: 7b7d 2073 6563 0005 2b09 7c20 5b4e 573a  {} sec..+.| [NW:
-00000430: 2053 5441 5d20 5769 6669 206e 6574 776f   STA] Wifi netwo
-00000440: 726b 2077 6173 204e 4f54 2066 6f75 6e64  rk was NOT found
-00000450: 3a20 7b7d 0005 2109 7c09 7c20 5b4e 573a  : {}..!.|.| [NW:
-00000460: 2053 5441 5d20 6e65 7477 6f72 6b20 636f   STA] network co
-00000470: 6e66 6967 3a20 7b7d 0005 1c09 7c09 7c20  nfig: {}....|.| 
-00000480: 5b4e 573a 2053 5441 5d20 434f 4e4e 4543  [NW: STA] CONNEC
-00000490: 5445 443a 207b 7d00 051f 5b4e 573a 2053  TED: {}...[NW: S
-000004a0: 5441 5d20 5365 7420 6465 7669 6365 2073  TA] Set device s
-000004b0: 7461 7469 6320 4950 2e00 052d 097c 205b  tatic IP...-.| [
-000004c0: 4e57 3a20 5354 415d 206d 6963 724f 5320  NW: STA] micrOS 
-000004d0: 6465 762e 2053 7461 7469 6349 5020 7265  dev. StaticIP re
-000004e0: 7175 6573 743a 207b 7d00 0527 0909 7c20  quest: {}..'..| 
-000004f0: 5b4e 573a 2053 5441 5d20 5374 6174 6963  [NW: STA] Static
-00000500: 4950 2063 6f6e 662e 2066 6169 6c65 643a  IP conf. failed:
-00000510: 207b 7d00 0522 5f5f 7365 745f 7769 6669   {}.."__set_wifi
-00000520: 5f64 6576 5f73 7461 7469 635f 6970 2065  _dev_static_ip e
-00000530: 7272 6f72 3a20 7b7d 0005 275b 4e57 3a20  rror: {}..'[NW: 
-00000540: 5354 415d 5b53 4b49 505d 2053 7461 7469  STA][SKIP] Stati
-00000550: 6349 5020 636f 6e66 2e3a 207b 7d20 3f20  cIP conf.: {} ? 
-00000560: 7b7d 0005 1f5b 4e57 3a20 5354 415d 2049  {}...[NW: STA] I
-00000570: 5020 7761 7320 6e6f 7420 7374 6f72 6564  P was not stored
-00000580: 3a20 7b7d 0005 3b5b 4e57 3a20 4150 5d20  : {}..;[NW: AP] 
-00000590: 5345 5420 4150 204d 4f44 453a 207b 7d20  SET AP MODE: {} 
-000005a0: 2d20 7b7d 202d 2061 7574 6820 6d6f 6465  - {} - auth mode
-000005b0: 3a20 7b7d 2028 6966 2070 6f73 7369 626c  : {} (if possibl
-000005c0: 6529 0005 125b 4e57 3a20 4150 5d20 436f  e)...[NW: AP] Co
-000005d0: 6e66 6967 7572 6500 0519 5b4e 573a 2041  nfigure...[NW: A
-000005e0: 505d 2043 6f6e 6669 6720 4572 726f 723a  P] Config Error:
-000005f0: 207b 7d00 0517 7c2d 2053 696d 706c 6966   {}...|- Simplif
-00000600: 6965 6420 636f 6e66 6967 2e2e 2e00 051c  ied config......
-00000610: 7c2d 205b 4e57 3a20 4150 5d20 436f 6e66  |- [NW: AP] Conf
-00000620: 6967 2045 7272 6f72 3a20 7b7d 0005 205b  ig Error: {}.. [
-00000630: 4552 525d 2073 6574 5f61 6363 6573 735f  ERR] set_access_
-00000640: 706f 696e 7420 6572 726f 723a 207b 7d00  point error: {}.
-00000650: 051a 5b45 5252 5d5b 5345 5420 4150 5d20  ..[ERR][SET AP] 
-00000660: 636f 6e66 6967 2065 7272 6f72 0005 2009  config error.. .
-00000670: 7c09 7c20 5b4e 573a 2041 505d 206e 6574  |.| [NW: AP] net
-00000680: 776f 726b 2063 6f6e 6669 673a 207b 7d00  work config: {}.
-00000690: 051b 7b7d 206d 6f64 6520 4e4f 4b2c 2077  ..{} mode NOK, w
-000006a0: 6966 6920 6176 6169 6c3a 207b 7d00 050b  ifi avail: {}...
-000006b0: 7b7d 206d 6f64 652c 204f 4b00 8a7c 1836  {} mode, OK..|.6
-000006c0: 0180 102c 2c38 2c32 5283 0784 1184 0784  ...,,8,2R.......
-000006d0: 0884 1589 3684 1c88 2684 1380 1002 2a01  ....6...&.....*.
-000006e0: 1b03 1c02 1602 5980 1004 2a01 1b05 1c04  ......Y...*.....
-000006f0: 1604 5980 1006 1007 1008 2a03 1b09 1c06  ..Y.......*.....
-00000700: 1606 1c07 1607 1c08 1608 5980 100a 2a01  ..........Y...*.
-00000710: 1b0b 1c0a 160a 5980 100c 100d 2a02 1b0e  ......Y.....*...
-00000720: 1c0c 160c 1c0d 160d 5980 100f 1010 2a02  ........Y.....*.
-00000730: 1b11 1c0f 160f 1c10 1610 5951 173f 3200  ..........YQ.?2.
-00000740: 1612 3201 1615 3202 161b 3203 161f 223c  ..2...2...2..."<
-00000750: 2a01 5333 0416 2432 0516 2c83 2a01 5333  *.S3..$2..,.*.S3
-00000760: 0616 3032 0716 3532 0816 3c51 6309 8300  ..02..52..<Qc...
-00000770: 2014 1280 1f60 2623 2327 2923 123f 51de   ....`&##')#.?Q.
-00000780: 4443 2300 6310 13c0 123f 1412 3600 c1b1  DC#.c....?..6...
-00000790: 8055 b182 55d9 4443 1014 c0b0 b12a 0263  .U..U.DC.....*.c
-000007a0: 8440 b802 0c15 8030 221f 4748 1d12 0d10  .@.....0".GH....
-000007b0: 1610 1714 1812 0412 0a34 0034 0114 1910  .........4.4....
-000007c0: 1a36 0136 0134 0259 4a1e 5712 40df 4457  .6.6.4.YJ.W.@.DW
-000007d0: c049 0d12 1023 0114 18b0 3601 3401 5951  .I...#....6.4.YQ
-000007e0: 51c0 2800 5d4a 015d 5163 8150 1806 1b80  Q.(.]J.]Qc.P....
-000007f0: 3712 0412 0834 0014 1c10 1d36 0110 1e34  7....4.....6...4
-00000800: 0214 1936 0063 8a54 9312 261f 4142 4380  ...6.c.T..&.ABC.
-00000810: 3f60 4033 4626 2f2c 221f 412c 3534 1244  ?`@3F&/,".A,54.D
-00000820: b114 2010 2136 0134 015f 4b82 0130 02c3  .. .!6.4._K..0..
-00000830: c4b4 1422 3600 c480 42ea 8057 c5b4 3200  ..."6...B..W..2.
-00000840: b014 2336 005e 3401 dd44 cf80 120f 2302  ..#6.^4..D....#.
-00000850: 1418 b436 0134 0159 4817 b412 45b2 1420  ...6.4.YH...E.. 
-00000860: 1021 3601 b355 3401 1422 3600 2a02 634a  .!6..U4.."6.*.cJ
-00000870: 2a57 1240 df44 63c6 4919 120f 2303 1418  *W.@.Dc.I...#...
-00000880: b636 0134 0159 1210 2304 1418 b636 0134  .6.4.Y..#....6.4
-00000890: 0159 5151 c628 065d 4a01 5d12 0222 8310  .YQQ.(.]J.].."..
-000008a0: 3401 5981 e557 82d7 4390 7f59 42fb 7e23  4.Y..W..C..YB.~#
-000008b0: 0563 0181 68c1 4008 3e4d 8048 53b0 5353  .c..h.@.>M.HS.SS
-000008c0: 4b0e c1b1 8055 1419 101a 3601 6759 4230  K....U....6.gYB0
-000008d0: 5163 9610 e303 4c24 3146 4780 5420 6c27  Qc....L$1FG.T l'
-000008e0: 2727 6227 4742 5a55 276f 6b27 4c48 222c  ''b'GBZU'ok'LH",
-000008f0: 2454 2e26 2249 2c22 3474 3225 2312 0f23  $T.&"I,"4t2%#..#
-00000900: 0614 18b0 3601 3401 5912 0812 0634 01c3  ....6.4.Y....4..
-00000910: b314 2536 0044 47b3 1425 5036 0159 2803  ..%6.DG..%P6.Y(.
-00000920: 1208 1207 3401 c4b4 1425 5236 0159 4811  ....4....%R6.YH.
-00000930: b414 1c10 2612 0c10 2734 0136 8200 594a  ....&...'4.6..YJ
-00000940: 1e57 1240 df44 57c5 490d 120f 2307 1418  .W.@.DW.I...#...
-00000950: b536 0134 0159 5151 c528 055d 4a01 5db4  .6.4.YQQ.(.]J.].
-00000960: 1428 3600 444f 120f 2308 1418 b036 0134  .(6.DO..#....6.4
-00000970: 0159 42a1 8112 1fb4 b0b1 3403 3002 c0c1  .YB.......4.0...
-00000980: b051 ded3 44d9 8012 0f23 0914 18b0 3601  .Q..D....#....6.
-00000990: 3401 59b4 1429 b0b1 3602 5942 5812 0f23  4.Y..)..6.YBX..#
-000009a0: 0a14 18b2 3601 3401 59b2 81e6 c212 0222  ....6.4.Y......"
-000009b0: 8374 3401 59b4 1428 3600 4345 b280 d843  .t4.Y..(6.CE...C
-000009c0: 1cb4 1428 3600 4456 122c b434 0144 4fb4  ...(6.DV.,.4.DO.
-000009d0: 142a 3600 5928 0412 24b0 b134 0263 424e  .*6.Y(..$..4.cBN
-000009e0: 120f 230b 1418 b036 0134 0159 5063 120f  ..#....6.4.YPc..
-000009f0: 230c 1418 1245 b414 1236 0034 0136 0134  #....E...6.4.6.4
-00000a00: 0159 120f 230d 1418 1245 b414 2836 0034  .Y..#....E..(6.4
-00000a10: 0136 0134 0159 120d 102b 1245 b414 1236  .6.4.Y...+.E...6
-00000a20: 0080 5534 0134 0259 1215 3400 59b4 173f  ..U4.4.Y..4.Y..?
-00000a30: b414 2836 0063 8d18 d102 262c 4180 8a27  ..(6.c....&,A..'
-00000a40: 2733 4a1f 272c 2442 2b4d 2c57 512c 120f  '3J.',$B+M,WQ,..
-00000a50: 230e 3401 5912 0c10 2b34 01c1 102d b114  #.4.Y...+4...-..
-00000a60: 2e36 00dd d344 9581 102f b1dd 448e 8112  .6...D.../..D...
-00000a70: 48b0 1412 3600 3401 c2b2 8055 b1dc 44eb  H...6.4....U..D.
-00000a80: 80b2 7f55 1420 102f 3601 8083 2e02 55b1  ...U. ./6.....U.
-00000a90: 1420 102f 3601 8083 2e02 55d9 44cd 8012  . ./6.....U.D...
-00000aa0: 0f23 0f14 18b1 3601 3401 59b1 b280 5648  .#....6.4.Y...VH
-00000ab0: 0fb0 1412 1249 b234 0136 0159 5263 4a2a  .....I.4.6.YRcJ*
-00000ac0: 5712 40df 4463 c349 1912 0f23 1014 18b3  W.@.Dc.I...#....
-00000ad0: 3601 3401 5912 1023 1114 18b3 3601 3401  6.4.Y..#....6.4.
-00000ae0: 5951 51c3 2803 5d4a 015d 424f 120f 2312  YQQ.(.]J.]BO..#.
-00000af0: 1418 b1b2 8055 3602 3401 5942 4c12 0f23  .....U6.4.YBL..#
-00000b00: 1314 18b1 3601 3401 5950 6391 1083 9102  ....6.4.YPc.....
-00000b10: 3630 4a4b 4c80 a620 4e27 2747 2747 4227  60JKL.. N''G'GB'
-00000b20: 7f2c 2247 582c 3e3a 2734 2523 120f 2314  .,"GX,>:'4%#..#.
-00000b30: 1418 b0b1 b236 0334 0159 1208 1207 3401  .....6.4.Y....4.
-00000b40: c3b3 1428 3600 4447 b314 2550 3601 5912  ...(6.DG..%P6.Y.
-00000b50: 0812 0634 01c4 b414 2552 3601 5948 1c12  ...4....%R6.YH..
-00000b60: 0f23 1534 0159 b414 1c10 31b0 1032 b110  .#.4.Y....1..2..
-00000b70: 33b2 1034 8536 8800 594a 6157 1240 df44  3..4.6..YJaW.@.D
-00000b80: d980 c549 4f12 0f23 1614 18b5 3601 3401  ...IO..#....6.4.
-00000b90: 5948 1612 0f23 1734 0159 b414 1c10 31b0  YH...#.4.Y....1.
-00000ba0: 1032 b136 8400 594a 2a57 1240 df44 63c6  .2.6..YJ*W.@.Dc.
-00000bb0: 4919 120f 2318 1418 b636 0134 0159 1210  I...#....6.4.Y..
-00000bc0: 2319 1418 b636 0134 0159 5151 c628 065d  #....6.4.YQQ.(.]
-00000bd0: 4a01 5d51 51c5 2805 5d4a 015d b414 2536  J.]QQ.(.]J.]..%6
-00000be0: 0044 5312 45b4 141c 1031 3601 3401 1245  .DS.E....16.4..E
-00000bf0: b034 01d9 4347 1210 231a 3401 5912 0f23  .4..CG..#.4.Y..#
-00000c00: 1b14 1812 45b4 1412 3600 3401 3601 3401  ....E...6.4.6.4.
-00000c10: 5912 1534 0059 b417 3fb4 1425 3600 6386  Y..4.Y..?..%6.c.
-00000c20: 2838 1835 80cd 2746 5031 4343 3143 2c12  (8.5..'FP1CC1C,.
-00000c30: 0c10 3634 01c0 8042 c280 57c1 b051 de43  ..64...B..W..Q.C
-00000c40: 4b10 14b0 1437 3600 ddd3 4457 1224 120c  K....76...DW.$..
-00000c50: 1038 3401 120c 1039 3401 3402 c2b2 4443  .84....94.4...DC
-00000c60: 1013 6312 3012 0c10 2734 0112 0c10 3a34  ..c.0...'4....:4
-00000c70: 0134 02c2 b244 4310 1463 81e5 5783 d743  .4...DC..c..W..C
-00000c80: b87f 5910 3b63 8a64 8010 263c 80df 6040  ..Y.;c.d..&<..`@
-00000c90: 2734 2742 3246 252e 4c47 4a2b 242e 1208  '4'B2F%.LGJ+$...
-00000ca0: 1207 3401 c012 0c10 3634 0110 13d9 44f6  ..4.....64....D.
-00000cb0: 80b0 1428 3600 43ee 8012 0c10 3834 01c1  ...(6.C.....84..
-00000cc0: 50c2 1244 b114 2010 2136 0134 015f 4b29  P..D.. .!6.4._K)
-00000cd0: 3002 c3c4 b414 2236 00c4 8042 5457 c5b4  0....."6...BTW..
-00000ce0: 3200 b014 2336 005e 3401 dd44 4252 c281  2...#6.^4..DBR..
-00000cf0: e557 82d7 4327 5942 1512 0812 0634 01c6  .W..C'YB.....4..
-00000d00: b243 47b6 1425 3600 434f 8010 3d2a 011b  .CG..%6.CO..=*..
-00000d10: 0b1c 3dc7 59b7 3400 5923 1c14 1812 0c10  ..=.Y.4.Y#......
-00000d20: 3634 01b2 3602 6323 1d14 1812 0c10 3634  64..6.c#......64
-00000d30: 0136 0163 0181 68c1 4008 3e4d 80ed 53b0  .6.c..h.@.>M..S.
-00000d40: 5353 4b0e c1b1 8055 1419 101a 3601 6759  SSK....U....6.gY
-00000d50: 4230 5163                                B0Qc
+000001d0: 5f63 6c69 656e 7473 001c 6175 746f 5f6e  _clients..auto_n
+000001e0: 775f 636f 6e66 6967 0008 6e77 6d64 0082  w_config..nwmd..
+000001f0: 4110 7374 6165 7373 6964 000c 7374 6170  A.staessid..stap
+00000200: 7764 000a 6170 7077 6400 0e55 6e6b 6e6f  wd..appwd..Unkno
+00000210: 776e 001c 7374 615f 6869 6768 5f61 7661  wn..sta_high_ava
+00000220: 696c 000a 7265 7365 7400 123c 6765 6e65  il..reset..<gene
+00000230: 7870 723e 000a 4e57 5f49 4600 490c 7374  xpr>..NW_IF.I.st
+00000240: 615f 6966 0012 7261 775f 6573 7369 6400  a_if..raw_essid.
+00000250: 0e72 6177 5f70 7764 0012 656e 756d 6572  .raw_pwd..enumer
+00000260: 6174 6500 822f 0670 7764 000e 7469 6d65  ate../.pwd..time
+00000270: 6f75 7400 8159 823b 0c5f 6573 7369 6400  out..Y.;._essid.
+00000280: 085f 7077 6400 125f 6175 7468 6d6f 6465  ._pwd.._authmode
+00000290: 000b 0a02 0500 000a 0405 0730 2e30 2e30  ...........0.0.0
+000002a0: 2e30 0005 0730 2e30 2e30 2e30 0005 0730  .0...0.0.0.0...0
+000002b0: 2e30 2e30 2e30 0005 0730 2e30 2e30 2e30  .0.0.0...0.0.0.0
+000002c0: 0005 1b5b 4552 525d 2073 6574 5f64 6576  ...[ERR] set_dev
+000002d0: 5f75 6964 2065 7272 6f72 3a20 7b7d 0005  _uid error: {}..
+000002e0: 2209 7c20 2d20 5b4e 573a 2053 5441 5d20  ".| - [NW: STA] 
+000002f0: 4553 5349 4420 5741 5320 464f 554e 443a  ESSID WAS FOUND:
+00000300: 207b 7d00 052b 097c 202d 205b 4e57 3a20   {}..+.| - [NW: 
+00000310: 5354 415d 2077 6966 6920 7374 6170 7764  STA] wifi stapwd
+00000320: 2063 6f6e 6669 6720 6572 726f 723a 207b   config error: {
+00000330: 7d00 0526 5b45 5252 5d5b 5345 5420 5354  }..&[ERR][SET ST
+00000340: 415d 2073 7461 7077 6420 636f 6e66 6967  A] stapwd config
+00000350: 2065 7272 6f72 3a20 7b7d 000a 0201 0500   error: {}......
+00000360: 0005 1c5b 4e57 3a20 5354 415d 2053 4554  ...[NW: STA] SET
+00000370: 2057 4946 4920 5354 4120 4e57 207b 7d00   WIFI STA NW {}.
+00000380: 051c 6468 6370 5f68 6f73 746e 616d 6520  ..dhcp_hostname 
+00000390: 636f 6e66 2065 7272 6f72 3a20 7b7d 0005  conf error: {}..
+000003a0: 2409 7c20 5b4e 573a 2053 5441 5d20 414c  $.| [NW: STA] AL
+000003b0: 5245 4144 5920 434f 4e4e 4543 5445 4420  READY CONNECTED 
+000003c0: 544f 207b 7d00 0522 097c 205b 4e57 3a20  TO {}..".| [NW: 
+000003d0: 5354 415d 2043 4f4e 4e45 4354 2054 4f20  STA] CONNECT TO 
+000003e0: 4e45 5457 4f52 4b20 7b7d 0005 2d09 7c20  NETWORK {}..-.| 
+000003f0: 5b4e 573a 2053 5441 5d20 5761 6974 696e  [NW: STA] Waitin
+00000400: 6720 666f 7220 636f 6e6e 6563 7469 6f6e  g for connection
+00000410: 2e2e 2e20 7b7d 2073 6563 0005 2b09 7c20  ... {} sec..+.| 
+00000420: 5b4e 573a 2053 5441 5d20 5769 6669 206e  [NW: STA] Wifi n
+00000430: 6574 776f 726b 2077 6173 204e 4f54 2066  etwork was NOT f
+00000440: 6f75 6e64 3a20 7b7d 0005 2109 7c09 7c20  ound: {}..!.|.| 
+00000450: 5b4e 573a 2053 5441 5d20 6e65 7477 6f72  [NW: STA] networ
+00000460: 6b20 636f 6e66 6967 3a20 7b7d 0005 1c09  k config: {}....
+00000470: 7c09 7c20 5b4e 573a 2053 5441 5d20 434f  |.| [NW: STA] CO
+00000480: 4e4e 4543 5445 443a 207b 7d00 051f 5b4e  NNECTED: {}...[N
+00000490: 573a 2053 5441 5d20 5365 7420 6465 7669  W: STA] Set devi
+000004a0: 6365 2073 7461 7469 6320 4950 2e00 052d  ce static IP...-
+000004b0: 097c 205b 4e57 3a20 5354 415d 206d 6963  .| [NW: STA] mic
+000004c0: 724f 5320 6465 762e 2053 7461 7469 6349  rOS dev. StaticI
+000004d0: 5020 7265 7175 6573 743a 207b 7d00 0527  P request: {}..'
+000004e0: 0909 7c20 5b4e 573a 2053 5441 5d20 5374  ..| [NW: STA] St
+000004f0: 6174 6963 4950 2063 6f6e 662e 2066 6169  aticIP conf. fai
+00000500: 6c65 643a 207b 7d00 0522 5f5f 7365 745f  led: {}.."__set_
+00000510: 7769 6669 5f64 6576 5f73 7461 7469 635f  wifi_dev_static_
+00000520: 6970 2065 7272 6f72 3a20 7b7d 0005 275b  ip error: {}..'[
+00000530: 4e57 3a20 5354 415d 5b53 4b49 505d 2053  NW: STA][SKIP] S
+00000540: 7461 7469 6349 5020 636f 6e66 2e3a 207b  taticIP conf.: {
+00000550: 7d20 3f20 7b7d 0005 1f5b 4e57 3a20 5354  } ? {}...[NW: ST
+00000560: 415d 2049 5020 7761 7320 6e6f 7420 7374  A] IP was not st
+00000570: 6f72 6564 3a20 7b7d 0005 3b5b 4e57 3a20  ored: {}..;[NW: 
+00000580: 4150 5d20 5345 5420 4150 204d 4f44 453a  AP] SET AP MODE:
+00000590: 207b 7d20 2d20 7b7d 202d 2061 7574 6820   {} - {} - auth 
+000005a0: 6d6f 6465 3a20 7b7d 2028 6966 2070 6f73  mode: {} (if pos
+000005b0: 7369 626c 6529 0005 125b 4e57 3a20 4150  sible)...[NW: AP
+000005c0: 5d20 436f 6e66 6967 7572 6500 0519 5b4e  ] Configure...[N
+000005d0: 573a 2041 505d 2043 6f6e 6669 6720 4572  W: AP] Config Er
+000005e0: 726f 723a 207b 7d00 0517 7c2d 2053 696d  ror: {}...|- Sim
+000005f0: 706c 6966 6965 6420 636f 6e66 6967 2e2e  plified config..
+00000600: 2e00 051c 7c2d 205b 4e57 3a20 4150 5d20  ....|- [NW: AP] 
+00000610: 436f 6e66 6967 2045 7272 6f72 3a20 7b7d  Config Error: {}
+00000620: 0005 205b 4552 525d 2073 6574 5f61 6363  .. [ERR] set_acc
+00000630: 6573 735f 706f 696e 7420 6572 726f 723a  ess_point error:
+00000640: 207b 7d00 051a 5b45 5252 5d5b 5345 5420   {}...[ERR][SET 
+00000650: 4150 5d20 636f 6e66 6967 2065 7272 6f72  AP] config error
+00000660: 0005 2009 7c09 7c20 5b4e 573a 2041 505d  .. .|.| [NW: AP]
+00000670: 206e 6574 776f 726b 2063 6f6e 6669 673a   network config:
+00000680: 207b 7d00 051b 7b7d 206d 6f64 6520 4e4f   {}...{} mode NO
+00000690: 4b2c 2077 6966 6920 6176 6169 6c3a 207b  K, wifi avail: {
+000006a0: 7d00 050b 7b7d 206d 6f64 652c 204f 4b00  }...{} mode, OK.
+000006b0: 8a7c 1836 0180 102c 2c38 2c32 5283 0784  .|.6...,,8,2R...
+000006c0: 1184 0784 0884 1589 3684 1c88 2684 1380  ........6...&...
+000006d0: 1002 2a01 1b03 1c02 1602 5980 1004 2a01  ..*.......Y...*.
+000006e0: 1b05 1c04 1604 5980 1006 1007 1008 2a03  ......Y.......*.
+000006f0: 1b09 1c06 1606 1c07 1607 1c08 1608 5980  ..............Y.
+00000700: 100a 2a01 1b0b 1c0a 160a 5980 100c 100d  ..*.......Y.....
+00000710: 2a02 1b0e 1c0c 160c 1c0d 160d 5980 100f  *...........Y...
+00000720: 1010 2a02 1b11 1c0f 160f 1c10 1610 5951  ..*...........YQ
+00000730: 173f 3200 1612 3201 1615 3202 161b 3203  .?2...2...2...2.
+00000740: 161f 223c 2a01 5333 0416 2432 0516 2c83  .."<*.S3..$2..,.
+00000750: 2a01 5333 0616 3032 0716 3532 0816 3c51  *.S3..02..52..<Q
+00000760: 6309 8300 2014 1280 1f60 2623 2327 2923  c... ....`&##')#
+00000770: 123f 51de 4443 2300 6310 13c0 123f 1412  .?Q.DC#.c....?..
+00000780: 3600 c1b1 8055 b182 55d9 4443 1014 c0b0  6....U..U.DC....
+00000790: b12a 0263 8440 b802 0c15 8030 221f 4748  .*.c.@.....0".GH
+000007a0: 1d12 0d10 1610 1714 1812 0412 0a34 0034  .............4.4
+000007b0: 0114 1910 1a36 0136 0134 0259 4a1e 5712  .....6.6.4.YJ.W.
+000007c0: 40df 4457 c049 0d12 1023 0114 18b0 3601  @.DW.I...#....6.
+000007d0: 3401 5951 51c0 2800 5d4a 015d 5163 8150  4.YQQ.(.]J.]Qc.P
+000007e0: 1806 1b80 3712 0412 0834 0014 1c10 1d36  ....7....4.....6
+000007f0: 0110 1e34 0214 1936 0063 8a54 9312 261f  ...4...6.c.T..&.
+00000800: 4142 4380 3f60 4033 4626 2f2c 221f 412c  ABC.?`@3F&/,".A,
+00000810: 3534 1244 b114 2010 2136 0134 015f 4b82  54.D.. .!6.4._K.
+00000820: 0130 02c3 c4b4 1422 3600 c480 42ea 8057  .0....."6...B..W
+00000830: c5b4 3200 b014 2336 005e 3401 dd44 cf80  ..2...#6.^4..D..
+00000840: 120f 2302 1418 b436 0134 0159 4817 b412  ..#....6.4.YH...
+00000850: 45b2 1420 1021 3601 b355 3401 1422 3600  E.. .!6..U4.."6.
+00000860: 2a02 634a 2a57 1240 df44 63c6 4919 120f  *.cJ*W.@.Dc.I...
+00000870: 2303 1418 b636 0134 0159 1210 2304 1418  #....6.4.Y..#...
+00000880: b636 0134 0159 5151 c628 065d 4a01 5d12  .6.4.YQQ.(.]J.].
+00000890: 0222 8310 3401 5981 e557 82d7 4390 7f59  ."..4.Y..W..C..Y
+000008a0: 42fb 7e23 0563 0181 68c1 4008 3e4d 8048  B.~#.c..h.@.>M.H
+000008b0: 53b0 5353 4b0e c1b1 8055 1419 101a 3601  S.SSK....U....6.
+000008c0: 6759 4230 5163 9610 e303 4c24 3146 4780  gYB0Qc....L$1FG.
+000008d0: 5420 6c27 2727 6227 4742 5a55 276f 6b27  T l'''b'GBZU'ok'
+000008e0: 4c48 222c 2454 2e26 2249 2c22 3474 3225  LH",$T.&"I,"4t2%
+000008f0: 2312 0f23 0614 18b0 3601 3401 5912 0812  #..#....6.4.Y...
+00000900: 0634 01c3 b314 2536 0044 47b3 1425 5036  .4....%6.DG..%P6
+00000910: 0159 2803 1208 1207 3401 c4b4 1425 5236  .Y(.....4....%R6
+00000920: 0159 4811 b414 1c10 2612 0c10 2734 0136  .YH.....&...'4.6
+00000930: 8200 594a 1e57 1240 df44 57c5 490d 120f  ..YJ.W.@.DW.I...
+00000940: 2307 1418 b536 0134 0159 5151 c528 055d  #....6.4.YQQ.(.]
+00000950: 4a01 5db4 1428 3600 444f 120f 2308 1418  J.]..(6.DO..#...
+00000960: b036 0134 0159 42a1 8112 1fb4 b0b1 3403  .6.4.YB.......4.
+00000970: 3002 c0c1 b051 ded3 44d9 8012 0f23 0914  0....Q..D....#..
+00000980: 18b0 3601 3401 59b4 1429 b0b1 3602 5942  ..6.4.Y..)..6.YB
+00000990: 5812 0f23 0a14 18b2 3601 3401 59b2 81e6  X..#....6.4.Y...
+000009a0: c212 0222 8374 3401 59b4 1428 3600 4345  ...".t4.Y..(6.CE
+000009b0: b280 d843 1cb4 1428 3600 4456 122c b434  ...C...(6.DV.,.4
+000009c0: 0144 4fb4 142a 3600 5928 0412 24b0 b134  .DO..*6.Y(..$..4
+000009d0: 0263 424e 120f 230b 1418 b036 0134 0159  .cBN..#....6.4.Y
+000009e0: 5063 120f 230c 1418 1245 b414 1236 0034  Pc..#....E...6.4
+000009f0: 0136 0134 0159 120f 230d 1418 1245 b414  .6.4.Y..#....E..
+00000a00: 2836 0034 0136 0134 0159 120d 102b 1245  (6.4.6.4.Y...+.E
+00000a10: b414 1236 0080 5534 0134 0259 1215 3400  ...6..U4.4.Y..4.
+00000a20: 59b4 173f b414 2836 0063 8d18 d102 262c  Y..?..(6.c....&,
+00000a30: 4180 8a27 2733 4a1f 272c 2442 2b4d 2c57  A..''3J.',$B+M,W
+00000a40: 512c 120f 230e 3401 5912 0c10 2b34 01c1  Q,..#.4.Y...+4..
+00000a50: 102d b114 2e36 00dd d344 9581 102f b1dd  .-...6...D.../..
+00000a60: 448e 8112 48b0 1412 3600 3401 c2b2 8055  D...H...6.4....U
+00000a70: b1dc 44eb 80b2 7f55 1420 102f 3601 8083  ..D....U. ./6...
+00000a80: 2e02 55b1 1420 102f 3601 8083 2e02 55d9  ..U.. ./6.....U.
+00000a90: 44cd 8012 0f23 0f14 18b1 3601 3401 59b1  D....#....6.4.Y.
+00000aa0: b280 5648 0fb0 1412 1249 b234 0136 0159  ..VH.....I.4.6.Y
+00000ab0: 5263 4a2a 5712 40df 4463 c349 1912 0f23  RcJ*W.@.Dc.I...#
+00000ac0: 1014 18b3 3601 3401 5912 1023 1114 18b3  ....6.4.Y..#....
+00000ad0: 3601 3401 5951 51c3 2803 5d4a 015d 424f  6.4.YQQ.(.]J.]BO
+00000ae0: 120f 2312 1418 b1b2 8055 3602 3401 5942  ..#......U6.4.YB
+00000af0: 4c12 0f23 1314 18b1 3601 3401 5950 6391  L..#....6.4.YPc.
+00000b00: 1083 9102 3630 4a4b 4c80 a620 4e27 2747  ....60JKL.. N''G
+00000b10: 2747 4227 7f2c 2247 582c 3e3a 2734 2523  'GB'.,"GX,>:'4%#
+00000b20: 120f 2314 1418 b0b1 b236 0334 0159 1208  ..#......6.4.Y..
+00000b30: 1207 3401 c3b3 1428 3600 4447 b314 2550  ..4....(6.DG..%P
+00000b40: 3601 5912 0812 0634 01c4 b414 2552 3601  6.Y....4....%R6.
+00000b50: 5948 1c12 0f23 1534 0159 b414 1c10 31b0  YH...#.4.Y....1.
+00000b60: 1032 b110 33b2 1034 8536 8800 594a 6157  .2..3..4.6..YJaW
+00000b70: 1240 df44 d980 c549 4f12 0f23 1614 18b5  .@.D...IO..#....
+00000b80: 3601 3401 5948 1612 0f23 1734 0159 b414  6.4.YH...#.4.Y..
+00000b90: 1c10 31b0 1032 b136 8400 594a 2a57 1240  ..1..2.6..YJ*W.@
+00000ba0: df44 63c6 4919 120f 2318 1418 b636 0134  .Dc.I...#....6.4
+00000bb0: 0159 1210 2319 1418 b636 0134 0159 5151  .Y..#....6.4.YQQ
+00000bc0: c628 065d 4a01 5d51 51c5 2805 5d4a 015d  .(.]J.]QQ.(.]J.]
+00000bd0: b414 2536 0044 5312 45b4 141c 1031 3601  ..%6.DS.E....16.
+00000be0: 3401 1245 b034 01d9 4347 1210 231a 3401  4..E.4..CG..#.4.
+00000bf0: 5912 0f23 1b14 1812 45b4 1412 3600 3401  Y..#....E...6.4.
+00000c00: 3601 3401 5912 1534 0059 b417 3fb4 1425  6.4.Y..4.Y..?..%
+00000c10: 3600 6386 2838 1835 80cd 2746 5031 4343  6.c.(8.5..'FP1CC
+00000c20: 3143 2c12 0c10 3634 01c0 8042 c280 57c1  1C,...64...B..W.
+00000c30: b051 de43 4b10 14b0 1437 3600 ddd3 4457  .Q.CK....76...DW
+00000c40: 1224 120c 1038 3401 120c 1039 3401 3402  .$...84....94.4.
+00000c50: c2b2 4443 1013 6312 3012 0c10 2734 0112  ..DC..c.0...'4..
+00000c60: 0c10 3a34 0134 02c2 b244 4310 1463 81e5  ..:4.4...DC..c..
+00000c70: 5783 d743 b87f 5910 3b63 8a64 8010 263c  W..C..Y.;c.d..&<
+00000c80: 80df 6040 2734 2742 3246 252e 4c47 4a2b  ..`@'4'B2F%.LGJ+
+00000c90: 242e 1208 1207 3401 c012 0c10 3634 0110  $.....4.....64..
+00000ca0: 13d9 44f6 80b0 1428 3600 43ee 8012 0c10  ..D....(6.C.....
+00000cb0: 3834 01c1 50c2 1244 b114 2010 2136 0134  84..P..D.. .!6.4
+00000cc0: 015f 4b29 3002 c3c4 b414 2236 00c4 8042  ._K)0....."6...B
+00000cd0: 5457 c5b4 3200 b014 2336 005e 3401 dd44  TW..2...#6.^4..D
+00000ce0: 4252 c281 e557 82d7 4327 5942 1512 0812  BR...W..C'YB....
+00000cf0: 0634 01c6 b243 47b6 1425 3600 434f 8010  .4...CG..%6.CO..
+00000d00: 3d2a 011b 0b1c 3dc7 59b7 3400 5923 1c14  =*....=.Y.4.Y#..
+00000d10: 1812 0c10 3634 01b2 3602 6323 1d14 1812  ....64..6.c#....
+00000d20: 0c10 3634 0136 0163 0181 68c1 4008 3e4d  ..64.6.c..h.@.>M
+00000d30: 80ed 53b0 5353 4b0e c1b1 8055 1419 101a  ..S.SSK....U....
+00000d40: 3601 6759 4230 5163                      6.gYB0Qc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-00000000: 4d06 001f 8122 1d1c 5461 736b 4d61 6e61  M...."..TaskMana
-00000010: 6765 722e 7079 000f 0e6d 6f64 756c 6573  ger.py...modules
-00000020: 0006 7379 7300 0a64 756d 7073 0008 6a73  ..sys..dumps..js
-00000030: 6f6e 0010 7363 6865 6475 6c65 0081 6710  on..schedule..g.
-00000040: 7561 7379 6e63 696f 001a 636f 6e73 6f6c  uasyncio..consol
+00000000: 4d06 001f 8121 1c1c 5461 736b 4d61 6e61  M....!..TaskMana
+00000010: 6765 722e 7079 000f 1075 6173 796e 6369  ger.py...uasynci
+00000020: 6f00 1073 6368 6564 756c 6500 8167 0e6d  o..schedule..g.m
+00000030: 6f64 756c 6573 0006 7379 7300 0a64 756d  odules..sys..dum
+00000040: 7073 0008 6a73 6f6e 001a 636f 6e73 6f6c  ps..json..consol
 00000050: 655f 7772 6974 6500 1465 7272 6c6f 675f  e_write..errlog_
 00000060: 6164 6400 0a44 6562 7567 000c 6366 6767  add..Debug..cfgg
 00000070: 6574 001a 436f 6e66 6967 4861 6e64 6c65  et..ConfigHandle
 00000080: 7200 1074 6963 6b73 5f6d 7300 1474 6963  r..ticks_ms..tic
 00000090: 6b73 5f64 6966 6600 0a75 7469 6d65 000e  ks_diff..utime..
 000000a0: 636f 6c6c 6563 7400 0467 6300 0a73 696d  collect..gc..sim
 000000b0: 6763 0008 5461 736b 000e 4d61 6e61 6765  gc..Task..Manage
@@ -15,350 +15,346 @@
 000000e0: 0082 2302 3b00 8129 2a65 7865 635f 6c6d  ..#.;..)*exec_lm
 000000f0: 5f70 6970 655f 7363 6865 6475 6c65 0018  _pipe_schedule..
 00000100: 6578 6563 5f6c 6d5f 636f 7265 001a 5f65  exec_lm_core.._e
 00000110: 7865 635f 6c6d 5f63 6f72 6500 0a3e 6a73  xec_lm_core..>js
 00000120: 6f6e 000a 4c4d 5f7b 7d00 0981 5112 696d  on..LM_{}...Q.im
 00000130: 706f 7274 207b 7d00 127b 7d2e 7b7d 287b  port {}..{}.{}({
 00000140: 7d29 0081 552a 6578 6563 5f6c 6d5f 636f  })..U*exec_lm_co
-00000150: 7265 5f73 6368 6564 756c 6500 2314 5f5f  re_schedule.#.__
-00000160: 6361 6c6c 6261 636b 0010 5f5f 696e 6c6f  callback..__inlo
-00000170: 6f70 000e 5f5f 736c 6565 7000 0874 6173  op..__sleep..tas
-00000180: 6b00 0a45 7665 6e74 0008 646f 6e65 0003  k..Event..done..
+00000150: 7265 5f73 6368 6564 756c 6500 2308 7461  re_schedule.#.ta
+00000160: 736b 0014 5f5f 6361 6c6c 6261 636b 0010  sk..__callback..
+00000170: 5f5f 696e 6c6f 6f70 000e 5f5f 736c 6565  __inloop..__slee
+00000180: 7000 0a45 7665 6e74 0008 646f 6e65 0003  p..Event..done..
 00000190: 066f 7574 0006 7461 6700 0e69 735f 6275  .out..tag..is_bu
 000001a0: 7379 000a 5441 534b 5300 812d 0c69 735f  sy..TASKS..-.is_
 000001b0: 7365 7400 145f 5f74 6173 6b5f 6465 6c00  set..__task_del.
 000001c0: 8219 1981 0d1b 0c63 7265 6174 6500 0a61  .......create..a
 000001d0: 696f 7b7d 001c 6765 745f 6576 656e 745f  io{}..get_event_
 000001e0: 6c6f 6f70 0016 6372 6561 7465 5f74 6173  loop..create_tas
 000001f0: 6b00 1263 7265 6174 655f 6c6d 0002 2e00  k..create_lm....
 00000200: 1874 6173 6b5f 7772 6170 7065 7200 0c63  .task_wrapper..c
 00000210: 616e 6365 6c00 1073 6c65 6570 5f6d 7300  ancel..sleep_ms.
 00000220: 0c6d 7367 6f62 6a00 0e5f 5f64 656c 5f5f  .msgobj..__del__
-00000230: 0014 6b65 6570 5f63 6163 6865 0031 145f  ..keep_cache.1._
-00000240: 5f69 6e73 7461 6e63 6500 2a73 6574 5f65  _instance.*set_e
-00000250: 7863 6570 7469 6f6e 5f68 616e 646c 6572  xception_handler
-00000260: 000c 6178 6365 7074 0010 6361 6c6c 6261  ..axcept..callba
-00000270: 636b 0012 6964 6c65 5f74 6173 6b00 0869  ck..idle_task..i
-00000280: 646c 6500 145f 7175 6575 655f 6c65 6e00  dle.._queue_len.
-00000290: 814d 1c5f 7175 6575 655f 6c69 6d69 7465  .M._queue_limite
-000002a0: 7200 1451 5545 5545 5f53 495a 4500 0a4f  r..QUEUE_SIZE..O
-000002b0: 4c4f 4144 0008 6c6f 6f70 000a 736c 6565  LOAD..loop..slee
-000002c0: 7000 146c 6973 745f 7461 736b 7300 044e  p..list_tasks..N
-000002d0: 6f00 0659 6573 000c 7b7d 7b7d 7b7d 0079  o..Yes..{}{}{}.y
-000002e0: 145f 7061 7273 655f 7461 6700 0b08 7368  ._parse_tag...sh
-000002f0: 6f77 000c 7b7d 3a20 7b7d 0007 086b 696c  ow..{}: {}...kil
-00000300: 6c00 0a7b 7d7c 7b7d 0010 4b69 6c6c 3a20  l..{}|{}..Kill: 
-00000310: 7b7d 0004 2c20 0016 7275 6e5f 666f 7265  {}.., ..run_fore
-00000320: 7665 7200 810f 1e73 6572 7665 725f 7461  ver....server_ta
-00000330: 736b 5f6d 7367 000c 7365 7276 6572 0012  sk_msg..server..
-00000340: 3c67 656e 6578 7072 3e00 8231 103c 6c61  <genexpr>..1.<la
-00000350: 6d62 6461 3e00 1874 6173 6b5f 6d61 6e61  mbda>..task_mana
-00000360: 6765 7200 8159 067b 7d0a 0002 2600 8171  ger..Y.{}...&..q
-00000370: 8115 8203 8141 0a64 656c 6179 0010 5374  .....A.delay..St
-00000380: 6172 7420 7b7d 0014 7b7d 2069 7320 4275  art {}..{} is Bu
-00000390: 7379 0024 5f5f 636f 6e76 5f66 756e 635f  sy.$__conv_func_
-000003a0: 7061 7261 6d73 0002 2700 0222 0004 7b7d  params..'.."..{}
-000003b0: 0018 5f5f 666f 726d 6174 5f6f 7574 0008  ..__format_out..
-000003c0: 6865 6c70 0014 3c6c 6973 7463 6f6d 703e  help..<listcomp>
-000003d0: 0012 7465 726d 696e 6174 6500 0e20 7b7d  ..terminate.. {}
-000003e0: 3a20 7b7d 0008 207b 7d2c 000e 6173 796e  : {}.. {},..asyn
-000003f0: 6369 6f00 2f2d 3582 290e 7461 736b 7374  cio./-5.).taskst
-00000400: 7200 4910 6172 675f 6c69 7374 0081 5781  r.I.arg_list..W.
-00000410: 2381 2182 2f82 1381 7710 6578 635f 7479  #.!./...w.exc_ty
-00000420: 7065 0012 6578 635f 7661 6c75 6500 1274  pe..exc_value..t
-00000430: 7261 6365 6261 636b 0006 636c 7300 8235  raceback..cls..5
-00000440: 0e63 6f6e 7465 7874 0082 3381 3d81 4382  .context..3.=.C.
-00000450: 3b06 6d73 6700 106d 7367 5f6c 6973 7400  ;.msg..msg_list.
-00000460: 0a70 6172 616d 0012 656e 756d 6572 6174  .param..enumerat
-00000470: 6500 8179 126a 736f 6e5f 6d6f 6465 000e  e..y.json_mode..
-00000480: 6c6d 5f66 756e 6300 0c6f 7574 7075 7400  lm_func..output.
-00000490: 8117 821b 085f 7461 6700 051a 5b53 494d  ....._tag...[SIM
-000004a0: 554c 4154 4f52 204d 4f44 4520 4743 2049  ULATOR MODE GC I
-000004b0: 4d50 4f52 545d 0005 1a7c 2d5b 4c4d 2d50  MPORT]...|-[LM-P
-000004c0: 4950 455d 2074 6173 6b20 6572 726f 723a  IPE] task error:
-000004d0: 207b 7d00 0517 5b49 5251 2d50 4950 455d   {}...[IRQ-PIPE]
-000004e0: 2065 7272 6f72 3a20 7b7d 0a7b 7d00 051c   error: {}.{}...
-000004f0: 5b45 5252 5d20 6578 6563 5f6c 6d5f 7069  [ERR] exec_lm_pi
-00000500: 7065 2065 7272 6f72 3a20 7b7d 0005 1f65  pe error: {}...e
-00000510: 7865 635f 6c6d 5f70 6970 655f 7363 6865  xec_lm_pipe_sche
-00000520: 6475 6c65 2065 7272 6f72 3a20 7b7d 0005  dule error: {}..
-00000530: 1b5f 6578 6563 5f6c 6d5f 636f 7265 2072  ._exec_lm_core r
-00000540: 652d 696d 706f 7274 207b 7d21 0005 1765  e-import {}!...e
-00000550: 7865 635f 6c6d 5f63 6f72 6520 7b7d 2d3e  xec_lm_core {}->
-00000560: 7b7d 3a20 7b7d 0005 186d 656d 6f72 7920  {}: {}...memory 
-00000570: 616c 6c6f 6361 7469 6f6e 2066 6169 6c65  allocation faile
-00000580: 6400 050e 6973 206e 6f74 2064 6566 696e  d...is not defin
-00000590: 6564 0005 3453 4845 4c4c 3a20 7479 7065  ed..4SHELL: type
-000005a0: 2068 656c 7020 666f 7220 7369 6e67 6c65   help for single
-000005b0: 2077 6f72 6420 636f 6d6d 616e 6473 2028   word commands (
-000005c0: 6275 696c 742d 696e 2900 0543 5348 454c  built-in)..CSHEL
-000005d0: 4c3a 2066 6f72 204c 4d20 6578 6563 3a20  L: for LM exec: 
-000005e0: 5b31 5d28 4c4d 296d 6f64 756c 6520 5b32  [1](LM)module [2
-000005f0: 5d66 756e 6374 696f 6e20 5b33 2e2e 2e5d  ]function [3...]
-00000600: 6f70 7469 6f6e 616c 2070 6172 616d 7300  optional params.
-00000610: 051d 7363 6865 6475 6c65 5f6c 6d5f 6578  ..schedule_lm_ex
-00000620: 6563 207b 7d20 6572 726f 723a 207b 7d00  ec {} error: {}.
-00000630: 0526 2b2b 2b2b 2b2b 205f 5f74 6173 6b5f  .&++++++ __task_
-00000640: 6465 6c20 6b65 6570 5f63 6163 6865 3d7b  del keep_cache={
-00000650: 7d20 2b2b 2b2b 2b2b 0005 1163 616e 2774  } ++++++...can't
-00000660: 2063 616e 6365 6c20 7365 6c66 0005 265b   cancel self..&[
-00000670: 4952 5120 6c69 6d69 7461 7469 6f6e 5d20  IRQ limitation] 
-00000680: 5461 736b 2063 616e 6365 6c20 6572 726f  Task cancel erro
-00000690: 723a 207b 7d00 0519 5b45 5252 5d20 5461  r: {}...[ERR] Ta
-000006a0: 736b 206b 696c 6c20 6572 726f 723a 207b  sk kill error: {
-000006b0: 7d00 0516 5b45 5252 5d20 5461 736b 2e5f  }...[ERR] Task._
-000006c0: 5f64 656c 5f5f 3a20 7b7d 0005 165b 6169  _del__: {}...[ai
-000006d0: 6f5d 2065 7863 6570 7469 6f6e 3a20 7b7d  o] exception: {}
-000006e0: 3a7b 7d00 0519 5b61 696f 5d20 5461 736b  :{}...[aio] Task
-000006f0: 2071 7565 7565 2066 756c 6c3a 207b 7d00   queue full: {}.
-00000700: 050e 692e 642e 6c2e 653a 2032 3030 6d73  ..i.d.l.e: 200ms
-00000710: 0005 1a5b 4552 525d 2049 646c 6520 7461  ...[ERR] Idle ta
-00000720: 736b 2065 7869 7374 733a 207b 7d00 0515  sk exists: {}...
-00000730: 2d2d 2d2d 206d 6963 724f 5320 2074 6f70  ---- micrOS  top
-00000740: 202d 2d2d 2d00 0516 2371 7565 7565 3a20   ----...#queue: 
-00000750: 7b7d 2023 6c6f 6164 3a20 7b7d 250a 0005  {} #load: {}%...
-00000760: 1123 4163 7469 7665 2020 2023 7461 736b  .#Active   #task
-00000770: 4944 0005 114e 6f20 7461 736b 2066 6f75  ID...No task fou
-00000780: 6e64 3a20 7b7d 0005 0b4b 696c 6c3a 207b  nd: {}...Kill: {
-00000790: 7d7c 7b7d 0005 165b 6169 6f5d 206c 6f6f  }|{}...[aio] loo
-000007a0: 7020 7374 6f70 7065 643a 207b 7d00 0541  p stopped: {}..A
-000007b0: 496e 7661 6c69 6420 7461 736b 2063 6d64  Invalid task cmd
-000007c0: 2120 4865 6c70 3a20 7461 736b 206c 6973  ! Help: task lis
-000007d0: 7420 2f20 6b69 6c6c 203c 7461 736b 4944  t / kill <taskID
-000007e0: 3e20 2f20 7368 6f77 203c 7461 736b 4944  > / show <taskID
-000007f0: 3e00 0513 5b45 5252 5d20 5461 736b 206b  >...[ERR] Task k
-00000800: 696c 6c3a 207b 7d00 8c54 2436 0180 0e2c  ill: {}..T$6...,
-00000810: 2c2c 2632 2c52 224f 278f 0789 9189 b884  ,,&2,R"O'.......
-00000820: 1484 0d88 4084 5180 1002 2a01 1b03 1c02  ....@.Q...*.....
-00000830: 1602 5980 1004 2a01 1b05 1c04 1604 5980  ..Y...*.......Y.
-00000840: 1006 2a01 1b07 1c06 1606 5980 511b 0816  ..*.......Y.Q...
-00000850: 7f80 1009 100a 2a02 1b0b 1c09 1609 1c0a  ......*.........
-00000860: 160a 5980 100c 2a01 1b0d 1c0c 160c 5980  ..Y...*.......Y.
-00000870: 100e 100f 2a02 1b10 1c0e 160e 1c0f 160f  ....*...........
-00000880: 5948 0e80 1011 2a01 1b12 1c11 1611 594a  YH....*.......YJ
-00000890: 1759 1109 2300 3401 5980 1011 2a01 1b13  .Y..#.4.Y...*...
-000008a0: 1c11 1611 594a 015d 5432 0010 1434 0216  ....YJ.]T2...4..
-000008b0: 1454 3201 1015 3402 1615 3202 1617 3203  .T2...4...2...2.
-000008c0: 161d 512a 0153 3304 161e 3205 161f 3206  ..Q*.S3...2...2.
-000008d0: 1627 5163 0786 2c10 2c14 8b22 4484 0989  .'Qc..,.,.."D...
-000008e0: 0d88 0c84 0984 0989 128a 1984 1484 0f11  ................
-000008f0: 8100 1681 0110 1416 8102 2c00 1633 3200  ..........,..32.
-00000900: 1628 1181 0332 0134 0116 3250 2a01 5333  .(...2.4..2P*.S3
-00000910: 0216 3632 0316 3832 0416 3a51 512a 0253  ..62..82..:QQ*.S
-00000920: 3305 163b 5151 512a 0353 3306 163f 3207  3..;QQQ*.S3..?2.
-00000930: 1642 3208 1641 3209 1645 5163 0a83 0811  .B2..A2..EQc....
-00000940: 1628 810b 8025 2424 2424 2925 51b0 1829  .(...%$$$$)%Q..)
-00000950: 50b0 182a 94b0 182b 51b0 182c 127f 142d  P..*...+Q..,...-
-00000960: 3600 b018 2e10 2fb0 1830 51b0 1831 5163  6...../..0Q..1Qc
-00000970: 8248 2912 3231 802f 6020 2b4f 4212 1413  .H).21./` +OB...
-00000980: 3314 34b0 5136 02c1 b151 ded3 444b b113  3.4.Q6...Q..DK..
-00000990: 2e14 3536 0043 4252 6350 6384 60aa 011a  ..56.CBRcPc.`...
-000009a0: 3681 0b46 803b 602d 282e 232a 2512 810c  6..F.;`-(.#*%...
-000009b0: 230c 141c b136 0134 0159 b013 2e14 3736  #....6.4.Y....76
-000009c0: 0059 b013 3112 1413 3314 2636 00dd 4452  .Y..1...3.&6..DR
-000009d0: b144 4a12 1413 33b0 1331 535b 56b0 535a  .DJ...3..1S[V.SZ
-000009e0: 182c 1211 3400 5951 6381 2011 1038 810b  .,..4.YQc. ..8..
-000009f0: 8047 6040 28b0 132e 1439 3600 59b0 6382  .G`@(....96.Y.c.
-00000a00: 00a8 041c 3a81 0b81 0d81 0e81 0f80 5060  ....:.........P`
-00000a10: 4028 b013 2e14 3736 0059 1211 3400 5951  @(....76.Y..4.YQ
-00000a20: 6385 00b3 8001 1c3b 810b 4b31 8059 6060  c......;..K1.Y``
-00000a30: 3a4b 624e 27b2 51de 4451 103c 141c 1281  :KbN'.Q.DQ.<....
-00000a40: 0712 1413 3334 0136 0142 41b2 b018 3112  ....34.6.BA...1.
-00000a50: 1414 32b0 1331 3601 4442 5063 127f 143d  ..2..16.DBPc...=
-00000a60: 3600 143e b136 01b0 182c b012 1413 33b2  6..>.6...,....3.
-00000a70: 5652 6387 48c0 8501 243f 810b 4b53 5480  VRc.H...$?..KST.
-00000a80: 6b80 082f 4b62 244e 5852 2910 4014 23b1  k../Kb$NXR).@.#.
-00000a90: 8082 2e02 5536 01b0 1831 1214 1432 b013  ....U6...1...2..
-00000aa0: 3136 0144 4250 63b1 b018 29b2 51de 4445  16.DBPc...).Q.DE
-00000ab0: b013 2a42 41b2 b018 2ab3 51de 4445 b013  ..*BA...*.Q.DE..
-00000ac0: 2b42 4bb3 93d8 4443 b342 43b0 132b b018  +BK...DC.BC..+..
-00000ad0: 2b12 7f14 3d36 0014 3eb0 1441 3600 3601  +...=6..>..A6.6.
-00000ae0: b018 2cb0 1214 1333 b013 3156 5263 8840  ..,....3..1VRc.@
-00000af0: c502 2242 810b 8084 6022 2924 2254 2b35  .."B....`")$"T+5
-00000b00: 484e 2c2b 484f b013 2c51 ded3 44c2 8050  HN,+HO..,Q..D..P
-00000b10: b018 2a48 0ab0 132c 1442 3600 594a 2a57  ..*H...,.B6.YJ*W
-00000b20: 1281 05df 4462 c149 1823 0d12 810a b134  ....Db.I.#.....4
-00000b30: 01dc 444c 120a 230e 141c b136 0134 0159  ..DL..#....6.4.Y
-00000b40: 5151 c128 015d 4a01 5db0 1436 3600 5942  QQ.(.]J.]..66.YB
-00000b50: 4250 634a 2157 1281 05df 4459 c149 0f12  BPcJ!W....DY.I..
-00000b60: 0a23 0f14 1cb1 3601 3401 5950 6351 51c1  .#....6.4.YPcQQ.
-00000b70: 2801 5d4a 015d 5263 841c a140 1941 810b  (.]J.]Rc...@.A..
-00000b80: 8098 8007 202e 3026 2400 127f 1443 2500  .... .0&$....C%.
-00000b90: 132b 3601 5e51 6859 121f 2500 1329 1044  .+6.^QhY..%..).D
-00000ba0: b020 0001 3482 0159 2500 132a 4342 4242  . ..4..Y%..*CBBB
-00000bb0: 4218 2500 132e 1437 3600 5951 6301 8138  B.%....76.YQc..8
-00000bc0: 320c 695b 8117 80a1 1281 2025 0010 30b1  2.i[...... %..0.
-00000bd0: 1468 3600 3403 6383 48c1 020e 4581 0b80  .h6.4.c.H...E...
-00000be0: a722 5648 0cb0 1436 1046 5236 8200 594a  ."VH...6.FR6..YJ
-00000bf0: 1f57 1281 05df 4457 c149 0d12 0a23 1014  .W....DW.I...#..
-00000c00: 1cb1 3601 3401 5951 51c1 2801 5d4a 015d  ..6.4.YQQ.(.]J.]
-00000c10: 5163 8a74 2039 158b b323 2843 8610 8e07  Qc.t 9...#(C....
-00000c20: 6940 890c 8919 8f0d 890f 890f 8910 8920  i@............. 
-00000c30: 890b 0011 8100 1681 0110 1516 8102 5116  ..............Q.
-00000c40: 4811 0c10 1634 0116 5180 1652 b020 0001  H....4..Q..R. ..
-00000c50: 1647 1181 0351 512a 0253 3301 3401 164a  .G...QQ*.S3.4..J
-00000c60: 1181 0332 0234 0116 4e11 8103 3203 3401  ...2.4..N...2.4.
-00000c70: 1650 1181 0332 0434 0116 4c11 8103 5150  .P...2.4..L...QP
-00000c80: 512a 0353 3305 3401 163e 1181 0332 0634  Q*.S3.4..>...2.4
-00000c90: 0116 5511 8103 3207 3401 165a 1181 0332  ..U...2.4..Z...2
-00000ca0: 0834 0116 5c11 8103 3209 3401 165f 1181  .4..\...2.4.._..
-00000cb0: 0332 0a34 0116 6311 8103 320b 3401 1665  .2.4..c...2.4..e
-00000cc0: b063 0c84 703a 1847 5b81 1080 b860 4048  .c..p:.G[....`@H
-00000cd0: 4f4e 5612 1513 4851 de44 7312 8111 2500  ONV...HQ.Ds...%.
-00000ce0: b115 47b1 3601 1215 1848 127f 143d 3600  ..G.6....H...=6.
-00000cf0: 1449 b113 4a36 0159 1215 1348 143e 104b  .I..J6.Y...H.>.K
-00000d00: 1215 144c 3600 1031 104d 3684 0059 1215  ...L6..1.M6..Y..
-00000d10: 1348 6381 50b2 8001 0e4a 5381 1280 c960  .Hc.P....JS....`
-00000d20: 120a 2311 141c b0b1 3602 3401 5951 6381  ..#.....6.4.YQc.
-00000d30: 3c18 064e 80d1 1281 1332 0012 1413 3314  <..N.....2....3.
-00000d40: 4f36 0034 0134 0163 0182 2849 087b 5b80  O6.4.4.c..(I.{[.
-00000d50: d12b 00b0 5f4b 1830 02c1 c2b2 132e 1435  .+.._K.0.......5
-00000d60: 3600 4331 1040 b1dd 442b 812f 1442 2663  6.C1.@..D+./.B&c
-00000d70: 8308 1810 5080 d560 402d 2b26 1215 144e  ....P..`@-+&...N
-00000d80: 3600 1215 1351 db44 5823 1214 1c12 1513  6....Q.DX#......
-00000d90: 5136 01c0 120a b034 0159 1281 05b0 3401  Q6.....4.Y....4.
-00000da0: 6551 638c 50d0 4226 4c80 e160 402b 2922  eQc.P.B&L..`@+)"
-00000db0: 202d 2d2d 4d25 4d39 1f41 3512 1413 3314   ---M%M9.A5...3.
-00000dc0: 3410 4d36 01c0 2313 141c 3600 b018 3048  4.M6..#...6...0H
-00000dd0: 7512 7f14 4322 8148 3601 5e51 6859 127f  u...C".H6.^QhY..
-00000de0: 1443 2281 4836 015e 5168 5912 7f14 4322  .C".H6.^QhY...C"
-00000df0: 8148 3601 5e51 6859 127f 1443 2281 4836  .H6.^QhY...C".H6
-00000e00: 015e 5168 5912 0e34 00c1 127f 1443 2281  .^QhY..4.....C".
-00000e10: 4836 015e 5168 5912 8114 120f 120e 3400  H6.^QhY.......4.
-00000e20: b134 0222 8148 f781 f322 8064 f434 01c2  .4.".H...".d.4..
-00000e30: 1281 1412 1513 52b2 f282 f734 0112 1518  ......R....4....
-00000e40: 5242 8d7f 4a1f 5712 8105 df44 57c3 490d  RB..J.W....DW.I.
-00000e50: 120a 2314 141c b336 0134 0159 5151 c328  ..#....6.4.YQQ.(
-00000e60: 035d 4a01 5db0 132e 1437 3600 5951 6384  .]J.]....76.YQc.
-00000e70: 20d8 8501 183e 4b31 5372 80fa 6040 4a27   ....>K1Sr..`@J'
-00000e80: 3312 8115 b012 6b34 0244 5a12 1514 5036  3.....k4.DZ...P6
-00000e90: 0059 1214 3400 143f 104b b010 53b2 1054  .Y..4..?.K..S..T
-00000ea0: b336 8600 6312 1434 0014 3b10 4bb0 1031  .6..c..4..;.K..1
-00000eb0: b136 8400 6387 0878 1855 9007 6020 2c32  .6..c..x.U..` ,2
-00000ec0: 2f30 2c2a 2912 1513 5112 1514 4e36 00f3  /0,*)...Q...N6..
-00000ed0: c023 1523 1614 1cb0 1215 1352 3602 2317  .#.#.......R6.#.
-00000ee0: 2b03 c112 1413 3314 4f36 005f 4b33 3002  +.....3.O6._K30.
-00000ef0: c2c3 b313 2e14 3536 0044 4410 5642 4210  ......56.DD.VBB.
-00000f00: 57c4 1022 8a12 8107 b434 01f3 f4c5 1058  W..".....4.....X
-00000f10: 141c b4b5 b236 03c6 b114 59b6 3601 5942  .....6....Y.6.YB
-00000f20: 0b12 8116 b134 0163 8708 611e 5a31 9016  .....4.c..a.Z1..
-00000f30: 202b 2623 282c 3c29 2a23 2212 1413 3314   +&#(,<)*#"...3.
-00000f40: 34b0 5136 02c1 b151 de44 cb80 2b00 c2b0  4.Q6...Q.D..+...
-00000f50: 141a 1040 3601 c312 1413 3314 2636 005f  ...@6.....3.&6._
-00000f60: 4b26 c4b4 1418 b380 5536 0144 5912 8107  K&......U6.DY...
-00000f70: b334 0181 d844 4fb3 8155 105b d944 47b2  .4...DO..U.[.DG.
-00000f80: 1459 b436 0159 4218 1281 07b2 3401 80d9  .Y.6.YB.....4...
-00000f90: 4443 2b00 63b2 63b0 2b01 6386 3071 1c5c  DC+.c.c.+.c.0q.\
-00000fa0: 3190 2560 2028 2a28 2a2b 2325 3712 1514  1.%` (*(*+#%7...
-00000fb0: 5ab0 3601 c112 8107 b134 0180 d944 4823  Z.6......4...DH#
-00000fc0: 1814 1cb0 3601 6312 8107 b134 0181 d944  ....6.c....4...D
-00000fd0: 4b12 1413 33b1 8055 5513 3063 2b00 c2b1  K...3..UU.0c+...
-00000fe0: 5f4b 18c3 b214 5910 5d14 1cb3 1214 1333  _K....Y.]......3
-00000ff0: b355 1330 3602 3601 5942 2610 5e14 23b2  .U.06.6.YB&.^.#.
-00001000: 3601 6388 5481 1028 5f31 9035 8007 8309  6.c.T..(_1.5....
-00001010: 2822 2a2b 2a2b 2a23 2527 302e 3200 c112  ("*+*+*#%'0.2...
-00001020: 1514 5ab0 3601 c252 c312 8107 b234 0180  ..Z.6..R.....4..
-00001030: d944 4bb3 2318 141c b036 012a 0263 1281  .DK.#....6.*.c..
-00001040: 07b2 3401 81d9 4455 2319 141c b280 55b3  ..4...DU#.....U.
-00001050: 3602 c4b1 b280 5534 01b4 2a02 632b 00c5  6.....U4..*.c+..
-00001060: b25f 4b18 c6b3 b1b6 3401 e2c3 b514 5910  ._K.....4.....Y.
-00001070: 6014 1cb6 b336 0236 0159 4226 1061 141c  `....6.6.YB&.a..
-00001080: 1062 1423 b536 0136 01c4 b3b4 2a02 6301  .b.#.6.6....*.c.
-00001090: 8458 c902 127c 8121 903d 2b22 592c 1214  .X...|.!.=+"Y,..
-000010a0: 1333 1434 b051 3602 c148 0fb1 51de 4442  .3.4.Q6..H..Q.DB
-000010b0: 5063 b114 4236 0063 4a21 5712 8105 df44  Pc..B6.cJ!W....D
-000010c0: 59c2 490f 120a 231c 141c b236 0134 0159  Y.I...#....6.4.Y
-000010d0: 5063 5151 c228 025d 4a01 5d51 6384 28b8  PcQQ.(.]J.]Qc.(.
-000010e0: 020e 6390 5560 2257 2c48 0d12 7f14 3d36  ..c.U`"W,H....=6
-000010f0: 0014 6336 0059 4a2a 5712 8105 df44 62c0  ..c6.YJ*W....Db.
-00001100: 4918 120a 231a 141c b036 0134 0159 127f  I...#....6.4.Y..
-00001110: 143d 3600 1464 3600 5951 51c0 2800 5d4a  .=6..d6.YQQ.(.]J
-00001120: 015d 5163 8218 2910 6581 1790 602c 2522  .]Qc..).e...`,%"
-00001130: 1214 1333 1434 1066 5136 02c1 b151 de44  ...3.4.fQ6...Q.D
-00001140: 4251 63b0 b118 3051 6387 3cd1 0220 1781  BQc...0Qc.<.. ..
-00001150: 0490 6b60 2042 2942 3027 5a2d 2c2b 4832  ..k` B)B0'Z-,+H2
-00001160: b014 1810 1936 0144 4252 6332 00b0 141a  .....6.DBRc2....
-00001170: 101b 3601 5e34 015f 4b16 c112 1eb1 3401  ..6.^4._K.....4.
-00001180: 434c 1209 2301 141c b136 0134 0159 4228  CL..#....6.4.YB(
-00001190: 4a2e 5712 8105 df44 66c2 491c 1209 2302  J.W....Df.I...#.
-000011a0: 141c b0b2 3602 3401 5912 0a23 0314 1cb2  ....6.4.Y..#....
-000011b0: 3601 3401 5950 6351 51c2 2802 5d4a 015d  6.4.YPcQQ.(.]J.]
-000011c0: 5263 0182 38b9 4008 675b 9074 53b0 5353  Rc..8.@.g[.tS.SS
-000011d0: 4b18 c112 8107 b134 0180 d844 33b1 1468  K......4...D3..h
-000011e0: 3600 141a 3600 6759 4226 5163 8378 c102  6...6.gYB&Qc.x..
-000011f0: 161d 8104 907f 6020 2228 4e2c 480c 1206  ......` "(N,H...
-00001200: 1217 b034 0259 5263 4a21 5712 8105 df44  ...4.YRcJ!W....D
-00001210: 59c1 490f 120a 2304 141c b136 0134 0159  Y.I...#....6.4.Y
-00001220: 5063 5151 c128 015d 4a01 5d51 6383 3caa  PcQQ.(.]J.]Qc.<.
-00001230: 019e 011e 8106 4490 8c80 0726 4486 2c60  ......D....&D.,`
-00001240: 2742 0001 2501 51de 4444 3200 2701 b0b1  'B..%.Q.DD2.'...
-00001250: 2001 02c2 b225 0034 0144 4252 6312 1f25   ....%.4.DBRc..%
-00001260: 0025 0134 0263 0248 090a 6981 1790 9451  .%.4.c.H..i....Q
-00001270: 6395 0893 124c 6a5b 5b81 1890 9747 492d  c....Lj[[....GI-
-00001280: 2d28 2642 2528 3026 2228 3122 2742 5028  -(&B%(0&"(1"'BP(
-00001290: 302e 5122 5c46 2b2e 234e 4c42 1281 07b2  0.Q"\F+.#NLB....
-000012a0: 3401 c310 2cb2 8055 d944 f380 b382 d944  4...,..U.D.....D
-000012b0: 6510 6bb2 8155 d944 5d10 5e14 2312 1514  e.k..U.D].^.#...
-000012c0: 5536 0036 01c4 106c 141c b436 01c4 2501  U6.6...l...6..%.
-000012d0: b434 0159 5263 b382 d844 7b10 5fb2 8155  .4.YRc...D{._..U
-000012e0: d944 5812 1514 5f10 31b2 8255 3682 0030  .DX..._.1..U6..0
-000012f0: 02c5 c625 01b6 3401 5952 6310 5cb2 8155  ...%..4.YRc.\..U
-00001300: d944 5325 0112 1514 5c10 31b2 8255 3682  .DS%....\.1..U6.
-00001310: 0034 0159 5263 2501 231b 3401 5952 63b3  .4.YRc%.#.4.YRc.
-00001320: 82d8 449d 8110 6d25 007f 55dd 4493 8125  ..D...m%..U.D..%
-00001330: 0014 6e7f 3601 c7b7 146f 106d 3601 82d9  ..n.6....o.m6...
-00001340: 4443 5242 4150 c8b7 1470 106d 102f 3602  DCRBAP...p.m./6.
-00001350: 1468 3600 c9b9 1471 3600 4448 1281 14b9  .h6....q6.DH....
-00001360: 3401 4241 51c9 4812 1215 143e 2500 1053  4.BAQ.H....>%..S
-00001370: b810 72b9 3684 01c5 4a1b 5712 8105 df44  ..r.6...J.W....D
-00001380: 53ca 4909 2501 ba34 0159 5263 5151 ca28  S.I.%..4.YRcQQ.(
-00001390: 0a5d 4a01 5d10 4014 2325 0080 822e 0255  .]J.].@.#%.....U
-000013a0: 3601 cbb5 444e 2501 1073 141c bb36 0134  6...DN%..s...6.4
-000013b0: 0159 424c 2501 1074 141c bb36 0134 0159  .YBL%..t...6.4.Y
-000013c0: 5263 5063 9554 9e12 4b1f 8106 4490 cc80  RcPc.T..K...D...
-000013d0: 0883 0d85 0f27 4d2b 1f21 6327 2d42 7d2a  .....'M+.!c'-B}*
-000013e0: 4c4d 5270 492b 6f2d 562a 462b 2646 0a32  LMRpI+o-V*F+&F.2
-000013f0: 00c2 ba20 0101 c3b0 7f55 1020 d9c4 b444  ... .....U. ...D
-00001400: 48b0 807f 2e02 5542 41b0 c512 8107 b534  H.....UBA......4
-00001410: 0182 db44 fc81 1021 141c b580 5536 01b5  ...D...!....U6..
-00001420: 8155 b210 2214 23b5 8251 2e02 5536 0134  .U..".#..Q..U6.4
-00001430: 015b 5ac6 c7c8 4890 01b6 1202 ddd3 444d  .[Z...H.......DM
-00001440: 1281 0810 2414 1cb6 3601 3401 5948 1212  ....$...6.4.YH..
-00001450: 8109 1025 141c b6b7 b836 0334 0127 0a4a  ...%.....6.4.'.J
-00001460: 5057 1281 05df 44c7 80c9 493d b612 810a  PW....D...I=....
-00001470: b934 01dd 446b 120a 2305 141c b636 0134  .4..Dk..#....6.4
-00001480: 0159 1281 0810 2414 1cb6 3601 3401 5912  .Y....$...6.4.Y.
-00001490: 8109 1025 141c b6b7 b836 0334 0127 0a42  ...%.....6.4.'.B
-000014a0: 4712 8105 b934 0165 5151 c928 095d 4a01  G....4.eQQ.(.]J.
-000014b0: 5db3 b4b7 250a 3403 270a b112 810a 250a  ]...%.4.'.....%.
-000014c0: 3401 3401 5952 634a 4957 1281 05df 44c0  4.4.YRcJIW....D.
-000014d0: 80c9 4936 b123 0614 1cb6 b7b9 3603 3401  ..I6.#......6.4.
-000014e0: 5923 0712 810a b934 01dd 434b 2308 1281  Y#.....4..CK#...
-000014f0: 0ab9 3401 dd44 52b6 1202 1426 3600 dd44  ..4..DR....&6..D
-00001500: 4612 02b6 535b 5650 6351 51c9 2809 5d4a  F...S[VPcQQ.(.]J
-00001510: 015d b123 0934 0159 b123 0a34 0159 5263  .].#.4.Y.#.4.YRc
-00001520: 0287 5c59 9c01 7581 1990 d522 2e2d 3625  ..\Y..u....".-6%
-00001530: 2d2c 2a2a 0003 51c1 1076 2500 dd43 4710  -,**..Q..v%..CG.
-00001540: 7725 00dd 4475 3200 1281 1a25 0034 0134  w%..Du2....%.4.4
-00001550: 0127 03b0 b320 0102 1281 1b80 1281 0725  .'... .........%
-00001560: 0334 0182 3403 3401 c1b1 5f4b 0ec2 2500  .4..4.4..._K..%.
-00001570: 1470 b210 7836 0227 0042 3025 0014 7010  .p..x6.'.B0%..p.
-00001580: 2210 6236 0227 0012 8115 b112 6b34 0244  ".b6.'......k4.D
-00001590: 4a25 0014 1cb1 8137 0127 0025 0063 0282  J%.....7.'.%.c..
-000015a0: 1049 087b 5b90 d72b 00b0 5f4b 1530 02c1  .I.{[..+.._K.0..
-000015b0: c2b2 1077 d943 46b2 1076 d944 2eb1 2f14  ...w.CF..v.D../.
-000015c0: 4229 6382 286b 0c7b 5b5b 5b90 d82b 00b2  B)c.(k.{[[[..+..
-000015d0: 5f4b 16c3 2500 2501 b355 2501 b381 f255  _K..%.%..U%....U
-000015e0: 81f2 2e02 552f 1442 2863 853c c004 2479  ....U/.B(c.<..$y
-000015f0: 5b81 1c81 1d81 1e90 e22b 2346 5126 2346  [........+#FQ&#F
-00001600: 2c12 8115 b312 811f 3402 445a b144 4612  ,.......4.DZ.DF.
-00001610: 04b3 3401 6310 5e14 2332 0025 0014 4f36  ..4.c.^.#2.%..O6
-00001620: 0034 0136 0163 b210 7ad9 4455 b144 4612  .4.6.c..z.DU.DF.
-00001630: 04b3 3401 6310 5e14 2332 01b3 3401 3601  ..4.c.^.#2..4.6.
-00001640: 63b3 6302 8168 5908 7b5b 90e6 2b00 b05f  c.c..hY.{[..+.._
-00001650: 4b10 3002 c1c2 107d 141c b1b2 3602 2f14  K.0....}....6./.
-00001660: 422e 6381 4849 087b 5b90 ec2b 00b0 5f4b  B.c.HI.{[..+.._K
-00001670: 0cc1 107e 141c b136 012f 1442 3263 8400  ...~...6./.B2c..
-00001680: c902 1627 8106 a01d 6040 2228 4e2d 480c  ...'....`@"(N-H.
-00001690: 1206 121e b034 0259 5263 4a22 5712 8105  .....4.YRcJ"W...
-000016a0: df44 5ac1 4910 120a 230b 141c b0b1 3602  .DZ.I...#.....6.
-000016b0: 3401 5950 6351 51c1 2801 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
+00000230: 0014 6b65 6570 5f63 6163 6865 0031 064f  ..keep_cache.1.O
+00000240: 424a 002a 7365 745f 6578 6365 7074 696f  BJ.*set_exceptio
+00000250: 6e5f 6861 6e64 6c65 7200 0c61 7863 6570  n_handler..axcep
+00000260: 7400 1063 616c 6c62 6163 6b00 1269 646c  t..callback..idl
+00000270: 655f 7461 736b 0008 6964 6c65 0014 5f71  e_task..idle.._q
+00000280: 7565 7565 5f6c 656e 0081 4d1c 5f71 7565  ueue_len..M._que
+00000290: 7565 5f6c 696d 6974 6572 0014 5155 4555  ue_limiter..QUEU
+000002a0: 455f 5349 5a45 000a 4f4c 4f41 4400 086c  E_SIZE..OLOAD..l
+000002b0: 6f6f 7000 0a73 6c65 6570 0014 6c69 7374  oop..sleep..list
+000002c0: 5f74 6173 6b73 0004 4e6f 0006 5965 7300  _tasks..No..Yes.
+000002d0: 0c7b 7d7b 7d7b 7d00 7914 5f70 6172 7365  .{}{}{}.y._parse
+000002e0: 5f74 6167 000b 0873 686f 7700 0c7b 7d3a  _tag...show..{}:
+000002f0: 207b 7d00 0708 6b69 6c6c 000a 7b7d 7c7b   {}...kill..{}|{
+00000300: 7d00 104b 696c 6c3a 207b 7d00 042c 2000  }..Kill: {}.., .
+00000310: 1672 756e 5f66 6f72 6576 6572 0081 0f1e  .run_forever....
+00000320: 7365 7276 6572 5f74 6173 6b5f 6d73 6700  server_task_msg.
+00000330: 0c73 6572 7665 7200 123c 6765 6e65 7870  .server..<genexp
+00000340: 723e 0082 3110 3c6c 616d 6264 613e 0018  r>..1.<lambda>..
+00000350: 7461 736b 5f6d 616e 6167 6572 0081 5906  task_manager..Y.
+00000360: 7b7d 0a00 0226 0081 7181 1582 0381 410a  {}...&..q.....A.
+00000370: 6465 6c61 7900 1053 7461 7274 207b 7d00  delay..Start {}.
+00000380: 147b 7d20 6973 2042 7573 7900 245f 5f63  .{} is Busy.$__c
+00000390: 6f6e 765f 6675 6e63 5f70 6172 616d 7300  onv_func_params.
+000003a0: 0227 0002 2200 047b 7d00 185f 5f66 6f72  .'.."..{}..__for
+000003b0: 6d61 745f 6f75 7400 0868 656c 7000 143c  mat_out..help..<
+000003c0: 6c69 7374 636f 6d70 3e00 1274 6572 6d69  listcomp>..termi
+000003d0: 6e61 7465 000e 207b 7d3a 207b 7d00 0820  nate.. {}: {}.. 
+000003e0: 7b7d 2c00 0e61 7379 6e63 696f 002f 2d35  {},..asyncio./-5
+000003f0: 8229 0e74 6173 6b73 7472 0049 1061 7267  .).taskstr.I.arg
+00000400: 5f6c 6973 7400 8157 8123 8121 822f 8213  _list..W.#.!./..
+00000410: 1065 7863 5f74 7970 6500 1265 7863 5f76  .exc_type..exc_v
+00000420: 616c 7565 0012 7472 6163 6562 6163 6b00  alue..traceback.
+00000430: 0663 6c73 0082 350e 636f 6e74 6578 7400  .cls..5.context.
+00000440: 8233 813d 8143 823b 066d 7367 0010 6d73  .3.=.C.;.msg..ms
+00000450: 675f 6c69 7374 000a 7061 7261 6d00 1265  g_list..param..e
+00000460: 6e75 6d65 7261 7465 0081 7912 6a73 6f6e  numerate..y.json
+00000470: 5f6d 6f64 6500 0e6c 6d5f 6675 6e63 000c  _mode..lm_func..
+00000480: 6f75 7470 7574 0081 1782 1b08 5f74 6167  output......_tag
+00000490: 0005 1a5b 5349 4d55 4c41 544f 5220 4d4f  ...[SIMULATOR MO
+000004a0: 4445 2047 4320 494d 504f 5254 5d00 051a  DE GC IMPORT]...
+000004b0: 7c2d 5b4c 4d2d 5049 5045 5d20 7461 736b  |-[LM-PIPE] task
+000004c0: 2065 7272 6f72 3a20 7b7d 0005 175b 4952   error: {}...[IR
+000004d0: 512d 5049 5045 5d20 6572 726f 723a 207b  Q-PIPE] error: {
+000004e0: 7d0a 7b7d 0005 1c5b 4552 525d 2065 7865  }.{}...[ERR] exe
+000004f0: 635f 6c6d 5f70 6970 6520 6572 726f 723a  c_lm_pipe error:
+00000500: 207b 7d00 051f 6578 6563 5f6c 6d5f 7069   {}...exec_lm_pi
+00000510: 7065 5f73 6368 6564 756c 6520 6572 726f  pe_schedule erro
+00000520: 723a 207b 7d00 051b 5f65 7865 635f 6c6d  r: {}..._exec_lm
+00000530: 5f63 6f72 6520 7265 2d69 6d70 6f72 7420  _core re-import 
+00000540: 7b7d 2100 0517 6578 6563 5f6c 6d5f 636f  {}!...exec_lm_co
+00000550: 7265 207b 7d2d 3e7b 7d3a 207b 7d00 0518  re {}->{}: {}...
+00000560: 6d65 6d6f 7279 2061 6c6c 6f63 6174 696f  memory allocatio
+00000570: 6e20 6661 696c 6564 0005 0e69 7320 6e6f  n failed...is no
+00000580: 7420 6465 6669 6e65 6400 0534 5348 454c  t defined..4SHEL
+00000590: 4c3a 2074 7970 6520 6865 6c70 2066 6f72  L: type help for
+000005a0: 2073 696e 676c 6520 776f 7264 2063 6f6d   single word com
+000005b0: 6d61 6e64 7320 2862 7569 6c74 2d69 6e29  mands (built-in)
+000005c0: 0005 4353 4845 4c4c 3a20 666f 7220 4c4d  ..CSHELL: for LM
+000005d0: 2065 7865 633a 205b 315d 284c 4d29 6d6f   exec: [1](LM)mo
+000005e0: 6475 6c65 205b 325d 6675 6e63 7469 6f6e  dule [2]function
+000005f0: 205b 332e 2e2e 5d6f 7074 696f 6e61 6c20   [3...]optional 
+00000600: 7061 7261 6d73 0005 1d73 6368 6564 756c  params...schedul
+00000610: 655f 6c6d 5f65 7865 6320 7b7d 2065 7272  e_lm_exec {} err
+00000620: 6f72 3a20 7b7d 0005 1163 616e 2774 2063  or: {}...can't c
+00000630: 616e 6365 6c20 7365 6c66 0005 265b 4952  ancel self..&[IR
+00000640: 5120 6c69 6d69 7461 7469 6f6e 5d20 5461  Q limitation] Ta
+00000650: 736b 2063 616e 6365 6c20 6572 726f 723a  sk cancel error:
+00000660: 207b 7d00 0519 5b45 5252 5d20 5461 736b   {}...[ERR] Task
+00000670: 206b 696c 6c20 6572 726f 723a 207b 7d00   kill error: {}.
+00000680: 0516 5b45 5252 5d20 5461 736b 2e5f 5f64  ..[ERR] Task.__d
+00000690: 656c 5f5f 3a20 7b7d 0005 165b 6169 6f5d  el__: {}...[aio]
+000006a0: 2065 7863 6570 7469 6f6e 3a20 7b7d 3a7b   exception: {}:{
+000006b0: 7d00 0519 5b61 696f 5d20 5461 736b 2071  }...[aio] Task q
+000006c0: 7565 7565 2066 756c 6c3a 207b 7d00 050e  ueue full: {}...
+000006d0: 692e 642e 6c2e 653a 2032 3030 6d73 0005  i.d.l.e: 200ms..
+000006e0: 1a5b 4552 525d 2049 646c 6520 7461 736b  .[ERR] Idle task
+000006f0: 2065 7869 7374 733a 207b 7d00 0515 2d2d   exists: {}...--
+00000700: 2d2d 206d 6963 724f 5320 2074 6f70 202d  -- micrOS  top -
+00000710: 2d2d 2d00 0516 2371 7565 7565 3a20 7b7d  ---...#queue: {}
+00000720: 2023 6c6f 6164 3a20 7b7d 250a 0005 1123   #load: {}%....#
+00000730: 4163 7469 7665 2020 2023 7461 736b 4944  Active   #taskID
+00000740: 0005 114e 6f20 7461 736b 2066 6f75 6e64  ...No task found
+00000750: 3a20 7b7d 0005 0b4b 696c 6c3a 207b 7d7c  : {}...Kill: {}|
+00000760: 7b7d 0005 165b 6169 6f5d 206c 6f6f 7020  {}...[aio] loop 
+00000770: 7374 6f70 7065 643a 207b 7d00 0541 496e  stopped: {}..AIn
+00000780: 7661 6c69 6420 7461 736b 2063 6d64 2120  valid task cmd! 
+00000790: 4865 6c70 3a20 7461 736b 206c 6973 7420  Help: task list 
+000007a0: 2f20 6b69 6c6c 203c 7461 736b 4944 3e20  / kill <taskID> 
+000007b0: 2f20 7368 6f77 203c 7461 736b 4944 3e00  / show <taskID>.
+000007c0: 0513 5b45 5252 5d20 5461 736b 206b 696c  ..[ERR] Task kil
+000007d0: 6c3a 207b 7d00 8c54 2436 0180 0e26 2c2c  l: {}..T$6...&,,
+000007e0: 2c32 2c52 224f 278f 0789 9089 b884 1484  ,2,R"O'.........
+000007f0: 0d88 4084 5180 511b 0216 7f80 1003 2a01  ..@.Q.Q.......*.
+00000800: 1b04 1c03 1603 5980 1005 2a01 1b06 1c05  ......Y...*.....
+00000810: 1605 5980 1007 2a01 1b08 1c07 1607 5980  ..Y...*.......Y.
+00000820: 1009 100a 2a02 1b0b 1c09 1609 1c0a 160a  ....*...........
+00000830: 5980 100c 2a01 1b0d 1c0c 160c 5980 100e  Y...*.......Y...
+00000840: 100f 2a02 1b10 1c0e 160e 1c0f 160f 5948  ..*...........YH
+00000850: 0e80 1011 2a01 1b12 1c11 1611 594a 1759  ....*.......YJ.Y
+00000860: 1109 2300 3401 5980 1011 2a01 1b13 1c11  ..#.4.Y...*.....
+00000870: 1611 594a 015d 5432 0010 1434 0216 1454  ..YJ.]T2...4...T
+00000880: 3201 1015 3402 1615 3202 1617 3203 161d  2...4...2...2...
+00000890: 512a 0153 3304 161e 3205 161f 3206 1627  Q*.S3...2...2..'
+000008a0: 5163 0786 2c10 2c14 8b22 4484 0989 0d88  Qc..,.,.."D.....
+000008b0: 0b84 0984 0989 128a 1984 1484 0f11 8100  ................
+000008c0: 1681 0110 1416 8102 2c00 1633 3200 1628  ........,..32..(
+000008d0: 1181 0332 0134 0116 3250 2a01 5333 0216  ...2.4..2P*.S3..
+000008e0: 3632 0316 3832 0416 3a51 512a 0253 3305  62..82..:QQ*.S3.
+000008f0: 163b 5151 512a 0353 3306 163f 3207 1642  .;QQQ*.S3..?2..B
+00000900: 3208 1641 3209 1645 5163 0a83 0811 1628  2..A2..EQc.....(
+00000910: 810b 8025 2424 2424 2925 51b0 1829 51b0  ...%$$$$)%Q..)Q.
+00000920: 182a 50b0 182b 94b0 182c 127f 142d 3600  .*P..+...,...-6.
+00000930: b018 2e10 2fb0 1830 51b0 1831 5163 8248  ..../..0Q..1Qc.H
+00000940: 2912 3231 802f 6020 2b4f 4212 1413 3314  ).21./` +OB...3.
+00000950: 34b0 5136 02c1 b151 ded3 444b b113 2e14  4.Q6...Q..DK....
+00000960: 3536 0043 4252 6350 6383 70a2 0118 3681  56.CBRcPc.p...6.
+00000970: 0b46 803b 6028 2e23 2a25 b013 2e14 3736  .F.;`(.#*%....76
+00000980: 0059 b013 3112 1413 3314 2636 00dd 4452  .Y..1...3.&6..DR
+00000990: b144 4a12 1413 33b0 1331 535b 56b0 535a  .DJ...3..1S[V.SZ
+000009a0: 1829 1211 3400 5951 6381 2011 1038 810b  .)..4.YQc. ..8..
+000009b0: 8046 6040 28b0 132e 1439 3600 59b0 6382  .F`@(....96.Y.c.
+000009c0: 00a8 041c 3a81 0b81 0c81 0d81 0e80 4f60  ....:.........O`
+000009d0: 4028 b013 2e14 3736 0059 1211 3400 5951  @(....76.Y..4.YQ
+000009e0: 6385 00b3 8001 1c3b 810b 4b31 8058 6060  c......;..K1.X``
+000009f0: 3a4b 624e 27b2 51de 4451 103c 141c 1281  :KbN'.Q.DQ.<....
+00000a00: 0712 1413 3334 0136 0142 41b2 b018 3112  ....34.6.BA...1.
+00000a10: 1414 32b0 1331 3601 4442 5063 127f 143d  ..2..16.DBPc...=
+00000a20: 3600 143e b136 01b0 1829 b012 1413 33b2  6..>.6...)....3.
+00000a30: 5652 6387 48c0 8501 243f 810b 4b53 5480  VRc.H...$?..KST.
+00000a40: 6a80 082f 4b62 244e 5852 2910 4014 23b1  j../Kb$NXR).@.#.
+00000a50: 8082 2e02 5536 01b0 1831 1214 1432 b013  ....U6...1...2..
+00000a60: 3136 0144 4250 63b1 b018 2ab2 51de 4445  16.DBPc...*.Q.DE
+00000a70: b013 2b42 41b2 b018 2bb3 51de 4445 b013  ..+BA...+.Q.DE..
+00000a80: 2c42 4bb3 93d8 4443 b342 43b0 132c b018  ,BK...DC.BC..,..
+00000a90: 2c12 7f14 3d36 0014 3eb0 1441 3600 3601  ,...=6..>..A6.6.
+00000aa0: b018 29b0 1214 1333 b013 3156 5263 8840  ..)....3..1VRc.@
+00000ab0: c502 2242 810b 8083 6022 2924 2254 2b35  .."B....`")$"T+5
+00000ac0: 484e 2c2b 484f b013 2951 ded3 44c2 8050  HN,+HO..)Q..D..P
+00000ad0: b018 2b48 0ab0 1329 1442 3600 594a 2a57  ..+H...).B6.YJ*W
+00000ae0: 1281 05df 4462 c149 1823 0c12 810a b134  ....Db.I.#.....4
+00000af0: 01dc 444c 120a 230d 141c b136 0134 0159  ..DL..#....6.4.Y
+00000b00: 5151 c128 015d 4a01 5db0 1436 3600 5942  QQ.(.]J.]..66.YB
+00000b10: 4250 634a 2157 1281 05df 4459 c149 0f12  BPcJ!W....DY.I..
+00000b20: 0a23 0e14 1cb1 3601 3401 5950 6351 51c1  .#....6.4.YPcQQ.
+00000b30: 2801 5d4a 015d 5263 841c a140 1941 810b  (.]J.]Rc...@.A..
+00000b40: 8097 8007 202e 3026 2400 127f 1443 2500  .... .0&$....C%.
+00000b50: 132c 3601 5e51 6859 121f 2500 132a 1044  .,6.^QhY..%..*.D
+00000b60: b020 0001 3482 0159 2500 132b 4342 4242  . ..4..Y%..+CBBB
+00000b70: 4218 2500 132e 1437 3600 5951 6301 8138  B.%....76.YQc..8
+00000b80: 320c 695b 8116 80a0 1281 1f25 0010 30b1  2.i[.......%..0.
+00000b90: 1468 3600 3403 6383 48c1 020e 4581 0b80  .h6.4.c.H...E...
+00000ba0: a622 5648 0cb0 1436 1046 5236 8200 594a  ."VH...6.FR6..YJ
+00000bb0: 1f57 1281 05df 4457 c149 0d12 0a23 0f14  .W....DW.I...#..
+00000bc0: 1cb1 3601 3401 5951 51c1 2801 5d4a 015d  ..6.4.YQQ.(.]J.]
+00000bd0: 5163 8a74 2039 158b b223 2843 8610 8e07  Qc.t 9...#(C....
+00000be0: 6940 890c 8919 8f0d 890f 890f 8910 8920  i@............. 
+00000bf0: 890b 0011 8100 1681 0110 1516 8102 5116  ..............Q.
+00000c00: 4811 0c10 1634 0116 5180 1652 b020 0001  H....4..Q..R. ..
+00000c10: 1647 1181 0351 512a 0253 3301 3401 164a  .G...QQ*.S3.4..J
+00000c20: 1181 0332 0234 0116 4e11 8103 3203 3401  ...2.4..N...2.4.
+00000c30: 1650 1181 0332 0434 0116 4c11 8103 5150  .P...2.4..L...QP
+00000c40: 512a 0353 3305 3401 163e 1181 0332 0634  Q*.S3.4..>...2.4
+00000c50: 0116 5511 8103 3207 3401 165a 1181 0332  ..U...2.4..Z...2
+00000c60: 0834 0116 5c11 8103 3209 3401 165f 1181  .4..\...2.4.._..
+00000c70: 0332 0a34 0116 6311 8103 320b 3401 1665  .2.4..c...2.4..e
+00000c80: b063 0c84 703a 1847 5b81 0f80 b760 4048  .c..p:.G[....`@H
+00000c90: 4f4e 5612 1513 4851 de44 7312 8110 2500  ONV...HQ.Ds...%.
+00000ca0: b115 47b1 3601 1215 1848 127f 143d 3600  ..G.6....H...=6.
+00000cb0: 1449 b113 4a36 0159 1215 1348 143e 104b  .I..J6.Y...H.>.K
+00000cc0: 1215 144c 3600 1031 104d 3684 0059 1215  ...L6..1.M6..Y..
+00000cd0: 1348 6381 50b2 8001 0e4a 5381 1180 c860  .Hc.P....JS....`
+00000ce0: 120a 2310 141c b0b1 3602 3401 5951 6381  ..#.....6.4.YQc.
+00000cf0: 3c18 064e 80d0 1281 1232 0012 1413 3314  <..N.....2....3.
+00000d00: 4f36 0034 0134 0163 0182 2849 087b 5b80  O6.4.4.c..(I.{[.
+00000d10: d02b 00b0 5f4b 1830 02c1 c2b2 132e 1435  .+.._K.0.......5
+00000d20: 3600 4331 1040 b1dd 442b 812f 1442 2663  6.C1.@..D+./.B&c
+00000d30: 8308 1810 5080 d460 402d 2b26 1215 144e  ....P..`@-+&...N
+00000d40: 3600 1215 1351 db44 5823 1114 1c12 1513  6....Q.DX#......
+00000d50: 5136 01c0 120a b034 0159 1281 05b0 3401  Q6.....4.Y....4.
+00000d60: 6551 638c 50d0 4226 4c80 e060 402b 2922  eQc.P.B&L..`@+)"
+00000d70: 202d 2d2d 4d25 4d39 1f41 3512 1413 3314   ---M%M9.A5...3.
+00000d80: 3410 4d36 01c0 2312 141c 3600 b018 3048  4.M6..#...6...0H
+00000d90: 7512 7f14 4322 8148 3601 5e51 6859 127f  u...C".H6.^QhY..
+00000da0: 1443 2281 4836 015e 5168 5912 7f14 4322  .C".H6.^QhY...C"
+00000db0: 8148 3601 5e51 6859 127f 1443 2281 4836  .H6.^QhY...C".H6
+00000dc0: 015e 5168 5912 0e34 00c1 127f 1443 2281  .^QhY..4.....C".
+00000dd0: 4836 015e 5168 5912 8113 120f 120e 3400  H6.^QhY.......4.
+00000de0: b134 0222 8148 f781 f322 8064 f434 01c2  .4.".H...".d.4..
+00000df0: 1281 1312 1513 52b2 f282 f734 0112 1518  ......R....4....
+00000e00: 5242 8d7f 4a1f 5712 8105 df44 57c3 490d  RB..J.W....DW.I.
+00000e10: 120a 2313 141c b336 0134 0159 5151 c328  ..#....6.4.YQQ.(
+00000e20: 035d 4a01 5db0 132e 1437 3600 5951 6384  .]J.]....76.YQc.
+00000e30: 20d8 8501 183e 4b31 5372 80f9 6040 4a27   ....>K1Sr..`@J'
+00000e40: 3312 8114 b012 6b34 0244 5a12 1514 5036  3.....k4.DZ...P6
+00000e50: 0059 1214 3400 143f 104b b010 53b2 1054  .Y..4..?.K..S..T
+00000e60: b336 8600 6312 1434 0014 3b10 4bb0 1031  .6..c..4..;.K..1
+00000e70: b136 8400 6387 0878 1855 9006 6020 2c32  .6..c..x.U..` ,2
+00000e80: 2f30 2c2a 2912 1513 5112 1514 4e36 00f3  /0,*)...Q...N6..
+00000e90: c023 1423 1514 1cb0 1215 1352 3602 2316  .#.#.......R6.#.
+00000ea0: 2b03 c112 1413 3314 4f36 005f 4b33 3002  +.....3.O6._K30.
+00000eb0: c2c3 b313 2e14 3536 0044 4410 5642 4210  ......56.DD.VBB.
+00000ec0: 57c4 1022 8a12 8107 b434 01f3 f4c5 1058  W..".....4.....X
+00000ed0: 141c b4b5 b236 03c6 b114 59b6 3601 5942  .....6....Y.6.YB
+00000ee0: 0b12 8115 b134 0163 8708 611e 5a31 9015  .....4.c..a.Z1..
+00000ef0: 202b 2623 282c 3c29 2a23 2212 1413 3314   +&#(,<)*#"...3.
+00000f00: 34b0 5136 02c1 b151 de44 cb80 2b00 c2b0  4.Q6...Q.D..+...
+00000f10: 141a 1040 3601 c312 1413 3314 2636 005f  ...@6.....3.&6._
+00000f20: 4b26 c4b4 1418 b380 5536 0144 5912 8107  K&......U6.DY...
+00000f30: b334 0181 d844 4fb3 8155 105b d944 47b2  .4...DO..U.[.DG.
+00000f40: 1459 b436 0159 4218 1281 07b2 3401 80d9  .Y.6.YB.....4...
+00000f50: 4443 2b00 63b2 63b0 2b01 6386 3071 1c5c  DC+.c.c.+.c.0q.\
+00000f60: 3190 2460 2028 2a28 2a2b 2325 3712 1514  1.$` (*(*+#%7...
+00000f70: 5ab0 3601 c112 8107 b134 0180 d944 4823  Z.6......4...DH#
+00000f80: 1714 1cb0 3601 6312 8107 b134 0181 d944  ....6.c....4...D
+00000f90: 4b12 1413 33b1 8055 5513 3063 2b00 c2b1  K...3..UU.0c+...
+00000fa0: 5f4b 18c3 b214 5910 5d14 1cb3 1214 1333  _K....Y.]......3
+00000fb0: b355 1330 3602 3601 5942 2610 5e14 23b2  .U.06.6.YB&.^.#.
+00000fc0: 3601 6388 5481 1028 5f31 9034 8007 8309  6.c.T..(_1.4....
+00000fd0: 2822 2a2b 2a2b 2a23 2527 302e 3200 c112  ("*+*+*#%'0.2...
+00000fe0: 1514 5ab0 3601 c252 c312 8107 b234 0180  ..Z.6..R.....4..
+00000ff0: d944 4bb3 2317 141c b036 012a 0263 1281  .DK.#....6.*.c..
+00001000: 07b2 3401 81d9 4455 2318 141c b280 55b3  ..4...DU#.....U.
+00001010: 3602 c4b1 b280 5534 01b4 2a02 632b 00c5  6.....U4..*.c+..
+00001020: b25f 4b18 c6b3 b1b6 3401 e2c3 b514 5910  ._K.....4.....Y.
+00001030: 6014 1cb6 b336 0236 0159 4226 1061 141c  `....6.6.YB&.a..
+00001040: 1062 1423 b536 0136 01c4 b3b4 2a02 6301  .b.#.6.6....*.c.
+00001050: 8458 c902 127c 8120 903c 2b22 592c 1214  .X...|. .<+"Y,..
+00001060: 1333 1434 b051 3602 c148 0fb1 51de 4442  .3.4.Q6..H..Q.DB
+00001070: 5063 b114 4236 0063 4a21 5712 8105 df44  Pc..B6.cJ!W....D
+00001080: 59c2 490f 120a 231b 141c b236 0134 0159  Y.I...#....6.4.Y
+00001090: 5063 5151 c228 025d 4a01 5d51 6384 28b8  PcQQ.(.]J.]Qc.(.
+000010a0: 020e 6390 5460 2257 2c48 0d12 7f14 3d36  ..c.T`"W,H....=6
+000010b0: 0014 6336 0059 4a2a 5712 8105 df44 62c0  ..c6.YJ*W....Db.
+000010c0: 4918 120a 2319 141c b036 0134 0159 127f  I...#....6.4.Y..
+000010d0: 143d 3600 1464 3600 5951 51c0 2800 5d4a  .=6..d6.YQQ.(.]J
+000010e0: 015d 5163 8218 2910 6581 1690 5f2c 2522  .]Qc..).e..._,%"
+000010f0: 1214 1333 1434 1066 5136 02c1 b151 de44  ...3.4.fQ6...Q.D
+00001100: 4251 63b0 b118 3051 6387 3cd1 0220 1781  BQc...0Qc.<.. ..
+00001110: 0490 6a60 2042 2942 3027 5a2d 2c2b 4832  ..j` B)B0'Z-,+H2
+00001120: b014 1810 1936 0144 4252 6332 00b0 141a  .....6.DBRc2....
+00001130: 101b 3601 5e34 015f 4b16 c112 1eb1 3401  ..6.^4._K.....4.
+00001140: 434c 1209 2301 141c b136 0134 0159 4228  CL..#....6.4.YB(
+00001150: 4a2e 5712 8105 df44 66c2 491c 1209 2302  J.W....Df.I...#.
+00001160: 141c b0b2 3602 3401 5912 0a23 0314 1cb2  ....6.4.Y..#....
+00001170: 3601 3401 5950 6351 51c2 2802 5d4a 015d  6.4.YPcQQ.(.]J.]
+00001180: 5263 0182 38b9 4008 675b 9073 53b0 5353  Rc..8.@.g[.sS.SS
+00001190: 4b18 c112 8107 b134 0180 d844 33b1 1468  K......4...D3..h
+000011a0: 3600 141a 3600 6759 4226 5163 8378 c102  6...6.gYB&Qc.x..
+000011b0: 161d 8104 907e 6020 2228 4e2c 480c 1203  .....~` "(N,H...
+000011c0: 1217 b034 0259 5263 4a21 5712 8105 df44  ...4.YRcJ!W....D
+000011d0: 59c1 490f 120a 2304 141c b136 0134 0159  Y.I...#....6.4.Y
+000011e0: 5063 5151 c128 015d 4a01 5d51 6383 3caa  PcQQ.(.]J.]Qc.<.
+000011f0: 019e 011e 8106 4490 8b80 0726 4486 2c60  ......D....&D.,`
+00001200: 2742 0001 2501 51de 4444 3200 2701 b0b1  'B..%.Q.DD2.'...
+00001210: 2001 02c2 b225 0034 0144 4252 6312 1f25   ....%.4.DBRc..%
+00001220: 0025 0134 0263 0248 090a 6981 1690 9351  .%.4.c.H..i....Q
+00001230: 6395 0893 124c 6a5b 5b81 1790 9647 492d  c....Lj[[....GI-
+00001240: 2d28 2642 2528 3026 2228 3122 2742 5028  -(&B%(0&"(1"'BP(
+00001250: 302e 5122 5c46 2b2e 234e 4c42 1281 07b2  0.Q"\F+.#NLB....
+00001260: 3401 c310 29b2 8055 d944 f380 b382 d944  4...)..U.D.....D
+00001270: 6510 6bb2 8155 d944 5d10 5e14 2312 1514  e.k..U.D].^.#...
+00001280: 5536 0036 01c4 106c 141c b436 01c4 2501  U6.6...l...6..%.
+00001290: b434 0159 5263 b382 d844 7b10 5fb2 8155  .4.YRc...D{._..U
+000012a0: d944 5812 1514 5f10 31b2 8255 3682 0030  .DX..._.1..U6..0
+000012b0: 02c5 c625 01b6 3401 5952 6310 5cb2 8155  ...%..4.YRc.\..U
+000012c0: d944 5325 0112 1514 5c10 31b2 8255 3682  .DS%....\.1..U6.
+000012d0: 0034 0159 5263 2501 231a 3401 5952 63b3  .4.YRc%.#.4.YRc.
+000012e0: 82d8 449d 8110 6d25 007f 55dd 4493 8125  ..D...m%..U.D..%
+000012f0: 0014 6e7f 3601 c7b7 146f 106d 3601 82d9  ..n.6....o.m6...
+00001300: 4443 5242 4150 c8b7 1470 106d 102f 3602  DCRBAP...p.m./6.
+00001310: 1468 3600 c9b9 1471 3600 4448 1281 13b9  .h6....q6.DH....
+00001320: 3401 4241 51c9 4812 1215 143e 2500 1053  4.BAQ.H....>%..S
+00001330: b810 72b9 3684 01c5 4a1b 5712 8105 df44  ..r.6...J.W....D
+00001340: 53ca 4909 2501 ba34 0159 5263 5151 ca28  S.I.%..4.YRcQQ.(
+00001350: 0a5d 4a01 5d10 4014 2325 0080 822e 0255  .]J.].@.#%.....U
+00001360: 3601 cbb5 444e 2501 1073 141c bb36 0134  6...DN%..s...6.4
+00001370: 0159 424c 2501 1074 141c bb36 0134 0159  .YBL%..t...6.4.Y
+00001380: 5263 5063 9554 9e12 4b1f 8106 4490 cb80  RcPc.T..K...D...
+00001390: 0883 0d85 0f27 4d2b 1f21 6327 2d42 7d2a  .....'M+.!c'-B}*
+000013a0: 4c4d 5270 492b 6f2d 562a 462b 2646 0a32  LMRpI+o-V*F+&F.2
+000013b0: 00c2 ba20 0101 c3b0 7f55 1020 d9c4 b444  ... .....U. ...D
+000013c0: 48b0 807f 2e02 5542 41b0 c512 8107 b534  H.....UBA......4
+000013d0: 0182 db44 fc81 1021 141c b580 5536 01b5  ...D...!....U6..
+000013e0: 8155 b210 2214 23b5 8251 2e02 5536 0134  .U..".#..Q..U6.4
+000013f0: 015b 5ac6 c7c8 4890 01b6 1205 ddd3 444d  .[Z...H.......DM
+00001400: 1281 0810 2414 1cb6 3601 3401 5948 1212  ....$...6.4.YH..
+00001410: 8109 1025 141c b6b7 b836 0334 0127 0a4a  ...%.....6.4.'.J
+00001420: 5057 1281 05df 44c7 80c9 493d b612 810a  PW....D...I=....
+00001430: b934 01dd 446b 120a 2305 141c b636 0134  .4..Dk..#....6.4
+00001440: 0159 1281 0810 2414 1cb6 3601 3401 5912  .Y....$...6.4.Y.
+00001450: 8109 1025 141c b6b7 b836 0334 0127 0a42  ...%.....6.4.'.B
+00001460: 4712 8105 b934 0165 5151 c928 095d 4a01  G....4.eQQ.(.]J.
+00001470: 5db3 b4b7 250a 3403 270a b112 810a 250a  ]...%.4.'.....%.
+00001480: 3401 3401 5952 634a 4957 1281 05df 44c0  4.4.YRcJIW....D.
+00001490: 80c9 4936 b123 0614 1cb6 b7b9 3603 3401  ..I6.#......6.4.
+000014a0: 5923 0712 810a b934 01dd 434b 2308 1281  Y#.....4..CK#...
+000014b0: 0ab9 3401 dd44 52b6 1205 1426 3600 dd44  ..4..DR....&6..D
+000014c0: 4612 05b6 535b 5650 6351 51c9 2809 5d4a  F...S[VPcQQ.(.]J
+000014d0: 015d b123 0934 0159 b123 0a34 0159 5263  .].#.4.Y.#.4.YRc
+000014e0: 0287 5c59 9c01 7581 1890 d422 2e2d 3625  ..\Y..u....".-6%
+000014f0: 2d2c 2a2a 0003 51c1 1076 2500 dd43 4710  -,**..Q..v%..CG.
+00001500: 7725 00dd 4475 3200 1281 1925 0034 0134  w%..Du2....%.4.4
+00001510: 0127 03b0 b320 0102 1281 1a80 1281 0725  .'... .........%
+00001520: 0334 0182 3403 3401 c1b1 5f4b 0ec2 2500  .4..4.4..._K..%.
+00001530: 1470 b210 7836 0227 0042 3025 0014 7010  .p..x6.'.B0%..p.
+00001540: 2210 6236 0227 0012 8114 b112 6b34 0244  ".b6.'......k4.D
+00001550: 4a25 0014 1cb1 8137 0127 0025 0063 0282  J%.....7.'.%.c..
+00001560: 1049 087b 5b90 d62b 00b0 5f4b 1530 02c1  .I.{[..+.._K.0..
+00001570: c2b2 1077 d943 46b2 1076 d944 2eb1 2f14  ...w.CF..v.D../.
+00001580: 4229 6382 286b 0c7b 5b5b 5b90 d72b 00b2  B)c.(k.{[[[..+..
+00001590: 5f4b 16c3 2500 2501 b355 2501 b381 f255  _K..%.%..U%....U
+000015a0: 81f2 2e02 552f 1442 2863 853c c004 2479  ....U/.B(c.<..$y
+000015b0: 5b81 1b81 1c81 1d90 e12b 2346 5126 2346  [........+#FQ&#F
+000015c0: 2c12 8114 b312 811e 3402 445a b144 4612  ,.......4.DZ.DF.
+000015d0: 07b3 3401 6310 5e14 2332 0025 0014 4f36  ..4.c.^.#2.%..O6
+000015e0: 0034 0136 0163 b210 7ad9 4455 b144 4612  .4.6.c..z.DU.DF.
+000015f0: 07b3 3401 6310 5e14 2332 01b3 3401 3601  ..4.c.^.#2..4.6.
+00001600: 63b3 6302 8168 5908 7b5b 90e5 2b00 b05f  c.c..hY.{[..+.._
+00001610: 4b10 3002 c1c2 107d 141c b1b2 3602 2f14  K.0....}....6./.
+00001620: 422e 6381 4849 087b 5b90 eb2b 00b0 5f4b  B.c.HI.{[..+.._K
+00001630: 0cc1 107e 141c b136 012f 1442 3263 8400  ...~...6./.B2c..
+00001640: c902 1627 8106 a01c 6040 2228 4e2d 480c  ...'....`@"(N-H.
+00001650: 1203 121e b034 0259 5263 4a22 5712 8105  .....4.YRcJ"W...
+00001660: df44 5ac1 4910 120a 230b 141c b0b1 3602  .DZ.I...#.....6.
+00001670: 3401 5950 6351 51c1 2801 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 00000000: 4d06 001f 2309 126d 6963 724f 532e 7079  M...#..micrOS.py
 00000010: 000f 0e4d 616e 6167 6572 0016 5461 736b  ...Manager..Task
 00000020: 4d61 6e61 6765 7200 1853 6f63 6b65 7453  Manager..SocketS
-00000030: 6572 7665 7200 3461 7574 6f5f 6e65 7477  erver.4auto_netw
-00000040: 6f72 6b5f 636f 6e66 6967 7572 6174 696f  ork_configuratio
-00000050: 6e00 0e4e 6574 776f 726b 0016 626f 6f74  n..Network..boot
-00000060: 7570 5f68 6f6f 6b00 1c70 726f 6669 6c69  up_hook..profili
-00000070: 6e67 5f69 6e66 6f00 0a48 6f6f 6b73 001e  ng_info..Hooks..
-00000080: 656e 6162 6c65 496e 7465 7272 7570 7400  enableInterrupt.
-00000090: 1465 6e61 626c 6543 726f 6e00 2049 6e74  .enableCron. Int
-000000a0: 6572 7275 7074 4861 6e64 6c65 7200 1a69  erruptHandler..i
-000000b0: 6e69 7445 7665 6e74 4952 5173 0014 6572  nitEventIRQs..er
-000000c0: 726c 6f67 5f61 6464 000a 4465 6275 6700  rlog_add..Debug.
-000000d0: 106e 7470 5f74 696d 6500 0e73 756e 7469  .ntp_time..sunti
-000000e0: 6d65 0008 5469 6d65 001c 7361 6665 5f62  me..Time..safe_b
-000000f0: 6f6f 745f 686f 6f6b 0081 2922 696e 7465  oot_hook..)"inte
-00000100: 7272 7570 745f 6861 6e64 6c65 7200 3465  rrupt_handler.4e
-00000110: 7874 6572 6e61 6c5f 696e 7465 7272 7570  xternal_interrup
-00000120: 745f 6861 6e64 6c65 7200 0c6d 6963 724f  t_handler..micrO
-00000130: 5300 0a6c 6162 656c 0006 5354 4100 0c75  S..label..STA..u
-00000140: 7074 696d 6500 823f 1663 7265 6174 655f  ptime..?.create_
-00000150: 7461 736b 0014 7275 6e5f 7365 7276 6572  task..run_server
-00000160: 0006 7461 6700 0c73 6572 7665 7200 1672  ..tag..server..r
-00000170: 756e 5f66 6f72 6576 6572 0049 8177 052b  un_forever.I.w.+
-00000180: 5b6d 6963 724f 5320 6d61 696e 5d20 486f  [micrOS main] Ho
-00000190: 6f6b 732e 626f 6f74 7570 5f68 6f6f 6b28  oks.bootup_hook(
-000001a0: 2920 6572 726f 723a 207b 7d00 051e 5b45  ) error: {}...[E
-000001b0: 5252 5d20 7361 6665 5f62 6f6f 745f 686f  RR] safe_boot_ho
-000001c0: 6f6b 2065 7272 6f72 3a20 7b7d 0005 465b  ok error: {}..F[
-000001d0: 6d69 6372 4f53 206d 6169 6e5d 2049 6e74  micrOS main] Int
-000001e0: 6572 7275 7074 4861 6e64 6c65 722e 656e  erruptHandler.en
-000001f0: 6162 6c65 496e 7465 7272 7570 742f 4372  ableInterrupt/Cr
-00000200: 6f6e 496e 7465 7272 7570 7420 6572 726f  onInterrupt erro
-00000210: 723a 207b 7d00 0521 5b45 5252 5d20 696e  r: {}..![ERR] in
-00000220: 7465 7272 7570 745f 6861 6e64 6c65 7220  terrupt_handler 
-00000230: 6572 726f 723a 207b 7d00 0536 5b6d 6963  error: {}..6[mic
-00000240: 724f 5320 6d61 696e 5d20 496e 7465 7272  rOS main] Interr
-00000250: 7570 7448 616e 646c 6572 2e69 6e69 7445  uptHandler.initE
-00000260: 7665 6e74 4952 5173 2065 7272 6f72 3a20  ventIRQs error: 
-00000270: 7b7d 0005 2a5b 4552 525d 2065 7874 6572  {}..*[ERR] exter
-00000280: 6e61 6c5f 696e 7465 7272 7570 745f 6861  nal_interrupt_ha
-00000290: 6e64 6c65 7220 6572 726f 723a 207b 7d00  ndler error: {}.
-000002a0: 0514 5b6d 656d 5573 6167 655d 204d 4149  ..[memUsage] MAI
-000002b0: 4e20 4c4f 4144 0005 175b 6d65 6d55 7361  N LOAD...[memUsa
-000002c0: 6765 5d20 5359 5354 454d 2049 5320 5550  ge] SYSTEM IS UP
-000002d0: 0005 235b 4552 525d 2021 2121 2055 6e65  ..#[ERR] !!! Une
-000002e0: 7870 6563 7465 6420 6d69 6372 4f53 2072  xpected micrOS r
-000002f0: 6573 7461 7274 0089 4c10 2601 8009 2c2c  estart..L.&...,,
-00000300: 2c32 322c 2c72 6040 8408 8409 840d 8010  ,22,,r`@........
-00000310: 022a 011b 031c 0216 0259 8010 042a 011b  .*.......Y...*..
-00000320: 041c 0416 0459 8010 052a 011b 061c 0516  .....Y...*......
-00000330: 0559 8010 0710 082a 021b 091c 0716 071c  .Y.....*........
-00000340: 0816 0859 8010 0a10 0b2a 021b 0c1c 0a16  ...Y.....*......
-00000350: 0a1c 0b16 0b59 8010 0d2a 011b 0c1c 0d16  .....Y...*......
-00000360: 0d59 8010 0e2a 011b 0f1c 0e16 0e59 8010  .Y...*.......Y..
-00000370: 1010 112a 021b 121c 1016 101c 1116 1159  ...*...........Y
-00000380: 3200 1613 3201 1615 3202 1616 3203 1617  2...2...2...2...
-00000390: 5163 0483 70b8 020c 1380 1922 502c 4807  Qc..p......"P,H.
-000003a0: 1207 3400 594a 2a57 1221 df44 63c0 4919  ..4.YJ*W.!.Dc.I.
-000003b0: 1222 2300 1414 b036 0134 0159 120e 2301  ."#....6.4.Y..#.
-000003c0: 1414 b036 0134 0159 5151 c028 005d 4a01  ...6.4.YQQ.(.]J.
-000003d0: 5d51 6384 20b8 020e 1580 2122 2550 2c48  ]Qc. .....!"%P,H
-000003e0: 0c12 0a34 0059 120b 3400 594a 2a57 1221  ...4.Y..4.YJ*W.!
-000003f0: df44 63c0 4919 1222 2302 1414 b036 0134  .Dc.I.."#....6.4
-00000400: 0159 120e 2303 1414 b036 0134 0159 5151  .Y..#....6.4.YQQ
-00000410: c028 005d 4a01 5d51 6383 70b8 020c 1680  .(.]J.]Qc.p.....
-00000420: 2a22 502c 4807 120d 3400 594a 2a57 1221  *"P,H...4.YJ*W.!
-00000430: df44 63c0 4919 1222 2304 1414 b036 0134  .Dc.I.."#....6.4
-00000440: 0159 120e 2305 1414 b036 0134 0159 5151  .Y..#....6.4.YQQ
-00000450: c028 005d 4a01 5d51 6388 3838 2217 8037  .(.]J.]Qc.88"..7
-00000460: 6a65 6565 2546 4567 2b68 256a 5366 1208  jeee%FEg+h%jSf..
-00000470: 1018 2306 3482 0059 1202 3400 c012 1334  ..#.4..Y..4....4
-00000480: 0059 1216 3400 5912 0534 00c1 b110 19d9  .Y..4.Y..4......
-00000490: 444c 1211 3400 5912 1034 0059 4253 8010  DL..4.Y..4.YBS..
-000004a0: 1a2a 011b 121c 1ac2 59b2 101b 5234 8200  .*......Y...R4..
-000004b0: 5912 1534 0059 1208 1018 2307 3482 0059  Y..4.Y....#.4..Y
-000004c0: b014 1c12 0434 0014 1d36 0010 1e10 1f36  .....4...6.....6
-000004d0: 8201 59b0 1420 3600 5912 0e23 0834 0159  ..Y.. 6.Y..#.4.Y
-000004e0: 5163                                     Qc
+00000030: 6572 7665 7200 1c61 7574 6f5f 6e77 5f63  erver..auto_nw_c
+00000040: 6f6e 6669 6700 0e4e 6574 776f 726b 000c  onfig..Network..
+00000050: 626f 6f74 7570 001c 7072 6f66 696c 696e  bootup..profilin
+00000060: 675f 696e 666f 000a 486f 6f6b 7300 1e65  g_info..Hooks..e
+00000070: 6e61 626c 6549 6e74 6572 7275 7074 0014  nableInterrupt..
+00000080: 656e 6162 6c65 4372 6f6e 0020 496e 7465  enableCron. Inte
+00000090: 7272 7570 7448 616e 646c 6572 001a 696e  rruptHandler..in
+000000a0: 6974 4576 656e 7449 5251 7300 1465 7272  itEventIRQs..err
+000000b0: 6c6f 675f 6164 6400 0a44 6562 7567 0010  log_add..Debug..
+000000c0: 6e74 705f 7469 6d65 000e 7375 6e74 696d  ntp_time..suntim
+000000d0: 6500 0854 696d 6500 1273 6166 655f 626f  e..Time..safe_bo
+000000e0: 6f74 0081 2916 6972 715f 6861 6e64 6c65  ot..).irq_handle
+000000f0: 7200 2865 7874 6572 6e61 6c5f 6972 715f  r.(external_irq_
+00000100: 6861 6e64 6c65 7200 0c6d 6963 724f 5300  handler..micrOS.
+00000110: 0a6c 6162 656c 0006 5354 4100 0c75 7074  .label..STA..upt
+00000120: 696d 6500 823f 1663 7265 6174 655f 7461  ime..?.create_ta
+00000130: 736b 0014 7275 6e5f 7365 7276 6572 0006  sk..run_server..
+00000140: 7461 6700 0c73 6572 7665 7200 1672 756e  tag..server..run
+00000150: 5f66 6f72 6576 6572 0049 8177 0524 5b6d  _forever.I.w.$[m
+00000160: 6963 724f 5320 6d61 696e 5d20 486f 6f6b  icrOS main] Hook
+00000170: 732e 626f 6f74 2829 2065 7272 6f72 3a20  s.boot() error: 
+00000180: 7b7d 0005 135b 4552 525d 2073 6166 655f  {}...[ERR] safe_
+00000190: 626f 6f74 3a20 7b7d 0005 465b 6d69 6372  boot: {}..F[micr
+000001a0: 4f53 206d 6169 6e5d 2049 6e74 6572 7275  OS main] Interru
+000001b0: 7074 4861 6e64 6c65 722e 656e 6162 6c65  ptHandler.enable
+000001c0: 496e 7465 7272 7570 742f 4372 6f6e 496e  Interrupt/CronIn
+000001d0: 7465 7272 7570 7420 6572 726f 723a 207b  terrupt error: {
+000001e0: 7d00 051b 5b45 5252 5d20 6972 715f 6861  }...[ERR] irq_ha
+000001f0: 6e64 6c65 7220 6572 726f 723a 207b 7d00  ndler error: {}.
+00000200: 0536 5b6d 6963 724f 5320 6d61 696e 5d20  .6[micrOS main] 
+00000210: 496e 7465 7272 7570 7448 616e 646c 6572  InterruptHandler
+00000220: 2e69 6e69 7445 7665 6e74 4952 5173 2065  .initEventIRQs e
+00000230: 7272 6f72 3a20 7b7d 0005 245b 4552 525d  rror: {}..$[ERR]
+00000240: 2065 7874 6572 6e61 6c5f 6972 715f 6861   external_irq_ha
+00000250: 6e64 6c65 7220 6572 726f 723a 207b 7d00  ndler error: {}.
+00000260: 0514 5b6d 656d 5573 6167 655d 204d 4149  ..[memUsage] MAI
+00000270: 4e20 4c4f 4144 0005 175b 6d65 6d55 7361  N LOAD...[memUsa
+00000280: 6765 5d20 5359 5354 454d 2049 5320 5550  ge] SYSTEM IS UP
+00000290: 0005 235b 4552 525d 2021 2121 2055 6e65  ..#[ERR] !!! Une
+000002a0: 7870 6563 7465 6420 6d69 6372 4f53 2072  xpected micrOS r
+000002b0: 6573 7461 7274 0089 4c10 2601 8009 2c2c  estart..L.&...,,
+000002c0: 2c32 322c 2c72 6040 8408 8409 840d 8010  ,22,,r`@........
+000002d0: 022a 011b 031c 0216 0259 8010 042a 011b  .*.......Y...*..
+000002e0: 041c 0416 0459 8010 052a 011b 061c 0516  .....Y...*......
+000002f0: 0559 8010 0710 082a 021b 091c 0716 071c  .Y.....*........
+00000300: 0816 0859 8010 0a10 0b2a 021b 0c1c 0a16  ...Y.....*......
+00000310: 0a1c 0b16 0b59 8010 0d2a 011b 0c1c 0d16  .....Y...*......
+00000320: 0d59 8010 0e2a 011b 0f1c 0e16 0e59 8010  .Y...*.......Y..
+00000330: 1010 112a 021b 121c 1016 101c 1116 1159  ...*...........Y
+00000340: 3200 1613 3201 1615 3202 1616 3203 1617  2...2...2...2...
+00000350: 5163 0483 70b8 020c 1380 1922 502c 4807  Qc..p......"P,H.
+00000360: 1207 3400 594a 2a57 1221 df44 63c0 4919  ..4.YJ*W.!.Dc.I.
+00000370: 1222 2300 1414 b036 0134 0159 120e 2301  ."#....6.4.Y..#.
+00000380: 1414 b036 0134 0159 5151 c028 005d 4a01  ...6.4.YQQ.(.]J.
+00000390: 5d51 6384 20b8 020e 1580 2122 2550 2c48  ]Qc. .....!"%P,H
+000003a0: 0c12 0a34 0059 120b 3400 594a 2a57 1221  ...4.Y..4.YJ*W.!
+000003b0: df44 63c0 4919 1222 2302 1414 b036 0134  .Dc.I.."#....6.4
+000003c0: 0159 120e 2303 1414 b036 0134 0159 5151  .Y..#....6.4.YQQ
+000003d0: c028 005d 4a01 5d51 6383 70b8 020c 1680  .(.]J.]Qc.p.....
+000003e0: 2a22 502c 4807 120d 3400 594a 2a57 1221  *"P,H...4.YJ*W.!
+000003f0: df44 63c0 4919 1222 2304 1414 b036 0134  .Dc.I.."#....6.4
+00000400: 0159 120e 2305 1414 b036 0134 0159 5151  .Y..#....6.4.YQQ
+00000410: c028 005d 4a01 5d51 6388 3838 2217 8037  .(.]J.]Qc.88"..7
+00000420: 6a65 6565 2546 4567 2b68 6533 6a66 1208  jeee%FEg+he3jf..
+00000430: 1018 2306 3482 0059 1202 3400 c012 1334  ..#.4..Y..4....4
+00000440: 0059 1216 3400 5912 0534 00c1 b110 19d9  .Y..4.Y..4......
+00000450: 444c 1211 3400 5912 1034 0059 4253 8010  DL..4.Y..4.YBS..
+00000460: 1a2a 011b 121c 1ac2 59b2 101b 5234 8200  .*......Y...R4..
+00000470: 5912 1534 0059 b014 1c12 0434 0014 1d36  Y..4.Y.....4...6
+00000480: 0010 1e10 1f36 8201 5912 0810 1823 0734  .....6..Y....#.4
+00000490: 8200 59b0 1420 3600 5912 0e23 0834 0159  ..Y.. 6.Y..#.4.Y
+000004a0: 5163                                     Qc
```

### Comparing `micrOSDevToolKit-1.19.0/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files 8% similar despite different names*

```diff
@@ -2,108 +2,108 @@
 00000010: 6465 722e 7079 000f 1274 7261 6365 6261  der.py...traceba
 00000020: 636b 0014 6572 726c 6f67 5f61 6464 000a  ck..errlog_add..
 00000030: 4465 6275 6700 8129 2b16 5f5f 6973 5f6d  Debug..)+.__is_m
 00000040: 6963 724f 5300 0c6d 6963 726f 7300 102e  icrOS..micros...
 00000050: 6966 5f6d 6f64 6500 0272 0081 7b82 3181  if_mode..r..{.1.
 00000060: 5f06 6f66 6600 0865 7869 7400 0673 7973  _.off..exit..sys
 00000070: 001e 5f5f 7265 636f 7665 7279 5f6d 6f64  ..__recovery_mod
-00000080: 6500 3461 7574 6f5f 6e65 7477 6f72 6b5f  e.4auto_network_
-00000090: 636f 6e66 6967 7572 6174 696f 6e00 0e4e  configuration..N
-000000a0: 6574 776f 726b 000c 6366 6767 6574 001a  etwork..cfgget..
-000000b0: 436f 6e66 6967 4861 6e64 6c65 7200 0a61  ConfigHandler..a
-000000c0: 7070 7764 0010 4144 6d69 6e31 3233 000e  ppwd..ADmin123..
-000000d0: 7765 6272 6570 6c00 8225 1070 6173 7377  webrepl..%.passw
-000000e0: 6f72 6400 285f 5f61 7574 6f5f 7265 7374  ord.(__auto_rest
-000000f0: 6172 745f 6576 656e 7400 0a73 6c65 6570  art_event..sleep
-00000100: 000a 7574 696d 6500 0277 0082 4903 0a72  ..utime..w..I..r
-00000110: 6573 6574 000e 6d61 6368 696e 6500 8163  eset..machine..c
-00000120: 0c6d 6963 724f 5300 1270 7269 6e74 5f65  .micrOS..print_e
-00000130: 7863 0049 0265 0081 772f 816d 0510 496d  xc.I.e..w/.m..Im
-00000140: 706f 7274 2065 7272 6f72 3a20 7b7d 0005  port error: {}..
-00000150: 3a5b 6c6f 6164 6572 5d5b 6966 5f6d 6f64  :[loader][if_mod
-00000160: 653a 5472 7565 5d20 2e69 665f 6d6f 6465  e:True] .if_mode
-00000170: 3a6d 6963 726f 7320 2d3e 206d 6963 726f  :micros -> micro
-00000180: 7320 696e 7465 7266 6163 6500 0543 5b6c  s interface..C[l
-00000190: 6f61 6465 725d 5b69 665f 6d6f 6465 3a54  oader][if_mode:T
-000001a0: 7275 655d 202e 6966 5f6d 6f64 6520 6669  rue] .if_mode fi
-000001b0: 6c65 206e 6f74 2065 7869 7374 7320 2d3e  le not exists ->
-000001c0: 206d 6963 726f 7320 696e 7465 7266 6163   micros interfac
-000001d0: 6500 052b 5b6c 6f61 6465 725d 5b69 665f  e..+[loader][if_
-000001e0: 6d6f 6465 5d20 2e69 665f 6d6f 6465 3a6f  mode] .if_mode:o
-000001f0: 6666 202d 3e20 454f 452c 2042 7965 2100  ff -> EOE, Bye!.
-00000200: 053d 5b6c 6f61 6465 725d 5b69 665f 6d6f  .=[loader][if_mo
-00000210: 6465 3a46 616c 7365 5d20 2e69 665f 6d6f  de:False] .if_mo
-00000220: 6465 3a77 6562 7265 706c 202d 3e20 7765  de:webrepl -> we
-00000230: 6272 6570 6c20 696e 7465 7266 6163 6500  brepl interface.
-00000240: 053c 5b6c 6f61 6465 725d 5b72 6563 6f76  .<[loader][recov
-00000250: 6572 7920 6d6f 6465 5d20 2d20 6d61 6e75  ery mode] - manu
-00000260: 616c 6c79 2073 656c 6563 7465 6420 696e  ally selected in
-00000270: 202e 6966 5f6d 6f64 6520 6669 6c65 0005   .if_mode file..
-00000280: 1857 6562 7265 706c 2069 6d70 6f72 7420  .Webrepl import 
-00000290: 6572 726f 723a 207b 7d00 054a 5b6c 6f61  error: {}..J[loa
-000002a0: 6465 725d 5b6f 7461 2061 7574 6f2d 7265  der][ota auto-re
-000002b0: 626f 6f74 6572 5d5b 6d69 6372 6f73 5d5b  booter][micros][
-000002c0: 7b7d 5d20 5761 6974 2066 6f72 204f 5441  {}] Wait for OTA
-000002d0: 2075 7064 6174 6520 706f 7373 6962 6c65   update possible
-000002e0: 2073 7461 7274 0005 475b 6c6f 6164 6572   start..G[loader
-000002f0: 5d5b 6f74 6120 6175 746f 2d72 6562 6f6f  ][ota auto-reboo
-00000300: 7465 725d 5b77 6562 7265 706c 2f4e 6f6e  ter][webrepl/Non
-00000310: 655d 5b7b 7d5d 2055 7064 6174 6520 7374  e][{}] Update st
-00000320: 6174 7573 3a20 496e 5072 6f67 7265 7373  atus: InProgress
-00000330: 0005 4c5b 6c6f 6164 6572 5d5b 6f74 6120  ..L[loader][ota 
-00000340: 6175 746f 2d72 6562 6f6f 7465 725d 5b6d  auto-rebooter][m
-00000350: 6963 726f 735d 5b74 7269 6767 6572 3a20  icros][trigger: 
-00000360: 5472 7565 5d20 4f54 4120 7761 7320 6669  True] OTA was fi
-00000370: 6e69 7368 6564 202d 2072 6562 6f6f 7400  nished - reboot.
-00000380: 050b 636c 6561 6e75 702e 7064 7300 052a  ..cleanup.pds..*
-00000390: 5b6c 6f61 6465 725d 5b6d 6169 6e20 6d6f  [loader][main mo
-000003a0: 6465 5d20 5374 6172 7420 6d69 6372 4f53  de] Start micrOS
-000003b0: 2028 6465 6661 756c 7429 0005 2b5b 6c6f   (default)..+[lo
-000003c0: 6164 6572 5d5b 6d61 696e 206d 6f64 655d  ader][main mode]
-000003d0: 206d 6963 724f 5320 7374 6172 7420 6661   micrOS start fa
-000003e0: 696c 6564 3a20 7b7d 0005 265b 6c6f 6164  iled: {}..&[load
-000003f0: 6572 5d5b 6d61 696e 206d 6f64 655d 202d  er][main mode] -
-00000400: 3e20 5b72 6563 6f76 6572 7920 6d6f 6465  > [recovery mode
-00000410: 5d00 052b 5b45 5252 5d5b 6d69 6372 4f53  ]..+[ERR][micrOS
-00000420: 6c6f 6164 6572 5d20 6d69 6372 4f53 2073  loader] micrOS s
-00000430: 7461 7274 2066 6169 6c65 643a 207b 7d00  tart failed: {}.
-00000440: 874c b002 2601 8008 4249 2622 582d 6d84  .L..&...BI&"X-m.
-00000450: 2884 1084 2284 1327 4808 8051 1b02 1602  (..."..'H..Q....
-00000460: 4a07 5951 1602 4a01 5d48 0e80 1003 2a01  J.YQ..J.]H....*.
-00000470: 1b04 1c03 1603 594a 2457 1126 df44 5d16  ......YJ$W.&.D].
-00000480: 2749 1111 2823 0014 0511 2736 0134 0159  'I..(#....'6.4.Y
-00000490: 5116 0351 5116 2719 275d 4a01 5d32 0016  Q..QQ.'.']J.]2..
-000004a0: 0732 0116 1132 0216 1b32 0316 2311 2910  .2...2...2..#.).
-000004b0: 06d9 4445 1123 3400 5951 6304 8848 c002  ..DE.#4.YQc..H..
-000004c0: 2807 8015 800f 2322 2b2e 4627 6e27 2566  (.....#"+.F'n'%f
-000004d0: 272b 4527 2710 08c0 482d 122a 1009 100a  '+E''...H-.*....
-000004e0: 3402 471f c1b1 140b 3600 140c 3600 140d  4.G.....6...6...
-000004f0: 3600 c0b0 1008 d944 4912 2823 0134 0159  6......DI.(#.4.Y
-00000500: 5263 515c 5d4a 1357 1226 df44 4c59 1228  RcQ\]J.W.&.DLY.(
-00000510: 2302 3401 5952 634a 015d b010 0ed9 4457  #.4.YRcJ.]....DW
-00000520: 1228 2303 3401 5980 100f 2a01 1b10 1c0f  .(#.4.Y...*.....
-00000530: c259 b280 3401 5912 2823 0434 0159 1228  .Y..4.Y.(#.4.Y.(
-00000540: 2305 3401 5950 6386 60d8 0216 1180 3e2b  #.4.YPc.`.....>+
-00000550: 2b26 4b44 2225 5580 1012 2a01 1b13 1c12  +&KD"%U...*.....
-00000560: c059 8010 142a 011b 151c 14c1 59b1 1016  .Y...*......Y...
-00000570: 3401 c2b2 51de 4444 1017 4241 b2c2 b034  4...Q.DD..BA...4
-00000580: 0059 4811 8051 1b18 c3b3 1419 101a b236  .YH..Q.........6
-00000590: 8200 594a 1e57 1226 df44 57c4 490d 1228  ..YJ.W.&.DW.I..(
-000005a0: 2306 1405 b436 0134 0159 5151 c428 045d  #....6.4.YQQ.(.]
-000005b0: 4a01 5d51 6389 004c 281b 804d 8007 2b22  J.]Qc..L(..M..+"
-000005c0: 4243 462c 464c 4229 472b 4b2b 2480 101c  BCF,FLB)G+K+$...
-000005d0: 2a01 1b1d 1c1c c059 50c1 88c2 42e0 8012  *......YP...B...
-000005e0: 0734 0044 5212 2823 0714 05b2 3601 3401  .4.DR.(#....6.4.
-000005f0: 59b2 81e6 c242 4e12 2823 0814 05b2 3601  Y....BN.(#....6.
-00000600: 3401 5952 c1b1 4472 1207 3400 446c 1228  4.YR..Dr..4.Dl.(
-00000610: 2309 3401 5912 2a23 0a10 1e34 0247 0ac3  #.4.Y.*#...4.G..
-00000620: b314 1f10 2036 0159 515c 5d80 1021 2a01  .... 6.YQ\]..!*.
-00000630: 1b22 1c21 c459 b434 0059 b082 3401 59b2  .".!.Y.4.Y..4.Y.
-00000640: 80d8 439a 7f51 6388 28c0 021c 2380 6f47  ..C..Qc.(...#.oG
-00000650: 2227 2b50 4e2c 2727 5525 1207 3400 44e1  "'+PN,''U%..4.D.
-00000660: 8048 1812 2823 0b34 0159 8010 242a 011b  .H..(#.4.Y..$*..
-00000670: 241c 24c0 59b0 3400 594a 4757 1226 df44  $.$.Y.4.YJGW.&.D
-00000680: bf80 c149 3512 0251 ded3 4447 1202 1425  ...I5..Q..DG...%
-00000690: 3600 5912 2823 0c14 05b1 3601 3401 5912  6.Y.(#....6.4.Y.
-000006a0: 2823 0d34 0159 1203 51de d344 4c12 0323  (#.4.Y..Q..DL..#
-000006b0: 0e14 05b1 3601 3401 5951 51c1 2801 5d4a  ....6.4.YQQ.(.]J
-000006c0: 015d 1211 3400 5912 1b34 0059 5163       .]..4.Y..4.YQc
+00000080: 6500 1c61 7574 6f5f 6e77 5f63 6f6e 6669  e..auto_nw_confi
+00000090: 6700 0e4e 6574 776f 726b 000c 6366 6767  g..Network..cfgg
+000000a0: 6574 001a 436f 6e66 6967 4861 6e64 6c65  et..ConfigHandle
+000000b0: 7200 0a61 7070 7764 0010 4144 6d69 6e31  r..appwd..ADmin1
+000000c0: 3233 000e 7765 6272 6570 6c00 8225 1070  23..webrepl..%.p
+000000d0: 6173 7377 6f72 6400 285f 5f61 7574 6f5f  assword.(__auto_
+000000e0: 7265 7374 6172 745f 6576 656e 7400 0a73  restart_event..s
+000000f0: 6c65 6570 000a 7574 696d 6500 0277 0082  leep..utime..w..
+00000100: 4903 0a72 6573 6574 000e 6d61 6368 696e  I..reset..machin
+00000110: 6500 8163 0c6d 6963 724f 5300 1270 7269  e..c.micrOS..pri
+00000120: 6e74 5f65 7863 0049 0265 0081 772f 816d  nt_exc.I.e..w/.m
+00000130: 0510 496d 706f 7274 2065 7272 6f72 3a20  ..Import error: 
+00000140: 7b7d 0005 3a5b 6c6f 6164 6572 5d5b 6966  {}..:[loader][if
+00000150: 5f6d 6f64 653a 5472 7565 5d20 2e69 665f  _mode:True] .if_
+00000160: 6d6f 6465 3a6d 6963 726f 7320 2d3e 206d  mode:micros -> m
+00000170: 6963 726f 7320 696e 7465 7266 6163 6500  icros interface.
+00000180: 0543 5b6c 6f61 6465 725d 5b69 665f 6d6f  .C[loader][if_mo
+00000190: 6465 3a54 7275 655d 202e 6966 5f6d 6f64  de:True] .if_mod
+000001a0: 6520 6669 6c65 206e 6f74 2065 7869 7374  e file not exist
+000001b0: 7320 2d3e 206d 6963 726f 7320 696e 7465  s -> micros inte
+000001c0: 7266 6163 6500 052b 5b6c 6f61 6465 725d  rface..+[loader]
+000001d0: 5b69 665f 6d6f 6465 5d20 2e69 665f 6d6f  [if_mode] .if_mo
+000001e0: 6465 3a6f 6666 202d 3e20 454f 452c 2042  de:off -> EOE, B
+000001f0: 7965 2100 053d 5b6c 6f61 6465 725d 5b69  ye!..=[loader][i
+00000200: 665f 6d6f 6465 3a46 616c 7365 5d20 2e69  f_mode:False] .i
+00000210: 665f 6d6f 6465 3a77 6562 7265 706c 202d  f_mode:webrepl -
+00000220: 3e20 7765 6272 6570 6c20 696e 7465 7266  > webrepl interf
+00000230: 6163 6500 053c 5b6c 6f61 6465 725d 5b72  ace..<[loader][r
+00000240: 6563 6f76 6572 7920 6d6f 6465 5d20 2d20  ecovery mode] - 
+00000250: 6d61 6e75 616c 6c79 2073 656c 6563 7465  manually selecte
+00000260: 6420 696e 202e 6966 5f6d 6f64 6520 6669  d in .if_mode fi
+00000270: 6c65 0005 1857 6562 7265 706c 2069 6d70  le...Webrepl imp
+00000280: 6f72 7420 6572 726f 723a 207b 7d00 054a  ort error: {}..J
+00000290: 5b6c 6f61 6465 725d 5b6f 7461 2061 7574  [loader][ota aut
+000002a0: 6f2d 7265 626f 6f74 6572 5d5b 6d69 6372  o-rebooter][micr
+000002b0: 6f73 5d5b 7b7d 5d20 5761 6974 2066 6f72  os][{}] Wait for
+000002c0: 204f 5441 2075 7064 6174 6520 706f 7373   OTA update poss
+000002d0: 6962 6c65 2073 7461 7274 0005 475b 6c6f  ible start..G[lo
+000002e0: 6164 6572 5d5b 6f74 6120 6175 746f 2d72  ader][ota auto-r
+000002f0: 6562 6f6f 7465 725d 5b77 6562 7265 706c  ebooter][webrepl
+00000300: 2f4e 6f6e 655d 5b7b 7d5d 2055 7064 6174  /None][{}] Updat
+00000310: 6520 7374 6174 7573 3a20 496e 5072 6f67  e status: InProg
+00000320: 7265 7373 0005 4c5b 6c6f 6164 6572 5d5b  ress..L[loader][
+00000330: 6f74 6120 6175 746f 2d72 6562 6f6f 7465  ota auto-reboote
+00000340: 725d 5b6d 6963 726f 735d 5b74 7269 6767  r][micros][trigg
+00000350: 6572 3a20 5472 7565 5d20 4f54 4120 7761  er: True] OTA wa
+00000360: 7320 6669 6e69 7368 6564 202d 2072 6562  s finished - reb
+00000370: 6f6f 7400 050b 636c 6561 6e75 702e 7064  oot...cleanup.pd
+00000380: 7300 052a 5b6c 6f61 6465 725d 5b6d 6169  s..*[loader][mai
+00000390: 6e20 6d6f 6465 5d20 5374 6172 7420 6d69  n mode] Start mi
+000003a0: 6372 4f53 2028 6465 6661 756c 7429 0005  crOS (default)..
+000003b0: 2b5b 6c6f 6164 6572 5d5b 6d61 696e 206d  +[loader][main m
+000003c0: 6f64 655d 206d 6963 724f 5320 7374 6172  ode] micrOS star
+000003d0: 7420 6661 696c 6564 3a20 7b7d 0005 265b  t failed: {}..&[
+000003e0: 6c6f 6164 6572 5d5b 6d61 696e 206d 6f64  loader][main mod
+000003f0: 655d 202d 3e20 5b72 6563 6f76 6572 7920  e] -> [recovery 
+00000400: 6d6f 6465 5d00 052b 5b45 5252 5d5b 6d69  mode]..+[ERR][mi
+00000410: 6372 4f53 6c6f 6164 6572 5d20 6d69 6372  crOSloader] micr
+00000420: 4f53 2073 7461 7274 2066 6169 6c65 643a  OS start failed:
+00000430: 207b 7d00 874c b002 2601 8008 4249 2622   {}..L..&...BI&"
+00000440: 582d 6d84 2884 1084 2284 1327 4808 8051  X-m.(..."..'H..Q
+00000450: 1b02 1602 4a07 5951 1602 4a01 5d48 0e80  ....J.YQ..J.]H..
+00000460: 1003 2a01 1b04 1c03 1603 594a 2457 1126  ..*.......YJ$W.&
+00000470: df44 5d16 2749 1111 2823 0014 0511 2736  .D].'I..(#....'6
+00000480: 0134 0159 5116 0351 5116 2719 275d 4a01  .4.YQ..QQ.'.']J.
+00000490: 5d32 0016 0732 0116 1132 0216 1b32 0316  ]2...2...2...2..
+000004a0: 2311 2910 06d9 4445 1123 3400 5951 6304  #.)...DE.#4.YQc.
+000004b0: 8848 c002 2807 8015 800f 2322 2b2e 4627  .H..(.....#"+.F'
+000004c0: 6e27 2566 272b 4527 2710 08c0 482d 122a  n'%f'+E''...H-.*
+000004d0: 1009 100a 3402 471f c1b1 140b 3600 140c  ....4.G.....6...
+000004e0: 3600 140d 3600 c0b0 1008 d944 4912 2823  6...6......DI.(#
+000004f0: 0134 0159 5263 515c 5d4a 1357 1226 df44  .4.YRcQ\]J.W.&.D
+00000500: 4c59 1228 2302 3401 5952 634a 015d b010  LY.(#.4.YRcJ.]..
+00000510: 0ed9 4457 1228 2303 3401 5980 100f 2a01  ..DW.(#.4.Y...*.
+00000520: 1b10 1c0f c259 b280 3401 5912 2823 0434  .....Y..4.Y.(#.4
+00000530: 0159 1228 2305 3401 5950 6386 60d8 0216  .Y.(#.4.YPc.`...
+00000540: 1180 3e2b 2b26 4b44 2225 5580 1012 2a01  ..>++&KD"%U...*.
+00000550: 1b13 1c12 c059 8010 142a 011b 151c 14c1  .....Y...*......
+00000560: 59b1 1016 3401 c2b2 51de 4444 1017 4241  Y...4...Q.DD..BA
+00000570: b2c2 b034 0059 4811 8051 1b18 c3b3 1419  ...4.YH..Q......
+00000580: 101a b236 8200 594a 1e57 1226 df44 57c4  ...6..YJ.W.&.DW.
+00000590: 490d 1228 2306 1405 b436 0134 0159 5151  I..(#....6.4.YQQ
+000005a0: c428 045d 4a01 5d51 6389 004c 281b 804d  .(.]J.]Qc..L(..M
+000005b0: 8007 2b22 4243 462c 464c 4229 472b 4b2b  ..+"BCF,FLB)G+K+
+000005c0: 2480 101c 2a01 1b1d 1c1c c059 50c1 88c2  $...*......YP...
+000005d0: 42e0 8012 0734 0044 5212 2823 0714 05b2  B....4.DR.(#....
+000005e0: 3601 3401 59b2 81e6 c242 4e12 2823 0814  6.4.Y....BN.(#..
+000005f0: 05b2 3601 3401 5952 c1b1 4472 1207 3400  ..6.4.YR..Dr..4.
+00000600: 446c 1228 2309 3401 5912 2a23 0a10 1e34  Dl.(#.4.Y.*#...4
+00000610: 0247 0ac3 b314 1f10 2036 0159 515c 5d80  .G...... 6.YQ\].
+00000620: 1021 2a01 1b22 1c21 c459 b434 0059 b082  .!*..".!.Y.4.Y..
+00000630: 3401 59b2 80d8 439a 7f51 6388 28c0 021c  4.Y...C..Qc.(...
+00000640: 2380 6f47 2227 2b50 4e2c 2727 5525 1207  #.oG"'+PN,''U%..
+00000650: 3400 44e1 8048 1812 2823 0b34 0159 8010  4.D..H..(#.4.Y..
+00000660: 242a 011b 241c 24c0 59b0 3400 594a 4757  $*..$.$.Y.4.YJGW
+00000670: 1226 df44 bf80 c149 3512 0251 ded3 4447  .&.D...I5..Q..DG
+00000680: 1202 1425 3600 5912 2823 0c14 05b1 3601  ...%6.Y.(#....6.
+00000690: 3401 5912 2823 0d34 0159 1203 51de d344  4.Y.(#.4.Y..Q..D
+000006a0: 4c12 0323 0e14 05b1 3601 3401 5951 51c1  L..#....6.4.YQQ.
+000006b0: 2801 5d4a 015d 1211 3400 5912 1b34 0059  (.]J.]..4.Y..4.Y
+000006c0: 5163                                     Qc
```

