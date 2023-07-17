# Comparing `tmp/panda-python-0.5.0.tar.gz` & `tmp/panda-python-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-python-0.5.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "panda-python-0.5.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `panda-python-0.5.0.tar` & `panda-python-0.5.1.tar`

### file list

```diff
@@ -1,71 +1,73 @@
--rw-r--r--   0        0        0     2135 2022-11-09 12:37:21.000000 panda-python-0.5.0/.github/workflows/build.yml
--rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 panda-python-0.5.0/.gitignore
--rw-r--r--   0        0        0    19334 2022-11-09 12:37:21.000000 panda-python-0.5.0/.pylintrc
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/c_cpp_properties.json
--rwxr-xr-x   0        0        0      481 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/generate_docs_api.sh
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 panda-python-0.5.0/.vscode/tasks.json
--rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 panda-python-0.5.0/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 panda-python-0.5.0/LICENSE
--rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 panda-python-0.5.0/README.md
--rwxr-xr-x   0        0        0     1214 2022-11-09 12:37:21.000000 panda-python-0.5.0/bin/before_install.sh
--rwxr-xr-x   0        0        0     1251 2022-11-09 12:37:21.000000 panda-python-0.5.0/bin/build_all.sh
--rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/Makefile
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/index.rst
--rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/make.bat
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.cli.rst
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.constants.rst
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.controllers.rst
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.libfranka.rst
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.motion.rst
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 panda-python-0.5.0/docs/panda_py.rst
--rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/cartesian_impedance.py
--rw-r--r--   0        0        0     2531 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/communication_test.py
--rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/mmc.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/notebooks/benchmark.ipynb
--rw-r--r--   0        0        0    31180 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/notebooks/motion.ipynb
--rw-r--r--   0        0        0    38752 2022-11-09 12:37:21.000000 panda-python-0.5.0/examples/notebooks/paper.ipynb
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/constants.h
--rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/applied_force.h
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/applied_torque.h
--rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/cartesian_impedance.h
--rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/controller.h
--rw-r--r--   0        0        0     1683 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/force.h
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/integrated_velocity.h
--rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/joint_limits/virtual_wall.h
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/joint_limits/virtual_wall_controller.h
--rw-r--r--   0        0        0     1335 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/joint_position.h
--rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/controllers/trajectory.h
--rw-r--r--   0        0        0    16534 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/kinematics/fk.h
--rw-r--r--   0        0        0    14073 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/kinematics/ik.h
--rw-r--r--   0        0        0     3949 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/motion/generators.h
--rw-r--r--   0        0        0     3473 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/motion/time_optimal/path.h
--rw-r--r--   0        0        0     5278 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/motion/time_optimal/trajectory.h
--rw-r--r--   0        0        0     5819 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/panda.h
--rw-r--r--   0        0        0     3864 2022-11-09 12:37:21.000000 panda-python-0.5.0/include/utils.h
--rw-r--r--   0        0        0    51837 2022-11-09 12:37:21.000000 panda-python-0.5.0/logo.jpg
--rw-r--r--   0        0        0     1673 2022-11-09 12:37:21.000000 panda-python-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    21367 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/_core.cpp
--rw-r--r--   0        0        0     2284 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/applied_force.cpp
--rw-r--r--   0        0        0     2080 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/applied_torque.cpp
--rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/cartesian_impedance.cpp
--rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/force.cpp
--rw-r--r--   0        0        0     2287 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/integrated_velocity.cpp
--rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/joint_limits/virtual_wall.cpp
--rw-r--r--   0        0        0     3069 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/joint_position.cpp
--rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/controllers/trajectory.cpp
--rw-r--r--   0        0        0    25036 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/libfranka.cpp
--rw-r--r--   0        0        0     6824 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/motion/generators.cpp
--rw-r--r--   0        0        0     9987 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/motion/time_optimal/path.cpp
--rw-r--r--   0        0        0    23965 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/motion/time_optimal/trajectory.cpp
--rw-r--r--   0        0        0    14329 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda.cpp
--rw-r--r--   0        0        0    10245 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/__init__.py
--rw-r--r--   0        0        0     5211 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/__init__.pyi
--rw-r--r--   0        0        0    17071 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/_core/__init__.pyi
--rw-r--r--   0        0        0     2611 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/cli.py
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/constants.py
--rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/controllers.py
--rw-r--r--   0        0        0    34215 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/libfranka/__init__.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 panda-python-0.5.0/src/panda_py/motion.py
--rw-r--r--   0        0        0    14846 2022-11-09 12:37:21.000000 panda-python-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 panda-python-0.5.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 panda-python-0.5.1/.gitignore
+-rw-r--r--   0        0        0    19334 2022-11-09 12:37:21.000000 panda-python-0.5.1/.pylintrc
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 panda-python-0.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/c_cpp_properties.json
+-rwxr-xr-x   0        0        0      481 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/generate_docs_api.sh
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/settings.json
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 panda-python-0.5.1/.vscode/tasks.json
+-rw-r--r--   0        0        0     1591 2022-11-09 12:37:21.000000 panda-python-0.5.1/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 panda-python-0.5.1/LICENSE
+-rw-r--r--   0        0        0      881 2022-11-09 12:37:21.000000 panda-python-0.5.1/README.md
+-rwxr-xr-x   0        0        0     1214 2022-11-09 12:37:21.000000 panda-python-0.5.1/bin/before_install.sh
+-rwxr-xr-x   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.1/bin/build_all.sh
+-rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/make.bat
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.cli.rst
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.constants.rst
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.controllers.rst
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.libfranka.rst
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.motion.rst
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/panda_py.rst
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 panda-python-0.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/cartesian_impedance.py
+-rw-r--r--   0        0        0     2531 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/communication_test.py
+-rw-r--r--   0        0        0     2340 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/mmc.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/notebooks/benchmark.ipynb
+-rw-r--r--   0        0        0    31180 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/notebooks/motion.ipynb
+-rw-r--r--   0        0        0    38752 2022-11-09 12:37:21.000000 panda-python-0.5.1/examples/notebooks/paper.ipynb
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/constants.h
+-rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/applied_force.h
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/applied_torque.h
+-rw-r--r--   0        0        0     2063 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/cartesian_impedance.h
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/controller.h
+-rw-r--r--   0        0        0     1683 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/force.h
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/integrated_velocity.h
+-rw-r--r--   0        0        0     1337 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/joint_limits/virtual_wall.h
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/joint_limits/virtual_wall_controller.h
+-rw-r--r--   0        0        0     1335 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/joint_position.h
+-rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/controllers/trajectory.h
+-rw-r--r--   0        0        0    16534 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/kinematics/fk.h
+-rw-r--r--   0        0        0    14073 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/kinematics/ik.h
+-rw-r--r--   0        0        0     3949 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/motion/generators.h
+-rw-r--r--   0        0        0     3473 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/motion/time_optimal/path.h
+-rw-r--r--   0        0        0     5278 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/motion/time_optimal/trajectory.h
+-rw-r--r--   0        0        0     5819 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/panda.h
+-rw-r--r--   0        0        0     3864 2022-11-09 12:37:21.000000 panda-python-0.5.1/include/utils.h
+-rw-r--r--   0        0        0    51837 2022-11-09 12:37:21.000000 panda-python-0.5.1/logo.jpg
+-rw-r--r--   0        0        0     1672 2022-11-09 12:37:21.000000 panda-python-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    21367 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/_core.cpp
+-rw-r--r--   0        0        0     2284 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/applied_force.cpp
+-rw-r--r--   0        0        0     2080 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/applied_torque.cpp
+-rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/cartesian_impedance.cpp
+-rw-r--r--   0        0        0     4628 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/force.cpp
+-rw-r--r--   0        0        0     2287 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/integrated_velocity.cpp
+-rw-r--r--   0        0        0     5337 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/joint_limits/virtual_wall.cpp
+-rw-r--r--   0        0        0     3069 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/joint_position.cpp
+-rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/controllers/trajectory.cpp
+-rw-r--r--   0        0        0    25036 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/libfranka.cpp
+-rw-r--r--   0        0        0     6824 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/motion/generators.cpp
+-rw-r--r--   0        0        0     9987 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/motion/time_optimal/path.cpp
+-rw-r--r--   0        0        0    23965 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/motion/time_optimal/trajectory.cpp
+-rw-r--r--   0        0        0    14329 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda.cpp
+-rw-r--r--   0        0        0    10245 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/__init__.py
+-rw-r--r--   0        0        0     5211 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/__init__.pyi
+-rw-r--r--   0        0        0    17071 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/_core/__init__.pyi
+-rw-r--r--   0        0        0     2611 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/cli.py
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/constants.py
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/controllers.py
+-rw-r--r--   0        0        0    34215 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/libfranka/__init__.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 panda-python-0.5.1/src/panda_py/motion.py
+-rw-r--r--   0        0        0    14908 2022-11-09 12:37:21.000000 panda-python-0.5.1/PKG-INFO
```

