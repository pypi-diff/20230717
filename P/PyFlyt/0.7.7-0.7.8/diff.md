# Comparing `tmp/PyFlyt-0.7.7.tar.gz` & `tmp/PyFlyt-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.7.7.tar", last modified: Mon Jul 17 12:28:26 2023, max compression
+gzip compressed data, was "PyFlyt-0.7.8.tar", last modified: Mon Jul 17 12:29:49 2023, max compression
```

## Comparing `PyFlyt-0.7.7.tar` & `PyFlyt-0.7.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.7.7/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.145840 PyFlyt-0.7.7/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.7.7/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.145840 PyFlyt-0.7.7/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.7.7/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12141 2023-06-07 19:07:52.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7560 2023-07-17 12:21:59.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.7.7/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.7.7/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-14 18:31:25.000000 PyFlyt-0.7.7/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.7.7/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.7.7/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.7.7/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.7.7/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.7.7/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.145840 PyFlyt-0.7.7/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.7.7/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.145840 PyFlyt-0.7.7/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-07-17 12:28:26.000000 PyFlyt-0.7.7/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-07-17 12:28:26.000000 PyFlyt-0.7.7/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-17 12:28:26.000000 PyFlyt-0.7.7/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-17 12:28:26.000000 PyFlyt-0.7.7/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-17 12:28:26.000000 PyFlyt-0.7.7/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-17 12:28:13.000000 PyFlyt-0.7.7/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.7.7/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-07-17 12:24:22.000000 PyFlyt-0.7.7/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:28:26.149840 PyFlyt-0.7.7/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-12 23:01:51.000000 PyFlyt-0.7.7/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-05-29 18:32:17.000000 PyFlyt-0.7.7/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.7.8/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.788816 PyFlyt-0.7.8/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.7.8/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.788816 PyFlyt-0.7.8/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.7.8/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.788816 PyFlyt-0.7.8/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12141 2023-06-07 19:07:52.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7560 2023-07-17 12:29:32.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.7.8/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.7.8/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-14 18:31:25.000000 PyFlyt-0.7.8/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.7.8/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.7.8/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.7.8/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.7.8/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.7.8/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.788816 PyFlyt-0.7.8/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.7.8/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.788816 PyFlyt-0.7.8/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-07-17 12:29:49.000000 PyFlyt-0.7.8/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-07-17 12:29:49.000000 PyFlyt-0.7.8/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-17 12:29:49.000000 PyFlyt-0.7.8/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-17 12:29:49.000000 PyFlyt-0.7.8/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-17 12:29:49.000000 PyFlyt-0.7.8/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-17 12:29:41.000000 PyFlyt-0.7.8/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.7.8/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-07-17 12:24:22.000000 PyFlyt-0.7.8/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 12:29:49.792816 PyFlyt-0.7.8/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-12 23:01:51.000000 PyFlyt-0.7.8/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-05-29 18:32:17.000000 PyFlyt-0.7.8/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.7.7/LICENSE.txt` & `PyFlyt-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PKG-INFO` & `PyFlyt-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.7
+Version: 0.7.8
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.p = p
         self.uav_id = uav_id
         self.camera_id = camera_id
 
         # camera parameters
         self.proj_mat = self.p.computeProjectionMatrixFOV(
             fov=camera_FOV_degrees,
-            aspect=float(camera_resolution[0] / camera_resolution[1]),
+            aspect=float(camera_resolution[1] / camera_resolution[0]),
             nearVal=0.1,
             farVal=255.0,
         )
         self.use_gimbal = use_gimbal
         self.camera_angle_degrees = camera_angle_degrees
         self.camera_FOV_degrees = camera_FOV_degrees
         self.camera_resolution = np.array(camera_resolution)
```

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.7.8/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/aviary.py` & `PyFlyt-0.7.8/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.7.8/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.7.8/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.7.8/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/core/load_objs.py` & `PyFlyt-0.7.8/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.7.8/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.7.8/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.7.8/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.7.8/PyFlyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.7
+Version: 0.7.8
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.7.7/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.7.8/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/pyproject.toml` & `PyFlyt-0.7.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.7.7"
+version = "0.7.8"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.7.7/readme.md` & `PyFlyt-0.7.8/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/tests/test_core.py` & `PyFlyt-0.7.8/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.7/tests/test_gym_envs.py` & `PyFlyt-0.7.8/tests/test_gym_envs.py`

 * *Files identical despite different names*