### Comparing `panda-python-0.5.0/.pylintrc` & `panda-python-0.5.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/.vscode/settings.json` & `panda-python-0.5.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/.vscode/tasks.json` & `panda-python-0.5.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/CMakeLists.txt` & `panda-python-0.5.1/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.15...3.25)
 project(
-  "${SKBUILD_PROJECT_NAME}"
+  "panda_py"
   LANGUAGES CXX)
 #  VERSION "${SKBUILD_PROJECT_VERSION}")
 
 set (CMAKE_CXX_STANDARD 17)
 set(CMAKE_BUILD_TYPE "Release")
 set(THREADS_PREFER_PTHREAD_FLAG ON)
 
@@ -44,15 +44,15 @@
   ${EIGEN3_INCLUDE_DIRS}
   ${Franka_INCLUDE_DIRS}
 )
 
 #target_compile_definitions(_core
 #  PRIVATE VERSION_INFO=${PROJECT_VERSION})
 
-install(TARGETS _core LIBRARY DESTINATION ${SKBUILD_PROJECT_NAME})
+install(TARGETS _core LIBRARY DESTINATION panda_py)
 
 ## libfranka module
 pybind11_add_module(libfranka
   src/libfranka.cpp)
 
 target_link_libraries(libfranka PUBLIC
   ${Franka_LIBRARIES}
@@ -61,8 +61,8 @@
 target_include_directories(libfranka SYSTEM PUBLIC
   ${Franka_INCLUDE_DIRS}
 )
 
 #target_compile_definitions(libfranka
 #  PRIVATE VERSION_INFO=${PROJECT_VERSION})
 
-install(TARGETS libfranka LIBRARY DESTINATION ${SKBUILD_PROJECT_NAME})
+install(TARGETS libfranka LIBRARY DESTINATION panda_py)
```

### Comparing `panda-python-0.5.0/LICENSE` & `panda-python-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/README.md` & `panda-python-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # panda-py
-![logo](logo.jpg)
+![logo](https://github.com/JeanElsner/panda-py/blob/main/logo.jpg?raw=true)
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JeanElsner/panda-py/build.yml)](https://github.com/JeanElsner/panda-py/actions/workflows/build.yml)
 [![GitHub](https://img.shields.io/github/license/JeanElsner/panda-py)](https://www.apache.org/licenses/LICENSE-2.0)
-[![PyPI](https://img.shields.io/pypi/v/panda-py)](https://pypi.org/project/panda-python/)
+[![PyPI](https://img.shields.io/pypi/v/panda-python)](https://pypi.org/project/panda-python/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/panda-python)
 
 Finally, Python bindings for the Panda. These will increase your productivity by 1000%, guaranteed[^1]!
 
 > **Info**
 >
 > Please consider this a work in progress. Documentation, continuous integration pipeline and a companion paper are currently being prepared.
```

### Comparing `panda-python-0.5.0/bin/before_install.sh` & `panda-python-0.5.1/bin/before_install.sh`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/bin/build_all.sh` & `panda-python-0.5.1/bin/build_all.sh`

 * *Files 19% similar despite different names*

```diff
@@ -32,21 +32,25 @@
 data['tool']['cibuildwheel']['environment'] = '$2'
 
 with open('$toml', 'w') as f:
     toml.dump(data, f)
 END
 }
 
+mkdir $root/archive
+
 # Build wheels for common libfranka versions
 libfranka=("0.7.1" "0.8.0" "0.9.2" "0.10.0")
 for value in "${libfranka[@]}"; do
   echo "Changing libfranka version in pyproject.toml to: $value"
   change_version "$version+libfranka-$value" "LIBFRANKA_VER=$value"
   export LIBFRANKA_VER=$value
-  python -m cibuildwheel --output-dir $root/wheelhouse $root
+  archive=panda_py_${version}_libfranka_${value}
+  python -m cibuildwheel --output-dir $root/$archive $root
+  zip -j $root/archive/$archive.zip $root/$archive/*.whl
 done
 
 # Change back to default version
 change_version "$version" "LIBFRANKA_VER=0.9.2"
 
 # Build default version
 python -m cibuildwheel --output-dir $root/dist $root
```

### Comparing `panda-python-0.5.0/docs/Makefile` & `panda-python-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/docs/conf.py` & `panda-python-0.5.1/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'panda-py'
 copyright = '2023, Jean Elsner'
 author = 'Jean Elsner'
-release = '0.5.0'
+release = '0.5.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
```

### Comparing `panda-python-0.5.0/docs/make.bat` & `panda-python-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/examples/cartesian_impedance.py` & `panda-python-0.5.1/examples/cartesian_impedance.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/examples/communication_test.py` & `panda-python-0.5.1/examples/communication_test.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/examples/mmc.py` & `panda-python-0.5.1/examples/mmc.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/examples/notebooks/benchmark.ipynb` & `panda-python-0.5.1/examples/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/examples/notebooks/motion.ipynb` & `panda-python-0.5.1/examples/notebooks/motion.ipynb`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/examples/notebooks/paper.ipynb` & `panda-python-0.5.1/examples/notebooks/paper.ipynb`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/constants.h` & `panda-python-0.5.1/include/constants.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/applied_force.h` & `panda-python-0.5.1/include/controllers/applied_force.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/applied_torque.h` & `panda-python-0.5.1/include/controllers/applied_torque.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/cartesian_impedance.h` & `panda-python-0.5.1/include/controllers/cartesian_impedance.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/controller.h` & `panda-python-0.5.1/include/controllers/controller.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/force.h` & `panda-python-0.5.1/include/controllers/force.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/integrated_velocity.h` & `panda-python-0.5.1/include/controllers/integrated_velocity.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/joint_limits/virtual_wall.h` & `panda-python-0.5.1/include/controllers/joint_limits/virtual_wall.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/joint_limits/virtual_wall_controller.h` & `panda-python-0.5.1/include/controllers/joint_limits/virtual_wall_controller.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/joint_position.h` & `panda-python-0.5.1/include/controllers/joint_position.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/controllers/trajectory.h` & `panda-python-0.5.1/include/controllers/trajectory.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/kinematics/fk.h` & `panda-python-0.5.1/include/kinematics/fk.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/kinematics/ik.h` & `panda-python-0.5.1/include/kinematics/ik.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/motion/generators.h` & `panda-python-0.5.1/include/motion/generators.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/motion/time_optimal/path.h` & `panda-python-0.5.1/include/motion/time_optimal/path.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/motion/time_optimal/trajectory.h` & `panda-python-0.5.1/include/motion/time_optimal/trajectory.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/panda.h` & `panda-python-0.5.1/include/panda.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/include/utils.h` & `panda-python-0.5.1/include/utils.h`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/logo.jpg` & `panda-python-0.5.1/logo.jpg`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/pyproject.toml` & `panda-python-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "panda-python"
 description = "Python bindings for the Panda"
 requires-python = ">=3.7"
 dependencies = ["websockets>=11.0", "requests", "numpy"]
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     { name = "Jean Elsner", email = "jean.elsner@tum.de" },
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["python", "real-time", "control", "robot", "franka", "emika"]
 classifiers = [
@@ -49,9 +49,9 @@
 [tool.cibuildwheel.linux]
 before-all = [ "./bin/before_install.sh",]
 archs = [ "x86_64",]
 
 [tool.scikit-build.cmake]
 build-type = "Release"
 
-[tool.scikit-build.sdist]
-include = [ "src/**/*.pyi",]
+[tool.scikit-build.wheel]
+packages = ["src/panda_py"]
```

### Comparing `panda-python-0.5.0/src/_core.cpp` & `panda-python-0.5.1/src/_core.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/applied_force.cpp` & `panda-python-0.5.1/src/controllers/applied_force.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/applied_torque.cpp` & `panda-python-0.5.1/src/controllers/applied_torque.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/cartesian_impedance.cpp` & `panda-python-0.5.1/src/controllers/cartesian_impedance.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/force.cpp` & `panda-python-0.5.1/src/controllers/force.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/integrated_velocity.cpp` & `panda-python-0.5.1/src/controllers/integrated_velocity.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/joint_limits/virtual_wall.cpp` & `panda-python-0.5.1/src/controllers/joint_limits/virtual_wall.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/joint_position.cpp` & `panda-python-0.5.1/src/controllers/joint_position.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/controllers/trajectory.cpp` & `panda-python-0.5.1/src/controllers/trajectory.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/libfranka.cpp` & `panda-python-0.5.1/src/libfranka.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/motion/generators.cpp` & `panda-python-0.5.1/src/motion/generators.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/motion/time_optimal/path.cpp` & `panda-python-0.5.1/src/motion/time_optimal/path.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/motion/time_optimal/trajectory.cpp` & `panda-python-0.5.1/src/motion/time_optimal/trajectory.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda.cpp` & `panda-python-0.5.1/src/panda.cpp`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/__init__.py` & `panda-python-0.5.1/src/panda_py/__init__.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/__init__.pyi` & `panda-python-0.5.1/src/panda_py/__init__.pyi`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/_core/__init__.pyi` & `panda-python-0.5.1/src/panda_py/_core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/cli.py` & `panda-python-0.5.1/src/panda_py/cli.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/constants.py` & `panda-python-0.5.1/src/panda_py/constants.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/controllers.py` & `panda-python-0.5.1/src/panda_py/controllers.py`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/src/panda_py/libfranka/__init__.pyi` & `panda-python-0.5.1/src/panda_py/libfranka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `panda-python-0.5.0/PKG-INFO` & `panda-python-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-python
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python bindings for the Panda
 Keywords: python real-time control robot franka emika
 Author-Email: Jean Elsner <jean.elsner@tum.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,19 +223,19 @@
 Requires-Dist: spatialmath; extra == "examples"
 Requires-Dist: ansitable; extra == "examples"
 Requires-Dist: qpsolvers; extra == "examples"
 Provides-Extra: examples
 Description-Content-Type: text/markdown
 
 # panda-py
-![logo](logo.jpg)
+![logo](https://github.com/JeanElsner/panda-py/blob/main/logo.jpg?raw=true)
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JeanElsner/panda-py/build.yml)](https://github.com/JeanElsner/panda-py/actions/workflows/build.yml)
 [![GitHub](https://img.shields.io/github/license/JeanElsner/panda-py)](https://www.apache.org/licenses/LICENSE-2.0)
-[![PyPI](https://img.shields.io/pypi/v/panda-py)](https://pypi.org/project/panda-python/)
+[![PyPI](https://img.shields.io/pypi/v/panda-python)](https://pypi.org/project/panda-python/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/panda-python)
 
 Finally, Python bindings for the Panda. These will increase your productivity by 1000%, guaranteed[^1]!
 
 > **Info**
 >
 > Please consider this a work in progress. Documentation, continuous integration pipeline and a companion paper are currently being prepared.
```

