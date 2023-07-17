# Comparing `tmp/aestream-0.5.1.tar.gz` & `tmp/aestream-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aestream-0.5.1.tar", last modified: Tue Mar 28 17:45:00 2023, max compression
+gzip compressed data, was "aestream-0.6.0.tar", last modified: Mon Jul 17 11:33:31 2023, max compression
```

## Comparing `aestream-0.5.1.tar` & `aestream-0.6.0.tar`

### file list

```diff
@@ -1,89 +1,92 @@
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.548962 aestream-0.5.1/
--rw-rw-r--   0 jens      (1002) jens      (1002)      226 2023-03-01 13:38:29.000000 aestream-0.5.1/AUTHORS
--rw-rw-r--   0 jens      (1002) jens      (1002)      736 2023-03-23 15:08:51.000000 aestream-0.5.1/CMakeLists.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)     1073 2023-01-19 14:20:33.000000 aestream-0.5.1/LICENSE
--rw-rw-r--   0 jens      (1002) jens      (1002)       91 2023-01-19 14:20:33.000000 aestream-0.5.1/MANIFEST.in
--rw-rw-r--   0 jens      (1002) jens      (1002)     9734 2023-03-28 17:45:00.548962 aestream-0.5.1/PKG-INFO
--rw-rw-r--   0 jens      (1002) jens      (1002)     9057 2023-03-23 15:08:51.000000 aestream-0.5.1/README.md
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.536962 aestream-0.5.1/aestream/
--rw-rw-r--   0 jens      (1002) jens      (1002)      683 2023-03-23 15:08:51.000000 aestream-0.5.1/aestream/__init__.py
--rw-rw-r--   0 jens      (1002) jens      (1002)     2696 2023-03-01 13:38:29.000000 aestream-0.5.1/aestream/__init__.pyi
--rw-rw-r--   0 jens      (1002) jens      (1002)      944 2023-03-23 15:08:51.000000 aestream-0.5.1/aestream/_input.py
--rw-rw-r--   0 jens      (1002) jens      (1002)        0 2023-03-01 13:38:29.000000 aestream-0.5.1/aestream/py.typed
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.536962 aestream-0.5.1/aestream.egg-info/
--rw-rw-r--   0 jens      (1002) jens      (1002)     9734 2023-03-28 17:45:00.000000 aestream-0.5.1/aestream.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1002) jens      (1002)     1821 2023-03-28 17:45:00.000000 aestream-0.5.1/aestream.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)        1 2023-03-28 17:45:00.000000 aestream-0.5.1/aestream.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)       21 2023-03-28 17:45:00.000000 aestream-0.5.1/aestream.egg-info/requires.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)        9 2023-03-28 17:45:00.000000 aestream-0.5.1/aestream.egg-info/top_level.txt
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.540962 aestream-0.5.1/include/
--rw-rw-r--   0 jens      (1002) jens      (1002)   349879 2023-01-19 14:20:34.000000 aestream-0.5.1/include/CLI11.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      851 2023-01-20 06:25:01.000000 aestream-0.5.1/include/CPM.cmake
--rw-rw-r--   0 jens      (1002) jens      (1002)   115918 2023-01-19 14:20:34.000000 aestream-0.5.1/include/rapidxml.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      222 2023-03-27 22:28:22.000000 aestream-0.5.1/pyproject.toml
--rw-rw-r--   0 jens      (1002) jens      (1002)       38 2023-03-28 17:45:00.548962 aestream-0.5.1/setup.cfg
--rw-rw-r--   0 jens      (1002) jens      (1002)     1611 2023-03-28 17:24:47.000000 aestream-0.5.1/setup.py
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.540962 aestream-0.5.1/src/
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.540962 aestream-0.5.1/src/.ipynb_checkpoints/
--rw-r--r--   0 jens      (1002) jens      (1002)     8580 2023-01-04 17:21:35.000000 aestream-0.5.1/src/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-rw-r--   0 jens      (1002) jens      (1002)     1144 2023-03-27 22:49:46.000000 aestream-0.5.1/src/CMakeLists.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)      170 2023-01-20 06:25:01.000000 aestream-0.5.1/src/aer.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     6205 2023-03-27 22:28:22.000000 aestream-0.5.1/src/aestream.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1760 2023-01-19 14:20:34.000000 aestream-0.5.1/src/dvs_gesture.hpp
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.540962 aestream-0.5.1/src/file/
--rw-rw-r--   0 jens      (1002) jens      (1002)     1840 2023-03-27 22:48:28.000000 aestream-0.5.1/src/file/CMakeLists.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)     5159 2023-03-27 21:37:09.000000 aestream-0.5.1/src/file/aedat.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)    14913 2023-03-27 22:52:29.000000 aestream-0.5.1/src/file/aedat4.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     3803 2023-03-27 22:50:54.000000 aestream-0.5.1/src/file/dat.hpp
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.540962 aestream-0.5.1/src/file/flatbuffers/
--rw-rw-r--   0 jens      (1002) jens      (1002)      127 2023-01-20 06:25:01.000000 aestream-0.5.1/src/file/flatbuffers/events.fbs
--rw-rw-r--   0 jens      (1002) jens      (1002)      304 2023-03-20 10:05:10.000000 aestream-0.5.1/src/file/flatbuffers/file_data_table.fbs
--rw-rw-r--   0 jens      (1002) jens      (1002)      346 2023-01-20 06:25:01.000000 aestream-0.5.1/src/file/flatbuffers/frame.fbs
--rw-rw-r--   0 jens      (1002) jens      (1002)      353 2023-01-20 06:25:01.000000 aestream-0.5.1/src/file/flatbuffers/imus.fbs
--rw-rw-r--   0 jens      (1002) jens      (1002)      208 2023-01-20 06:25:01.000000 aestream-0.5.1/src/file/flatbuffers/ioheader.fbs
--rw-rw-r--   0 jens      (1002) jens      (1002)      452 2023-01-20 06:25:01.000000 aestream-0.5.1/src/file/flatbuffers/trigger.fbs
--rw-rw-r--   0 jens      (1002) jens      (1002)     1094 2023-03-27 22:48:56.000000 aestream-0.5.1/src/file/utils.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     2617 2023-02-27 22:10:28.000000 aestream-0.5.1/src/generator.hpp
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.544962 aestream-0.5.1/src/input/
--rw-rw-r--   0 jens      (1002) jens      (1002)     2819 2023-02-27 22:10:28.000000 aestream-0.5.1/src/input/CMakeLists.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)      422 2023-03-28 17:24:41.000000 aestream-0.5.1/src/input/file.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      559 2023-03-27 22:49:08.000000 aestream-0.5.1/src/input/file.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     4139 2023-01-20 06:25:01.000000 aestream-0.5.1/src/input/inivation.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1191 2023-01-20 06:25:01.000000 aestream-0.5.1/src/input/inivation.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     2309 2023-01-20 06:25:01.000000 aestream-0.5.1/src/input/prophesee.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      332 2023-01-20 06:25:01.000000 aestream-0.5.1/src/input/prophesee.hpp
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.544962 aestream-0.5.1/src/output/
--rw-rw-r--   0 jens      (1002) jens      (1002)      524 2023-02-27 22:14:23.000000 aestream-0.5.1/src/output/CMakeLists.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)     1579 2023-01-20 06:25:01.000000 aestream-0.5.1/src/output/dvs_to_file.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      442 2023-01-20 06:25:01.000000 aestream-0.5.1/src/output/dvs_to_file.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     2121 2023-01-20 06:25:01.000000 aestream-0.5.1/src/output/dvs_to_tensor.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      658 2023-01-20 06:25:01.000000 aestream-0.5.1/src/output/dvs_to_tensor.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     3511 2023-01-20 06:25:01.000000 aestream-0.5.1/src/output/dvs_to_udp.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      695 2023-01-20 06:25:01.000000 aestream-0.5.1/src/output/dvs_to_udp.hpp
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.544962 aestream-0.5.1/src/pybind/
--rw-rw-r--   0 jens      (1002) jens      (1002)     2719 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/CMakeLists.txt
--rw-rw-r--   0 jens      (1002) jens      (1002)     3626 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/convert.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      604 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/convert.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     3408 2023-03-27 22:51:47.000000 aestream-0.5.1/src/pybind/file.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1272 2023-03-27 22:49:22.000000 aestream-0.5.1/src/pybind/file.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      112 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/input.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     2787 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/iterator.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     4581 2023-03-27 22:28:22.000000 aestream-0.5.1/src/pybind/module.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     3799 2023-03-27 22:52:22.000000 aestream-0.5.1/src/pybind/tensor_buffer.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1800 2023-03-27 22:28:22.000000 aestream-0.5.1/src/pybind/tensor_buffer.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1080 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/tensor_buffer_kernel.cu
--rw-rw-r--   0 jens      (1002) jens      (1002)      697 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/tensor_iterator.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      524 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/tensor_iterator.hpp
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.548962 aestream-0.5.1/src/pybind/test/
--rw-rw-r--   0 jens      (1002) jens      (1002)      263 2023-03-27 22:28:22.000000 aestream-0.5.1/src/pybind/test/__init__.py
-drwxrwxr-x   0 jens      (1002) jens      (1002)        0 2023-03-28 17:45:00.548962 aestream-0.5.1/src/pybind/test/__pycache__/
--rw-rw-r--   0 jens      (1002) jens      (1002)      494 2023-03-27 22:01:43.000000 aestream-0.5.1/src/pybind/test/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jens      (1002) jens      (1002)     5522 2023-03-27 22:01:43.000000 aestream-0.5.1/src/pybind/test/__pycache__/test_file.cpython-310-pytest-7.2.2.pyc
--rw-rw-r--   0 jens      (1002) jens      (1002)     2600 2023-03-27 22:52:08.000000 aestream-0.5.1/src/pybind/test/test_file.py
--rw-rw-r--   0 jens      (1002) jens      (1002)     1477 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/test/test_udp.py
--rw-rw-r--   0 jens      (1002) jens      (1002)      176 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/types.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1483 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/udp.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1155 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/udp_client.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)      126 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/udp_client.hpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     1704 2023-03-23 16:08:49.000000 aestream-0.5.1/src/pybind/usb.cpp
--rw-rw-r--   0 jens      (1002) jens      (1002)     5244 2023-01-19 14:20:34.000000 aestream-0.5.1/src/viewer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.559353 aestream-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-17 11:33:08.000000 aestream-0.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-17 11:33:08.000000 aestream-0.6.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-17 11:33:08.000000 aestream-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 11:33:08.000000 aestream-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-17 11:33:31.559353 aestream-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-17 11:33:08.000000 aestream-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.551353 aestream-0.6.0/aestream/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-17 11:33:08.000000 aestream-0.6.0/aestream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-17 11:33:08.000000 aestream-0.6.0/aestream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-17 11:33:08.000000 aestream-0.6.0/aestream/_genn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-17 11:33:08.000000 aestream-0.6.0/aestream/_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:08.000000 aestream-0.6.0/aestream/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.551353 aestream-0.6.0/aestream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-17 11:33:31.000000 aestream-0.6.0/aestream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-17 11:33:31.000000 aestream-0.6.0/aestream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:33:31.000000 aestream-0.6.0/aestream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 11:33:31.000000 aestream-0.6.0/aestream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 11:33:31.000000 aestream-0.6.0/aestream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.551353 aestream-0.6.0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)   370620 2023-07-17 11:33:08.000000 aestream-0.6.0/include/CLI11.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-17 11:33:08.000000 aestream-0.6.0/include/CPM.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)   115918 2023-07-17 11:33:08.000000 aestream-0.6.0/include/rapidxml.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 11:33:08.000000 aestream-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:33:31.559353 aestream-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-17 11:33:08.000000 aestream-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.551353 aestream-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-17 11:33:08.000000 aestream-0.6.0/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 11:33:08.000000 aestream-0.6.0/src/aer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-17 11:33:08.000000 aestream-0.6.0/src/aestream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 11:33:08.000000 aestream-0.6.0/src/dvs_gesture.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.555353 aestream-0.6.0/src/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/aedat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/aedat4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/csv.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/dat.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/evt3.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.555353 aestream-0.6.0/src/file/flatbuffers/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/flatbuffers/events.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/flatbuffers/file_data_table.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/flatbuffers/frame.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/flatbuffers/imus.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/flatbuffers/ioheader.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/flatbuffers/trigger.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-17 11:33:08.000000 aestream-0.6.0/src/file/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-17 11:33:08.000000 aestream-0.6.0/src/generator.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.555353 aestream-0.6.0/src/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/file.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/file.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/inivation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/inivation.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/prophesee.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/prophesee.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/zmq.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 11:33:08.000000 aestream-0.6.0/src/input/zmq.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.555353 aestream-0.6.0/src/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/dvs_to_file.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/dvs_to_file.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/dvs_to_tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/dvs_to_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/dvs_to_udp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 11:33:08.000000 aestream-0.6.0/src/output/dvs_to_udp.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.559353 aestream-0.6.0/src/pybind/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/convert.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/file.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/file.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/iterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/tensor_buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/tensor_buffer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/tensor_buffer_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/tensor_iterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/tensor_iterator.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.559353 aestream-0.6.0/src/pybind/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/test/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/test/test_udp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/types.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/udp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/udp_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/udp_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/usb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-17 11:33:08.000000 aestream-0.6.0/src/pybind/zmq.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:33:31.559353 aestream-0.6.0/src/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-17 11:33:08.000000 aestream-0.6.0/src/viewer/viewer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 11:33:08.000000 aestream-0.6.0/src/viewer/viewer.hpp
```

### Comparing `aestream-0.5.1/CMakeLists.txt` & `aestream-0.6.0/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,35 @@
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")
 
 option(USE_PYTHON "Buid Python lib" OFF)
 option(USE_CUDA "Build CUDA tensor export" OFF)
 
+find_package(libcaer CONFIG QUIET)
+option(USE_CAMERA "Build with camera drivers?" ${libcaer_FOUND})
+
 set(default_build_type Release)
 add_definitions(${GCC_COVERAGE_COMPILE_FLAGS})
 
 # Add includes
 include_directories("include/")
 include_directories("/opt/homebrew/opt/lz4/include")
 link_directories("/opt/homebrew/opt/lz4/lib")
+include_directories("/opt/local/include")
+link_directories("/opt/local/lib")
+include_directories("/opt/homebrew/opt/sdl2/include/")
+link_directories("/opt/homebrew/opt/sdl2/lib")
 include(include/CPM.cmake)
 
 # Add tests
 if (CMAKE_BUILD_TYPE STREQUAL "Debug")
     set(USE_TORCH ON)
     add_subdirectory("test")
+    set(CMAKE_CXX_FLAGS_DEBUG "-g -O0")
 else()
     set(GCC_COVERAGE_COMPILE_FLAGS ${GCC_COVERAGE_COMPILE_FLAGS} "-03")
 endif()
 
 
 # Add sources
 add_subdirectory("src")
```

### Comparing `aestream-0.5.1/LICENSE` & `aestream-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/PKG-INFO` & `aestream-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,75 @@
 Metadata-Version: 2.1
 Name: aestream
-Version: 0.5.1
+Version: 0.6.0
 Summary: Streaming library for Address-Event Representation (AER) data
-Home-page: https://github.com/norse/aestream
-Author: Jens E. Pedersen, Christian Pehle
-Author-email: jens@jepedersen.dk, christian.pehle@gmail.com
+Home-page: https://github.com/aestream/aestream
+Author: Jens E. Pedersen
+Author-email: jens@jepedersen.dk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 License-File: LICENSE
 License-File: AUTHORS
 
-# AEStream - Address Event streaming library
+
+<img src="https://github.com/aestream/aestream/raw/main/logo.png" />
 
 <p align="center">
-    <a href="https://github.com/norse/aestream/actions">
-        <img src="https://github.com/norse/aestream/workflows/Build%20and%20test/badge.svg" alt="Test status"></a>
+    <a href="https://github.com/aestream/aestream/actions">
+        <img src="https://github.com/aestream/aestream/workflows/Build%20and%20test/badge.svg" alt="Test status"></a>
     <a href="https://pypi.org/project/aestream/" alt="PyPi">
         <img src="https://img.shields.io/pypi/v/aestream" />
     </a>
-    <a href="https://github.com/norse/aestream/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/last-commit/norse/aestream" />
+    <a href="https://github.com/aestream/aestream/pulse" alt="Activity">
+        <img src="https://img.shields.io/github/last-commit/aestream/aestream" />
     </a>
     <a href="https://discord.gg/7fGN359">
         <img src="https://img.shields.io/discord/723215296399147089"
             alt="chat on Discord"></a>
-    <a href="https://www.codacy.com/gh/norse/aestream/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=norse/aestream&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7"/></a>
+    <a href="https://www.codacy.com/gh/aestream/aestream/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=aestream/aestream&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7"/></a>
     <a href="https://doi.org/10.5281/zenodo.6322829"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6322829.svg" alt="DOI"></a>
 </p>
 
-AEStream efficiently reads sparse events from an input source and streams it to an output sink.
-AEStream supports reading from files, USB cameras, as well as network via UDP and can stream events to files, network over UDP, and peripherals such as [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit)s and [neuromorphic hardware](https://en.wikipedia.org/wiki/Neuromorphic_engineering).
+AEStream effiently sends event-based data from A to B.
+AEStream can be used from the command-line, via Python, or as a C++ library.
+We support multiple inputs and outputs, providing seamless integration with files, [event cameras](https://en.wikipedia.org/wiki/Event_camera), network data, Python libraries via Numpy or PyTorch, and visualization tools.
 
-<img src="https://jegp.github.io/aestream-paper/2212_aestream.svg" />
+<img src="https://github.com/aestream/aestream/raw/main/docs/aestream_flow.png" />
 
-Read more in [the AEStream publication](https://jegp.github.io/aestream-paper/).
+Read more about the inner workings of the library in [the AEStream publication](https://jegp.github.io/aestream-paper/).
 
 ## Installation
 
-AEStream is usable both as a command-line binary or Python tool.
+> Read more in our [installation guide](https://aestream.github.io/aestream/install.html)
+
+The fastest way to install AEStream is by using pip: `pip install aestream`.
+See below for other sources.
 
-| **Source** | **Installation** |
-| -------------------- | --- |
-| [pip](https://pypi.org/) | <code>pip install aestream <br/> pip install aestream[torch]</code> ([PyTorch support](https://pytorch.com)) |
-| [nix](https://nixos.org/) | <code>nix run github:norse/aestream</code> (CLI) <br/> <code>nix develop github:norse/aestream</code> (Python environment) |
-| [docker](https://docker.com/) | See [Installation documentation](https://norse.github.io/aestream/install.html) |
+| **Source** | **Installation** | **Description** |
+| -------------------- | --- | --- |
+| [pip](https://pypi.org/) | <code>pip install aestream</code> <br/> <code>pip install aestream[torch]</code> <br/> <code>pip install aestream --no-binary</code> | <br/> [PyTorch support](https://pytorch.com) <br/> <a href="https://aestream.github.io/aestream/install.html#Event-camera-support">Requires camera drivers*</a> |
+| [nix](https://nixos.org/) | <code>nix run github:aestream/aestream</code> <br/> <code>nix develop github:aestream/aestream</code> | Command-line interface <br/> Python environment |
+| [docker](https://docker.com/) | See <a href="https://aestream.github.io/aestream/install.html">Installation documentation</a> |
+
+<span style="font-size: 80%">
+* Event camera support requires available drivers. <a href="https://aestream.github.io/aestream/install.html">A step-by-step guide is available in our documentation</a>.
+</span>
 
 Contributions to support AEStream on additional platforms are always welcome.
 
-## Usage: read event-address files in Python
+## Usage (Python)
+
+> Read more in our [Python usage guide](https://aestream.github.io/aestream/python_usage.html)
 
 AEStream can process fixed input sources like files like so:
 
 ```python
 FileInput("file", (640, 480)).load()
 ```
 
@@ -78,101 +89,77 @@
 # Stream events from UDP port 3333 (default)
 with UDPInput((640, 480), port=3333) as stream:
     while True:
         frame = stream.read() # Provides a (640, 480) tensor
         ...
 ```
 
-More examples can be found in [our example folder](https://github.com/norse/aestream/tree/master/example).
+More examples can be found in [our example folder](https://github.com/aestream/aestream/tree/master/example).
 Please note the examples may require additional dependencies (such as [Norse](https://github.com/norse/norse) for spiking networks or [PySDL](https://github.com/py-sdl/py-sdl2) for rendering). To install all the requirements, simply stand in the `aestream` root directory and run `pip install -r example/requirements.txt`
 
 ### Example: real-time edge detection with spiking neural networks
 
-![](example/usb_edgedetection.gif)
+![](https://media.githubusercontent.com/media/aestream/aestream/main/example/usb_edgedetection.gif)
 
 We stream events from a camera connected via USB and process them on a GPU in real-time using the [spiking neural network library, Norse](https://github.com/norse/norse) using fewer than 50 lines of Python.
 The left panel in the video shows the raw signal, while the middle and right panels show horizontal and vertical edge detection respectively.
-The full example can be found in [`example/usb_edgedetection.py`](https://github.com/norse/aestream/blob/main/example/usb_edgedetection.py)
+The full example can be found in [`example/usb_edgedetection.py`](https://github.com/aestream/aestream/blob/main/example/usb_edgedetection.py)
 
 ## Usage (CLI)
+> Read more in our [CLI usage documentation page](https://aestream.github.io/aestream/install.html)
 
 Installing AEStream also gives access to the command-line interface (CLI) `aestream`.
 To use `aestraem`, simply provide an `input` source and an optional `output` sink (defaulting to STDOUT):
 
 ```bash
 aestream input <input source> [output <output sink>]
 ```
 ## Supported Inputs and Outputs
 
-| Input | Description | Usage |
+| Input | Description | Example usage |
 | --------- | :----------- | ----- |
 | DAVIS, DVXPlorer | [Inivation](https://inivation.com/) DVS Camera over USB | `input inivation` |
 | EVK Cameras      | [Prophesee](https://www.prophesee.ai/) DVS camera over USB  | `input prophesee` |
-| File             | [AEDAT file format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md) as `.aedat`, `.aedat4`, or `.dat` | `input file x.aedat4` |
+| File             | Reads `.aedat`, `.aedat4`, `.csv`, `.dat`, or `.raw` files | `input file x.aedat4` |
+| [SynSense Speck](https://www.synsense.ai/products/speck-2/) | Stream events via ZMQ | `input speck` |
+| UDP network | Receives stream of events via the [SPIF protocol](https://github.com/SpiNNakerManchester/spif/tree/master/spiffer) | `input udp`
 
-| Output | Description | Usage |
+| Output | Description | Example usage |
 | --------- | ----------- | ----- |
 | STDOUT    | Standard output (default output) | `output stdout`
 | Ethernet over UDP | Outputs to a given IP and port using the [SPIF protocol](https://github.com/SpiNNakerManchester/spif)  | `output udp 10.0.0.1 1234` |
-| `.aedat4` file  | Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` |
-| CSV file       | Output to comma-separated-value (CSV) file format | `output file my_file.txt` |
+| File: `.aedat4`  | Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` |
+| File: `.csv`       | Output to comma-separated-value (CSV) file format | `output file my_file.csv` |
+| Viewer | View live event stream | `output view`
 
-### CLI examples
+## CLI examples
 
 | Example | Syntax |
 | ------------- | ------------------------------|
-| Echo file to STDOUT | `aestream input file example/sample.aedat4` |
-| Stream DVS cameara from iniVation AG to STDOUT (Note, requires Inivation libraries) | `aestream input inivation output stdout` |
-| Stream DVS camera from Prophesee to STDOUT (Note, requires Metavision SDK) | `aestream input output stdout` |
-| Read file to remote IP X.X.X.X | `aestream input file example/sample.aedat4 output udp X.X.X.X` |
-
-## Custom installation (C++)
-
-[Metavision SDK](https://docs.prophesee.ai/stable/metavision_sdk/index.html) and [libcaer](https://github.com/inivation/libcaer) are optional dependencies, but are needed for connecting to Prophesee and Inivation cameras respectively.
-
-AEStream is based on [C++20](https://en.cppreference.com/w/cpp/20). Since C++20 is not yet fully supported by all compilers, we recommend using `GCC >= 10.2`. 
-
-To build the binaries of this repository, run the following code:
-```
-# Optional: Ensure paths to libcaer or Metavision are in place
-mkdir build/
-cd build/
-cmake -GNinja ..
-ninja
-```
-
-If your default C++ compiler doesn't support C++ 20, you will have to install an up-to-date compiler and provide the environmental variable `CXX`.
-For instance like this: `CXX=/path/to/g++-10 cmake -GNinja ..`
-
-### Inivation cameras
-For [Inivation](https://inivation.com/) cameras, the [libcaer](https://gitlab.com/inivation/dv/libcaer/) library needs to be available, either by a `-DCMAKE_PREFIX_PATH` flag to `cmake` or included in the `PATH` environmental variable.
-For examble: `cmake -GNinja -DCMAKE_PREFIX_PATH=/path/to/libcaer`.
-Inivation made the library available for most operating systems, but you may have to build it yourself.
-
-### Prophesee cameras
-For [Prophesee](https://www.prophesee.ai/) cameras, a version of the [Metavision SDK](https://www.prophesee.ai/metavision-intelligence/) needs to be present.
-The open-source version the SDK `openeb` is available with installation instructions at https://github.com/prophesee-ai/openeb.
-Using `openeb`, it should be sufficient to install it using `cmake && make && make install` to put it in your path.
-Otherwise, you can point to it using the `-DCMAKE_PREFIX_PATH` option in `cmake`.
+| View live stream of Inivation camera (requires Inivation drivers) | `aestream input inivation output view` |
+| Stream Prophesee camera over the network to 10.0.0.1 (requires Metavision SDK) | `aestream input output udp 10.0.0.1` |
+| Convert `.dat` file to `.aedat4` | `aestream input example/sample.dat output file converted.aedat4` |
 
 ## Acknowledgments
 
 AEStream is developed by (in alphabetical order):
 
 * Cameron Barker (@GitHub [cameron-git](https://github.com/cameron-git/))
+* [Juan Pablo Romero Bermudez](https://www.kth.se/profile/jprb) (@GitHub [jpromerob](https://github.com/jpromerob/))
 * Alexander Hadjivanov (@Github [cantordust](https://github.com/cantordust))
+* Emil Jansson (@GitHub [emijan-kth](https://github.com/emijan-kth))
 * [Jens E. Pedersen](https://www.kth.se/profile/jeped) (@GitHub [jegp](https://github.com/jegp/))
 * [Christian Pehle](https://www.kip.uni-heidelberg.de/people/10110) (@GitHub [cpehle](https://github.com/cpehle/))
 
 The work has received funding from the EC Horizon 2020 Framework Programme under Grant Agreements 785907 and 945539 (HBP) and by the Deutsche Forschungsgemeinschaft (DFG, German Research Fundation) under Germany's Excellence Strategy EXC 2181/1 - 390900948 (the Heidelberg STRUCTURES Excellence Cluster).
 
 Thanks to [Philipp Mondorf](https://github.com/PMMon) for interfacing with Metavision SDK and preliminary network code.
 
-<a href="https://github.com/norse/aestream/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=norse/aestream" />
+<a href="https://github.com/aestream/aestream/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=aestream/aestream" />
 </a>
 
 
 ## Citation
 
 Please cite `aestream` if you use it in your work:
```

#### html2text {}

```diff
@@ -1,117 +1,107 @@
-Metadata-Version: 2.1 Name: aestream Version: 0.5.1 Summary: Streaming library
+Metadata-Version: 2.1 Name: aestream Version: 0.6.0 Summary: Streaming library
 for Address-Event Representation (AER) data Home-page: https://github.com/
-norse/aestream Author: Jens E. Pedersen, Christian Pehle Author-email:
-jens@jepedersen.dk, christian.pehle@gmail.com License: MIT Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C++ Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: System :: Hardware :: Universal
-Serial Bus (USB) Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: torch License-File: LICENSE License-File: AUTHORS # AEStream -
-Address Event streaming library
+aestream/aestream Author: Jens E. Pedersen Author-email: jens@jepedersen.dk
+License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: C++
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+System :: Hardware :: Universal Serial Bus (USB) Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: torch License-File:
+LICENSE License-File: AUTHORS [https://github.com/aestream/aestream/raw/main/
+logo.png]
 [Test_status] [https://img.shields.io/pypi/v/aestream] [https://img.shields.io/
- github/last-commit/norse/aestream] [chat_on_Discord] [https://app.codacy.com/
-          project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7] [DOI]
-AEStream efficiently reads sparse events from an input source and streams it to
-an output sink. AEStream supports reading from files, USB cameras, as well as
-network via UDP and can stream events to files, network over UDP, and
-peripherals such as [GPU](https://en.wikipedia.org/wiki/
-Graphics_processing_unit)s and [neuromorphic hardware](https://
-en.wikipedia.org/wiki/Neuromorphic_engineering). [https://jegp.github.io/
-aestream-paper/2212_aestream.svg] Read more in [the AEStream publication]
-(https://jegp.github.io/aestream-paper/). ## Installation AEStream is usable
-both as a command-line binary or Python tool. | **Source** | **Installation** |
-| -------------------- | --- | | [pip](https://pypi.org/) | pip install
-aestream
-pip install aestream[torch] ([PyTorch support](https://pytorch.com)) | | [nix]
-(https://nixos.org/) | nix run github:norse/aestream (CLI)
-nix develop github:norse/aestream (Python environment) | | [docker](https://
-docker.com/) | See [Installation documentation](https://norse.github.io/
-aestream/install.html) | Contributions to support AEStream on additional
-platforms are always welcome. ## Usage: read event-address files in Python
-AEStream can process fixed input sources like files like so: ```python
-FileInput("file", (640, 480)).load() ``` ## Usage: stream real-time data in
-Python AEStream also supports streaming data in real-time *without strict
-guarantees on orders*. This is particularly useful in real-time scenarios, for
-instance when operating with `USBInput` or `UDPInput` ```python # Stream events
-from a DVS camera over USB with USBInput((640, 480)) as stream: while True:
-frame = stream.read() # Provides a (640, 480) tensor ... ``` ```python # Stream
-events from UDP port 3333 (default) with UDPInput((640, 480), port=3333) as
-stream: while True: frame = stream.read() # Provides a (640, 480) tensor ...
-``` More examples can be found in [our example folder](https://github.com/
-norse/aestream/tree/master/example). Please note the examples may require
-additional dependencies (such as [Norse](https://github.com/norse/norse) for
-spiking networks or [PySDL](https://github.com/py-sdl/py-sdl2) for rendering).
-To install all the requirements, simply stand in the `aestream` root directory
-and run `pip install -r example/requirements.txt` ### Example: real-time edge
-detection with spiking neural networks ![](example/usb_edgedetection.gif) We
-stream events from a camera connected via USB and process them on a GPU in
-real-time using the [spiking neural network library, Norse](https://github.com/
-norse/norse) using fewer than 50 lines of Python. The left panel in the video
-shows the raw signal, while the middle and right panels show horizontal and
-vertical edge detection respectively. The full example can be found in
-[`example/usb_edgedetection.py`](https://github.com/norse/aestream/blob/main/
-example/usb_edgedetection.py) ## Usage (CLI) Installing AEStream also gives
-access to the command-line interface (CLI) `aestream`. To use `aestraem`,
-simply provide an `input` source and an optional `output` sink (defaulting to
-STDOUT): ```bash aestream input [                    ] [output ] ``` ##
-Supported Inputs and Outputs | Input | Description | Usage | | --------- | :---
--------- | ----- | | DAVIS, DVXPlorer | [Inivation](https://inivation.com/) DVS
-Camera over USB | `input inivation` | | EVK Cameras | [Prophesee](https://
-www.prophesee.ai/) DVS camera over USB | `input prophesee` | | File | [AEDAT
-file format](https://gitlab.com/inivation/inivation-docs/blob/master/
-Software%20user%20guides/AEDAT_file_formats.md) as `.aedat`, `.aedat4`, or
-`.dat` | `input file x.aedat4` | | Output | Description | Usage | | --------- |
------------ | ----- | | STDOUT | Standard output (default output) | `output
-stdout` | Ethernet over UDP | Outputs to a given IP and port using the [SPIF
-protocol](https://github.com/SpiNNakerManchester/spif) | `output udp 10.0.0.1
-1234` | | `.aedat4` file | Output to [`.aedat4` format](https://gitlab.com/
-inivation/inivation-docs/blob/master/Software%20user%20guides/
-AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` | | CSV file |
-Output to comma-separated-value (CSV) file format | `output file my_file.txt` |
-### CLI examples | Example | Syntax | | ------------- | -----------------------
--------| | Echo file to STDOUT | `aestream input file example/sample.aedat4` |
-| Stream DVS cameara from iniVation AG to STDOUT (Note, requires Inivation
-libraries) | `aestream input inivation output stdout` | | Stream DVS camera
-from Prophesee to STDOUT (Note, requires Metavision SDK) | `aestream input
-output stdout` | | Read file to remote IP X.X.X.X | `aestream input file
-example/sample.aedat4 output udp X.X.X.X` | ## Custom installation (C++)
-[Metavision SDK](https://docs.prophesee.ai/stable/metavision_sdk/index.html)
-and [libcaer](https://github.com/inivation/libcaer) are optional dependencies,
-but are needed for connecting to Prophesee and Inivation cameras respectively.
-AEStream is based on [C++20](https://en.cppreference.com/w/cpp/20). Since C++20
-is not yet fully supported by all compilers, we recommend using `GCC >= 10.2`.
-To build the binaries of this repository, run the following code: ``` #
-Optional: Ensure paths to libcaer or Metavision are in place mkdir build/ cd
-build/ cmake -GNinja .. ninja ``` If your default C++ compiler doesn't support
-C++ 20, you will have to install an up-to-date compiler and provide the
-environmental variable `CXX`. For instance like this: `CXX=/path/to/g++-10
-cmake -GNinja ..` ### Inivation cameras For [Inivation](https://inivation.com/
-) cameras, the [libcaer](https://gitlab.com/inivation/dv/libcaer/) library
-needs to be available, either by a `-DCMAKE_PREFIX_PATH` flag to `cmake` or
-included in the `PATH` environmental variable. For examble: `cmake -GNinja -
-DCMAKE_PREFIX_PATH=/path/to/libcaer`. Inivation made the library available for
-most operating systems, but you may have to build it yourself. ### Prophesee
-cameras For [Prophesee](https://www.prophesee.ai/) cameras, a version of the
-[Metavision SDK](https://www.prophesee.ai/metavision-intelligence/) needs to be
-present. The open-source version the SDK `openeb` is available with
-installation instructions at https://github.com/prophesee-ai/openeb. Using
-`openeb`, it should be sufficient to install it using `cmake && make && make
-install` to put it in your path. Otherwise, you can point to it using the `-
-DCMAKE_PREFIX_PATH` option in `cmake`. ## Acknowledgments AEStream is developed
-by (in alphabetical order): * Cameron Barker (@GitHub [cameron-git](https://
-github.com/cameron-git/)) * Alexander Hadjivanov (@Github [cantordust](https://
-github.com/cantordust)) * [Jens E. Pedersen](https://www.kth.se/profile/jeped)
+       github/last-commit/aestream/aestream] [chat_on_Discord] [https://
+  app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7] [DOI]
+AEStream effiently sends event-based data from A to B. AEStream can be used
+from the command-line, via Python, or as a C++ library. We support multiple
+inputs and outputs, providing seamless integration with files, [event cameras]
+(https://en.wikipedia.org/wiki/Event_camera), network data, Python libraries
+via Numpy or PyTorch, and visualization tools. [https://github.com/aestream/
+aestream/raw/main/docs/aestream_flow.png] Read more about the inner workings of
+the library in [the AEStream publication](https://jegp.github.io/aestream-
+paper/). ## Installation > Read more in our [installation guide](https://
+aestream.github.io/aestream/install.html) The fastest way to install AEStream
+is by using pip: `pip install aestream`. See below for other sources. |
+**Source** | **Installation** | **Description** | | -------------------- | --
+- | --- | | [pip](https://pypi.org/) | pip install aestream
+pip install aestream[torch]
+pip install aestream --no-binary |
+[PyTorch support](https://pytorch.com)
+Requires_camera_drivers* | | [nix](https://nixos.org/) | nix run github:
+aestream/aestream
+nix develop github:aestream/aestream | Command-line interface
+Python environment | | [docker](https://docker.com/) | See Installation
+documentation |  * Event camera support requires available drivers. A_step-by-
+step_guide_is_available_in_our_documentation.  Contributions to support
+AEStream on additional platforms are always welcome. ## Usage (Python) > Read
+more in our [Python usage guide](https://aestream.github.io/aestream/
+python_usage.html) AEStream can process fixed input sources like files like so:
+```python FileInput("file", (640, 480)).load() ``` ## Usage: stream real-time
+data in Python AEStream also supports streaming data in real-time *without
+strict guarantees on orders*. This is particularly useful in real-time
+scenarios, for instance when operating with `USBInput` or `UDPInput` ```python
+# Stream events from a DVS camera over USB with USBInput((640, 480)) as stream:
+while True: frame = stream.read() # Provides a (640, 480) tensor ... ```
+```python # Stream events from UDP port 3333 (default) with UDPInput((640,
+480), port=3333) as stream: while True: frame = stream.read() # Provides a
+(640, 480) tensor ... ``` More examples can be found in [our example folder]
+(https://github.com/aestream/aestream/tree/master/example). Please note the
+examples may require additional dependencies (such as [Norse](https://
+github.com/norse/norse) for spiking networks or [PySDL](https://github.com/py-
+sdl/py-sdl2) for rendering). To install all the requirements, simply stand in
+the `aestream` root directory and run `pip install -r example/requirements.txt`
+### Example: real-time edge detection with spiking neural networks ![](https://
+media.githubusercontent.com/media/aestream/aestream/main/example/
+usb_edgedetection.gif) We stream events from a camera connected via USB and
+process them on a GPU in real-time using the [spiking neural network library,
+Norse](https://github.com/norse/norse) using fewer than 50 lines of Python. The
+left panel in the video shows the raw signal, while the middle and right panels
+show horizontal and vertical edge detection respectively. The full example can
+be found in [`example/usb_edgedetection.py`](https://github.com/aestream/
+aestream/blob/main/example/usb_edgedetection.py) ## Usage (CLI) > Read more in
+our [CLI usage documentation page](https://aestream.github.io/aestream/
+install.html) Installing AEStream also gives access to the command-line
+interface (CLI) `aestream`. To use `aestraem`, simply provide an `input` source
+and an optional `output` sink (defaulting to STDOUT): ```bash aestream input
+[                    ] [output ] ``` ## Supported Inputs and Outputs | Input |
+Description | Example usage | | --------- | :----------- | ----- | | DAVIS,
+DVXPlorer | [Inivation](https://inivation.com/) DVS Camera over USB | `input
+inivation` | | EVK Cameras | [Prophesee](https://www.prophesee.ai/) DVS camera
+over USB | `input prophesee` | | File | Reads `.aedat`, `.aedat4`, `.csv`,
+`.dat`, or `.raw` files | `input file x.aedat4` | | [SynSense Speck](https://
+www.synsense.ai/products/speck-2/) | Stream events via ZMQ | `input speck` | |
+UDP network | Receives stream of events via the [SPIF protocol](https://
+github.com/SpiNNakerManchester/spif/tree/master/spiffer) | `input udp` | Output
+| Description | Example usage | | --------- | ----------- | ----- | | STDOUT |
+Standard output (default output) | `output stdout` | Ethernet over UDP |
+Outputs to a given IP and port using the [SPIF protocol](https://github.com/
+SpiNNakerManchester/spif) | `output udp 10.0.0.1 1234` | | File: `.aedat4` |
+Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/
+master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file
+my_file.aedat4` | | File: `.csv` | Output to comma-separated-value (CSV) file
+format | `output file my_file.csv` | | Viewer | View live event stream |
+`output view` ## CLI examples | Example | Syntax | | ------------- | ----------
+--------------------| | View live stream of Inivation camera (requires
+Inivation drivers) | `aestream input inivation output view` | | Stream
+Prophesee camera over the network to 10.0.0.1 (requires Metavision SDK) |
+`aestream input output udp 10.0.0.1` | | Convert `.dat` file to `.aedat4` |
+`aestream input example/sample.dat output file converted.aedat4` | ##
+Acknowledgments AEStream is developed by (in alphabetical order): * Cameron
+Barker (@GitHub [cameron-git](https://github.com/cameron-git/)) * [Juan Pablo
+Romero Bermudez](https://www.kth.se/profile/jprb) (@GitHub [jpromerob](https://
+github.com/jpromerob/)) * Alexander Hadjivanov (@Github [cantordust](https://
+github.com/cantordust)) * Emil Jansson (@GitHub [emijan-kth](https://
+github.com/emijan-kth)) * [Jens E. Pedersen](https://www.kth.se/profile/jeped)
 (@GitHub [jegp](https://github.com/jegp/)) * [Christian Pehle](https://
 www.kip.uni-heidelberg.de/people/10110) (@GitHub [cpehle](https://github.com/
 cpehle/)) The work has received funding from the EC Horizon 2020 Framework
 Programme under Grant Agreements 785907 and 945539 (HBP) and by the Deutsche
 Forschungsgemeinschaft (DFG, German Research Fundation) under Germany's
 Excellence Strategy EXC 2181/1 - 390900948 (the Heidelberg STRUCTURES
 Excellence Cluster). Thanks to [Philipp Mondorf](https://github.com/PMMon) for
 interfacing with Metavision SDK and preliminary network code. [https://
-contrib.rocks/image?repo=norse/aestream] ## Citation Please cite `aestream` if
-you use it in your work: ```bibtex @misc{aestream, doi = {10.48550/
+contrib.rocks/image?repo=aestream/aestream] ## Citation Please cite `aestream`
+if you use it in your work: ```bibtex @misc{aestream, doi = {10.48550/
 ARXIV.2212.10719}, url = {https://arxiv.org/abs/2212.10719}, author =
 {Pedersen, Jens Egholm and Conradt, JÃ¶rg}, title = {AEStream: Accelerated
 event-based processing with coroutines}, publisher = {arXiv}, year = {2022}, }
 ```
```

### Comparing `aestream-0.5.1/README.md` & `aestream-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-# AEStream - Address Event streaming library
+
+<img src="https://github.com/aestream/aestream/raw/main/logo.png" />
 
 <p align="center">
-    <a href="https://github.com/norse/aestream/actions">
-        <img src="https://github.com/norse/aestream/workflows/Build%20and%20test/badge.svg" alt="Test status"></a>
+    <a href="https://github.com/aestream/aestream/actions">
+        <img src="https://github.com/aestream/aestream/workflows/Build%20and%20test/badge.svg" alt="Test status"></a>
     <a href="https://pypi.org/project/aestream/" alt="PyPi">
         <img src="https://img.shields.io/pypi/v/aestream" />
     </a>
-    <a href="https://github.com/norse/aestream/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/last-commit/norse/aestream" />
+    <a href="https://github.com/aestream/aestream/pulse" alt="Activity">
+        <img src="https://img.shields.io/github/last-commit/aestream/aestream" />
     </a>
     <a href="https://discord.gg/7fGN359">
         <img src="https://img.shields.io/discord/723215296399147089"
             alt="chat on Discord"></a>
-    <a href="https://www.codacy.com/gh/norse/aestream/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=norse/aestream&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7"/></a>
+    <a href="https://www.codacy.com/gh/aestream/aestream/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=aestream/aestream&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7"/></a>
     <a href="https://doi.org/10.5281/zenodo.6322829"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6322829.svg" alt="DOI"></a>
 </p>
 
-AEStream efficiently reads sparse events from an input source and streams it to an output sink.
-AEStream supports reading from files, USB cameras, as well as network via UDP and can stream events to files, network over UDP, and peripherals such as [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit)s and [neuromorphic hardware](https://en.wikipedia.org/wiki/Neuromorphic_engineering).
+AEStream effiently sends event-based data from A to B.
+AEStream can be used from the command-line, via Python, or as a C++ library.
+We support multiple inputs and outputs, providing seamless integration with files, [event cameras](https://en.wikipedia.org/wiki/Event_camera), network data, Python libraries via Numpy or PyTorch, and visualization tools.
 
-<img src="https://jegp.github.io/aestream-paper/2212_aestream.svg" />
+<img src="https://github.com/aestream/aestream/raw/main/docs/aestream_flow.png" />
 
-Read more in [the AEStream publication](https://jegp.github.io/aestream-paper/).
+Read more about the inner workings of the library in [the AEStream publication](https://jegp.github.io/aestream-paper/).
 
 ## Installation
 
-AEStream is usable both as a command-line binary or Python tool.
+> Read more in our [installation guide](https://aestream.github.io/aestream/install.html)
+
+The fastest way to install AEStream is by using pip: `pip install aestream`.
+See below for other sources.
 
-| **Source** | **Installation** |
-| -------------------- | --- |
-| [pip](https://pypi.org/) | <code>pip install aestream <br/> pip install aestream[torch]</code> ([PyTorch support](https://pytorch.com)) |
-| [nix](https://nixos.org/) | <code>nix run github:norse/aestream</code> (CLI) <br/> <code>nix develop github:norse/aestream</code> (Python environment) |
-| [docker](https://docker.com/) | See [Installation documentation](https://norse.github.io/aestream/install.html) |
+| **Source** | **Installation** | **Description** |
+| -------------------- | --- | --- |
+| [pip](https://pypi.org/) | <code>pip install aestream</code> <br/> <code>pip install aestream[torch]</code> <br/> <code>pip install aestream --no-binary</code> | <br/> [PyTorch support](https://pytorch.com) <br/> <a href="https://aestream.github.io/aestream/install.html#Event-camera-support">Requires camera drivers*</a> |
+| [nix](https://nixos.org/) | <code>nix run github:aestream/aestream</code> <br/> <code>nix develop github:aestream/aestream</code> | Command-line interface <br/> Python environment |
+| [docker](https://docker.com/) | See <a href="https://aestream.github.io/aestream/install.html">Installation documentation</a> |
+
+<span style="font-size: 80%">
+* Event camera support requires available drivers. <a href="https://aestream.github.io/aestream/install.html">A step-by-step guide is available in our documentation</a>.
+</span>
 
 Contributions to support AEStream on additional platforms are always welcome.
 
-## Usage: read event-address files in Python
+## Usage (Python)
+
+> Read more in our [Python usage guide](https://aestream.github.io/aestream/python_usage.html)
 
 AEStream can process fixed input sources like files like so:
 
 ```python
 FileInput("file", (640, 480)).load()
 ```
 
@@ -59,101 +70,77 @@
 # Stream events from UDP port 3333 (default)
 with UDPInput((640, 480), port=3333) as stream:
     while True:
         frame = stream.read() # Provides a (640, 480) tensor
         ...
 ```
 
-More examples can be found in [our example folder](https://github.com/norse/aestream/tree/master/example).
+More examples can be found in [our example folder](https://github.com/aestream/aestream/tree/master/example).
 Please note the examples may require additional dependencies (such as [Norse](https://github.com/norse/norse) for spiking networks or [PySDL](https://github.com/py-sdl/py-sdl2) for rendering). To install all the requirements, simply stand in the `aestream` root directory and run `pip install -r example/requirements.txt`
 
 ### Example: real-time edge detection with spiking neural networks
 
-![](example/usb_edgedetection.gif)
+![](https://media.githubusercontent.com/media/aestream/aestream/main/example/usb_edgedetection.gif)
 
 We stream events from a camera connected via USB and process them on a GPU in real-time using the [spiking neural network library, Norse](https://github.com/norse/norse) using fewer than 50 lines of Python.
 The left panel in the video shows the raw signal, while the middle and right panels show horizontal and vertical edge detection respectively.
-The full example can be found in [`example/usb_edgedetection.py`](https://github.com/norse/aestream/blob/main/example/usb_edgedetection.py)
+The full example can be found in [`example/usb_edgedetection.py`](https://github.com/aestream/aestream/blob/main/example/usb_edgedetection.py)
 
 ## Usage (CLI)
+> Read more in our [CLI usage documentation page](https://aestream.github.io/aestream/install.html)
 
 Installing AEStream also gives access to the command-line interface (CLI) `aestream`.
 To use `aestraem`, simply provide an `input` source and an optional `output` sink (defaulting to STDOUT):
 
 ```bash
 aestream input <input source> [output <output sink>]
 ```
 ## Supported Inputs and Outputs
 
-| Input | Description | Usage |
+| Input | Description | Example usage |
 | --------- | :----------- | ----- |
 | DAVIS, DVXPlorer | [Inivation](https://inivation.com/) DVS Camera over USB | `input inivation` |
 | EVK Cameras      | [Prophesee](https://www.prophesee.ai/) DVS camera over USB  | `input prophesee` |
-| File             | [AEDAT file format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md) as `.aedat`, `.aedat4`, or `.dat` | `input file x.aedat4` |
+| File             | Reads `.aedat`, `.aedat4`, `.csv`, `.dat`, or `.raw` files | `input file x.aedat4` |
+| [SynSense Speck](https://www.synsense.ai/products/speck-2/) | Stream events via ZMQ | `input speck` |
+| UDP network | Receives stream of events via the [SPIF protocol](https://github.com/SpiNNakerManchester/spif/tree/master/spiffer) | `input udp`
 
-| Output | Description | Usage |
+| Output | Description | Example usage |
 | --------- | ----------- | ----- |
 | STDOUT    | Standard output (default output) | `output stdout`
 | Ethernet over UDP | Outputs to a given IP and port using the [SPIF protocol](https://github.com/SpiNNakerManchester/spif)  | `output udp 10.0.0.1 1234` |
-| `.aedat4` file  | Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` |
-| CSV file       | Output to comma-separated-value (CSV) file format | `output file my_file.txt` |
+| File: `.aedat4`  | Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` |
+| File: `.csv`       | Output to comma-separated-value (CSV) file format | `output file my_file.csv` |
+| Viewer | View live event stream | `output view`
 
-### CLI examples
+## CLI examples
 
 | Example | Syntax |
 | ------------- | ------------------------------|
-| Echo file to STDOUT | `aestream input file example/sample.aedat4` |
-| Stream DVS cameara from iniVation AG to STDOUT (Note, requires Inivation libraries) | `aestream input inivation output stdout` |
-| Stream DVS camera from Prophesee to STDOUT (Note, requires Metavision SDK) | `aestream input output stdout` |
-| Read file to remote IP X.X.X.X | `aestream input file example/sample.aedat4 output udp X.X.X.X` |
-
-## Custom installation (C++)
-
-[Metavision SDK](https://docs.prophesee.ai/stable/metavision_sdk/index.html) and [libcaer](https://github.com/inivation/libcaer) are optional dependencies, but are needed for connecting to Prophesee and Inivation cameras respectively.
-
-AEStream is based on [C++20](https://en.cppreference.com/w/cpp/20). Since C++20 is not yet fully supported by all compilers, we recommend using `GCC >= 10.2`. 
-
-To build the binaries of this repository, run the following code:
-```
-# Optional: Ensure paths to libcaer or Metavision are in place
-mkdir build/
-cd build/
-cmake -GNinja ..
-ninja
-```
-
-If your default C++ compiler doesn't support C++ 20, you will have to install an up-to-date compiler and provide the environmental variable `CXX`.
-For instance like this: `CXX=/path/to/g++-10 cmake -GNinja ..`
-
-### Inivation cameras
-For [Inivation](https://inivation.com/) cameras, the [libcaer](https://gitlab.com/inivation/dv/libcaer/) library needs to be available, either by a `-DCMAKE_PREFIX_PATH` flag to `cmake` or included in the `PATH` environmental variable.
-For examble: `cmake -GNinja -DCMAKE_PREFIX_PATH=/path/to/libcaer`.
-Inivation made the library available for most operating systems, but you may have to build it yourself.
-
-### Prophesee cameras
-For [Prophesee](https://www.prophesee.ai/) cameras, a version of the [Metavision SDK](https://www.prophesee.ai/metavision-intelligence/) needs to be present.
-The open-source version the SDK `openeb` is available with installation instructions at https://github.com/prophesee-ai/openeb.
-Using `openeb`, it should be sufficient to install it using `cmake && make && make install` to put it in your path.
-Otherwise, you can point to it using the `-DCMAKE_PREFIX_PATH` option in `cmake`.
+| View live stream of Inivation camera (requires Inivation drivers) | `aestream input inivation output view` |
+| Stream Prophesee camera over the network to 10.0.0.1 (requires Metavision SDK) | `aestream input output udp 10.0.0.1` |
+| Convert `.dat` file to `.aedat4` | `aestream input example/sample.dat output file converted.aedat4` |
 
 ## Acknowledgments
 
 AEStream is developed by (in alphabetical order):
 
 * Cameron Barker (@GitHub [cameron-git](https://github.com/cameron-git/))
+* [Juan Pablo Romero Bermudez](https://www.kth.se/profile/jprb) (@GitHub [jpromerob](https://github.com/jpromerob/))
 * Alexander Hadjivanov (@Github [cantordust](https://github.com/cantordust))
+* Emil Jansson (@GitHub [emijan-kth](https://github.com/emijan-kth))
 * [Jens E. Pedersen](https://www.kth.se/profile/jeped) (@GitHub [jegp](https://github.com/jegp/))
 * [Christian Pehle](https://www.kip.uni-heidelberg.de/people/10110) (@GitHub [cpehle](https://github.com/cpehle/))
 
 The work has received funding from the EC Horizon 2020 Framework Programme under Grant Agreements 785907 and 945539 (HBP) and by the Deutsche Forschungsgemeinschaft (DFG, German Research Fundation) under Germany's Excellence Strategy EXC 2181/1 - 390900948 (the Heidelberg STRUCTURES Excellence Cluster).
 
 Thanks to [Philipp Mondorf](https://github.com/PMMon) for interfacing with Metavision SDK and preliminary network code.
 
-<a href="https://github.com/norse/aestream/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=norse/aestream" />
+<a href="https://github.com/aestream/aestream/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=aestream/aestream" />
 </a>
 
 
 ## Citation
 
 Please cite `aestream` if you use it in your work:
```

#### html2text {}

```diff
@@ -1,108 +1,98 @@
-# AEStream - Address Event streaming library
+ [https://github.com/aestream/aestream/raw/main/logo.png]
 [Test_status] [https://img.shields.io/pypi/v/aestream] [https://img.shields.io/
- github/last-commit/norse/aestream] [chat_on_Discord] [https://app.codacy.com/
-          project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7] [DOI]
-AEStream efficiently reads sparse events from an input source and streams it to
-an output sink. AEStream supports reading from files, USB cameras, as well as
-network via UDP and can stream events to files, network over UDP, and
-peripherals such as [GPU](https://en.wikipedia.org/wiki/
-Graphics_processing_unit)s and [neuromorphic hardware](https://
-en.wikipedia.org/wiki/Neuromorphic_engineering). [https://jegp.github.io/
-aestream-paper/2212_aestream.svg] Read more in [the AEStream publication]
-(https://jegp.github.io/aestream-paper/). ## Installation AEStream is usable
-both as a command-line binary or Python tool. | **Source** | **Installation** |
-| -------------------- | --- | | [pip](https://pypi.org/) | pip install
-aestream
-pip install aestream[torch] ([PyTorch support](https://pytorch.com)) | | [nix]
-(https://nixos.org/) | nix run github:norse/aestream (CLI)
-nix develop github:norse/aestream (Python environment) | | [docker](https://
-docker.com/) | See [Installation documentation](https://norse.github.io/
-aestream/install.html) | Contributions to support AEStream on additional
-platforms are always welcome. ## Usage: read event-address files in Python
-AEStream can process fixed input sources like files like so: ```python
-FileInput("file", (640, 480)).load() ``` ## Usage: stream real-time data in
-Python AEStream also supports streaming data in real-time *without strict
-guarantees on orders*. This is particularly useful in real-time scenarios, for
-instance when operating with `USBInput` or `UDPInput` ```python # Stream events
-from a DVS camera over USB with USBInput((640, 480)) as stream: while True:
-frame = stream.read() # Provides a (640, 480) tensor ... ``` ```python # Stream
-events from UDP port 3333 (default) with UDPInput((640, 480), port=3333) as
-stream: while True: frame = stream.read() # Provides a (640, 480) tensor ...
-``` More examples can be found in [our example folder](https://github.com/
-norse/aestream/tree/master/example). Please note the examples may require
-additional dependencies (such as [Norse](https://github.com/norse/norse) for
-spiking networks or [PySDL](https://github.com/py-sdl/py-sdl2) for rendering).
-To install all the requirements, simply stand in the `aestream` root directory
-and run `pip install -r example/requirements.txt` ### Example: real-time edge
-detection with spiking neural networks ![](example/usb_edgedetection.gif) We
-stream events from a camera connected via USB and process them on a GPU in
-real-time using the [spiking neural network library, Norse](https://github.com/
-norse/norse) using fewer than 50 lines of Python. The left panel in the video
-shows the raw signal, while the middle and right panels show horizontal and
-vertical edge detection respectively. The full example can be found in
-[`example/usb_edgedetection.py`](https://github.com/norse/aestream/blob/main/
-example/usb_edgedetection.py) ## Usage (CLI) Installing AEStream also gives
-access to the command-line interface (CLI) `aestream`. To use `aestraem`,
-simply provide an `input` source and an optional `output` sink (defaulting to
-STDOUT): ```bash aestream input [                    ] [output ] ``` ##
-Supported Inputs and Outputs | Input | Description | Usage | | --------- | :---
--------- | ----- | | DAVIS, DVXPlorer | [Inivation](https://inivation.com/) DVS
-Camera over USB | `input inivation` | | EVK Cameras | [Prophesee](https://
-www.prophesee.ai/) DVS camera over USB | `input prophesee` | | File | [AEDAT
-file format](https://gitlab.com/inivation/inivation-docs/blob/master/
-Software%20user%20guides/AEDAT_file_formats.md) as `.aedat`, `.aedat4`, or
-`.dat` | `input file x.aedat4` | | Output | Description | Usage | | --------- |
------------ | ----- | | STDOUT | Standard output (default output) | `output
-stdout` | Ethernet over UDP | Outputs to a given IP and port using the [SPIF
-protocol](https://github.com/SpiNNakerManchester/spif) | `output udp 10.0.0.1
-1234` | | `.aedat4` file | Output to [`.aedat4` format](https://gitlab.com/
-inivation/inivation-docs/blob/master/Software%20user%20guides/
-AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` | | CSV file |
-Output to comma-separated-value (CSV) file format | `output file my_file.txt` |
-### CLI examples | Example | Syntax | | ------------- | -----------------------
--------| | Echo file to STDOUT | `aestream input file example/sample.aedat4` |
-| Stream DVS cameara from iniVation AG to STDOUT (Note, requires Inivation
-libraries) | `aestream input inivation output stdout` | | Stream DVS camera
-from Prophesee to STDOUT (Note, requires Metavision SDK) | `aestream input
-output stdout` | | Read file to remote IP X.X.X.X | `aestream input file
-example/sample.aedat4 output udp X.X.X.X` | ## Custom installation (C++)
-[Metavision SDK](https://docs.prophesee.ai/stable/metavision_sdk/index.html)
-and [libcaer](https://github.com/inivation/libcaer) are optional dependencies,
-but are needed for connecting to Prophesee and Inivation cameras respectively.
-AEStream is based on [C++20](https://en.cppreference.com/w/cpp/20). Since C++20
-is not yet fully supported by all compilers, we recommend using `GCC >= 10.2`.
-To build the binaries of this repository, run the following code: ``` #
-Optional: Ensure paths to libcaer or Metavision are in place mkdir build/ cd
-build/ cmake -GNinja .. ninja ``` If your default C++ compiler doesn't support
-C++ 20, you will have to install an up-to-date compiler and provide the
-environmental variable `CXX`. For instance like this: `CXX=/path/to/g++-10
-cmake -GNinja ..` ### Inivation cameras For [Inivation](https://inivation.com/
-) cameras, the [libcaer](https://gitlab.com/inivation/dv/libcaer/) library
-needs to be available, either by a `-DCMAKE_PREFIX_PATH` flag to `cmake` or
-included in the `PATH` environmental variable. For examble: `cmake -GNinja -
-DCMAKE_PREFIX_PATH=/path/to/libcaer`. Inivation made the library available for
-most operating systems, but you may have to build it yourself. ### Prophesee
-cameras For [Prophesee](https://www.prophesee.ai/) cameras, a version of the
-[Metavision SDK](https://www.prophesee.ai/metavision-intelligence/) needs to be
-present. The open-source version the SDK `openeb` is available with
-installation instructions at https://github.com/prophesee-ai/openeb. Using
-`openeb`, it should be sufficient to install it using `cmake && make && make
-install` to put it in your path. Otherwise, you can point to it using the `-
-DCMAKE_PREFIX_PATH` option in `cmake`. ## Acknowledgments AEStream is developed
-by (in alphabetical order): * Cameron Barker (@GitHub [cameron-git](https://
-github.com/cameron-git/)) * Alexander Hadjivanov (@Github [cantordust](https://
-github.com/cantordust)) * [Jens E. Pedersen](https://www.kth.se/profile/jeped)
+       github/last-commit/aestream/aestream] [chat_on_Discord] [https://
+  app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7] [DOI]
+AEStream effiently sends event-based data from A to B. AEStream can be used
+from the command-line, via Python, or as a C++ library. We support multiple
+inputs and outputs, providing seamless integration with files, [event cameras]
+(https://en.wikipedia.org/wiki/Event_camera), network data, Python libraries
+via Numpy or PyTorch, and visualization tools. [https://github.com/aestream/
+aestream/raw/main/docs/aestream_flow.png] Read more about the inner workings of
+the library in [the AEStream publication](https://jegp.github.io/aestream-
+paper/). ## Installation > Read more in our [installation guide](https://
+aestream.github.io/aestream/install.html) The fastest way to install AEStream
+is by using pip: `pip install aestream`. See below for other sources. |
+**Source** | **Installation** | **Description** | | -------------------- | --
+- | --- | | [pip](https://pypi.org/) | pip install aestream
+pip install aestream[torch]
+pip install aestream --no-binary |
+[PyTorch support](https://pytorch.com)
+Requires_camera_drivers* | | [nix](https://nixos.org/) | nix run github:
+aestream/aestream
+nix develop github:aestream/aestream | Command-line interface
+Python environment | | [docker](https://docker.com/) | See Installation
+documentation |  * Event camera support requires available drivers. A_step-by-
+step_guide_is_available_in_our_documentation.  Contributions to support
+AEStream on additional platforms are always welcome. ## Usage (Python) > Read
+more in our [Python usage guide](https://aestream.github.io/aestream/
+python_usage.html) AEStream can process fixed input sources like files like so:
+```python FileInput("file", (640, 480)).load() ``` ## Usage: stream real-time
+data in Python AEStream also supports streaming data in real-time *without
+strict guarantees on orders*. This is particularly useful in real-time
+scenarios, for instance when operating with `USBInput` or `UDPInput` ```python
+# Stream events from a DVS camera over USB with USBInput((640, 480)) as stream:
+while True: frame = stream.read() # Provides a (640, 480) tensor ... ```
+```python # Stream events from UDP port 3333 (default) with UDPInput((640,
+480), port=3333) as stream: while True: frame = stream.read() # Provides a
+(640, 480) tensor ... ``` More examples can be found in [our example folder]
+(https://github.com/aestream/aestream/tree/master/example). Please note the
+examples may require additional dependencies (such as [Norse](https://
+github.com/norse/norse) for spiking networks or [PySDL](https://github.com/py-
+sdl/py-sdl2) for rendering). To install all the requirements, simply stand in
+the `aestream` root directory and run `pip install -r example/requirements.txt`
+### Example: real-time edge detection with spiking neural networks ![](https://
+media.githubusercontent.com/media/aestream/aestream/main/example/
+usb_edgedetection.gif) We stream events from a camera connected via USB and
+process them on a GPU in real-time using the [spiking neural network library,
+Norse](https://github.com/norse/norse) using fewer than 50 lines of Python. The
+left panel in the video shows the raw signal, while the middle and right panels
+show horizontal and vertical edge detection respectively. The full example can
+be found in [`example/usb_edgedetection.py`](https://github.com/aestream/
+aestream/blob/main/example/usb_edgedetection.py) ## Usage (CLI) > Read more in
+our [CLI usage documentation page](https://aestream.github.io/aestream/
+install.html) Installing AEStream also gives access to the command-line
+interface (CLI) `aestream`. To use `aestraem`, simply provide an `input` source
+and an optional `output` sink (defaulting to STDOUT): ```bash aestream input
+[                    ] [output ] ``` ## Supported Inputs and Outputs | Input |
+Description | Example usage | | --------- | :----------- | ----- | | DAVIS,
+DVXPlorer | [Inivation](https://inivation.com/) DVS Camera over USB | `input
+inivation` | | EVK Cameras | [Prophesee](https://www.prophesee.ai/) DVS camera
+over USB | `input prophesee` | | File | Reads `.aedat`, `.aedat4`, `.csv`,
+`.dat`, or `.raw` files | `input file x.aedat4` | | [SynSense Speck](https://
+www.synsense.ai/products/speck-2/) | Stream events via ZMQ | `input speck` | |
+UDP network | Receives stream of events via the [SPIF protocol](https://
+github.com/SpiNNakerManchester/spif/tree/master/spiffer) | `input udp` | Output
+| Description | Example usage | | --------- | ----------- | ----- | | STDOUT |
+Standard output (default output) | `output stdout` | Ethernet over UDP |
+Outputs to a given IP and port using the [SPIF protocol](https://github.com/
+SpiNNakerManchester/spif) | `output udp 10.0.0.1 1234` | | File: `.aedat4` |
+Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/
+master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file
+my_file.aedat4` | | File: `.csv` | Output to comma-separated-value (CSV) file
+format | `output file my_file.csv` | | Viewer | View live event stream |
+`output view` ## CLI examples | Example | Syntax | | ------------- | ----------
+--------------------| | View live stream of Inivation camera (requires
+Inivation drivers) | `aestream input inivation output view` | | Stream
+Prophesee camera over the network to 10.0.0.1 (requires Metavision SDK) |
+`aestream input output udp 10.0.0.1` | | Convert `.dat` file to `.aedat4` |
+`aestream input example/sample.dat output file converted.aedat4` | ##
+Acknowledgments AEStream is developed by (in alphabetical order): * Cameron
+Barker (@GitHub [cameron-git](https://github.com/cameron-git/)) * [Juan Pablo
+Romero Bermudez](https://www.kth.se/profile/jprb) (@GitHub [jpromerob](https://
+github.com/jpromerob/)) * Alexander Hadjivanov (@Github [cantordust](https://
+github.com/cantordust)) * Emil Jansson (@GitHub [emijan-kth](https://
+github.com/emijan-kth)) * [Jens E. Pedersen](https://www.kth.se/profile/jeped)
 (@GitHub [jegp](https://github.com/jegp/)) * [Christian Pehle](https://
 www.kip.uni-heidelberg.de/people/10110) (@GitHub [cpehle](https://github.com/
 cpehle/)) The work has received funding from the EC Horizon 2020 Framework
 Programme under Grant Agreements 785907 and 945539 (HBP) and by the Deutsche
 Forschungsgemeinschaft (DFG, German Research Fundation) under Germany's
 Excellence Strategy EXC 2181/1 - 390900948 (the Heidelberg STRUCTURES
 Excellence Cluster). Thanks to [Philipp Mondorf](https://github.com/PMMon) for
 interfacing with Metavision SDK and preliminary network code. [https://
-contrib.rocks/image?repo=norse/aestream] ## Citation Please cite `aestream` if
-you use it in your work: ```bibtex @misc{aestream, doi = {10.48550/
+contrib.rocks/image?repo=aestream/aestream] ## Citation Please cite `aestream`
+if you use it in your work: ```bibtex @misc{aestream, doi = {10.48550/
 ARXIV.2212.10719}, url = {https://arxiv.org/abs/2212.10719}, author =
 {Pedersen, Jens Egholm and Conradt, JÃ¶rg}, title = {AEStream: Accelerated
 event-based processing with coroutines}, publisher = {arXiv}, year = {2022}, }
 ```
```

### Comparing `aestream-0.5.1/aestream/__init__.py` & `aestream-0.6.0/aestream/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 """
 AEStream library for streaming address-event representations.
 
-Please refer to https://github.com/norse/aestream for usage
+Please refer to https://github.com/aestream/aestream for usage
 """
+import logging
+
 try:
     import torch
 except ImportError:
-    import logging
-
     logging.debug("Failed to import Torch: AEStream is running in Numpy mode")
-    del logging
 
 # Import AEStream modules
 from aestream.aestream_ext import Event
 from aestream._input import FileInput, UDPInput
 
 modules = []
 try:
-    from aestream.aestream_ext import USBInput
+    from aestream._input import USBInput
 
     modules.append("USBInput")
 except ImportError:
-    import logging
-
     logging.debug("Failed to import AEStream USB Input")
-    del logging
 
-__all__ = ["Event", "FileInput", "UDPInput"] + modules
+try:
+    import aestream._genn as genn
+
+    modules.append("genn")
+except ImportError as ex:
+    logging.debug("Failed to import GeNN: AEStream cannot use GeNN device")
 
+try:
+    from aestream._input import SpeckInput
+
+    modules.append("SpeckInput")
+except ImportError:
+    logging.debug("Failed to import ZMQ: AEStream cannot use ZMQ input")
+
+del logging
+
+__all__ = ["Event", "FileInput", "UDPInput"] + modules
 del modules
```

### Comparing `aestream-0.5.1/aestream/__init__.pyi` & `aestream-0.6.0/aestream/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 # AEStream API Prototyping
 
 from typing import Union, Tuple
 import numpy as np
+
 try:
     import torch
 except:
     "torch not found, proceeding with numpy only"
 
-class FileInput():
+class FileInput:
     """
     If you see this, its good :)
     """
-    def init():
-        ...
-    
+
+    def init(): ...
     def read():
         """
         Read :P
         """
         ...
 
-class FileInputReader():
+class FileInputReader:
     """
     Load or Iterate Events or Frames from a file
 
     Supported file formats: aedat, aedat4, dat
 
     Args:
         file_path (str): Path of file to be used
         resolution (int, int): X,Y resolution of file
 
     Attributes:
         file_path (str): Path of file to be used
         resolution (int, int): X,Y resolution of file
     """
-    def __init__(self, file_path: str, resolution: Tuple[int, int]) -> None:
-        ...
 
-    def load(self, frame_ms: int = 0, device: str = "cpu") -> Union[np.ndarray, torch.tensor]  :
+    def __init__(self, file_path: str, resolution: Tuple[int, int]) -> None: ...
+    def load(
+        self, frame_ms: int = 0, device: str = "cpu"
+    ) -> Union[np.ndarray, torch.tensor]:
         """
         Loads the whole file onto device memory
 
         Args:
             frame_ms (int): Selects data format. When `0`, events are loaded as is.
                 Otherwise, events are accumulated into frames with synchronous period of `frame_ms`
             device (str: `cpu`, `cuda`): Selects the device to which the file is loaded
 
         Returns:
             Array/Tensor containing the contents of the file
         """
         ...
-    
-    def get_iterator(self, frame_ms: int = 0, device: str = "cpu", mode: str = "safe", memory_limit: int = 1024) -> FileInputIterator:
+    def get_iterator(
+        self,
+        frame_ms: int = 0,
+        device: str = "cpu",
+        mode: str = "safe",
+        memory_limit: int = 1024,
+    ) -> FileInputIterator:
         """
         Provides functionality that allows files larger than device memory to be iteratively loaded
 
         Args:
             frame_ms (int): Selects data format. When `0`, events are loaded as is. Otherwise, events are accumulated into frames with synchronous period of `frame_ms`
             device (str: `cpu`, `cuda`): Selects the device to which the file is loaded.
             mode (str: `safe`, `unsafe`): Selects if slower deterministic (`safe`) or faster nondeterministic (`unsafe`) method is used to create frames. When using `unsafe` the exact frame a event is part of is subject to jitter at runtime.
-        
+
         Returns:
             A generator that loads events or frames to `device` as specified.
         """
         ...
 
-class FileInputIterator():
+class FileInputIterator:
     """
     Load or Iterate Events or Frames from a file
 
     Supported file formats: aedat, aedat4, dat
 
     Args:
         file_path (str): Path of file to be used
         resolution (int, int): X,Y resolution of file
 
     Attributes:
         file_path (str): Path of file to be used
         resolution (int, int): X,Y resolution of file
     """
-    def __init__(self, file_path: str, resolution: Tuple[int, int]) -> None:
-        ...
+
+    def __init__(self, file_path: str, resolution: Tuple[int, int]) -> None: ...
```

### Comparing `aestream-0.5.1/aestream.egg-info/PKG-INFO` & `aestream-0.6.0/aestream.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,75 @@
 Metadata-Version: 2.1
 Name: aestream
-Version: 0.5.1
+Version: 0.6.0
 Summary: Streaming library for Address-Event Representation (AER) data
-Home-page: https://github.com/norse/aestream
-Author: Jens E. Pedersen, Christian Pehle
-Author-email: jens@jepedersen.dk, christian.pehle@gmail.com
+Home-page: https://github.com/aestream/aestream
+Author: Jens E. Pedersen
+Author-email: jens@jepedersen.dk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: torch
 License-File: LICENSE
 License-File: AUTHORS
 
-# AEStream - Address Event streaming library
+
+<img src="https://github.com/aestream/aestream/raw/main/logo.png" />
 
 <p align="center">
-    <a href="https://github.com/norse/aestream/actions">
-        <img src="https://github.com/norse/aestream/workflows/Build%20and%20test/badge.svg" alt="Test status"></a>
+    <a href="https://github.com/aestream/aestream/actions">
+        <img src="https://github.com/aestream/aestream/workflows/Build%20and%20test/badge.svg" alt="Test status"></a>
     <a href="https://pypi.org/project/aestream/" alt="PyPi">
         <img src="https://img.shields.io/pypi/v/aestream" />
     </a>
-    <a href="https://github.com/norse/aestream/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/last-commit/norse/aestream" />
+    <a href="https://github.com/aestream/aestream/pulse" alt="Activity">
+        <img src="https://img.shields.io/github/last-commit/aestream/aestream" />
     </a>
     <a href="https://discord.gg/7fGN359">
         <img src="https://img.shields.io/discord/723215296399147089"
             alt="chat on Discord"></a>
-    <a href="https://www.codacy.com/gh/norse/aestream/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=norse/aestream&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7"/></a>
+    <a href="https://www.codacy.com/gh/aestream/aestream/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=aestream/aestream&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7"/></a>
     <a href="https://doi.org/10.5281/zenodo.6322829"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.6322829.svg" alt="DOI"></a>
 </p>
 
-AEStream efficiently reads sparse events from an input source and streams it to an output sink.
-AEStream supports reading from files, USB cameras, as well as network via UDP and can stream events to files, network over UDP, and peripherals such as [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit)s and [neuromorphic hardware](https://en.wikipedia.org/wiki/Neuromorphic_engineering).
+AEStream effiently sends event-based data from A to B.
+AEStream can be used from the command-line, via Python, or as a C++ library.
+We support multiple inputs and outputs, providing seamless integration with files, [event cameras](https://en.wikipedia.org/wiki/Event_camera), network data, Python libraries via Numpy or PyTorch, and visualization tools.
 
-<img src="https://jegp.github.io/aestream-paper/2212_aestream.svg" />
+<img src="https://github.com/aestream/aestream/raw/main/docs/aestream_flow.png" />
 
-Read more in [the AEStream publication](https://jegp.github.io/aestream-paper/).
+Read more about the inner workings of the library in [the AEStream publication](https://jegp.github.io/aestream-paper/).
 
 ## Installation
 
-AEStream is usable both as a command-line binary or Python tool.
+> Read more in our [installation guide](https://aestream.github.io/aestream/install.html)
+
+The fastest way to install AEStream is by using pip: `pip install aestream`.
+See below for other sources.
 
-| **Source** | **Installation** |
-| -------------------- | --- |
-| [pip](https://pypi.org/) | <code>pip install aestream <br/> pip install aestream[torch]</code> ([PyTorch support](https://pytorch.com)) |
-| [nix](https://nixos.org/) | <code>nix run github:norse/aestream</code> (CLI) <br/> <code>nix develop github:norse/aestream</code> (Python environment) |
-| [docker](https://docker.com/) | See [Installation documentation](https://norse.github.io/aestream/install.html) |
+| **Source** | **Installation** | **Description** |
+| -------------------- | --- | --- |
+| [pip](https://pypi.org/) | <code>pip install aestream</code> <br/> <code>pip install aestream[torch]</code> <br/> <code>pip install aestream --no-binary</code> | <br/> [PyTorch support](https://pytorch.com) <br/> <a href="https://aestream.github.io/aestream/install.html#Event-camera-support">Requires camera drivers*</a> |
+| [nix](https://nixos.org/) | <code>nix run github:aestream/aestream</code> <br/> <code>nix develop github:aestream/aestream</code> | Command-line interface <br/> Python environment |
+| [docker](https://docker.com/) | See <a href="https://aestream.github.io/aestream/install.html">Installation documentation</a> |
+
+<span style="font-size: 80%">
+* Event camera support requires available drivers. <a href="https://aestream.github.io/aestream/install.html">A step-by-step guide is available in our documentation</a>.
+</span>
 
 Contributions to support AEStream on additional platforms are always welcome.
 
-## Usage: read event-address files in Python
+## Usage (Python)
+
+> Read more in our [Python usage guide](https://aestream.github.io/aestream/python_usage.html)
 
 AEStream can process fixed input sources like files like so:
 
 ```python
 FileInput("file", (640, 480)).load()
 ```
 
@@ -78,101 +89,77 @@
 # Stream events from UDP port 3333 (default)
 with UDPInput((640, 480), port=3333) as stream:
     while True:
         frame = stream.read() # Provides a (640, 480) tensor
         ...
 ```
 
-More examples can be found in [our example folder](https://github.com/norse/aestream/tree/master/example).
+More examples can be found in [our example folder](https://github.com/aestream/aestream/tree/master/example).
 Please note the examples may require additional dependencies (such as [Norse](https://github.com/norse/norse) for spiking networks or [PySDL](https://github.com/py-sdl/py-sdl2) for rendering). To install all the requirements, simply stand in the `aestream` root directory and run `pip install -r example/requirements.txt`
 
 ### Example: real-time edge detection with spiking neural networks
 
-![](example/usb_edgedetection.gif)
+![](https://media.githubusercontent.com/media/aestream/aestream/main/example/usb_edgedetection.gif)
 
 We stream events from a camera connected via USB and process them on a GPU in real-time using the [spiking neural network library, Norse](https://github.com/norse/norse) using fewer than 50 lines of Python.
 The left panel in the video shows the raw signal, while the middle and right panels show horizontal and vertical edge detection respectively.
-The full example can be found in [`example/usb_edgedetection.py`](https://github.com/norse/aestream/blob/main/example/usb_edgedetection.py)
+The full example can be found in [`example/usb_edgedetection.py`](https://github.com/aestream/aestream/blob/main/example/usb_edgedetection.py)
 
 ## Usage (CLI)
+> Read more in our [CLI usage documentation page](https://aestream.github.io/aestream/install.html)
 
 Installing AEStream also gives access to the command-line interface (CLI) `aestream`.
 To use `aestraem`, simply provide an `input` source and an optional `output` sink (defaulting to STDOUT):
 
 ```bash
 aestream input <input source> [output <output sink>]
 ```
 ## Supported Inputs and Outputs
 
-| Input | Description | Usage |
+| Input | Description | Example usage |
 | --------- | :----------- | ----- |
 | DAVIS, DVXPlorer | [Inivation](https://inivation.com/) DVS Camera over USB | `input inivation` |
 | EVK Cameras      | [Prophesee](https://www.prophesee.ai/) DVS camera over USB  | `input prophesee` |
-| File             | [AEDAT file format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md) as `.aedat`, `.aedat4`, or `.dat` | `input file x.aedat4` |
+| File             | Reads `.aedat`, `.aedat4`, `.csv`, `.dat`, or `.raw` files | `input file x.aedat4` |
+| [SynSense Speck](https://www.synsense.ai/products/speck-2/) | Stream events via ZMQ | `input speck` |
+| UDP network | Receives stream of events via the [SPIF protocol](https://github.com/SpiNNakerManchester/spif/tree/master/spiffer) | `input udp`
 
-| Output | Description | Usage |
+| Output | Description | Example usage |
 | --------- | ----------- | ----- |
 | STDOUT    | Standard output (default output) | `output stdout`
 | Ethernet over UDP | Outputs to a given IP and port using the [SPIF protocol](https://github.com/SpiNNakerManchester/spif)  | `output udp 10.0.0.1 1234` |
-| `.aedat4` file  | Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` |
-| CSV file       | Output to comma-separated-value (CSV) file format | `output file my_file.txt` |
+| File: `.aedat4`  | Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` |
+| File: `.csv`       | Output to comma-separated-value (CSV) file format | `output file my_file.csv` |
+| Viewer | View live event stream | `output view`
 
-### CLI examples
+## CLI examples
 
 | Example | Syntax |
 | ------------- | ------------------------------|
-| Echo file to STDOUT | `aestream input file example/sample.aedat4` |
-| Stream DVS cameara from iniVation AG to STDOUT (Note, requires Inivation libraries) | `aestream input inivation output stdout` |
-| Stream DVS camera from Prophesee to STDOUT (Note, requires Metavision SDK) | `aestream input output stdout` |
-| Read file to remote IP X.X.X.X | `aestream input file example/sample.aedat4 output udp X.X.X.X` |
-
-## Custom installation (C++)
-
-[Metavision SDK](https://docs.prophesee.ai/stable/metavision_sdk/index.html) and [libcaer](https://github.com/inivation/libcaer) are optional dependencies, but are needed for connecting to Prophesee and Inivation cameras respectively.
-
-AEStream is based on [C++20](https://en.cppreference.com/w/cpp/20). Since C++20 is not yet fully supported by all compilers, we recommend using `GCC >= 10.2`. 
-
-To build the binaries of this repository, run the following code:
-```
-# Optional: Ensure paths to libcaer or Metavision are in place
-mkdir build/
-cd build/
-cmake -GNinja ..
-ninja
-```
-
-If your default C++ compiler doesn't support C++ 20, you will have to install an up-to-date compiler and provide the environmental variable `CXX`.
-For instance like this: `CXX=/path/to/g++-10 cmake -GNinja ..`
-
-### Inivation cameras
-For [Inivation](https://inivation.com/) cameras, the [libcaer](https://gitlab.com/inivation/dv/libcaer/) library needs to be available, either by a `-DCMAKE_PREFIX_PATH` flag to `cmake` or included in the `PATH` environmental variable.
-For examble: `cmake -GNinja -DCMAKE_PREFIX_PATH=/path/to/libcaer`.
-Inivation made the library available for most operating systems, but you may have to build it yourself.
-
-### Prophesee cameras
-For [Prophesee](https://www.prophesee.ai/) cameras, a version of the [Metavision SDK](https://www.prophesee.ai/metavision-intelligence/) needs to be present.
-The open-source version the SDK `openeb` is available with installation instructions at https://github.com/prophesee-ai/openeb.
-Using `openeb`, it should be sufficient to install it using `cmake && make && make install` to put it in your path.
-Otherwise, you can point to it using the `-DCMAKE_PREFIX_PATH` option in `cmake`.
+| View live stream of Inivation camera (requires Inivation drivers) | `aestream input inivation output view` |
+| Stream Prophesee camera over the network to 10.0.0.1 (requires Metavision SDK) | `aestream input output udp 10.0.0.1` |
+| Convert `.dat` file to `.aedat4` | `aestream input example/sample.dat output file converted.aedat4` |
 
 ## Acknowledgments
 
 AEStream is developed by (in alphabetical order):
 
 * Cameron Barker (@GitHub [cameron-git](https://github.com/cameron-git/))
+* [Juan Pablo Romero Bermudez](https://www.kth.se/profile/jprb) (@GitHub [jpromerob](https://github.com/jpromerob/))
 * Alexander Hadjivanov (@Github [cantordust](https://github.com/cantordust))
+* Emil Jansson (@GitHub [emijan-kth](https://github.com/emijan-kth))
 * [Jens E. Pedersen](https://www.kth.se/profile/jeped) (@GitHub [jegp](https://github.com/jegp/))
 * [Christian Pehle](https://www.kip.uni-heidelberg.de/people/10110) (@GitHub [cpehle](https://github.com/cpehle/))
 
 The work has received funding from the EC Horizon 2020 Framework Programme under Grant Agreements 785907 and 945539 (HBP) and by the Deutsche Forschungsgemeinschaft (DFG, German Research Fundation) under Germany's Excellence Strategy EXC 2181/1 - 390900948 (the Heidelberg STRUCTURES Excellence Cluster).
 
 Thanks to [Philipp Mondorf](https://github.com/PMMon) for interfacing with Metavision SDK and preliminary network code.
 
-<a href="https://github.com/norse/aestream/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=norse/aestream" />
+<a href="https://github.com/aestream/aestream/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=aestream/aestream" />
 </a>
 
 
 ## Citation
 
 Please cite `aestream` if you use it in your work:
```

#### html2text {}

```diff
@@ -1,117 +1,107 @@
-Metadata-Version: 2.1 Name: aestream Version: 0.5.1 Summary: Streaming library
+Metadata-Version: 2.1 Name: aestream Version: 0.6.0 Summary: Streaming library
 for Address-Event Representation (AER) data Home-page: https://github.com/
-norse/aestream Author: Jens E. Pedersen, Christian Pehle Author-email:
-jens@jepedersen.dk, christian.pehle@gmail.com License: MIT Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C++ Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: System :: Hardware :: Universal
-Serial Bus (USB) Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: torch License-File: LICENSE License-File: AUTHORS # AEStream -
-Address Event streaming library
+aestream/aestream Author: Jens E. Pedersen Author-email: jens@jepedersen.dk
+License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: C++
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+System :: Hardware :: Universal Serial Bus (USB) Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: torch License-File:
+LICENSE License-File: AUTHORS [https://github.com/aestream/aestream/raw/main/
+logo.png]
 [Test_status] [https://img.shields.io/pypi/v/aestream] [https://img.shields.io/
- github/last-commit/norse/aestream] [chat_on_Discord] [https://app.codacy.com/
-          project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7] [DOI]
-AEStream efficiently reads sparse events from an input source and streams it to
-an output sink. AEStream supports reading from files, USB cameras, as well as
-network via UDP and can stream events to files, network over UDP, and
-peripherals such as [GPU](https://en.wikipedia.org/wiki/
-Graphics_processing_unit)s and [neuromorphic hardware](https://
-en.wikipedia.org/wiki/Neuromorphic_engineering). [https://jegp.github.io/
-aestream-paper/2212_aestream.svg] Read more in [the AEStream publication]
-(https://jegp.github.io/aestream-paper/). ## Installation AEStream is usable
-both as a command-line binary or Python tool. | **Source** | **Installation** |
-| -------------------- | --- | | [pip](https://pypi.org/) | pip install
-aestream
-pip install aestream[torch] ([PyTorch support](https://pytorch.com)) | | [nix]
-(https://nixos.org/) | nix run github:norse/aestream (CLI)
-nix develop github:norse/aestream (Python environment) | | [docker](https://
-docker.com/) | See [Installation documentation](https://norse.github.io/
-aestream/install.html) | Contributions to support AEStream on additional
-platforms are always welcome. ## Usage: read event-address files in Python
-AEStream can process fixed input sources like files like so: ```python
-FileInput("file", (640, 480)).load() ``` ## Usage: stream real-time data in
-Python AEStream also supports streaming data in real-time *without strict
-guarantees on orders*. This is particularly useful in real-time scenarios, for
-instance when operating with `USBInput` or `UDPInput` ```python # Stream events
-from a DVS camera over USB with USBInput((640, 480)) as stream: while True:
-frame = stream.read() # Provides a (640, 480) tensor ... ``` ```python # Stream
-events from UDP port 3333 (default) with UDPInput((640, 480), port=3333) as
-stream: while True: frame = stream.read() # Provides a (640, 480) tensor ...
-``` More examples can be found in [our example folder](https://github.com/
-norse/aestream/tree/master/example). Please note the examples may require
-additional dependencies (such as [Norse](https://github.com/norse/norse) for
-spiking networks or [PySDL](https://github.com/py-sdl/py-sdl2) for rendering).
-To install all the requirements, simply stand in the `aestream` root directory
-and run `pip install -r example/requirements.txt` ### Example: real-time edge
-detection with spiking neural networks ![](example/usb_edgedetection.gif) We
-stream events from a camera connected via USB and process them on a GPU in
-real-time using the [spiking neural network library, Norse](https://github.com/
-norse/norse) using fewer than 50 lines of Python. The left panel in the video
-shows the raw signal, while the middle and right panels show horizontal and
-vertical edge detection respectively. The full example can be found in
-[`example/usb_edgedetection.py`](https://github.com/norse/aestream/blob/main/
-example/usb_edgedetection.py) ## Usage (CLI) Installing AEStream also gives
-access to the command-line interface (CLI) `aestream`. To use `aestraem`,
-simply provide an `input` source and an optional `output` sink (defaulting to
-STDOUT): ```bash aestream input [                    ] [output ] ``` ##
-Supported Inputs and Outputs | Input | Description | Usage | | --------- | :---
--------- | ----- | | DAVIS, DVXPlorer | [Inivation](https://inivation.com/) DVS
-Camera over USB | `input inivation` | | EVK Cameras | [Prophesee](https://
-www.prophesee.ai/) DVS camera over USB | `input prophesee` | | File | [AEDAT
-file format](https://gitlab.com/inivation/inivation-docs/blob/master/
-Software%20user%20guides/AEDAT_file_formats.md) as `.aedat`, `.aedat4`, or
-`.dat` | `input file x.aedat4` | | Output | Description | Usage | | --------- |
------------ | ----- | | STDOUT | Standard output (default output) | `output
-stdout` | Ethernet over UDP | Outputs to a given IP and port using the [SPIF
-protocol](https://github.com/SpiNNakerManchester/spif) | `output udp 10.0.0.1
-1234` | | `.aedat4` file | Output to [`.aedat4` format](https://gitlab.com/
-inivation/inivation-docs/blob/master/Software%20user%20guides/
-AEDAT_file_formats.md#aedat-40) | `output file my_file.aedat4` | | CSV file |
-Output to comma-separated-value (CSV) file format | `output file my_file.txt` |
-### CLI examples | Example | Syntax | | ------------- | -----------------------
--------| | Echo file to STDOUT | `aestream input file example/sample.aedat4` |
-| Stream DVS cameara from iniVation AG to STDOUT (Note, requires Inivation
-libraries) | `aestream input inivation output stdout` | | Stream DVS camera
-from Prophesee to STDOUT (Note, requires Metavision SDK) | `aestream input
-output stdout` | | Read file to remote IP X.X.X.X | `aestream input file
-example/sample.aedat4 output udp X.X.X.X` | ## Custom installation (C++)
-[Metavision SDK](https://docs.prophesee.ai/stable/metavision_sdk/index.html)
-and [libcaer](https://github.com/inivation/libcaer) are optional dependencies,
-but are needed for connecting to Prophesee and Inivation cameras respectively.
-AEStream is based on [C++20](https://en.cppreference.com/w/cpp/20). Since C++20
-is not yet fully supported by all compilers, we recommend using `GCC >= 10.2`.
-To build the binaries of this repository, run the following code: ``` #
-Optional: Ensure paths to libcaer or Metavision are in place mkdir build/ cd
-build/ cmake -GNinja .. ninja ``` If your default C++ compiler doesn't support
-C++ 20, you will have to install an up-to-date compiler and provide the
-environmental variable `CXX`. For instance like this: `CXX=/path/to/g++-10
-cmake -GNinja ..` ### Inivation cameras For [Inivation](https://inivation.com/
-) cameras, the [libcaer](https://gitlab.com/inivation/dv/libcaer/) library
-needs to be available, either by a `-DCMAKE_PREFIX_PATH` flag to `cmake` or
-included in the `PATH` environmental variable. For examble: `cmake -GNinja -
-DCMAKE_PREFIX_PATH=/path/to/libcaer`. Inivation made the library available for
-most operating systems, but you may have to build it yourself. ### Prophesee
-cameras For [Prophesee](https://www.prophesee.ai/) cameras, a version of the
-[Metavision SDK](https://www.prophesee.ai/metavision-intelligence/) needs to be
-present. The open-source version the SDK `openeb` is available with
-installation instructions at https://github.com/prophesee-ai/openeb. Using
-`openeb`, it should be sufficient to install it using `cmake && make && make
-install` to put it in your path. Otherwise, you can point to it using the `-
-DCMAKE_PREFIX_PATH` option in `cmake`. ## Acknowledgments AEStream is developed
-by (in alphabetical order): * Cameron Barker (@GitHub [cameron-git](https://
-github.com/cameron-git/)) * Alexander Hadjivanov (@Github [cantordust](https://
-github.com/cantordust)) * [Jens E. Pedersen](https://www.kth.se/profile/jeped)
+       github/last-commit/aestream/aestream] [chat_on_Discord] [https://
+  app.codacy.com/project/badge/Grade/0a04a852daf540a9b9bbe9d78df9eea7] [DOI]
+AEStream effiently sends event-based data from A to B. AEStream can be used
+from the command-line, via Python, or as a C++ library. We support multiple
+inputs and outputs, providing seamless integration with files, [event cameras]
+(https://en.wikipedia.org/wiki/Event_camera), network data, Python libraries
+via Numpy or PyTorch, and visualization tools. [https://github.com/aestream/
+aestream/raw/main/docs/aestream_flow.png] Read more about the inner workings of
+the library in [the AEStream publication](https://jegp.github.io/aestream-
+paper/). ## Installation > Read more in our [installation guide](https://
+aestream.github.io/aestream/install.html) The fastest way to install AEStream
+is by using pip: `pip install aestream`. See below for other sources. |
+**Source** | **Installation** | **Description** | | -------------------- | --
+- | --- | | [pip](https://pypi.org/) | pip install aestream
+pip install aestream[torch]
+pip install aestream --no-binary |
+[PyTorch support](https://pytorch.com)
+Requires_camera_drivers* | | [nix](https://nixos.org/) | nix run github:
+aestream/aestream
+nix develop github:aestream/aestream | Command-line interface
+Python environment | | [docker](https://docker.com/) | See Installation
+documentation |  * Event camera support requires available drivers. A_step-by-
+step_guide_is_available_in_our_documentation.  Contributions to support
+AEStream on additional platforms are always welcome. ## Usage (Python) > Read
+more in our [Python usage guide](https://aestream.github.io/aestream/
+python_usage.html) AEStream can process fixed input sources like files like so:
+```python FileInput("file", (640, 480)).load() ``` ## Usage: stream real-time
+data in Python AEStream also supports streaming data in real-time *without
+strict guarantees on orders*. This is particularly useful in real-time
+scenarios, for instance when operating with `USBInput` or `UDPInput` ```python
+# Stream events from a DVS camera over USB with USBInput((640, 480)) as stream:
+while True: frame = stream.read() # Provides a (640, 480) tensor ... ```
+```python # Stream events from UDP port 3333 (default) with UDPInput((640,
+480), port=3333) as stream: while True: frame = stream.read() # Provides a
+(640, 480) tensor ... ``` More examples can be found in [our example folder]
+(https://github.com/aestream/aestream/tree/master/example). Please note the
+examples may require additional dependencies (such as [Norse](https://
+github.com/norse/norse) for spiking networks or [PySDL](https://github.com/py-
+sdl/py-sdl2) for rendering). To install all the requirements, simply stand in
+the `aestream` root directory and run `pip install -r example/requirements.txt`
+### Example: real-time edge detection with spiking neural networks ![](https://
+media.githubusercontent.com/media/aestream/aestream/main/example/
+usb_edgedetection.gif) We stream events from a camera connected via USB and
+process them on a GPU in real-time using the [spiking neural network library,
+Norse](https://github.com/norse/norse) using fewer than 50 lines of Python. The
+left panel in the video shows the raw signal, while the middle and right panels
+show horizontal and vertical edge detection respectively. The full example can
+be found in [`example/usb_edgedetection.py`](https://github.com/aestream/
+aestream/blob/main/example/usb_edgedetection.py) ## Usage (CLI) > Read more in
+our [CLI usage documentation page](https://aestream.github.io/aestream/
+install.html) Installing AEStream also gives access to the command-line
+interface (CLI) `aestream`. To use `aestraem`, simply provide an `input` source
+and an optional `output` sink (defaulting to STDOUT): ```bash aestream input
+[                    ] [output ] ``` ## Supported Inputs and Outputs | Input |
+Description | Example usage | | --------- | :----------- | ----- | | DAVIS,
+DVXPlorer | [Inivation](https://inivation.com/) DVS Camera over USB | `input
+inivation` | | EVK Cameras | [Prophesee](https://www.prophesee.ai/) DVS camera
+over USB | `input prophesee` | | File | Reads `.aedat`, `.aedat4`, `.csv`,
+`.dat`, or `.raw` files | `input file x.aedat4` | | [SynSense Speck](https://
+www.synsense.ai/products/speck-2/) | Stream events via ZMQ | `input speck` | |
+UDP network | Receives stream of events via the [SPIF protocol](https://
+github.com/SpiNNakerManchester/spif/tree/master/spiffer) | `input udp` | Output
+| Description | Example usage | | --------- | ----------- | ----- | | STDOUT |
+Standard output (default output) | `output stdout` | Ethernet over UDP |
+Outputs to a given IP and port using the [SPIF protocol](https://github.com/
+SpiNNakerManchester/spif) | `output udp 10.0.0.1 1234` | | File: `.aedat4` |
+Output to [`.aedat4` format](https://gitlab.com/inivation/inivation-docs/blob/
+master/Software%20user%20guides/AEDAT_file_formats.md#aedat-40) | `output file
+my_file.aedat4` | | File: `.csv` | Output to comma-separated-value (CSV) file
+format | `output file my_file.csv` | | Viewer | View live event stream |
+`output view` ## CLI examples | Example | Syntax | | ------------- | ----------
+--------------------| | View live stream of Inivation camera (requires
+Inivation drivers) | `aestream input inivation output view` | | Stream
+Prophesee camera over the network to 10.0.0.1 (requires Metavision SDK) |
+`aestream input output udp 10.0.0.1` | | Convert `.dat` file to `.aedat4` |
+`aestream input example/sample.dat output file converted.aedat4` | ##
+Acknowledgments AEStream is developed by (in alphabetical order): * Cameron
+Barker (@GitHub [cameron-git](https://github.com/cameron-git/)) * [Juan Pablo
+Romero Bermudez](https://www.kth.se/profile/jprb) (@GitHub [jpromerob](https://
+github.com/jpromerob/)) * Alexander Hadjivanov (@Github [cantordust](https://
+github.com/cantordust)) * Emil Jansson (@GitHub [emijan-kth](https://
+github.com/emijan-kth)) * [Jens E. Pedersen](https://www.kth.se/profile/jeped)
 (@GitHub [jegp](https://github.com/jegp/)) * [Christian Pehle](https://
 www.kip.uni-heidelberg.de/people/10110) (@GitHub [cpehle](https://github.com/
 cpehle/)) The work has received funding from the EC Horizon 2020 Framework
 Programme under Grant Agreements 785907 and 945539 (HBP) and by the Deutsche
 Forschungsgemeinschaft (DFG, German Research Fundation) under Germany's
 Excellence Strategy EXC 2181/1 - 390900948 (the Heidelberg STRUCTURES
 Excellence Cluster). Thanks to [Philipp Mondorf](https://github.com/PMMon) for
 interfacing with Metavision SDK and preliminary network code. [https://
-contrib.rocks/image?repo=norse/aestream] ## Citation Please cite `aestream` if
-you use it in your work: ```bibtex @misc{aestream, doi = {10.48550/
+contrib.rocks/image?repo=aestream/aestream] ## Citation Please cite `aestream`
+if you use it in your work: ```bibtex @misc{aestream, doi = {10.48550/
 ARXIV.2212.10719}, url = {https://arxiv.org/abs/2212.10719}, author =
 {Pedersen, Jens Egholm and Conradt, JÃ¶rg}, title = {AEStream: Accelerated
 event-based processing with coroutines}, publisher = {arXiv}, year = {2022}, }
 ```
```

### Comparing `aestream-0.5.1/aestream.egg-info/SOURCES.txt` & `aestream-0.6.0/aestream.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 aestream/__init__.py
 aestream/__init__.pyi
+aestream/_genn.py
 aestream/_input.py
 aestream/py.typed
 aestream.egg-info/PKG-INFO
 aestream.egg-info/SOURCES.txt
 aestream.egg-info/dependency_links.txt
 aestream.egg-info/requires.txt
 aestream.egg-info/top_level.txt
@@ -18,34 +19,36 @@
 include/CPM.cmake
 include/rapidxml.hpp
 src/CMakeLists.txt
 src/aer.hpp
 src/aestream.cpp
 src/dvs_gesture.hpp
 src/generator.hpp
-src/viewer.cpp
-src/.ipynb_checkpoints/Untitled-checkpoint.ipynb
 src/file/CMakeLists.txt
 src/file/aedat.hpp
 src/file/aedat4.hpp
+src/file/csv.hpp
 src/file/dat.hpp
+src/file/evt3.hpp
 src/file/utils.hpp
 src/file/flatbuffers/events.fbs
 src/file/flatbuffers/file_data_table.fbs
 src/file/flatbuffers/frame.fbs
 src/file/flatbuffers/imus.fbs
 src/file/flatbuffers/ioheader.fbs
 src/file/flatbuffers/trigger.fbs
 src/input/CMakeLists.txt
 src/input/file.cpp
 src/input/file.hpp
 src/input/inivation.cpp
 src/input/inivation.hpp
 src/input/prophesee.cpp
 src/input/prophesee.hpp
+src/input/zmq.cpp
+src/input/zmq.hpp
 src/output/CMakeLists.txt
 src/output/dvs_to_file.cpp
 src/output/dvs_to_file.hpp
 src/output/dvs_to_tensor.cpp
 src/output/dvs_to_tensor.hpp
 src/output/dvs_to_udp.cpp
 src/output/dvs_to_udp.hpp
@@ -63,12 +66,13 @@
 src/pybind/tensor_iterator.cpp
 src/pybind/tensor_iterator.hpp
 src/pybind/types.hpp
 src/pybind/udp.cpp
 src/pybind/udp_client.cpp
 src/pybind/udp_client.hpp
 src/pybind/usb.cpp
+src/pybind/zmq.cpp
 src/pybind/test/__init__.py
 src/pybind/test/test_file.py
 src/pybind/test/test_udp.py
-src/pybind/test/__pycache__/__init__.cpython-310.pyc
-src/pybind/test/__pycache__/test_file.cpython-310-pytest-7.2.2.pyc
+src/viewer/viewer.cpp
+src/viewer/viewer.hpp
```

### Comparing `aestream-0.5.1/include/CLI11.hpp` & `aestream-0.6.0/include/CLI11.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-// CLI11: Version 2.0.0
+// CLI11: Version 2.3.2
 // Originally designed by Henry Schreiner
 // https://github.com/CLIUtils/CLI11
 //
 // This is a standalone header file generated by MakeSingleHeader.py in CLI11/scripts
-// from: v2.0.0 (added include gaurd)
+// from: v2.3.2
 //
-// CLI11 2.0.0 Copyright (c) 2017-2020 University of Cincinnati, developed by Henry
+// CLI11 2.3.2 Copyright (c) 2017-2022 University of Cincinnati, developed by Henry
 // Schreiner under NSF AWARD 1414736. All rights reserved.
 //
 // Redistribution and use in source and binary forms of CLI11, with or without
 // modification, are permitted provided that the following conditions are met:
 //
 // 1. Redistributions of source code must retain the above copyright notice, this
 //    list of conditions and the following disclaimer.
@@ -30,42 +30,42 @@
 // ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 // (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 // SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #pragma once
 
 // Standard combined includes:
+#include <iomanip>
+#include <set>
 #include <memory>
-#include <string>
-#include <functional>
 #include <vector>
-#include <exception>
-#include <sstream>
-#include <cstdint>
 #include <utility>
-#include <iomanip>
-#include <iterator>
-#include <algorithm>
-#include <tuple>
 #include <stdexcept>
+#include <locale>
+#include <functional>
 #include <iostream>
+#include <iterator>
+#include <exception>
+#include <numeric>
 #include <fstream>
-#include <locale>
+#include <string>
 #include <type_traits>
+#include <tuple>
 #include <map>
-#include <limits>
-#include <numeric>
+#include <algorithm>
+#include <cstdint>
+#include <sstream>
 #include <cmath>
-#include <set>
+#include <limits>
 
 
 #define CLI11_VERSION_MAJOR 2
-#define CLI11_VERSION_MINOR 0
-#define CLI11_VERSION_PATCH 0
-#define CLI11_VERSION "2.0.0"
+#define CLI11_VERSION_MINOR 3
+#define CLI11_VERSION_PATCH 2
+#define CLI11_VERSION "2.3.2"
 
 
 
 
 // The following version macro is very similar to the one in pybind11
 #if !(defined(_MSC_VER) && __cplusplus == 199711L) && !defined(__INTEL_COMPILER)
 #if __cplusplus >= 201402L
@@ -80,39 +80,73 @@
 #elif defined(_MSC_VER) && __cplusplus == 199711L
 // MSVC sets _MSVC_LANG rather than __cplusplus (supposedly until the standard is fully implemented)
 // Unless you use the /Zc:__cplusplus flag on Visual Studio 2017 15.7 Preview 3 or newer
 #if _MSVC_LANG >= 201402L
 #define CLI11_CPP14
 #if _MSVC_LANG > 201402L && _MSC_VER >= 1910
 #define CLI11_CPP17
-#if __MSVC_LANG > 201703L && _MSC_VER >= 1910
+#if _MSVC_LANG > 201703L && _MSC_VER >= 1910
 #define CLI11_CPP20
 #endif
 #endif
 #endif
 #endif
 
 #if defined(CLI11_CPP14)
 #define CLI11_DEPRECATED(reason) [[deprecated(reason)]]
 #elif defined(_MSC_VER)
 #define CLI11_DEPRECATED(reason) __declspec(deprecated(reason))
 #else
 #define CLI11_DEPRECATED(reason) __attribute__((deprecated(reason)))
 #endif
 
+// GCC < 10 doesn't ignore this in unevaluated contexts
+#if !defined(CLI11_CPP17) ||                                                                                           \
+    (defined(__GNUC__) && !defined(__llvm__) && !defined(__INTEL_COMPILER) && __GNUC__ < 10 && __GNUC__ > 4)
+#define CLI11_NODISCARD
+#else
+#define CLI11_NODISCARD [[nodiscard]]
+#endif
+
+/** detection of rtti */
+#ifndef CLI11_USE_STATIC_RTTI
+#if(defined(_HAS_STATIC_RTTI) && _HAS_STATIC_RTTI)
+#define CLI11_USE_STATIC_RTTI 1
+#elif defined(__cpp_rtti)
+#if(defined(_CPPRTTI) && _CPPRTTI == 0)
+#define CLI11_USE_STATIC_RTTI 1
+#else
+#define CLI11_USE_STATIC_RTTI 0
+#endif
+#elif(defined(__GCC_RTTI) && __GXX_RTTI)
+#define CLI11_USE_STATIC_RTTI 0
+#else
+#define CLI11_USE_STATIC_RTTI 1
+#endif
+#endif
+
+/** Inline macro **/
+#ifdef CLI11_COMPILE
+#define CLI11_INLINE
+#else
+#define CLI11_INLINE inline
+#endif
 
 
 
 // C standard library
 // Only needed for existence checking
 #if defined CLI11_CPP17 && defined __has_include && !defined CLI11_HAS_FILESYSTEM
 #if __has_include(<filesystem>)
 // Filesystem cannot be used if targeting macOS < 10.15
 #if defined __MAC_OS_X_VERSION_MIN_REQUIRED && __MAC_OS_X_VERSION_MIN_REQUIRED < 101500
 #define CLI11_HAS_FILESYSTEM 0
+#elif defined(__wasi__)
+// As of wasi-sdk-14, filesystem is not implemented
+#define CLI11_HAS_FILESYSTEM 0
 #else
 #include <filesystem>
 #if defined __cpp_lib_filesystem && __cpp_lib_filesystem >= 201703
 #if defined _GLIBCXX_RELEASE && _GLIBCXX_RELEASE >= 9
 #define CLI11_HAS_FILESYSTEM 1
 #elif defined(__GLIBCXX__)
 // if we are using gcc and Version <9 default to no filesystem
@@ -157,29 +191,15 @@
 
 namespace detail {
 /// a constant defining an expected max vector size defined to be a big number that could be multiplied by 4 and not
 /// produce overflow for some expected uses
 constexpr int expected_max_vector_size{1 << 29};
 // Based on http://stackoverflow.com/questions/236129/split-a-string-in-c
 /// Split a string by a delim
-inline std::vector<std::string> split(const std::string &s, char delim) {
-    std::vector<std::string> elems;
-    // Check to see if empty string, give consistent result
-    if(s.empty()) {
-        elems.emplace_back();
-    } else {
-        std::stringstream ss;
-        ss.str(s);
-        std::string item;
-        while(std::getline(ss, item, delim)) {
-            elems.push_back(item);
-        }
-    }
-    return elems;
-}
+CLI11_INLINE std::vector<std::string> split(const std::string &s, char delim);
 
 /// Simple function to join a string
 template <typename T> std::string join(const T &v, std::string delim = ",") {
     std::ostringstream s;
     auto beg = std::begin(v);
     auto end = std::end(v);
     if(beg != end)
@@ -220,72 +240,214 @@
     }
     return s.str();
 }
 
 // Based roughly on http://stackoverflow.com/questions/25829143/c-trim-whitespace-from-a-string
 
 /// Trim whitespace from left of string
-inline std::string &ltrim(std::string &str) {
+CLI11_INLINE std::string &ltrim(std::string &str);
+
+/// Trim anything from left of string
+CLI11_INLINE std::string &ltrim(std::string &str, const std::string &filter);
+
+/// Trim whitespace from right of string
+CLI11_INLINE std::string &rtrim(std::string &str);
+
+/// Trim anything from right of string
+CLI11_INLINE std::string &rtrim(std::string &str, const std::string &filter);
+
+/// Trim whitespace from string
+inline std::string &trim(std::string &str) { return ltrim(rtrim(str)); }
+
+/// Trim anything from string
+inline std::string &trim(std::string &str, const std::string filter) { return ltrim(rtrim(str, filter), filter); }
+
+/// Make a copy of the string and then trim it
+inline std::string trim_copy(const std::string &str) {
+    std::string s = str;
+    return trim(s);
+}
+
+/// remove quotes at the front and back of a string either '"' or '\''
+CLI11_INLINE std::string &remove_quotes(std::string &str);
+
+/// Add a leader to the beginning of all new lines (nothing is added
+/// at the start of the first line). `"; "` would be for ini files
+///
+/// Can't use Regex, or this would be a subs.
+CLI11_INLINE std::string fix_newlines(const std::string &leader, std::string input);
+
+/// Make a copy of the string and then trim it, any filter string can be used (any char in string is filtered)
+inline std::string trim_copy(const std::string &str, const std::string &filter) {
+    std::string s = str;
+    return trim(s, filter);
+}
+/// Print a two part "help" string
+CLI11_INLINE std::ostream &
+format_help(std::ostream &out, std::string name, const std::string &description, std::size_t wid);
+
+/// Print subcommand aliases
+CLI11_INLINE std::ostream &format_aliases(std::ostream &out, const std::vector<std::string> &aliases, std::size_t wid);
+
+/// Verify the first character of an option
+/// - is a trigger character, ! has special meaning and new lines would just be annoying to deal with
+template <typename T> bool valid_first_char(T c) { return ((c != '-') && (c != '!') && (c != ' ') && c != '\n'); }
+
+/// Verify following characters of an option
+template <typename T> bool valid_later_char(T c) {
+    // = and : are value separators, { has special meaning for option defaults,
+    // and \n would just be annoying to deal with in many places allowing space here has too much potential for
+    // inadvertent entry errors and bugs
+    return ((c != '=') && (c != ':') && (c != '{') && (c != ' ') && c != '\n');
+}
+
+/// Verify an option/subcommand name
+CLI11_INLINE bool valid_name_string(const std::string &str);
+
+/// Verify an app name
+inline bool valid_alias_name_string(const std::string &str) {
+    static const std::string badChars(std::string("\n") + '\0');
+    return (str.find_first_of(badChars) == std::string::npos);
+}
+
+/// check if a string is a container segment separator (empty or "%%")
+inline bool is_separator(const std::string &str) {
+    static const std::string sep("%%");
+    return (str.empty() || str == sep);
+}
+
+/// Verify that str consists of letters only
+inline bool isalpha(const std::string &str) {
+    return std::all_of(str.begin(), str.end(), [](char c) { return std::isalpha(c, std::locale()); });
+}
+
+/// Return a lower case version of a string
+inline std::string to_lower(std::string str) {
+    std::transform(std::begin(str), std::end(str), std::begin(str), [](const std::string::value_type &x) {
+        return std::tolower(x, std::locale());
+    });
+    return str;
+}
+
+/// remove underscores from a string
+inline std::string remove_underscore(std::string str) {
+    str.erase(std::remove(std::begin(str), std::end(str), '_'), std::end(str));
+    return str;
+}
+
+/// Find and replace a substring with another substring
+CLI11_INLINE std::string find_and_replace(std::string str, std::string from, std::string to);
+
+/// check if the flag definitions has possible false flags
+inline bool has_default_flag_values(const std::string &flags) {
+    return (flags.find_first_of("{!") != std::string::npos);
+}
+
+CLI11_INLINE void remove_default_flag_values(std::string &flags);
+
+/// Check if a string is a member of a list of strings and optionally ignore case or ignore underscores
+CLI11_INLINE std::ptrdiff_t find_member(std::string name,
+                                        const std::vector<std::string> names,
+                                        bool ignore_case = false,
+                                        bool ignore_underscore = false);
+
+/// Find a trigger string and call a modify callable function that takes the current string and starting position of the
+/// trigger and returns the position in the string to search for the next trigger string
+template <typename Callable> inline std::string find_and_modify(std::string str, std::string trigger, Callable modify) {
+    std::size_t start_pos = 0;
+    while((start_pos = str.find(trigger, start_pos)) != std::string::npos) {
+        start_pos = modify(str, start_pos);
+    }
+    return str;
+}
+
+/// Split a string '"one two" "three"' into 'one two', 'three'
+/// Quote characters can be ` ' or "
+CLI11_INLINE std::vector<std::string> split_up(std::string str, char delimiter = '\0');
+
+/// This function detects an equal or colon followed by an escaped quote after an argument
+/// then modifies the string to replace the equality with a space.  This is needed
+/// to allow the split up function to work properly and is intended to be used with the find_and_modify function
+/// the return value is the offset+1 which is required by the find_and_modify function.
+CLI11_INLINE std::size_t escape_detect(std::string &str, std::size_t offset);
+
+/// Add quotes if the string contains spaces
+CLI11_INLINE std::string &add_quotes_if_needed(std::string &str);
+
+}  // namespace detail
+
+
+
+
+namespace detail {
+CLI11_INLINE std::vector<std::string> split(const std::string &s, char delim) {
+    std::vector<std::string> elems;
+    // Check to see if empty string, give consistent result
+    if(s.empty()) {
+        elems.emplace_back();
+    } else {
+        std::stringstream ss;
+        ss.str(s);
+        std::string item;
+        while(std::getline(ss, item, delim)) {
+            elems.push_back(item);
+        }
+    }
+    return elems;
+}
+
+CLI11_INLINE std::string &ltrim(std::string &str) {
     auto it = std::find_if(str.begin(), str.end(), [](char ch) { return !std::isspace<char>(ch, std::locale()); });
     str.erase(str.begin(), it);
     return str;
 }
 
-/// Trim anything from left of string
-inline std::string &ltrim(std::string &str, const std::string &filter) {
+CLI11_INLINE std::string &ltrim(std::string &str, const std::string &filter) {
     auto it = std::find_if(str.begin(), str.end(), [&filter](char ch) { return filter.find(ch) == std::string::npos; });
     str.erase(str.begin(), it);
     return str;
 }
 
-/// Trim whitespace from right of string
-inline std::string &rtrim(std::string &str) {
+CLI11_INLINE std::string &rtrim(std::string &str) {
     auto it = std::find_if(str.rbegin(), str.rend(), [](char ch) { return !std::isspace<char>(ch, std::locale()); });
     str.erase(it.base(), str.end());
     return str;
 }
 
-/// Trim anything from right of string
-inline std::string &rtrim(std::string &str, const std::string &filter) {
+CLI11_INLINE std::string &rtrim(std::string &str, const std::string &filter) {
     auto it =
         std::find_if(str.rbegin(), str.rend(), [&filter](char ch) { return filter.find(ch) == std::string::npos; });
     str.erase(it.base(), str.end());
     return str;
 }
 
-/// Trim whitespace from string
-inline std::string &trim(std::string &str) { return ltrim(rtrim(str)); }
-
-/// Trim anything from string
-inline std::string &trim(std::string &str, const std::string filter) { return ltrim(rtrim(str, filter), filter); }
-
-/// Make a copy of the string and then trim it
-inline std::string trim_copy(const std::string &str) {
-    std::string s = str;
-    return trim(s);
-}
-
-/// remove quotes at the front and back of a string either '"' or '\''
-inline std::string &remove_quotes(std::string &str) {
+CLI11_INLINE std::string &remove_quotes(std::string &str) {
     if(str.length() > 1 && (str.front() == '"' || str.front() == '\'')) {
         if(str.front() == str.back()) {
             str.pop_back();
             str.erase(str.begin(), str.begin() + 1);
         }
     }
     return str;
 }
 
-/// Make a copy of the string and then trim it, any filter string can be used (any char in string is filtered)
-inline std::string trim_copy(const std::string &str, const std::string &filter) {
-    std::string s = str;
-    return trim(s, filter);
+CLI11_INLINE std::string fix_newlines(const std::string &leader, std::string input) {
+    std::string::size_type n = 0;
+    while(n != std::string::npos && n < input.size()) {
+        n = input.find('\n', n);
+        if(n != std::string::npos) {
+            input = input.substr(0, n + 1) + leader + input.substr(n + 1);
+            n += leader.size();
+        }
+    }
+    return input;
 }
-/// Print a two part "help" string
-inline std::ostream &format_help(std::ostream &out, std::string name, const std::string &description, std::size_t wid) {
+
+CLI11_INLINE std::ostream &
+format_help(std::ostream &out, std::string name, const std::string &description, std::size_t wid) {
     name = "  " + name;
     out << std::setw(static_cast<int>(wid)) << std::left << name;
     if(!description.empty()) {
         if(name.length() >= wid)
             out << "\n" << std::setw(static_cast<int>(wid)) << "";
         for(const char c : description) {
             out.put(c);
@@ -294,111 +456,69 @@
             }
         }
     }
     out << "\n";
     return out;
 }
 
-/// Print subcommand aliases
-inline std::ostream &format_aliases(std::ostream &out, const std::vector<std::string> &aliases, std::size_t wid) {
+CLI11_INLINE std::ostream &format_aliases(std::ostream &out, const std::vector<std::string> &aliases, std::size_t wid) {
     if(!aliases.empty()) {
         out << std::setw(static_cast<int>(wid)) << "     aliases: ";
         bool front = true;
         for(const auto &alias : aliases) {
             if(!front) {
                 out << ", ";
             } else {
                 front = false;
             }
-            out << alias;
+            out << detail::fix_newlines("              ", alias);
         }
         out << "\n";
     }
     return out;
 }
 
-/// Verify the first character of an option
-template <typename T> bool valid_first_char(T c) {
-    return std::isalnum(c, std::locale()) || c == '_' || c == '?' || c == '@';
-}
-
-/// Verify following characters of an option
-template <typename T> bool valid_later_char(T c) { return valid_first_char(c) || c == '.' || c == '-'; }
-
-/// Verify an option name
-inline bool valid_name_string(const std::string &str) {
-    if(str.empty() || !valid_first_char(str[0]))
+CLI11_INLINE bool valid_name_string(const std::string &str) {
+    if(str.empty() || !valid_first_char(str[0])) {
         return false;
-    for(auto c : str.substr(1))
-        if(!valid_later_char(c))
+    }
+    auto e = str.end();
+    for(auto c = str.begin() + 1; c != e; ++c)
+        if(!valid_later_char(*c))
             return false;
     return true;
 }
 
-/// check if a string is a container segment separator (empty or "%%")
-inline bool is_separator(const std::string &str) {
-    static const std::string sep("%%");
-    return (str.empty() || str == sep);
-}
-
-/// Verify that str consists of letters only
-inline bool isalpha(const std::string &str) {
-    return std::all_of(str.begin(), str.end(), [](char c) { return std::isalpha(c, std::locale()); });
-}
-
-/// Return a lower case version of a string
-inline std::string to_lower(std::string str) {
-    std::transform(std::begin(str), std::end(str), std::begin(str), [](const std::string::value_type &x) {
-        return std::tolower(x, std::locale());
-    });
-    return str;
-}
-
-/// remove underscores from a string
-inline std::string remove_underscore(std::string str) {
-    str.erase(std::remove(std::begin(str), std::end(str), '_'), std::end(str));
-    return str;
-}
-
-/// Find and replace a substring with another substring
-inline std::string find_and_replace(std::string str, std::string from, std::string to) {
+CLI11_INLINE std::string find_and_replace(std::string str, std::string from, std::string to) {
 
     std::size_t start_pos = 0;
 
     while((start_pos = str.find(from, start_pos)) != std::string::npos) {
         str.replace(start_pos, from.length(), to);
         start_pos += to.length();
     }
 
     return str;
 }
 
-/// check if the flag definitions has possible false flags
-inline bool has_default_flag_values(const std::string &flags) {
-    return (flags.find_first_of("{!") != std::string::npos);
-}
-
-inline void remove_default_flag_values(std::string &flags) {
-    auto loc = flags.find_first_of('{');
+CLI11_INLINE void remove_default_flag_values(std::string &flags) {
+    auto loc = flags.find_first_of('{', 2);
     while(loc != std::string::npos) {
         auto finish = flags.find_first_of("},", loc + 1);
         if((finish != std::string::npos) && (flags[finish] == '}')) {
             flags.erase(flags.begin() + static_cast<std::ptrdiff_t>(loc),
                         flags.begin() + static_cast<std::ptrdiff_t>(finish) + 1);
         }
         loc = flags.find_first_of('{', loc + 1);
     }
     flags.erase(std::remove(flags.begin(), flags.end(), '!'), flags.end());
 }
 
-/// Check if a string is a member of a list of strings and optionally ignore case or ignore underscores
-inline std::ptrdiff_t find_member(std::string name,
-                                  const std::vector<std::string> names,
-                                  bool ignore_case = false,
-                                  bool ignore_underscore = false) {
+CLI11_INLINE std::ptrdiff_t
+find_member(std::string name, const std::vector<std::string> names, bool ignore_case, bool ignore_underscore) {
     auto it = std::end(names);
     if(ignore_case) {
         if(ignore_underscore) {
             name = detail::to_lower(detail::remove_underscore(name));
             it = std::find_if(std::begin(names), std::end(names), [&name](std::string local_name) {
                 return detail::to_lower(detail::remove_underscore(local_name)) == name;
             });
@@ -417,31 +537,19 @@
     } else {
         it = std::find(std::begin(names), std::end(names), name);
     }
 
     return (it != std::end(names)) ? (it - std::begin(names)) : (-1);
 }
 
-/// Find a trigger string and call a modify callable function that takes the current string and starting position of the
-/// trigger and returns the position in the string to search for the next trigger string
-template <typename Callable> inline std::string find_and_modify(std::string str, std::string trigger, Callable modify) {
-    std::size_t start_pos = 0;
-    while((start_pos = str.find(trigger, start_pos)) != std::string::npos) {
-        start_pos = modify(str, start_pos);
-    }
-    return str;
-}
-
-/// Split a string '"one two" "three"' into 'one two', 'three'
-/// Quote characters can be ` ' or "
-inline std::vector<std::string> split_up(std::string str, char delimiter = '\0') {
+CLI11_INLINE std::vector<std::string> split_up(std::string str, char delimiter) {
 
     const std::string delims("\'\"`");
     auto find_ws = [delimiter](char ch) {
-        return (delimiter == '\0') ? (std::isspace<char>(ch, std::locale()) != 0) : (ch == delimiter);
+        return (delimiter == '\0') ? std::isspace<char>(ch, std::locale()) : (ch == delimiter);
     };
     trim(str);
 
     std::vector<std::string> output;
     bool embeddedQuote = false;
     char keyChar = ' ';
     while(!str.empty()) {
@@ -481,63 +589,41 @@
             embeddedQuote = false;
         }
         trim(str);
     }
     return output;
 }
 
-/// Add a leader to the beginning of all new lines (nothing is added
-/// at the start of the first line). `"; "` would be for ini files
-///
-/// Can't use Regex, or this would be a subs.
-inline std::string fix_newlines(const std::string &leader, std::string input) {
-    std::string::size_type n = 0;
-    while(n != std::string::npos && n < input.size()) {
-        n = input.find('\n', n);
-        if(n != std::string::npos) {
-            input = input.substr(0, n + 1) + leader + input.substr(n + 1);
-            n += leader.size();
-        }
-    }
-    return input;
-}
-
-/// This function detects an equal or colon followed by an escaped quote after an argument
-/// then modifies the string to replace the equality with a space.  This is needed
-/// to allow the split up function to work properly and is intended to be used with the find_and_modify function
-/// the return value is the offset+1 which is required by the find_and_modify function.
-inline std::size_t escape_detect(std::string &str, std::size_t offset) {
+CLI11_INLINE std::size_t escape_detect(std::string &str, std::size_t offset) {
     auto next = str[offset + 1];
     if((next == '\"') || (next == '\'') || (next == '`')) {
         auto astart = str.find_last_of("-/ \"\'`", offset - 1);
         if(astart != std::string::npos) {
             if(str[astart] == ((str[offset] == '=') ? '-' : '/'))
                 str[offset] = ' ';  // interpret this as a space so the split_up works properly
         }
     }
     return offset + 1;
 }
 
-/// Add quotes if the string contains spaces
-inline std::string &add_quotes_if_needed(std::string &str) {
+CLI11_INLINE std::string &add_quotes_if_needed(std::string &str) {
     if((str.front() != '"' && str.front() != '\'') || str.front() != str.back()) {
         char quote = str.find('"') < str.find('\'') ? '\'' : '"';
         if(str.find(' ') != std::string::npos) {
             str.insert(0, 1, quote);
             str.append(1, quote);
         }
     }
     return str;
 }
 
 }  // namespace detail
 
 
 
-
 // Use one of these on all error classes.
 // These are temporary and are undef'd at the end of this file.
 #define CLI11_ERROR_DEF(parent, name)                                                                                  \
   protected:                                                                                                           \
     name(std::string ename, std::string msg, int exit_code) : parent(std::move(ename), std::move(msg), exit_code) {}   \
     name(std::string ename, std::string msg, ExitCodes exit_code)                                                      \
         : parent(std::move(ename), std::move(msg), exit_code) {}                                                       \
@@ -582,17 +668,17 @@
 
 /// All errors derive from this one
 class Error : public std::runtime_error {
     int actual_exit_code;
     std::string error_name{"Error"};
 
   public:
-    int get_exit_code() const { return actual_exit_code; }
+    CLI11_NODISCARD int get_exit_code() const { return actual_exit_code; }
 
-    std::string get_name() const { return error_name; }
+    CLI11_NODISCARD std::string get_name() const { return error_name; }
 
     Error(std::string name, std::string msg, int exit_code = static_cast<int>(ExitCodes::BaseClass))
         : runtime_error(msg), actual_exit_code(exit_code), error_name(std::move(name)) {}
 
     Error(std::string name, std::string msg, ExitCodes exit_code) : Error(name, msg, static_cast<int>(exit_code)) {}
 };
 
@@ -647,18 +733,18 @@
 
 /// Thrown when an option already exists
 class OptionAlreadyAdded : public ConstructionError {
     CLI11_ERROR_DEF(ConstructionError, OptionAlreadyAdded)
     explicit OptionAlreadyAdded(std::string name)
         : OptionAlreadyAdded(name + " is already added", ExitCodes::OptionAlreadyAdded) {}
     static OptionAlreadyAdded Requires(std::string name, std::string other) {
-        return OptionAlreadyAdded(name + " requires " + other, ExitCodes::OptionAlreadyAdded);
+        return {name + " requires " + other, ExitCodes::OptionAlreadyAdded};
     }
     static OptionAlreadyAdded Excludes(std::string name, std::string other) {
-        return OptionAlreadyAdded(name + " excludes " + other, ExitCodes::OptionAlreadyAdded);
+        return {name + " excludes " + other, ExitCodes::OptionAlreadyAdded};
     }
 };
 
 // Parsing errors
 
 /// Anything that can error in Parse
 class ParseError : public Error {
@@ -733,40 +819,38 @@
 class RequiredError : public ParseError {
     CLI11_ERROR_DEF(ParseError, RequiredError)
     explicit RequiredError(std::string name) : RequiredError(name + " is required", ExitCodes::RequiredError) {}
     static RequiredError Subcommand(std::size_t min_subcom) {
         if(min_subcom == 1) {
             return RequiredError("A subcommand");
         }
-        return RequiredError("Requires at least " + std::to_string(min_subcom) + " subcommands",
-                             ExitCodes::RequiredError);
+        return {"Requires at least " + std::to_string(min_subcom) + " subcommands", ExitCodes::RequiredError};
     }
     static RequiredError
     Option(std::size_t min_option, std::size_t max_option, std::size_t used, const std::string &option_list) {
         if((min_option == 1) && (max_option == 1) && (used == 0))
             return RequiredError("Exactly 1 option from [" + option_list + "]");
         if((min_option == 1) && (max_option == 1) && (used > 1)) {
-            return RequiredError("Exactly 1 option from [" + option_list + "] is required and " + std::to_string(used) +
-                                     " were given",
-                                 ExitCodes::RequiredError);
+            return {"Exactly 1 option from [" + option_list + "] is required and " + std::to_string(used) +
+                        " were given",
+                    ExitCodes::RequiredError};
         }
         if((min_option == 1) && (used == 0))
             return RequiredError("At least 1 option from [" + option_list + "]");
         if(used < min_option) {
-            return RequiredError("Requires at least " + std::to_string(min_option) + " options used and only " +
-                                     std::to_string(used) + "were given from [" + option_list + "]",
-                                 ExitCodes::RequiredError);
+            return {"Requires at least " + std::to_string(min_option) + " options used and only " +
+                        std::to_string(used) + "were given from [" + option_list + "]",
+                    ExitCodes::RequiredError};
         }
         if(max_option == 1)
-            return RequiredError("Requires at most 1 options be given from [" + option_list + "]",
-                                 ExitCodes::RequiredError);
+            return {"Requires at most 1 options be given from [" + option_list + "]", ExitCodes::RequiredError};
 
-        return RequiredError("Requires at most " + std::to_string(max_option) + " options be used and " +
-                                 std::to_string(used) + "were given from [" + option_list + "]",
-                             ExitCodes::RequiredError);
+        return {"Requires at most " + std::to_string(max_option) + " options be used and " + std::to_string(used) +
+                    "were given from [" + option_list + "]",
+                ExitCodes::RequiredError};
     }
 };
 
 /// Thrown when the wrong number of arguments has been received
 class ArgumentMismatch : public ParseError {
     CLI11_ERROR_DEF(ParseError, ArgumentMismatch)
     CLI11_ERROR_SIMPLE(ArgumentMismatch)
@@ -787,14 +871,18 @@
     }
     static ArgumentMismatch TypedAtLeast(std::string name, int num, std::string type) {
         return ArgumentMismatch(name + ": " + std::to_string(num) + " required " + type + " missing");
     }
     static ArgumentMismatch FlagOverride(std::string name) {
         return ArgumentMismatch(name + " was given a disallowed flag override");
     }
+    static ArgumentMismatch PartialType(std::string name, int num, std::string type) {
+        return ArgumentMismatch(name + ": " + type + " only partially specified: " + std::to_string(num) +
+                                " required for each element");
+    }
 };
 
 /// Thrown when a requires option is missing
 class RequiresError : public ParseError {
     CLI11_ERROR_DEF(ParseError, RequiresError)
     RequiresError(std::string curname, std::string subname)
         : RequiresError(curname + " requires " + subname, ExitCodes::RequiresError) {}
@@ -875,20 +963,22 @@
 /// An instance to use in EnableIf
 constexpr enabler dummy = {};
 }  // namespace detail
 
 /// A copy of enable_if_t from C++14, compatible with C++11.
 ///
 /// We could check to see if C++14 is being used, but it does not hurt to redefine this
-/// (even Google does this: https://github.com/google/skia/blob/master/include/private/SkTLogic.h)
+/// (even Google does this: https://github.com/google/skia/blob/main/include/private/SkTLogic.h)
 /// It is not in the std namespace anyway, so no harm done.
 template <bool B, class T = void> using enable_if_t = typename std::enable_if<B, T>::type;
 
 /// A copy of std::void_t from C++17 (helper for C++11 and C++14)
-template <typename... Ts> struct make_void { using type = void; };
+template <typename... Ts> struct make_void {
+    using type = void;
+};
 
 /// A copy of std::void_t from C++17 - same reasoning as enable_if_t, it does not hurt to redefine
 template <typename... Ts> using void_t = typename make_void<Ts...>::type;
 
 /// A copy of std::conditional_t from C++14 - same reasoning as enable_if_t, it does not hurt to redefine
 template <bool B, class T, class F> using conditional_t = typename std::conditional<B, T, F>::type;
 
@@ -909,36 +999,44 @@
 
 /// Check to see if something is copyable pointer
 template <typename T> struct is_copyable_ptr {
     static bool const value = is_shared_ptr<T>::value || std::is_pointer<T>::value;
 };
 
 /// This can be specialized to override the type deduction for IsMember.
-template <typename T> struct IsMemberType { using type = T; };
+template <typename T> struct IsMemberType {
+    using type = T;
+};
 
 /// The main custom type needed here is const char * should be a string.
-template <> struct IsMemberType<const char *> { using type = std::string; };
+template <> struct IsMemberType<const char *> {
+    using type = std::string;
+};
 
 namespace detail {
 
 // These are utilities for IsMember and other transforming objects
 
 /// Handy helper to access the element_type generically. This is not part of is_copyable_ptr because it requires that
 /// pointer_traits<T> be valid.
 
 /// not a pointer
-template <typename T, typename Enable = void> struct element_type { using type = T; };
+template <typename T, typename Enable = void> struct element_type {
+    using type = T;
+};
 
 template <typename T> struct element_type<T, typename std::enable_if<is_copyable_ptr<T>::value>::type> {
     using type = typename std::pointer_traits<T>::element_type;
 };
 
 /// Combination of the element type and value type - remove pointer (including smart pointers) and get the value_type of
 /// the container
-template <typename T> struct element_value_type { using type = typename element_type<T>::type::value_type; };
+template <typename T> struct element_value_type {
+    using type = typename element_type<T>::type::value_type;
+};
 
 /// Adaptor for set-like structure: This just wraps a normal container in a few utilities that do almost nothing.
 template <typename T, typename _ = void> struct pair_adaptor : std::false_type {
     using value_type = typename T::value_type;
     using first_type = typename std::remove_const<value_type>::type;
     using second_type = typename std::remove_const<value_type>::type;
 
@@ -987,15 +1085,15 @@
 template <typename T, typename C> class is_direct_constructible {
     template <typename TT, typename CC>
     static auto test(int, std::true_type) -> decltype(
 // NVCC warns about narrowing conversions here
 #ifdef __CUDACC__
 #pragma diag_suppress 2361
 #endif
-        TT { std::declval<CC>() }
+        TT{std::declval<CC>()}
 #ifdef __CUDACC__
 #pragma diag_default 2361
 #endif
         ,
         std::is_move_assignable<TT>());
 
     template <typename TT, typename CC> static auto test(int, std::false_type) -> std::false_type;
@@ -1114,15 +1212,15 @@
 }
 
 /// Construct a string from the object
 template <typename T,
           enable_if_t<std::is_constructible<std::string, T>::value && !std::is_convertible<T, std::string>::value,
                       detail::enabler> = detail::dummy>
 std::string to_string(const T &value) {
-    return std::string(value);
+    return std::string(value);  // NOLINT(google-readability-casting)
 }
 
 /// Convert an object to a string (streaming must be supported for that type)
 template <typename T,
           enable_if_t<!std::is_convertible<std::string, T>::value && !std::is_constructible<std::string, T>::value &&
                           is_ostreamable<T>::value,
                       detail::enabler> = detail::dummy>
@@ -1134,31 +1232,34 @@
 
 /// If conversion is not supported, return an empty string (streaming is not supported for that type)
 template <typename T,
           enable_if_t<!std::is_constructible<std::string, T>::value && !is_ostreamable<T>::value &&
                           !is_readable_container<typename std::remove_const<T>::type>::value,
                       detail::enabler> = detail::dummy>
 std::string to_string(T &&) {
-    return std::string{};
+    return {};
 }
 
 /// convert a readable container to a string
 template <typename T,
           enable_if_t<!std::is_constructible<std::string, T>::value && !is_ostreamable<T>::value &&
                           is_readable_container<T>::value,
                       detail::enabler> = detail::dummy>
 std::string to_string(T &&variable) {
-    std::vector<std::string> defaults;
     auto cval = variable.begin();
     auto end = variable.end();
+    if(cval == end) {
+        return {"{}"};
+    }
+    std::vector<std::string> defaults;
     while(cval != end) {
         defaults.emplace_back(CLI::detail::to_string(*cval));
         ++cval;
     }
-    return std::string("[" + detail::join(defaults) + "]");
+    return {"[" + detail::join(defaults) + "]"};
 }
 
 /// special template overload
 template <typename T1,
           typename T2,
           typename T,
           enable_if_t<std::is_same<T1, T2>::value, detail::enabler> = detail::dummy>
@@ -1188,23 +1289,27 @@
 template <typename T,
           enable_if_t<!std::is_enum<T>::value && !std::is_arithmetic<T>::value, detail::enabler> = detail::dummy>
 auto value_string(const T &value) -> decltype(to_string(value)) {
     return to_string(value);
 }
 
 /// template to get the underlying value type if it exists or use a default
-template <typename T, typename def, typename Enable = void> struct wrapped_type { using type = def; };
+template <typename T, typename def, typename Enable = void> struct wrapped_type {
+    using type = def;
+};
 
 /// Type size for regular object types that do not look like a tuple
 template <typename T, typename def> struct wrapped_type<T, def, typename std::enable_if<is_wrapper<T>::value>::type> {
     using type = typename T::value_type;
 };
 
 /// This will only trigger for actual void type
-template <typename T, typename Enable = void> struct type_count_base { static const int value{0}; };
+template <typename T, typename Enable = void> struct type_count_base {
+    static const int value{0};
+};
 
 /// Type size for regular object types that do not look like a tuple
 template <typename T>
 struct type_count_base<T,
                        typename std::enable_if<!is_tuple_like<T>::value && !is_mutable_container<T>::value &&
                                                !std::is_void<T>::value>::type> {
     static constexpr int value{1};
@@ -1226,15 +1331,17 @@
 /// forward declare the subtype_count structure
 template <typename T> struct subtype_count;
 
 /// forward declare the subtype_count_min structure
 template <typename T> struct subtype_count_min;
 
 /// This will only trigger for actual void type
-template <typename T, typename Enable = void> struct type_count { static const int value{0}; };
+template <typename T, typename Enable = void> struct type_count {
+    static const int value{0};
+};
 
 /// Type size for regular object types that do not look like a tuple
 template <typename T>
 struct type_count<T,
                   typename std::enable_if<!is_wrapper<T>::value && !is_tuple_like<T>::value && !is_complex<T>::value &&
                                           !std::is_void<T>::value>::type> {
     static constexpr int value{1};
@@ -1277,15 +1384,17 @@
 
 /// definition of subtype count
 template <typename T> struct subtype_count {
     static constexpr int value{is_mutable_container<T>::value ? expected_max_vector_size : type_count<T>::value};
 };
 
 /// This will only trigger for actual void type
-template <typename T, typename Enable = void> struct type_count_min { static const int value{0}; };
+template <typename T, typename Enable = void> struct type_count_min {
+    static const int value{0};
+};
 
 /// Type size for regular object types that do not look like a tuple
 template <typename T>
 struct type_count_min<
     T,
     typename std::enable_if<!is_mutable_container<T>::value && !is_tuple_like<T>::value && !is_wrapper<T>::value &&
                             !is_complex<T>::value && !std::is_void<T>::value>::type> {
@@ -1326,15 +1435,17 @@
 template <typename T> struct subtype_count_min {
     static constexpr int value{is_mutable_container<T>::value
                                    ? ((type_count<T>::value < expected_max_vector_size) ? type_count<T>::value : 0)
                                    : type_count_min<T>::value};
 };
 
 /// This will only trigger for actual void type
-template <typename T, typename Enable = void> struct expected_count { static const int value{0}; };
+template <typename T, typename Enable = void> struct expected_count {
+    static const int value{0};
+};
 
 /// For most types the number of expected items is 1
 template <typename T>
 struct expected_count<T,
                       typename std::enable_if<!is_mutable_container<T>::value && !is_wrapper<T>::value &&
                                               !std::is_void<T>::value>::type> {
     static constexpr int value{1};
@@ -1490,15 +1601,16 @@
 /// Tuple type
 template <typename T>
 struct classify_object<
     T,
     typename std::enable_if<is_tuple_like<T>::value &&
                             ((type_count<T>::value >= 2 && !is_wrapper<T>::value) ||
                              (uncommon_type<T>::value && !is_direct_constructible<T, double>::value &&
-                              !is_direct_constructible<T, int>::value))>::type> {
+                              !is_direct_constructible<T, int>::value) ||
+                             (uncommon_type<T>::value && type_count<T>::value >= 2))>::type> {
     static constexpr object_category value{object_category::tuple_value};
     // the condition on this class requires it be like a tuple, but on some compilers (like Xcode) tuples can be
     // constructed from just the first element so tuples of <string, int,int> can be constructed from a string, which
     // could lead to issues so there are two variants of the condition, the first isolates things with a type size >=2
     // mainly to get tuples on Xcode with the exception of wrappers, the second is the main one and just separating out
     // those cases that are caught by other object classifications
 };
@@ -1598,16 +1710,16 @@
 inline typename std::enable_if<I == type_count_base<T>::value, std::string>::type tuple_name() {
     return std::string{};
 }
 
 /// Recursively generate the tuple type name
 template <typename T, std::size_t I>
 inline typename std::enable_if<(I < type_count_base<T>::value), std::string>::type tuple_name() {
-    std::string str = std::string(type_name<typename std::decay<typename std::tuple_element<I, T>::type>::type>()) +
-                      ',' + tuple_name<T, I + 1>();
+    auto str = std::string{type_name<typename std::decay<typename std::tuple_element<I, T>::type>::type>()} + ',' +
+               tuple_name<T, I + 1>();
     if(str.back() == ',')
         str.pop_back();
     return str;
 }
 
 /// Print type name for tuples with 2 or more elements
 template <typename T,
@@ -1629,47 +1741,72 @@
 }
 
 // Lexical cast
 
 /// Convert to an unsigned integral
 template <typename T, enable_if_t<std::is_unsigned<T>::value, detail::enabler> = detail::dummy>
 bool integral_conversion(const std::string &input, T &output) noexcept {
-    if(input.empty()) {
+    if(input.empty() || input.front() == '-') {
         return false;
     }
     char *val = nullptr;
+    errno = 0;
     std::uint64_t output_ll = std::strtoull(input.c_str(), &val, 0);
+    if(errno == ERANGE) {
+        return false;
+    }
     output = static_cast<T>(output_ll);
-    return val == (input.c_str() + input.size()) && static_cast<std::uint64_t>(output) == output_ll;
+    if(val == (input.c_str() + input.size()) && static_cast<std::uint64_t>(output) == output_ll) {
+        return true;
+    }
+    val = nullptr;
+    std::int64_t output_sll = std::strtoll(input.c_str(), &val, 0);
+    if(val == (input.c_str() + input.size())) {
+        output = (output_sll < 0) ? static_cast<T>(0) : static_cast<T>(output_sll);
+        return (static_cast<std::int64_t>(output) == output_sll);
+    }
+    return false;
 }
 
 /// Convert to a signed integral
 template <typename T, enable_if_t<std::is_signed<T>::value, detail::enabler> = detail::dummy>
 bool integral_conversion(const std::string &input, T &output) noexcept {
     if(input.empty()) {
         return false;
     }
     char *val = nullptr;
+    errno = 0;
     std::int64_t output_ll = std::strtoll(input.c_str(), &val, 0);
+    if(errno == ERANGE) {
+        return false;
+    }
     output = static_cast<T>(output_ll);
-    return val == (input.c_str() + input.size()) && static_cast<std::int64_t>(output) == output_ll;
+    if(val == (input.c_str() + input.size()) && static_cast<std::int64_t>(output) == output_ll) {
+        return true;
+    }
+    if(input == "true") {
+        // this is to deal with a few oddities with flags and wrapper int types
+        output = static_cast<T>(1);
+        return true;
+    }
+    return false;
 }
 
 /// Convert a flag into an integer value  typically binary flags
 inline std::int64_t to_flag_value(std::string val) {
     static const std::string trueString("true");
     static const std::string falseString("false");
     if(val == trueString) {
         return 1;
     }
     if(val == falseString) {
         return -1;
     }
     val = detail::to_lower(val);
-    std::int64_t ret;
+    std::int64_t ret = 0;
     if(val.size() == 1) {
         if(val[0] >= '1' && val[0] <= '9') {
             return (static_cast<std::int64_t>(val[0]) - '0');
         }
         switch(val[0]) {
         case '0':
         case 'f':
@@ -1754,26 +1891,26 @@
 bool lexical_cast(const std::string &input, T &output) {
     using XC = typename wrapped_type<T, double>::type;
     XC x{0.0}, y{0.0};
     auto str1 = input;
     bool worked = false;
     auto nloc = str1.find_last_of("+-");
     if(nloc != std::string::npos && nloc > 0) {
-        worked = detail::lexical_cast(str1.substr(0, nloc), x);
+        worked = lexical_cast(str1.substr(0, nloc), x);
         str1 = str1.substr(nloc);
         if(str1.back() == 'i' || str1.back() == 'j')
             str1.pop_back();
-        worked = worked && detail::lexical_cast(str1, y);
+        worked = worked && lexical_cast(str1, y);
     } else {
         if(str1.back() == 'i' || str1.back() == 'j') {
             str1.pop_back();
-            worked = detail::lexical_cast(str1, y);
+            worked = lexical_cast(str1, y);
             x = XC{0};
         } else {
-            worked = detail::lexical_cast(str1, x);
+            worked = lexical_cast(str1, x);
             y = XC{0};
         }
     }
     if(worked) {
         output = T{x, y};
         return worked;
     }
@@ -1837,60 +1974,61 @@
 }
 
 /// Assignable from double or int
 template <
     typename T,
     enable_if_t<classify_object<T>::value == object_category::number_constructible, detail::enabler> = detail::dummy>
 bool lexical_cast(const std::string &input, T &output) {
-    int val;
+    int val = 0;
     if(integral_conversion(input, val)) {
         output = T(val);
         return true;
-    } else {
-        double dval;
-        if(lexical_cast(input, dval)) {
-            output = T{dval};
-            return true;
-        }
     }
+
+    double dval = 0.0;
+    if(lexical_cast(input, dval)) {
+        output = T{dval};
+        return true;
+    }
+
     return from_stream(input, output);
 }
 
 /// Assignable from int
 template <
     typename T,
     enable_if_t<classify_object<T>::value == object_category::integer_constructible, detail::enabler> = detail::dummy>
 bool lexical_cast(const std::string &input, T &output) {
-    int val;
+    int val = 0;
     if(integral_conversion(input, val)) {
         output = T(val);
         return true;
     }
     return from_stream(input, output);
 }
 
 /// Assignable from double
 template <
     typename T,
     enable_if_t<classify_object<T>::value == object_category::double_constructible, detail::enabler> = detail::dummy>
 bool lexical_cast(const std::string &input, T &output) {
-    double val;
+    double val = 0.0;
     if(lexical_cast(input, val)) {
         output = T{val};
         return true;
     }
     return from_stream(input, output);
 }
 
 /// Non-string convertible from an int
 template <typename T,
           enable_if_t<classify_object<T>::value == object_category::other && std::is_assignable<T &, int>::value,
                       detail::enabler> = detail::dummy>
 bool lexical_cast(const std::string &input, T &output) {
-    int val;
+    int val = 0;
     if(integral_conversion(input, val)) {
 #ifdef _MSC_VER
 #pragma warning(push)
 #pragma warning(disable : 4800)
 #endif
         // with Atomic<XX> this could produce a warning due to the conversion but if atomic gets here it is an old style
         // so will most likely still work
@@ -1970,30 +2108,30 @@
                           std::is_assignable<AssignTo &, int>::value,
                       detail::enabler> = detail::dummy>
 bool lexical_assign(const std::string &input, AssignTo &output) {
     if(input.empty()) {
         output = 0;
         return true;
     }
-    int val;
+    int val = 0;
     if(lexical_cast(input, val)) {
         output = val;
         return true;
     }
     return false;
 }
 
 /// Assign a value converted from a string in lexical cast to the output value directly
 template <typename AssignTo,
           typename ConvertTo,
           enable_if_t<!std::is_same<AssignTo, ConvertTo>::value && std::is_assignable<AssignTo &, ConvertTo &>::value,
                       detail::enabler> = detail::dummy>
 bool lexical_assign(const std::string &input, AssignTo &output) {
     ConvertTo val{};
-    bool parse_result = (!input.empty()) ? lexical_cast<ConvertTo>(input, val) : true;
+    bool parse_result = (!input.empty()) ? lexical_cast(input, val) : true;
     if(parse_result) {
         output = val;
     }
     return parse_result;
 }
 
 /// Assign a value from a lexical cast through constructing a value and move assigning it
@@ -2001,15 +2139,15 @@
     typename AssignTo,
     typename ConvertTo,
     enable_if_t<!std::is_same<AssignTo, ConvertTo>::value && !std::is_assignable<AssignTo &, ConvertTo &>::value &&
                     std::is_move_assignable<AssignTo>::value,
                 detail::enabler> = detail::dummy>
 bool lexical_assign(const std::string &input, AssignTo &output) {
     ConvertTo val{};
-    bool parse_result = input.empty() ? true : lexical_cast<ConvertTo>(input, val);
+    bool parse_result = input.empty() ? true : lexical_cast(input, val);
     if(parse_result) {
         output = AssignTo(val);  // use () form of constructor to allow some implicit conversions
     }
     return parse_result;
 }
 
 /// primary lexical conversion operation, 1 string to 1 type of some kind
@@ -2047,21 +2185,31 @@
 template <class AssignTo,
           class ConvertTo,
           enable_if_t<is_mutable_container<AssignTo>::value && is_mutable_container<ConvertTo>::value &&
                           type_count<ConvertTo>::value == 1,
                       detail::enabler> = detail::dummy>
 bool lexical_conversion(const std::vector<std ::string> &strings, AssignTo &output) {
     output.erase(output.begin(), output.end());
+    if(strings.size() == 1 && strings[0] == "{}") {
+        return true;
+    }
+    bool skip_remaining = false;
+    if(strings.size() == 2 && strings[0] == "{}" && is_separator(strings[1])) {
+        skip_remaining = true;
+    }
     for(const auto &elem : strings) {
         typename AssignTo::value_type out;
         bool retval = lexical_assign<typename AssignTo::value_type, typename ConvertTo::value_type>(elem, out);
         if(!retval) {
             return false;
         }
         output.insert(output.end(), std::move(out));
+        if(skip_remaining) {
+            break;
+        }
     }
     return (!output.empty());
 }
 
 /// Lexical conversion for complex types
 template <class AssignTo, class ConvertTo, enable_if_t<is_complex<ConvertTo>::value, detail::enabler> = detail::dummy>
 bool lexical_conversion(const std::vector<std::string> &strings, AssignTo &output) {
@@ -2069,22 +2217,21 @@
     if(strings.size() >= 2 && !strings[1].empty()) {
         using XC2 = typename wrapped_type<ConvertTo, double>::type;
         XC2 x{0.0}, y{0.0};
         auto str1 = strings[1];
         if(str1.back() == 'i' || str1.back() == 'j') {
             str1.pop_back();
         }
-        auto worked = detail::lexical_cast(strings[0], x) && detail::lexical_cast(str1, y);
+        auto worked = lexical_cast(strings[0], x) && lexical_cast(str1, y);
         if(worked) {
             output = ConvertTo{x, y};
         }
         return worked;
-    } else {
-        return lexical_assign<AssignTo, ConvertTo>(strings[0], output);
     }
+    return lexical_assign<AssignTo, ConvertTo>(strings[0], output);
 }
 
 /// Conversion to a vector type using a particular single type as the conversion type
 template <class AssignTo,
           class ConvertTo,
           enable_if_t<is_mutable_container<AssignTo>::value && (expected_count<ConvertTo>::value == 1) &&
                           (type_count<ConvertTo>::value == 1),
@@ -2327,131 +2474,130 @@
     if(lexical_conversion<typename ConvertTo::value_type, typename ConvertTo::value_type>(strings, val)) {
         output = val;
         return true;
     }
     return false;
 }
 
-/// Sum a vector of flag representations
-/// The flag vector produces a series of strings in a vector,  simple true is represented by a "1",  simple false is
-/// by
-/// "-1" an if numbers are passed by some fashion they are captured as well so the function just checks for the most
-/// common true and false strings then uses stoll to convert the rest for summing
-template <typename T, enable_if_t<std::is_unsigned<T>::value, detail::enabler> = detail::dummy>
-void sum_flag_vector(const std::vector<std::string> &flags, T &output) {
-    std::int64_t count{0};
-    for(auto &flag : flags) {
-        count += detail::to_flag_value(flag);
+/// Sum a vector of strings
+inline std::string sum_string_vector(const std::vector<std::string> &values) {
+    double val{0.0};
+    bool fail{false};
+    std::string output;
+    for(const auto &arg : values) {
+        double tv{0.0};
+        auto comp = lexical_cast(arg, tv);
+        if(!comp) {
+            try {
+                tv = static_cast<double>(detail::to_flag_value(arg));
+            } catch(const std::exception &) {
+                fail = true;
+                break;
+            }
+        }
+        val += tv;
     }
-    output = (count > 0) ? static_cast<T>(count) : T{0};
-}
-
-/// Sum a vector of flag representations
-/// The flag vector produces a series of strings in a vector,  simple true is represented by a "1",  simple false is
-/// by
-/// "-1" an if numbers are passed by some fashion they are captured as well so the function just checks for the most
-/// common true and false strings then uses stoll to convert the rest for summing
-template <typename T, enable_if_t<std::is_signed<T>::value, detail::enabler> = detail::dummy>
-void sum_flag_vector(const std::vector<std::string> &flags, T &output) {
-    std::int64_t count{0};
-    for(auto &flag : flags) {
-        count += detail::to_flag_value(flag);
+    if(fail) {
+        for(const auto &arg : values) {
+            output.append(arg);
+        }
+    } else {
+        if(val <= static_cast<double>((std::numeric_limits<std::int64_t>::min)()) ||
+           val >= static_cast<double>((std::numeric_limits<std::int64_t>::max)()) ||
+           std::ceil(val) == std::floor(val)) {
+            output = detail::value_string(static_cast<int64_t>(val));
+        } else {
+            output = detail::value_string(val);
+        }
     }
-    output = static_cast<T>(count);
+    return output;
 }
 
-#ifdef _MSC_VER
-#pragma warning(push)
-#pragma warning(disable : 4800)
-#endif
-// with Atomic<XX> this could produce a warning due to the conversion but if atomic gets here it is an old style so will
-// most likely still work
+}  // namespace detail
 
-/// Sum a vector of flag representations
-/// The flag vector produces a series of strings in a vector,  simple true is represented by a "1",  simple false is
-/// by
-/// "-1" an if numbers are passed by some fashion they are captured as well so the function just checks for the most
-/// common true and false strings then uses stoll to convert the rest for summing
-template <typename T,
-          enable_if_t<!std::is_signed<T>::value && !std::is_unsigned<T>::value, detail::enabler> = detail::dummy>
-void sum_flag_vector(const std::vector<std::string> &flags, T &output) {
-    std::int64_t count{0};
-    for(auto &flag : flags) {
-        count += detail::to_flag_value(flag);
-    }
-    std::string out = detail::to_string(count);
-    lexical_cast(out, output);
-}
 
-#ifdef _MSC_VER
-#pragma warning(pop)
-#endif
+
+namespace detail {
+
+// Returns false if not a short option. Otherwise, sets opt name and rest and returns true
+CLI11_INLINE bool split_short(const std::string &current, std::string &name, std::string &rest);
+
+// Returns false if not a long option. Otherwise, sets opt name and other side of = and returns true
+CLI11_INLINE bool split_long(const std::string &current, std::string &name, std::string &value);
+
+// Returns false if not a windows style option. Otherwise, sets opt name and value and returns true
+CLI11_INLINE bool split_windows_style(const std::string &current, std::string &name, std::string &value);
+
+// Splits a string into multiple long and short names
+CLI11_INLINE std::vector<std::string> split_names(std::string current);
+
+/// extract default flag values either {def} or starting with a !
+CLI11_INLINE std::vector<std::pair<std::string, std::string>> get_default_flag_values(const std::string &str);
+
+/// Get a vector of short names, one of long names, and a single name
+CLI11_INLINE std::tuple<std::vector<std::string>, std::vector<std::string>, std::string>
+get_names(const std::vector<std::string> &input);
 
 }  // namespace detail
 
 
 
 namespace detail {
 
-// Returns false if not a short option. Otherwise, sets opt name and rest and returns true
-inline bool split_short(const std::string &current, std::string &name, std::string &rest) {
+CLI11_INLINE bool split_short(const std::string &current, std::string &name, std::string &rest) {
     if(current.size() > 1 && current[0] == '-' && valid_first_char(current[1])) {
         name = current.substr(1, 1);
         rest = current.substr(2);
         return true;
     }
     return false;
 }
 
-// Returns false if not a long option. Otherwise, sets opt name and other side of = and returns true
-inline bool split_long(const std::string &current, std::string &name, std::string &value) {
+CLI11_INLINE bool split_long(const std::string &current, std::string &name, std::string &value) {
     if(current.size() > 2 && current.substr(0, 2) == "--" && valid_first_char(current[2])) {
         auto loc = current.find_first_of('=');
         if(loc != std::string::npos) {
             name = current.substr(2, loc - 2);
             value = current.substr(loc + 1);
         } else {
             name = current.substr(2);
             value = "";
         }
         return true;
     }
     return false;
 }
 
-// Returns false if not a windows style option. Otherwise, sets opt name and value and returns true
-inline bool split_windows_style(const std::string &current, std::string &name, std::string &value) {
+CLI11_INLINE bool split_windows_style(const std::string &current, std::string &name, std::string &value) {
     if(current.size() > 1 && current[0] == '/' && valid_first_char(current[1])) {
         auto loc = current.find_first_of(':');
         if(loc != std::string::npos) {
             name = current.substr(1, loc - 1);
             value = current.substr(loc + 1);
         } else {
             name = current.substr(1);
             value = "";
         }
         return true;
     }
     return false;
 }
 
-// Splits a string into multiple long and short names
-inline std::vector<std::string> split_names(std::string current) {
+CLI11_INLINE std::vector<std::string> split_names(std::string current) {
     std::vector<std::string> output;
-    std::size_t val;
-    while((val = current.find(",")) != std::string::npos) {
+    std::size_t val = 0;
+    while((val = current.find(',')) != std::string::npos) {
         output.push_back(trim_copy(current.substr(0, val)));
         current = current.substr(val + 1);
     }
     output.push_back(trim_copy(current));
     return output;
 }
 
-/// extract default flag values either {def} or starting with a !
-inline std::vector<std::pair<std::string, std::string>> get_default_flag_values(const std::string &str) {
+CLI11_INLINE std::vector<std::pair<std::string, std::string>> get_default_flag_values(const std::string &str) {
     std::vector<std::string> flags = split_names(str);
     flags.erase(std::remove_if(flags.begin(),
                                flags.end(),
                                [](const std::string &name) {
                                    return ((name.empty()) || (!(((name.find_first_of('{') != std::string::npos) &&
                                                                  (name.back() == '}')) ||
                                                                 (name[0] == '!'))));
@@ -2461,24 +2607,23 @@
     output.reserve(flags.size());
     for(auto &flag : flags) {
         auto def_start = flag.find_first_of('{');
         std::string defval = "false";
         if((def_start != std::string::npos) && (flag.back() == '}')) {
             defval = flag.substr(def_start + 1);
             defval.pop_back();
-            flag.erase(def_start, std::string::npos);
+            flag.erase(def_start, std::string::npos);  // NOLINT(readability-suspicious-call-argument)
         }
         flag.erase(0, flag.find_first_not_of("-!"));
         output.emplace_back(flag, defval);
     }
     return output;
 }
 
-/// Get a vector of short names, one of long names, and a single name
-inline std::tuple<std::vector<std::string>, std::vector<std::string>, std::string>
+CLI11_INLINE std::tuple<std::vector<std::string>, std::vector<std::string>, std::string>
 get_names(const std::vector<std::string> &input) {
 
     std::vector<std::string> short_names;
     std::vector<std::string> long_names;
     std::string pos_name;
 
     for(std::string name : input) {
@@ -2501,16 +2646,15 @@
         } else {
             if(pos_name.length() > 0)
                 throw BadNameString::MultiPositionalNames(name);
             pos_name = name;
         }
     }
 
-    return std::tuple<std::vector<std::string>, std::vector<std::string>, std::string>(
-        short_names, long_names, pos_name);
+    return std::make_tuple(short_names, long_names, pos_name);
 }
 
 }  // namespace detail
 
 
 
 class App;
@@ -2523,15 +2667,15 @@
     /// This is the name
     std::string name{};
 
     /// Listing of inputs
     std::vector<std::string> inputs{};
 
     /// The list of parents and name joined by "."
-    std::string fullname() const {
+    CLI11_NODISCARD std::string fullname() const {
         std::vector<std::string> tmp = parents;
         tmp.emplace_back(name);
         return detail::join(tmp, ".");
     }
 };
 
 /// This class provides a converter for configuration files.
@@ -2543,23 +2687,26 @@
     /// Convert an app into a configuration
     virtual std::string to_config(const App *, bool, bool, std::string) const = 0;
 
     /// Convert a configuration into an app
     virtual std::vector<ConfigItem> from_config(std::istream &) const = 0;
 
     /// Get a flag value
-    virtual std::string to_flag(const ConfigItem &item) const {
+    CLI11_NODISCARD virtual std::string to_flag(const ConfigItem &item) const {
         if(item.inputs.size() == 1) {
             return item.inputs.at(0);
         }
-        throw ConversionError::TooManyInputsFlag(item.fullname());
+        if(item.inputs.empty()) {
+            return "{}";
+        }
+        throw ConversionError::TooManyInputsFlag(item.fullname());  // LCOV_EXCL_LINE
     }
 
     /// Parse a config file, throw an error (ParseError:ConfigParseError or FileError) on failure
-    std::vector<ConfigItem> from_file(const std::string &name) {
+    CLI11_NODISCARD std::vector<ConfigItem> from_file(const std::string &name) const {
         std::ifstream input{name};
         if(!input.good())
             throw FileError::Missing(name);
 
         return from_config(input);
     }
 
@@ -2580,14 +2727,22 @@
     char arraySeparator = ',';
     /// the character used separate the name from the value
     char valueDelimiter = '=';
     /// the character to use around strings
     char stringQuote = '"';
     /// the character to use around single characters
     char characterQuote = '\'';
+    /// the maximum number of layers to allow
+    uint8_t maximumLayers{255};
+    /// the separator used to separator parent layers
+    char parentSeparatorChar{'.'};
+    /// Specify the configuration index to use for arrayed sections
+    int16_t configIndex{-1};
+    /// Specify the configuration section that should be used
+    std::string configSection{};
 
   public:
     std::string
     to_config(const App * /*app*/, bool default_also, bool write_description, std::string prefix) const override;
 
     std::vector<ConfigItem> from_config(std::istream &input) const override;
     /// Specify the configuration for comment characters
@@ -2613,14 +2768,43 @@
     }
     /// Specify the quote characters used around strings and characters
     ConfigBase *quoteCharacter(char qString, char qChar) {
         stringQuote = qString;
         characterQuote = qChar;
         return this;
     }
+    /// Specify the maximum number of parents
+    ConfigBase *maxLayers(uint8_t layers) {
+        maximumLayers = layers;
+        return this;
+    }
+    /// Specify the separator to use for parent layers
+    ConfigBase *parentSeparator(char sep) {
+        parentSeparatorChar = sep;
+        return this;
+    }
+    /// get a reference to the configuration section
+    std::string &sectionRef() { return configSection; }
+    /// get the section
+    CLI11_NODISCARD const std::string &section() const { return configSection; }
+    /// specify a particular section of the configuration file to use
+    ConfigBase *section(const std::string &sectionName) {
+        configSection = sectionName;
+        return this;
+    }
+
+    /// get a reference to the configuration index
+    int16_t &indexRef() { return configIndex; }
+    /// get the section index
+    CLI11_NODISCARD int16_t index() const { return configIndex; }
+    /// specify a particular index in the section to use (-1) for all sections to use
+    ConfigBase *index(int16_t sectionIndex) {
+        configIndex = sectionIndex;
+        return this;
+    }
 };
 
 /// the default Config is the TOML file format
 using ConfigTOML = ConfigBase;
 
 /// ConfigINI generates a "standard" INI compliant output
 class ConfigINI : public ConfigTOML {
@@ -2662,14 +2846,17 @@
     /// A Validator will only apply to an indexed value (-1 is all elements)
     int application_index_ = -1;
     /// Enable for Validator to allow it to be disabled if need be
     bool active_{true};
     /// specify that a validator should not modify the input
     bool non_modifying_{false};
 
+    Validator(std::string validator_desc, std::function<std::string(std::string &)> func)
+        : desc_function_([validator_desc]() { return validator_desc; }), func_(std::move(func)) {}
+
   public:
     Validator() = default;
     /// Construct a Validator with just the description string
     explicit Validator(std::string validator_desc) : desc_function_([validator_desc]() { return validator_desc; }) {}
     /// Construct Validator from basic information
     Validator(std::function<std::string(std::string &)> op, std::string validator_desc, std::string validator_name = "")
         : desc_function_([validator_desc]() { return validator_desc; }), func_(std::move(op)),
@@ -2677,72 +2864,58 @@
     /// Set the Validator operation function
     Validator &operation(std::function<std::string(std::string &)> op) {
         func_ = std::move(op);
         return *this;
     }
     /// This is the required operator for a Validator - provided to help
     /// users (CLI11 uses the member `func` directly)
-    std::string operator()(std::string &str) const {
-        std::string retstring;
-        if(active_) {
-            if(non_modifying_) {
-                std::string value = str;
-                retstring = func_(value);
-            } else {
-                retstring = func_(str);
-            }
-        }
-        return retstring;
-    }
+    std::string operator()(std::string &str) const;
 
     /// This is the required operator for a Validator - provided to help
     /// users (CLI11 uses the member `func` directly)
     std::string operator()(const std::string &str) const {
         std::string value = str;
         return (active_) ? func_(value) : std::string{};
     }
 
     /// Specify the type string
     Validator &description(std::string validator_desc) {
         desc_function_ = [validator_desc]() { return validator_desc; };
         return *this;
     }
     /// Specify the type string
-    Validator description(std::string validator_desc) const {
-        Validator newval(*this);
-        newval.desc_function_ = [validator_desc]() { return validator_desc; };
-        return newval;
-    }
+    CLI11_NODISCARD Validator description(std::string validator_desc) const;
+
     /// Generate type description information for the Validator
-    std::string get_description() const {
+    CLI11_NODISCARD std::string get_description() const {
         if(active_) {
             return desc_function_();
         }
         return std::string{};
     }
     /// Specify the type string
     Validator &name(std::string validator_name) {
         name_ = std::move(validator_name);
         return *this;
     }
     /// Specify the type string
-    Validator name(std::string validator_name) const {
+    CLI11_NODISCARD Validator name(std::string validator_name) const {
         Validator newval(*this);
         newval.name_ = std::move(validator_name);
         return newval;
     }
     /// Get the name of the Validator
-    const std::string &get_name() const { return name_; }
+    CLI11_NODISCARD const std::string &get_name() const { return name_; }
     /// Specify whether the Validator is active or not
     Validator &active(bool active_val = true) {
         active_ = active_val;
         return *this;
     }
     /// Specify whether the Validator is active or not
-    Validator active(bool active_val = true) const {
+    CLI11_NODISCARD Validator active(bool active_val = true) const {
         Validator newval(*this);
         newval.active_ = active_val;
         return newval;
     }
 
     /// Specify whether the Validator can be modifying or not
     Validator &non_modifying(bool no_modify = true) {
@@ -2751,254 +2924,85 @@
     }
     /// Specify the application index of a validator
     Validator &application_index(int app_index) {
         application_index_ = app_index;
         return *this;
     }
     /// Specify the application index of a validator
-    Validator application_index(int app_index) const {
+    CLI11_NODISCARD Validator application_index(int app_index) const {
         Validator newval(*this);
         newval.application_index_ = app_index;
         return newval;
     }
     /// Get the current value of the application index
-    int get_application_index() const { return application_index_; }
+    CLI11_NODISCARD int get_application_index() const { return application_index_; }
     /// Get a boolean if the validator is active
-    bool get_active() const { return active_; }
+    CLI11_NODISCARD bool get_active() const { return active_; }
 
     /// Get a boolean if the validator is allowed to modify the input returns true if it can modify the input
-    bool get_modifying() const { return !non_modifying_; }
+    CLI11_NODISCARD bool get_modifying() const { return !non_modifying_; }
 
     /// Combining validators is a new validator. Type comes from left validator if function, otherwise only set if the
     /// same.
-    Validator operator&(const Validator &other) const {
-        Validator newval;
-
-        newval._merge_description(*this, other, " AND ");
-
-        // Give references (will make a copy in lambda function)
-        const std::function<std::string(std::string & filename)> &f1 = func_;
-        const std::function<std::string(std::string & filename)> &f2 = other.func_;
-
-        newval.func_ = [f1, f2](std::string &input) {
-            std::string s1 = f1(input);
-            std::string s2 = f2(input);
-            if(!s1.empty() && !s2.empty())
-                return std::string("(") + s1 + ") AND (" + s2 + ")";
-            else
-                return s1 + s2;
-        };
-
-        newval.active_ = (active_ & other.active_);
-        newval.application_index_ = application_index_;
-        return newval;
-    }
+    Validator operator&(const Validator &other) const;
 
     /// Combining validators is a new validator. Type comes from left validator if function, otherwise only set if the
     /// same.
-    Validator operator|(const Validator &other) const {
-        Validator newval;
-
-        newval._merge_description(*this, other, " OR ");
-
-        // Give references (will make a copy in lambda function)
-        const std::function<std::string(std::string &)> &f1 = func_;
-        const std::function<std::string(std::string &)> &f2 = other.func_;
-
-        newval.func_ = [f1, f2](std::string &input) {
-            std::string s1 = f1(input);
-            std::string s2 = f2(input);
-            if(s1.empty() || s2.empty())
-                return std::string();
-
-            return std::string("(") + s1 + ") OR (" + s2 + ")";
-        };
-        newval.active_ = (active_ & other.active_);
-        newval.application_index_ = application_index_;
-        return newval;
-    }
+    Validator operator|(const Validator &other) const;
 
     /// Create a validator that fails when a given validator succeeds
-    Validator operator!() const {
-        Validator newval;
-        const std::function<std::string()> &dfunc1 = desc_function_;
-        newval.desc_function_ = [dfunc1]() {
-            auto str = dfunc1();
-            return (!str.empty()) ? std::string("NOT ") + str : std::string{};
-        };
-        // Give references (will make a copy in lambda function)
-        const std::function<std::string(std::string & res)> &f1 = func_;
-
-        newval.func_ = [f1, dfunc1](std::string &test) -> std::string {
-            std::string s1 = f1(test);
-            if(s1.empty()) {
-                return std::string("check ") + dfunc1() + " succeeded improperly";
-            }
-            return std::string{};
-        };
-        newval.active_ = active_;
-        newval.application_index_ = application_index_;
-        return newval;
-    }
+    Validator operator!() const;
 
   private:
-    void _merge_description(const Validator &val1, const Validator &val2, const std::string &merger) {
-
-        const std::function<std::string()> &dfunc1 = val1.desc_function_;
-        const std::function<std::string()> &dfunc2 = val2.desc_function_;
-
-        desc_function_ = [=]() {
-            std::string f1 = dfunc1();
-            std::string f2 = dfunc2();
-            if((f1.empty()) || (f2.empty())) {
-                return f1 + f2;
-            }
-            return std::string(1, '(') + f1 + ')' + merger + '(' + f2 + ')';
-        };
-    }
-};  // namespace CLI
+    void _merge_description(const Validator &val1, const Validator &val2, const std::string &merger);
+};
 
 /// Class wrapping some of the accessors of Validator
 class CustomValidator : public Validator {
   public:
 };
 // The implementation of the built in validators is using the Validator class;
 // the user is only expected to use the const (static) versions (since there's no setup).
 // Therefore, this is in detail.
 namespace detail {
 
 /// CLI enumeration of different file types
 enum class path_type { nonexistent, file, directory };
 
-#if defined CLI11_HAS_FILESYSTEM && CLI11_HAS_FILESYSTEM > 0
-/// get the type of the path from a file name
-inline path_type check_path(const char *file) noexcept {
-    std::error_code ec;
-    auto stat = std::filesystem::status(file, ec);
-    if(ec) {
-        return path_type::nonexistent;
-    }
-    switch(stat.type()) {
-    case std::filesystem::file_type::none:
-    case std::filesystem::file_type::not_found:
-        return path_type::nonexistent;
-    case std::filesystem::file_type::directory:
-        return path_type::directory;
-    case std::filesystem::file_type::symlink:
-    case std::filesystem::file_type::block:
-    case std::filesystem::file_type::character:
-    case std::filesystem::file_type::fifo:
-    case std::filesystem::file_type::socket:
-    case std::filesystem::file_type::regular:
-    case std::filesystem::file_type::unknown:
-    default:
-        return path_type::file;
-    }
-}
-#else
 /// get the type of the path from a file name
-inline path_type check_path(const char *file) noexcept {
-#if defined(_MSC_VER)
-    struct __stat64 buffer;
-    if(_stat64(file, &buffer) == 0) {
-        return ((buffer.st_mode & S_IFDIR) != 0) ? path_type::directory : path_type::file;
-    }
-#else
-    struct stat buffer;
-    if(stat(file, &buffer) == 0) {
-        return ((buffer.st_mode & S_IFDIR) != 0) ? path_type::directory : path_type::file;
-    }
-#endif
-    return path_type::nonexistent;
-}
-#endif
+CLI11_INLINE path_type check_path(const char *file) noexcept;
+
 /// Check for an existing file (returns error message if check fails)
 class ExistingFileValidator : public Validator {
   public:
-    ExistingFileValidator() : Validator("FILE") {
-        func_ = [](std::string &filename) {
-            auto path_result = check_path(filename.c_str());
-            if(path_result == path_type::nonexistent) {
-                return "File does not exist: " + filename;
-            }
-            if(path_result == path_type::directory) {
-                return "File is actually a directory: " + filename;
-            }
-            return std::string();
-        };
-    }
+    ExistingFileValidator();
 };
 
 /// Check for an existing directory (returns error message if check fails)
 class ExistingDirectoryValidator : public Validator {
   public:
-    ExistingDirectoryValidator() : Validator("DIR") {
-        func_ = [](std::string &filename) {
-            auto path_result = check_path(filename.c_str());
-            if(path_result == path_type::nonexistent) {
-                return "Directory does not exist: " + filename;
-            }
-            if(path_result == path_type::file) {
-                return "Directory is actually a file: " + filename;
-            }
-            return std::string();
-        };
-    }
+    ExistingDirectoryValidator();
 };
 
 /// Check for an existing path
 class ExistingPathValidator : public Validator {
   public:
-    ExistingPathValidator() : Validator("PATH(existing)") {
-        func_ = [](std::string &filename) {
-            auto path_result = check_path(filename.c_str());
-            if(path_result == path_type::nonexistent) {
-                return "Path does not exist: " + filename;
-            }
-            return std::string();
-        };
-    }
+    ExistingPathValidator();
 };
 
 /// Check for an non-existing path
 class NonexistentPathValidator : public Validator {
   public:
-    NonexistentPathValidator() : Validator("PATH(non-existing)") {
-        func_ = [](std::string &filename) {
-            auto path_result = check_path(filename.c_str());
-            if(path_result != path_type::nonexistent) {
-                return "Path already exists: " + filename;
-            }
-            return std::string();
-        };
-    }
+    NonexistentPathValidator();
 };
 
 /// Validate the given string is a legal ipv4 address
 class IPV4Validator : public Validator {
   public:
-    IPV4Validator() : Validator("IPV4") {
-        func_ = [](std::string &ip_addr) {
-            auto result = CLI::detail::split(ip_addr, '.');
-            if(result.size() != 4) {
-                return std::string("Invalid IPV4 address must have four parts (") + ip_addr + ')';
-            }
-            int num;
-            for(const auto &var : result) {
-                bool retval = detail::lexical_cast(var, num);
-                if(!retval) {
-                    return std::string("Failed parsing number (") + var + ')';
-                }
-                if(num < 0 || num > 255) {
-                    return std::string("Each IP number must be between 0 and 255 ") + var;
-                }
-            }
-            return std::string();
-        };
-    }
+    IPV4Validator();
 };
 
 }  // namespace detail
 
 // Static is not needed here, because global const implies static.
 
 /// Check for existing file (returns error message if check fails)
@@ -3015,96 +3019,107 @@
 
 /// Check for an IP4 address
 const detail::IPV4Validator ValidIPV4;
 
 /// Validate the input as a particular type
 template <typename DesiredType> class TypeValidator : public Validator {
   public:
-    explicit TypeValidator(const std::string &validator_name) : Validator(validator_name) {
-        func_ = [](std::string &input_string) {
-            auto val = DesiredType();
-            if(!detail::lexical_cast(input_string, val)) {
-                return std::string("Failed parsing ") + input_string + " as a " + detail::type_name<DesiredType>();
-            }
-            return std::string();
-        };
-    }
+    explicit TypeValidator(const std::string &validator_name)
+        : Validator(validator_name, [](std::string &input_string) {
+              using CLI::detail::lexical_cast;
+              auto val = DesiredType();
+              if(!lexical_cast(input_string, val)) {
+                  return std::string("Failed parsing ") + input_string + " as a " + detail::type_name<DesiredType>();
+              }
+              return std::string();
+          }) {}
     TypeValidator() : TypeValidator(detail::type_name<DesiredType>()) {}
 };
 
 /// Check for a number
 const TypeValidator<double> Number("NUMBER");
 
+/// Modify a path if the file is a particular default location, can be used as Check or transform
+/// with the error return optionally disabled
+class FileOnDefaultPath : public Validator {
+  public:
+    explicit FileOnDefaultPath(std::string default_path, bool enableErrorReturn = true);
+};
+
 /// Produce a range (factory). Min and max are inclusive.
 class Range : public Validator {
   public:
     /// This produces a range with min and max inclusive.
     ///
     /// Note that the constructor is templated, but the struct is not, so C++17 is not
     /// needed to provide nice syntax for Range(a,b).
     template <typename T>
-    Range(T min, T max, const std::string &validator_name = std::string{}) : Validator(validator_name) {
+    Range(T min_val, T max_val, const std::string &validator_name = std::string{}) : Validator(validator_name) {
         if(validator_name.empty()) {
             std::stringstream out;
-            out << detail::type_name<T>() << " in [" << min << " - " << max << "]";
+            out << detail::type_name<T>() << " in [" << min_val << " - " << max_val << "]";
             description(out.str());
         }
 
-        func_ = [min, max](std::string &input) {
+        func_ = [min_val, max_val](std::string &input) {
+            using CLI::detail::lexical_cast;
             T val;
-            bool converted = detail::lexical_cast(input, val);
-            if((!converted) || (val < min || val > max))
-                return std::string("Value ") + input + " not in range " + std::to_string(min) + " to " +
-                       std::to_string(max);
-
-            return std::string();
+            bool converted = lexical_cast(input, val);
+            if((!converted) || (val < min_val || val > max_val)) {
+                std::stringstream out;
+                out << "Value " << input << " not in range [";
+                out << min_val << " - " << max_val << "]";
+                return out.str();
+            }
+            return std::string{};
         };
     }
 
     /// Range of one value is 0 to value
     template <typename T>
-    explicit Range(T max, const std::string &validator_name = std::string{})
-        : Range(static_cast<T>(0), max, validator_name) {}
+    explicit Range(T max_val, const std::string &validator_name = std::string{})
+        : Range(static_cast<T>(0), max_val, validator_name) {}
 };
 
 /// Check for a non negative number
-const Range NonNegativeNumber(std::numeric_limits<double>::max(), "NONNEGATIVE");
+const Range NonNegativeNumber((std::numeric_limits<double>::max)(), "NONNEGATIVE");
 
-/// Check for a positive valued number (val>0.0), min() her is the smallest positive number
-const Range PositiveNumber(std::numeric_limits<double>::min(), std::numeric_limits<double>::max(), "POSITIVE");
+/// Check for a positive valued number (val>0.0), <double>::min  here is the smallest positive number
+const Range PositiveNumber((std::numeric_limits<double>::min)(), (std::numeric_limits<double>::max)(), "POSITIVE");
 
 /// Produce a bounded range (factory). Min and max are inclusive.
 class Bound : public Validator {
   public:
     /// This bounds a value with min and max inclusive.
     ///
     /// Note that the constructor is templated, but the struct is not, so C++17 is not
     /// needed to provide nice syntax for Range(a,b).
-    template <typename T> Bound(T min, T max) {
+    template <typename T> Bound(T min_val, T max_val) {
         std::stringstream out;
-        out << detail::type_name<T>() << " bounded to [" << min << " - " << max << "]";
+        out << detail::type_name<T>() << " bounded to [" << min_val << " - " << max_val << "]";
         description(out.str());
 
-        func_ = [min, max](std::string &input) {
+        func_ = [min_val, max_val](std::string &input) {
+            using CLI::detail::lexical_cast;
             T val;
-            bool converted = detail::lexical_cast(input, val);
+            bool converted = lexical_cast(input, val);
             if(!converted) {
                 return std::string("Value ") + input + " could not be converted";
             }
-            if(val < min)
-                input = detail::to_string(min);
-            else if(val > max)
-                input = detail::to_string(max);
+            if(val < min_val)
+                input = detail::to_string(min_val);
+            else if(val > max_val)
+                input = detail::to_string(max_val);
 
             return std::string{};
         };
     }
 
     /// Range of one value is 0 to value
-    template <typename T> explicit Bound(T max) : Bound(static_cast<T>(0), max) {}
+    template <typename T> explicit Bound(T max_val) : Bound(static_cast<T>(0), max_val) {}
 };
 
 namespace detail {
 template <typename T,
           enable_if_t<is_copyable_ptr<typename std::remove_reference<T>::type>::value, detail::enabler> = detail::dummy>
 auto smart_deref(T value) -> decltype(*value) {
     return *value;
@@ -3202,17 +3217,16 @@
 // done in templates to prevent compiler warnings on negation of unsigned numbers
 
 /// Do a check for overflow on signed numbers
 template <typename T>
 inline typename std::enable_if<std::is_signed<T>::value, T>::type overflowCheck(const T &a, const T &b) {
     if((a > 0) == (b > 0)) {
         return ((std::numeric_limits<T>::max)() / (std::abs)(a) < (std::abs)(b));
-    } else {
-        return ((std::numeric_limits<T>::min)() / (std::abs)(a) > -(std::abs)(b));
     }
+    return ((std::numeric_limits<T>::min)() / (std::abs)(a) > -(std::abs)(b));
 }
 /// Do a check for overflow on unsigned numbers
 template <typename T>
 inline typename std::enable_if<!std::is_signed<T>::value, T>::type overflowCheck(const T &a, const T &b) {
     return ((std::numeric_limits<T>::max)() / a < b);
 }
 
@@ -3247,15 +3261,15 @@
 /// Verify items are in a set
 class IsMember : public Validator {
   public:
     using filter_fn_t = std::function<std::string(std::string)>;
 
     /// This allows in-place construction using an initializer list
     template <typename T, typename... Args>
-    IsMember(std::initializer_list<T> values, Args &&... args)
+    IsMember(std::initializer_list<T> values, Args &&...args)
         : IsMember(std::vector<T>(values), std::forward<Args>(args)...) {}
 
     /// This checks to see if an item is in a set (empty function)
     template <typename T> explicit IsMember(T &&set) : IsMember(std::forward<T>(set), nullptr) {}
 
     /// This checks to see if an item is in a set: pointer or copy version. You can pass in a function that will filter
     /// both sides of the comparison before computing the comparison.
@@ -3274,16 +3288,17 @@
 
         // This is the type name for help, it will take the current version of the set contents
         desc_function_ = [set]() { return detail::generate_set(detail::smart_deref(set)); };
 
         // This is the function that validates
         // It stores a copy of the set pointer-like, so shared_ptr will stay alive
         func_ = [set, filter_fn](std::string &input) {
+            using CLI::detail::lexical_cast;
             local_item_t b;
-            if(!detail::lexical_cast(input, b)) {
+            if(!lexical_cast(input, b)) {
                 throw ValidationError(input);  // name is added later
             }
             if(filter_fn) {
                 b = filter_fn(b);
             }
             auto res = detail::search(set, b, filter_fn);
             if(res.first) {
@@ -3299,15 +3314,15 @@
             // If you reach this point, the result was not found
             return input + " not in " + detail::generate_set(detail::smart_deref(set));
         };
     }
 
     /// You can pass in as many filter functions as you like, they nest (string only currently)
     template <typename T, typename... Args>
-    IsMember(T &&set, filter_fn_t filter_fn_1, filter_fn_t filter_fn_2, Args &&... other)
+    IsMember(T &&set, filter_fn_t filter_fn_1, filter_fn_t filter_fn_2, Args &&...other)
         : IsMember(
               std::forward<T>(set),
               [filter_fn_1, filter_fn_2](std::string a) { return filter_fn_2(filter_fn_1(a)); },
               other...) {}
 };
 
 /// definition of the default transformation object
@@ -3316,15 +3331,15 @@
 /// Translate named items to other or a value set
 class Transformer : public Validator {
   public:
     using filter_fn_t = std::function<std::string(std::string)>;
 
     /// This allows in-place construction
     template <typename... Args>
-    Transformer(std::initializer_list<std::pair<std::string, std::string>> values, Args &&... args)
+    Transformer(std::initializer_list<std::pair<std::string, std::string>> values, Args &&...args)
         : Transformer(TransformPairs<std::string>(values), std::forward<Args>(args)...) {}
 
     /// direct map of std::string to std::string
     template <typename T> explicit Transformer(T &&mapping) : Transformer(std::forward<T>(mapping), nullptr) {}
 
     /// This checks to see if an item is in a set: pointer or copy version. You can pass in a function that will filter
     /// both sides of the comparison before computing the comparison.
@@ -3342,16 +3357,17 @@
         // Make a local copy of the filter function, using a std::function if not one already
         std::function<local_item_t(local_item_t)> filter_fn = filter_function;
 
         // This is the type name for help, it will take the current version of the set contents
         desc_function_ = [mapping]() { return detail::generate_map(detail::smart_deref(mapping)); };
 
         func_ = [mapping, filter_fn](std::string &input) {
+            using CLI::detail::lexical_cast;
             local_item_t b;
-            if(!detail::lexical_cast(input, b)) {
+            if(!lexical_cast(input, b)) {
                 return std::string();
                 // there is no possible way we can match anything in the mapping if we can't convert so just return
             }
             if(filter_fn) {
                 b = filter_fn(b);
             }
             auto res = detail::search(mapping, b, filter_fn);
@@ -3360,29 +3376,29 @@
             }
             return std::string{};
         };
     }
 
     /// You can pass in as many filter functions as you like, they nest
     template <typename T, typename... Args>
-    Transformer(T &&mapping, filter_fn_t filter_fn_1, filter_fn_t filter_fn_2, Args &&... other)
+    Transformer(T &&mapping, filter_fn_t filter_fn_1, filter_fn_t filter_fn_2, Args &&...other)
         : Transformer(
               std::forward<T>(mapping),
               [filter_fn_1, filter_fn_2](std::string a) { return filter_fn_2(filter_fn_1(a)); },
               other...) {}
 };
 
 /// translate named items to other or a value set
 class CheckedTransformer : public Validator {
   public:
     using filter_fn_t = std::function<std::string(std::string)>;
 
     /// This allows in-place construction
     template <typename... Args>
-    CheckedTransformer(std::initializer_list<std::pair<std::string, std::string>> values, Args &&... args)
+    CheckedTransformer(std::initializer_list<std::pair<std::string, std::string>> values, Args &&...args)
         : CheckedTransformer(TransformPairs<std::string>(values), std::forward<Args>(args)...) {}
 
     /// direct map of std::string to std::string
     template <typename T> explicit CheckedTransformer(T mapping) : CheckedTransformer(std::move(mapping), nullptr) {}
 
     /// This checks to see if an item is in a set: pointer or copy version. You can pass in a function that will filter
     /// both sides of the comparison before computing the comparison.
@@ -3411,16 +3427,17 @@
             out.push_back('}');
             return out;
         };
 
         desc_function_ = tfunc;
 
         func_ = [mapping, tfunc, filter_fn](std::string &input) {
+            using CLI::detail::lexical_cast;
             local_item_t b;
-            bool converted = detail::lexical_cast(input, b);
+            bool converted = lexical_cast(input, b);
             if(converted) {
                 if(filter_fn) {
                     b = filter_fn(b);
                 }
                 auto res = detail::search(mapping, b, filter_fn);
                 if(res.first) {
                     input = detail::value_string(detail::pair_adaptor<element_t>::second(*res.second));
@@ -3436,15 +3453,15 @@
 
             return "Check " + input + " " + tfunc() + " FAILED";
         };
     }
 
     /// You can pass in as many filter functions as you like, they nest
     template <typename T, typename... Args>
-    CheckedTransformer(T &&mapping, filter_fn_t filter_fn_1, filter_fn_t filter_fn_2, Args &&... other)
+    CheckedTransformer(T &&mapping, filter_fn_t filter_fn_1, filter_fn_t filter_fn_2, Args &&...other)
         : CheckedTransformer(
               std::forward<T>(mapping),
               [filter_fn_1, filter_fn_2](std::string a) { return filter_fn_2(filter_fn_1(a)); },
               other...) {}
 };
 
 /// Helper function to allow ignore_case to be passed to IsMember or Transform
@@ -3490,15 +3507,15 @@
                               Options opts = DEFAULT,
                               const std::string &unit_name = "UNIT") {
         description(generate_description<Number>(unit_name, opts));
         validate_mapping(mapping, opts);
 
         // transform function
         func_ = [mapping, opts](std::string &input) -> std::string {
-            Number num;
+            Number num{};
 
             detail::rtrim(input);
             if(input.empty()) {
                 throw ValidationError("Input is empty");
             }
 
             // Find split position between number and prefix
@@ -3514,15 +3531,16 @@
             if(opts & UNIT_REQUIRED && unit.empty()) {
                 throw ValidationError("Missing mandatory unit");
             }
             if(opts & CASE_INSENSITIVE) {
                 unit = detail::to_lower(unit);
             }
             if(unit.empty()) {
-                if(!detail::lexical_cast(input, num)) {
+                using CLI::detail::lexical_cast;
+                if(!lexical_cast(input, num)) {
                     throw ValidationError(std::string("Value ") + input + " could not be converted to " +
                                           detail::type_name<Number>());
                 }
                 // No need to modify input if no unit passed
                 return {};
             }
 
@@ -3532,15 +3550,16 @@
                 throw ValidationError(unit +
                                       " unit not recognized. "
                                       "Allowed values: " +
                                       detail::generate_map(mapping, true));
             }
 
             if(!input.empty()) {
-                bool converted = detail::lexical_cast(input, num);
+                using CLI::detail::lexical_cast;
+                bool converted = lexical_cast(input, num);
                 if(!converted) {
                     throw ValidationError(std::string("Value ") + input + " could not be converted to " +
                                           detail::type_name<Number>());
                 }
                 // perform safe multiplication
                 bool ok = detail::checked_multiply(num, it->second);
                 if(!ok) {
@@ -3594,14 +3613,18 @@
         } else {
             out << '[' << name << ']';
         }
         return out.str();
     }
 };
 
+inline AsNumberWithUnit::Options operator|(const AsNumberWithUnit::Options &a, const AsNumberWithUnit::Options &b) {
+    return static_cast<AsNumberWithUnit::Options>(static_cast<int>(a) | static_cast<int>(b));
+}
+
 /// Converts a human-readable size string (with unit literal) to uin64_t size.
 /// Example:
 ///   "100" => 100
 ///   "1 b" => 100
 ///   "10Kb" => 10240 // you can configure this to be interpreted as kilobyte (*1000) or kibibyte (*1024)
 ///   "10 KB" => 10240
 ///   "10 kb" => 10240
@@ -3616,60 +3639,312 @@
     /// If kb_is_1000 is true,
     /// interpret 'kb', 'k' as 1000 and 'kib', 'ki' as 1024
     /// (same applies to higher order units as well).
     /// Otherwise, interpret all literals as factors of 1024.
     /// The first option is formally correct, but
     /// the second interpretation is more wide-spread
     /// (see https://en.wikipedia.org/wiki/Binary_prefix).
-    explicit AsSizeValue(bool kb_is_1000) : AsNumberWithUnit(get_mapping(kb_is_1000)) {
-        if(kb_is_1000) {
-            description("SIZE [b, kb(=1000b), kib(=1024b), ...]");
-        } else {
-            description("SIZE [b, kb(=1024b), ...]");
-        }
-    }
+    explicit AsSizeValue(bool kb_is_1000);
 
   private:
     /// Get <size unit, factor> mapping
-    static std::map<std::string, result_t> init_mapping(bool kb_is_1000) {
-        std::map<std::string, result_t> m;
-        result_t k_factor = kb_is_1000 ? 1000 : 1024;
-        result_t ki_factor = 1024;
-        result_t k = 1;
-        result_t ki = 1;
-        m["b"] = 1;
-        for(std::string p : {"k", "m", "g", "t", "p", "e"}) {
-            k *= k_factor;
-            ki *= ki_factor;
-            m[p] = k;
-            m[p + "b"] = k;
-            m[p + "i"] = ki;
-            m[p + "ib"] = ki;
-        }
-        return m;
-    }
+    static std::map<std::string, result_t> init_mapping(bool kb_is_1000);
 
     /// Cache calculated mapping
-    static std::map<std::string, result_t> get_mapping(bool kb_is_1000) {
-        if(kb_is_1000) {
-            static auto m = init_mapping(true);
-            return m;
-        } else {
-            static auto m = init_mapping(false);
-            return m;
-        }
-    }
+    static std::map<std::string, result_t> get_mapping(bool kb_is_1000);
 };
 
 namespace detail {
 /// Split a string into a program name and command line arguments
 /// the string is assumed to contain a file name followed by other arguments
 /// the return value contains is a pair with the first argument containing the program name and the second
 /// everything else.
-inline std::pair<std::string, std::string> split_program_name(std::string commandline) {
+CLI11_INLINE std::pair<std::string, std::string> split_program_name(std::string commandline);
+
+}  // namespace detail
+/// @}
+
+
+
+
+CLI11_INLINE std::string Validator::operator()(std::string &str) const {
+    std::string retstring;
+    if(active_) {
+        if(non_modifying_) {
+            std::string value = str;
+            retstring = func_(value);
+        } else {
+            retstring = func_(str);
+        }
+    }
+    return retstring;
+}
+
+CLI11_NODISCARD CLI11_INLINE Validator Validator::description(std::string validator_desc) const {
+    Validator newval(*this);
+    newval.desc_function_ = [validator_desc]() { return validator_desc; };
+    return newval;
+}
+
+CLI11_INLINE Validator Validator::operator&(const Validator &other) const {
+    Validator newval;
+
+    newval._merge_description(*this, other, " AND ");
+
+    // Give references (will make a copy in lambda function)
+    const std::function<std::string(std::string & filename)> &f1 = func_;
+    const std::function<std::string(std::string & filename)> &f2 = other.func_;
+
+    newval.func_ = [f1, f2](std::string &input) {
+        std::string s1 = f1(input);
+        std::string s2 = f2(input);
+        if(!s1.empty() && !s2.empty())
+            return std::string("(") + s1 + ") AND (" + s2 + ")";
+        return s1 + s2;
+    };
+
+    newval.active_ = active_ && other.active_;
+    newval.application_index_ = application_index_;
+    return newval;
+}
+
+CLI11_INLINE Validator Validator::operator|(const Validator &other) const {
+    Validator newval;
+
+    newval._merge_description(*this, other, " OR ");
+
+    // Give references (will make a copy in lambda function)
+    const std::function<std::string(std::string &)> &f1 = func_;
+    const std::function<std::string(std::string &)> &f2 = other.func_;
+
+    newval.func_ = [f1, f2](std::string &input) {
+        std::string s1 = f1(input);
+        std::string s2 = f2(input);
+        if(s1.empty() || s2.empty())
+            return std::string();
+
+        return std::string("(") + s1 + ") OR (" + s2 + ")";
+    };
+    newval.active_ = active_ && other.active_;
+    newval.application_index_ = application_index_;
+    return newval;
+}
+
+CLI11_INLINE Validator Validator::operator!() const {
+    Validator newval;
+    const std::function<std::string()> &dfunc1 = desc_function_;
+    newval.desc_function_ = [dfunc1]() {
+        auto str = dfunc1();
+        return (!str.empty()) ? std::string("NOT ") + str : std::string{};
+    };
+    // Give references (will make a copy in lambda function)
+    const std::function<std::string(std::string & res)> &f1 = func_;
+
+    newval.func_ = [f1, dfunc1](std::string &test) -> std::string {
+        std::string s1 = f1(test);
+        if(s1.empty()) {
+            return std::string("check ") + dfunc1() + " succeeded improperly";
+        }
+        return std::string{};
+    };
+    newval.active_ = active_;
+    newval.application_index_ = application_index_;
+    return newval;
+}
+
+CLI11_INLINE void
+Validator::_merge_description(const Validator &val1, const Validator &val2, const std::string &merger) {
+
+    const std::function<std::string()> &dfunc1 = val1.desc_function_;
+    const std::function<std::string()> &dfunc2 = val2.desc_function_;
+
+    desc_function_ = [=]() {
+        std::string f1 = dfunc1();
+        std::string f2 = dfunc2();
+        if((f1.empty()) || (f2.empty())) {
+            return f1 + f2;
+        }
+        return std::string(1, '(') + f1 + ')' + merger + '(' + f2 + ')';
+    };
+}
+
+namespace detail {
+
+#if defined CLI11_HAS_FILESYSTEM && CLI11_HAS_FILESYSTEM > 0
+CLI11_INLINE path_type check_path(const char *file) noexcept {
+    std::error_code ec;
+    auto stat = std::filesystem::status(file, ec);
+    if(ec) {
+        return path_type::nonexistent;
+    }
+    switch(stat.type()) {
+    case std::filesystem::file_type::none:  // LCOV_EXCL_LINE
+    case std::filesystem::file_type::not_found:
+        return path_type::nonexistent;
+    case std::filesystem::file_type::directory:
+        return path_type::directory;
+    case std::filesystem::file_type::symlink:
+    case std::filesystem::file_type::block:
+    case std::filesystem::file_type::character:
+    case std::filesystem::file_type::fifo:
+    case std::filesystem::file_type::socket:
+    case std::filesystem::file_type::regular:
+    case std::filesystem::file_type::unknown:
+    default:
+        return path_type::file;
+    }
+}
+#else
+CLI11_INLINE path_type check_path(const char *file) noexcept {
+#if defined(_MSC_VER)
+    struct __stat64 buffer;
+    if(_stat64(file, &buffer) == 0) {
+        return ((buffer.st_mode & S_IFDIR) != 0) ? path_type::directory : path_type::file;
+    }
+#else
+    struct stat buffer;
+    if(stat(file, &buffer) == 0) {
+        return ((buffer.st_mode & S_IFDIR) != 0) ? path_type::directory : path_type::file;
+    }
+#endif
+    return path_type::nonexistent;
+}
+#endif
+
+CLI11_INLINE ExistingFileValidator::ExistingFileValidator() : Validator("FILE") {
+    func_ = [](std::string &filename) {
+        auto path_result = check_path(filename.c_str());
+        if(path_result == path_type::nonexistent) {
+            return "File does not exist: " + filename;
+        }
+        if(path_result == path_type::directory) {
+            return "File is actually a directory: " + filename;
+        }
+        return std::string();
+    };
+}
+
+CLI11_INLINE ExistingDirectoryValidator::ExistingDirectoryValidator() : Validator("DIR") {
+    func_ = [](std::string &filename) {
+        auto path_result = check_path(filename.c_str());
+        if(path_result == path_type::nonexistent) {
+            return "Directory does not exist: " + filename;
+        }
+        if(path_result == path_type::file) {
+            return "Directory is actually a file: " + filename;
+        }
+        return std::string();
+    };
+}
+
+CLI11_INLINE ExistingPathValidator::ExistingPathValidator() : Validator("PATH(existing)") {
+    func_ = [](std::string &filename) {
+        auto path_result = check_path(filename.c_str());
+        if(path_result == path_type::nonexistent) {
+            return "Path does not exist: " + filename;
+        }
+        return std::string();
+    };
+}
+
+CLI11_INLINE NonexistentPathValidator::NonexistentPathValidator() : Validator("PATH(non-existing)") {
+    func_ = [](std::string &filename) {
+        auto path_result = check_path(filename.c_str());
+        if(path_result != path_type::nonexistent) {
+            return "Path already exists: " + filename;
+        }
+        return std::string();
+    };
+}
+
+CLI11_INLINE IPV4Validator::IPV4Validator() : Validator("IPV4") {
+    func_ = [](std::string &ip_addr) {
+        auto result = CLI::detail::split(ip_addr, '.');
+        if(result.size() != 4) {
+            return std::string("Invalid IPV4 address must have four parts (") + ip_addr + ')';
+        }
+        int num = 0;
+        for(const auto &var : result) {
+            using CLI::detail::lexical_cast;
+            bool retval = lexical_cast(var, num);
+            if(!retval) {
+                return std::string("Failed parsing number (") + var + ')';
+            }
+            if(num < 0 || num > 255) {
+                return std::string("Each IP number must be between 0 and 255 ") + var;
+            }
+        }
+        return std::string();
+    };
+}
+
+}  // namespace detail
+
+CLI11_INLINE FileOnDefaultPath::FileOnDefaultPath(std::string default_path, bool enableErrorReturn)
+    : Validator("FILE") {
+    func_ = [default_path, enableErrorReturn](std::string &filename) {
+        auto path_result = detail::check_path(filename.c_str());
+        if(path_result == detail::path_type::nonexistent) {
+            std::string test_file_path = default_path;
+            if(default_path.back() != '/' && default_path.back() != '\\') {
+                // Add folder separator
+                test_file_path += '/';
+            }
+            test_file_path.append(filename);
+            path_result = detail::check_path(test_file_path.c_str());
+            if(path_result == detail::path_type::file) {
+                filename = test_file_path;
+            } else {
+                if(enableErrorReturn) {
+                    return "File does not exist: " + filename;
+                }
+            }
+        }
+        return std::string{};
+    };
+}
+
+CLI11_INLINE AsSizeValue::AsSizeValue(bool kb_is_1000) : AsNumberWithUnit(get_mapping(kb_is_1000)) {
+    if(kb_is_1000) {
+        description("SIZE [b, kb(=1000b), kib(=1024b), ...]");
+    } else {
+        description("SIZE [b, kb(=1024b), ...]");
+    }
+}
+
+CLI11_INLINE std::map<std::string, AsSizeValue::result_t> AsSizeValue::init_mapping(bool kb_is_1000) {
+    std::map<std::string, result_t> m;
+    result_t k_factor = kb_is_1000 ? 1000 : 1024;
+    result_t ki_factor = 1024;
+    result_t k = 1;
+    result_t ki = 1;
+    m["b"] = 1;
+    for(std::string p : {"k", "m", "g", "t", "p", "e"}) {
+        k *= k_factor;
+        ki *= ki_factor;
+        m[p] = k;
+        m[p + "b"] = k;
+        m[p + "i"] = ki;
+        m[p + "ib"] = ki;
+    }
+    return m;
+}
+
+CLI11_INLINE std::map<std::string, AsSizeValue::result_t> AsSizeValue::get_mapping(bool kb_is_1000) {
+    if(kb_is_1000) {
+        static auto m = init_mapping(true);
+        return m;
+    }
+    static auto m = init_mapping(false);
+    return m;
+}
+
+namespace detail {
+
+CLI11_INLINE std::pair<std::string, std::string> split_program_name(std::string commandline) {
     // try to determine the programName
     std::pair<std::string, std::string> vals;
     trim(commandline);
     auto esp = commandline.find_first_of(' ', 1);
     while(detail::check_path(commandline.substr(0, esp).c_str()) != path_type::file) {
         esp = commandline.find_first_of(' ', esp + 1);
         if(esp == std::string::npos) {
@@ -3684,15 +3959,14 @@
                     embeddedQuote = true;
                 }
                 if(end != std::string::npos) {
                     vals.first = commandline.substr(1, end - 1);
                     esp = end + 1;
                     if(embeddedQuote) {
                         vals.first = find_and_replace(vals.first, std::string("\\") + keyChar, std::string(1, keyChar));
-                        embeddedQuote = false;
                     }
                 } else {
                     esp = commandline.find_first_of(' ', 1);
                 }
             } else {
                 esp = commandline.find_first_of(' ', 1);
             }
@@ -3702,15 +3976,15 @@
     }
     if(vals.first.empty()) {
         vals.first = commandline.substr(0, esp);
         rtrim(vals.first);
     }
 
     // strip the program name
-    vals.second = (esp != std::string::npos) ? commandline.substr(esp + 1) : std::string{};
+    vals.second = (esp < commandline.length() - 1) ? commandline.substr(esp + 1) : std::string{};
     ltrim(vals.second);
     return vals;
 }
 
 }  // namespace detail
 /// @}
 
@@ -3751,14 +4025,16 @@
     /// @name Basic
     ///@{
 
   public:
     FormatterBase() = default;
     FormatterBase(const FormatterBase &) = default;
     FormatterBase(FormatterBase &&) = default;
+    FormatterBase &operator=(const FormatterBase &) = default;
+    FormatterBase &operator=(FormatterBase &&) = default;
 
     /// Adding a destructor in this form to work around bug in GCC 4.7
     virtual ~FormatterBase() noexcept {}  // NOLINT(modernize-use-equals-default)
 
     /// This is the key method that puts together help
     virtual std::string make_help(const App *, std::string, AppFormatMode) const = 0;
 
@@ -3773,23 +4049,22 @@
     void column_width(std::size_t val) { column_width_ = val; }
 
     ///@}
     /// @name Getters
     ///@{
 
     /// Get the current value of a name (REQUIRED, etc.)
-    std::string get_label(std::string key) const {
+    CLI11_NODISCARD std::string get_label(std::string key) const {
         if(labels_.find(key) == labels_.end())
             return key;
-        else
-            return labels_.at(key);
+        return labels_.at(key);
     }
 
     /// Get the current column width
-    std::size_t get_column_width() const { return column_width_; }
+    CLI11_NODISCARD std::size_t get_column_width() const { return column_width_; }
 
     ///@}
 };
 
 /// This is a specialty override for lambda functions
 class FormatterLambda final : public FormatterBase {
     using funct_t = std::function<std::string(const App *, std::string, AppFormatMode)>;
@@ -3813,21 +4088,24 @@
 /// This is the default Formatter for CLI11. It pretty prints help output, and is broken into quite a few
 /// overridable methods, to be highly customizable with minimal effort.
 class Formatter : public FormatterBase {
   public:
     Formatter() = default;
     Formatter(const Formatter &) = default;
     Formatter(Formatter &&) = default;
+    Formatter &operator=(const Formatter &) = default;
+    Formatter &operator=(Formatter &&) = default;
 
     /// @name Overridables
     ///@{
 
     /// This prints out a group of options with title
     ///
-    virtual std::string make_group(std::string group, bool is_positional, std::vector<const Option *> opts) const;
+    CLI11_NODISCARD virtual std::string
+    make_group(std::string group, bool is_positional, std::vector<const Option *> opts) const;
 
     /// This prints out just the positionals "group"
     virtual std::string make_positionals(const App *app) const;
 
     /// This prints out all the groups of options
     std::string make_groups(const App *app, AppFormatMode mode) const;
 
@@ -3892,15 +4170,16 @@
 using Option_p = std::unique_ptr<Option>;
 /// Enumeration of the multiOption Policy selection
 enum class MultiOptionPolicy : char {
     Throw,      //!< Throw an error if any extra arguments were given
     TakeLast,   //!< take only the last Expected number of arguments
     TakeFirst,  //!< take only the first Expected number of arguments
     Join,       //!< merge all the arguments together into a single string via the delimiter character default('\n')
-    TakeAll     //!< just get all the passed argument regardless
+    TakeAll,    //!< just get all the passed argument regardless
+    Sum         //!< sum all the arguments together if numerical or concatenate directly without delimiter
 };
 
 /// This is the CRTP base class for Option and OptionDefaults. It was designed this way
 /// to share parts of the class; an OptionDefaults can copy to an Option.
 template <typename CRTP> class OptionBase {
     friend App;
 
@@ -3929,31 +4208,24 @@
     /// Automatically capture default value
     bool always_capture_default_{false};
 
     /// Policy for handling multiple arguments beyond the expected Max
     MultiOptionPolicy multi_option_policy_{MultiOptionPolicy::Throw};
 
     /// Copy the contents to another similar class (one based on OptionBase)
-    template <typename T> void copy_to(T *other) const {
-        other->group(group_);
-        other->required(required_);
-        other->ignore_case(ignore_case_);
-        other->ignore_underscore(ignore_underscore_);
-        other->configurable(configurable_);
-        other->disable_flag_override(disable_flag_override_);
-        other->delimiter(delimiter_);
-        other->always_capture_default(always_capture_default_);
-        other->multi_option_policy(multi_option_policy_);
-    }
+    template <typename T> void copy_to(T *other) const;
 
   public:
     // setters
 
     /// Changes the group membership
     CRTP *group(const std::string &name) {
+        if(!detail::valid_alias_name_string(name)) {
+            throw IncorrectConstruction("Group names may not contain newlines or null characters");
+        }
         group_ = name;
         return static_cast<CRTP *>(this);
     }
 
     /// Set the option as required
     CRTP *required(bool value = true) {
         required_ = value;
@@ -3967,66 +4239,66 @@
         always_capture_default_ = value;
         return static_cast<CRTP *>(this);
     }
 
     // Getters
 
     /// Get the group of this option
-    const std::string &get_group() const { return group_; }
+    CLI11_NODISCARD const std::string &get_group() const { return group_; }
 
     /// True if this is a required option
-    bool get_required() const { return required_; }
+    CLI11_NODISCARD bool get_required() const { return required_; }
 
     /// The status of ignore case
-    bool get_ignore_case() const { return ignore_case_; }
+    CLI11_NODISCARD bool get_ignore_case() const { return ignore_case_; }
 
     /// The status of ignore_underscore
-    bool get_ignore_underscore() const { return ignore_underscore_; }
+    CLI11_NODISCARD bool get_ignore_underscore() const { return ignore_underscore_; }
 
     /// The status of configurable
-    bool get_configurable() const { return configurable_; }
+    CLI11_NODISCARD bool get_configurable() const { return configurable_; }
 
     /// The status of configurable
-    bool get_disable_flag_override() const { return disable_flag_override_; }
+    CLI11_NODISCARD bool get_disable_flag_override() const { return disable_flag_override_; }
 
     /// Get the current delimiter char
-    char get_delimiter() const { return delimiter_; }
+    CLI11_NODISCARD char get_delimiter() const { return delimiter_; }
 
     /// Return true if this will automatically capture the default value for help printing
-    bool get_always_capture_default() const { return always_capture_default_; }
+    CLI11_NODISCARD bool get_always_capture_default() const { return always_capture_default_; }
 
     /// The status of the multi option policy
-    MultiOptionPolicy get_multi_option_policy() const { return multi_option_policy_; }
+    CLI11_NODISCARD MultiOptionPolicy get_multi_option_policy() const { return multi_option_policy_; }
 
     // Shortcuts for multi option policy
 
     /// Set the multi option policy to take last
     CRTP *take_last() {
-        auto self = static_cast<CRTP *>(this);
+        auto *self = static_cast<CRTP *>(this);
         self->multi_option_policy(MultiOptionPolicy::TakeLast);
         return self;
     }
 
     /// Set the multi option policy to take last
     CRTP *take_first() {
-        auto self = static_cast<CRTP *>(this);
+        auto *self = static_cast<CRTP *>(this);
         self->multi_option_policy(MultiOptionPolicy::TakeFirst);
         return self;
     }
 
     /// Set the multi option policy to take all arguments
     CRTP *take_all() {
         auto self = static_cast<CRTP *>(this);
         self->multi_option_policy(MultiOptionPolicy::TakeAll);
         return self;
     }
 
     /// Set the multi option policy to join
     CRTP *join() {
-        auto self = static_cast<CRTP *>(this);
+        auto *self = static_cast<CRTP *>(this);
         self->multi_option_policy(MultiOptionPolicy::Join);
         return self;
     }
 
     /// Set the multi option policy to join with a specific delimiter
     CRTP *join(char delim) {
         auto self = static_cast<CRTP *>(this);
@@ -4189,14 +4461,18 @@
     bool allow_extra_args_{false};
     /// Specify that the option should act like a flag vs regular option
     bool flag_like_{false};
     /// Control option to run the callback to set the default
     bool run_callback_for_default_{false};
     /// flag indicating a separator needs to be injected after each argument call
     bool inject_separator_{false};
+    /// flag indicating that the option should trigger the validation and callback chain on each result when loaded
+    bool trigger_on_result_{false};
+    /// flag indicating that the option should force the callback regardless if any results present
+    bool force_callback_{false};
     ///@}
 
     /// Making an option by hand is not defined, it must be made by the App class
     Option(std::string option_name, std::string option_description, callback_t callback, App *parent)
         : description_(std::move(option_description)), parent_(parent), callback_(std::move(callback)) {
         std::tie(snames_, lnames_, pname_) = detail::get_names(detail::split_names(option_name));
     }
@@ -4205,164 +4481,95 @@
     /// @name Basic
     ///@{
 
     Option(const Option &) = delete;
     Option &operator=(const Option &) = delete;
 
     /// Count the total number of times an option was passed
-    std::size_t count() const { return results_.size(); }
+    CLI11_NODISCARD std::size_t count() const { return results_.size(); }
 
     /// True if the option was not passed
-    bool empty() const { return results_.empty(); }
+    CLI11_NODISCARD bool empty() const { return results_.empty(); }
 
-    /// This class is true if option is passed.
-    explicit operator bool() const { return !empty(); }
+    /// This bool operator returns true if any arguments were passed or the option callback is forced
+    explicit operator bool() const { return !empty() || force_callback_; }
 
     /// Clear the parsed results (mostly for testing)
     void clear() {
         results_.clear();
         current_option_state_ = option_state::parsing;
     }
 
     ///@}
     /// @name Setting options
     ///@{
 
     /// Set the number of expected arguments
-    Option *expected(int value) {
-        if(value < 0) {
-            expected_min_ = -value;
-            if(expected_max_ < expected_min_) {
-                expected_max_ = expected_min_;
-            }
-            allow_extra_args_ = true;
-            flag_like_ = false;
-        } else if(value == detail::expected_max_vector_size) {
-            expected_min_ = 1;
-            expected_max_ = detail::expected_max_vector_size;
-            allow_extra_args_ = true;
-            flag_like_ = false;
-        } else {
-            expected_min_ = value;
-            expected_max_ = value;
-            flag_like_ = (expected_min_ == 0);
-        }
-        return this;
-    }
+    Option *expected(int value);
 
     /// Set the range of expected arguments
-    Option *expected(int value_min, int value_max) {
-        if(value_min < 0) {
-            value_min = -value_min;
-        }
-
-        if(value_max < 0) {
-            value_max = detail::expected_max_vector_size;
-        }
-        if(value_max < value_min) {
-            expected_min_ = value_max;
-            expected_max_ = value_min;
-        } else {
-            expected_max_ = value_max;
-            expected_min_ = value_min;
-        }
+    Option *expected(int value_min, int value_max);
 
-        return this;
-    }
     /// Set the value of allow_extra_args which allows extra value arguments on the flag or option to be included
     /// with each instance
     Option *allow_extra_args(bool value = true) {
         allow_extra_args_ = value;
         return this;
     }
     /// Get the current value of allow extra args
-    bool get_allow_extra_args() const { return allow_extra_args_; }
+    CLI11_NODISCARD bool get_allow_extra_args() const { return allow_extra_args_; }
+    /// Set the value of trigger_on_parse which specifies that the option callback should be triggered on every parse
+    Option *trigger_on_parse(bool value = true) {
+        trigger_on_result_ = value;
+        return this;
+    }
+    /// The status of trigger on parse
+    CLI11_NODISCARD bool get_trigger_on_parse() const { return trigger_on_result_; }
+
+    /// Set the value of force_callback
+    Option *force_callback(bool value = true) {
+        force_callback_ = value;
+        return this;
+    }
+    /// The status of force_callback
+    CLI11_NODISCARD bool get_force_callback() const { return force_callback_; }
 
     /// Set the value of run_callback_for_default which controls whether the callback function should be called to set
     /// the default This is controlled automatically but could be manipulated by the user.
     Option *run_callback_for_default(bool value = true) {
         run_callback_for_default_ = value;
         return this;
     }
     /// Get the current value of run_callback_for_default
-    bool get_run_callback_for_default() const { return run_callback_for_default_; }
+    CLI11_NODISCARD bool get_run_callback_for_default() const { return run_callback_for_default_; }
 
     /// Adds a Validator with a built in type name
-    Option *check(Validator validator, const std::string &validator_name = "") {
-        validator.non_modifying();
-        validators_.push_back(std::move(validator));
-        if(!validator_name.empty())
-            validators_.back().name(validator_name);
-        return this;
-    }
+    Option *check(Validator validator, const std::string &validator_name = "");
 
     /// Adds a Validator. Takes a const string& and returns an error message (empty if conversion/check is okay).
     Option *check(std::function<std::string(const std::string &)> Validator,
                   std::string Validator_description = "",
-                  std::string Validator_name = "") {
-        validators_.emplace_back(Validator, std::move(Validator_description), std::move(Validator_name));
-        validators_.back().non_modifying();
-        return this;
-    }
+                  std::string Validator_name = "");
 
     /// Adds a transforming Validator with a built in type name
-    Option *transform(Validator Validator, const std::string &Validator_name = "") {
-        validators_.insert(validators_.begin(), std::move(Validator));
-        if(!Validator_name.empty())
-            validators_.front().name(Validator_name);
-        return this;
-    }
+    Option *transform(Validator Validator, const std::string &Validator_name = "");
 
     /// Adds a Validator-like function that can change result
     Option *transform(const std::function<std::string(std::string)> &func,
                       std::string transform_description = "",
-                      std::string transform_name = "") {
-        validators_.insert(validators_.begin(),
-                           Validator(
-                               [func](std::string &val) {
-                                   val = func(val);
-                                   return std::string{};
-                               },
-                               std::move(transform_description),
-                               std::move(transform_name)));
-
-        return this;
-    }
+                      std::string transform_name = "");
 
     /// Adds a user supplied function to run on each item passed in (communicate though lambda capture)
-    Option *each(const std::function<void(std::string)> &func) {
-        validators_.emplace_back(
-            [func](std::string &inout) {
-                func(inout);
-                return std::string{};
-            },
-            std::string{});
-        return this;
-    }
+    Option *each(const std::function<void(std::string)> &func);
+
     /// Get a named Validator
-    Validator *get_validator(const std::string &Validator_name = "") {
-        for(auto &Validator : validators_) {
-            if(Validator_name == Validator.get_name()) {
-                return &Validator;
-            }
-        }
-        if((Validator_name.empty()) && (!validators_.empty())) {
-            return &(validators_.front());
-        }
-        throw OptionNotFound(std::string{"Validator "} + Validator_name + " Not Found");
-    }
+    Validator *get_validator(const std::string &Validator_name = "");
 
     /// Get a Validator by index NOTE: this may not be the order of definition
-    Validator *get_validator(int index) {
-        // This is an signed int so that it is not equivalent to a pointer.
-        if(index >= 0 && index < static_cast<int>(validators_.size())) {
-            return &(validators_[static_cast<decltype(validators_)::size_type>(index)]);
-        }
-        throw OptionNotFound("Validator index is not valid");
-    }
+    Validator *get_validator(int index);
 
     /// Sets required options
     Option *needs(Option *opt) {
         if(opt != this) {
             needs_.insert(opt);
         }
         return this;
@@ -4376,43 +4583,22 @@
         }
         return needs(opt);
     }
 
     /// Any number supported, any mix of string and Opt
     template <typename A, typename B, typename... ARG> Option *needs(A opt, B opt1, ARG... args) {
         needs(opt);
-        return needs(opt1, args...);
+        return needs(opt1, args...);  // NOLINT(readability-suspicious-call-argument)
     }
 
     /// Remove needs link from an option. Returns true if the option really was in the needs list.
-    bool remove_needs(Option *opt) {
-        auto iterator = std::find(std::begin(needs_), std::end(needs_), opt);
-
-        if(iterator == std::end(needs_)) {
-            return false;
-        }
-        needs_.erase(iterator);
-        return true;
-    }
+    bool remove_needs(Option *opt);
 
     /// Sets excluded options
-    Option *excludes(Option *opt) {
-        if(opt == this) {
-            throw(IncorrectConstruction("and option cannot exclude itself"));
-        }
-        excludes_.insert(opt);
-
-        // Help text should be symmetric - excluding a should exclude b
-        opt->excludes_.insert(this);
-
-        // Ignoring the insert return value, excluding twice is now allowed.
-        // (Mostly to allow both directions to be excluded by user, even though the library does it for you.)
-
-        return this;
-    }
+    Option *excludes(Option *opt);
 
     /// Can find a string if needed
     template <typename T = App> Option *excludes(std::string opt_name) {
         auto opt = static_cast<T *>(parent_)->get_option_no_throw(opt_name);
         if(opt == nullptr) {
             throw IncorrectConstruction::MissingOption(opt_name);
         }
@@ -4422,450 +4608,205 @@
     /// Any number supported, any mix of string and Opt
     template <typename A, typename B, typename... ARG> Option *excludes(A opt, B opt1, ARG... args) {
         excludes(opt);
         return excludes(opt1, args...);
     }
 
     /// Remove needs link from an option. Returns true if the option really was in the needs list.
-    bool remove_excludes(Option *opt) {
-        auto iterator = std::find(std::begin(excludes_), std::end(excludes_), opt);
-
-        if(iterator == std::end(excludes_)) {
-            return false;
-        }
-        excludes_.erase(iterator);
-        return true;
-    }
+    bool remove_excludes(Option *opt);
 
     /// Sets environment variable to read if no option given
     Option *envname(std::string name) {
         envname_ = std::move(name);
         return this;
     }
 
     /// Ignore case
     ///
     /// The template hides the fact that we don't have the definition of App yet.
     /// You are never expected to add an argument to the template here.
-    template <typename T = App> Option *ignore_case(bool value = true) {
-        if(!ignore_case_ && value) {
-            ignore_case_ = value;
-            auto *parent = static_cast<T *>(parent_);
-            for(const Option_p &opt : parent->options_) {
-                if(opt.get() == this) {
-                    continue;
-                }
-                auto &omatch = opt->matching_name(*this);
-                if(!omatch.empty()) {
-                    ignore_case_ = false;
-                    throw OptionAlreadyAdded("adding ignore case caused a name conflict with " + omatch);
-                }
-            }
-        } else {
-            ignore_case_ = value;
-        }
-        return this;
-    }
+    template <typename T = App> Option *ignore_case(bool value = true);
 
     /// Ignore underscores in the option names
     ///
     /// The template hides the fact that we don't have the definition of App yet.
     /// You are never expected to add an argument to the template here.
-    template <typename T = App> Option *ignore_underscore(bool value = true) {
-
-        if(!ignore_underscore_ && value) {
-            ignore_underscore_ = value;
-            auto *parent = static_cast<T *>(parent_);
-            for(const Option_p &opt : parent->options_) {
-                if(opt.get() == this) {
-                    continue;
-                }
-                auto &omatch = opt->matching_name(*this);
-                if(!omatch.empty()) {
-                    ignore_underscore_ = false;
-                    throw OptionAlreadyAdded("adding ignore underscore caused a name conflict with " + omatch);
-                }
-            }
-        } else {
-            ignore_underscore_ = value;
-        }
-        return this;
-    }
+    template <typename T = App> Option *ignore_underscore(bool value = true);
 
     /// Take the last argument if given multiple times (or another policy)
-    Option *multi_option_policy(MultiOptionPolicy value = MultiOptionPolicy::Throw) {
-        if(value != multi_option_policy_) {
-            if(multi_option_policy_ == MultiOptionPolicy::Throw && expected_max_ == detail::expected_max_vector_size &&
-               expected_min_ > 1) {  // this bizarre condition is to maintain backwards compatibility
-                                     // with the previous behavior of expected_ with vectors
-                expected_max_ = expected_min_;
-            }
-            multi_option_policy_ = value;
-            current_option_state_ = option_state::parsing;
-        }
-        return this;
-    }
+    Option *multi_option_policy(MultiOptionPolicy value = MultiOptionPolicy::Throw);
 
     /// Disable flag overrides values, e.g. --flag=<value> is not allowed
     Option *disable_flag_override(bool value = true) {
         disable_flag_override_ = value;
         return this;
     }
     ///@}
     /// @name Accessors
     ///@{
 
     /// The number of arguments the option expects
-    int get_type_size() const { return type_size_min_; }
+    CLI11_NODISCARD int get_type_size() const { return type_size_min_; }
 
     /// The minimum number of arguments the option expects
-    int get_type_size_min() const { return type_size_min_; }
+    CLI11_NODISCARD int get_type_size_min() const { return type_size_min_; }
     /// The maximum number of arguments the option expects
-    int get_type_size_max() const { return type_size_max_; }
+    CLI11_NODISCARD int get_type_size_max() const { return type_size_max_; }
 
-    /// The number of arguments the option expects
-    int get_inject_separator() const { return inject_separator_; }
+    /// Return the inject_separator flag
+    CLI11_NODISCARD bool get_inject_separator() const { return inject_separator_; }
 
     /// The environment variable associated to this value
-    std::string get_envname() const { return envname_; }
+    CLI11_NODISCARD std::string get_envname() const { return envname_; }
 
     /// The set of options needed
-    std::set<Option *> get_needs() const { return needs_; }
+    CLI11_NODISCARD std::set<Option *> get_needs() const { return needs_; }
 
     /// The set of options excluded
-    std::set<Option *> get_excludes() const { return excludes_; }
+    CLI11_NODISCARD std::set<Option *> get_excludes() const { return excludes_; }
 
     /// The default value (for help printing)
-    std::string get_default_str() const { return default_str_; }
+    CLI11_NODISCARD std::string get_default_str() const { return default_str_; }
 
     /// Get the callback function
-    callback_t get_callback() const { return callback_; }
+    CLI11_NODISCARD callback_t get_callback() const { return callback_; }
 
     /// Get the long names
-    const std::vector<std::string> &get_lnames() const { return lnames_; }
+    CLI11_NODISCARD const std::vector<std::string> &get_lnames() const { return lnames_; }
 
     /// Get the short names
-    const std::vector<std::string> &get_snames() const { return snames_; }
+    CLI11_NODISCARD const std::vector<std::string> &get_snames() const { return snames_; }
 
     /// Get the flag names with specified default values
-    const std::vector<std::string> &get_fnames() const { return fnames_; }
+    CLI11_NODISCARD const std::vector<std::string> &get_fnames() const { return fnames_; }
     /// Get a single name for the option, first of lname, pname, sname, envname
-    const std::string &get_single_name() const {
+    CLI11_NODISCARD const std::string &get_single_name() const {
         if(!lnames_.empty()) {
             return lnames_[0];
         }
         if(!pname_.empty()) {
             return pname_;
         }
         if(!snames_.empty()) {
             return snames_[0];
         }
         return envname_;
     }
     /// The number of times the option expects to be included
-    int get_expected() const { return expected_min_; }
+    CLI11_NODISCARD int get_expected() const { return expected_min_; }
 
     /// The number of times the option expects to be included
-    int get_expected_min() const { return expected_min_; }
+    CLI11_NODISCARD int get_expected_min() const { return expected_min_; }
     /// The max number of times the option expects to be included
-    int get_expected_max() const { return expected_max_; }
+    CLI11_NODISCARD int get_expected_max() const { return expected_max_; }
 
     /// The total min number of expected  string values to be used
-    int get_items_expected_min() const { return type_size_min_ * expected_min_; }
+    CLI11_NODISCARD int get_items_expected_min() const { return type_size_min_ * expected_min_; }
 
     /// Get the maximum number of items expected to be returned and used for the callback
-    int get_items_expected_max() const {
+    CLI11_NODISCARD int get_items_expected_max() const {
         int t = type_size_max_;
         return detail::checked_multiply(t, expected_max_) ? t : detail::expected_max_vector_size;
     }
     /// The total min number of expected  string values to be used
-    int get_items_expected() const { return get_items_expected_min(); }
+    CLI11_NODISCARD int get_items_expected() const { return get_items_expected_min(); }
 
     /// True if the argument can be given directly
-    bool get_positional() const { return pname_.length() > 0; }
+    CLI11_NODISCARD bool get_positional() const { return pname_.length() > 0; }
 
     /// True if option has at least one non-positional name
-    bool nonpositional() const { return (snames_.size() + lnames_.size()) > 0; }
+    CLI11_NODISCARD bool nonpositional() const { return (snames_.size() + lnames_.size()) > 0; }
 
     /// True if option has description
-    bool has_description() const { return description_.length() > 0; }
+    CLI11_NODISCARD bool has_description() const { return description_.length() > 0; }
 
     /// Get the description
-    const std::string &get_description() const { return description_; }
+    CLI11_NODISCARD const std::string &get_description() const { return description_; }
 
     /// Set the description
     Option *description(std::string option_description) {
         description_ = std::move(option_description);
         return this;
     }
 
     Option *option_text(std::string text) {
         option_text_ = std::move(text);
         return this;
     }
 
-    const std::string &get_option_text() const { return option_text_; }
+    CLI11_NODISCARD const std::string &get_option_text() const { return option_text_; }
 
     ///@}
     /// @name Help tools
     ///@{
 
     /// \brief Gets a comma separated list of names.
     /// Will include / prefer the positional name if positional is true.
     /// If all_options is false, pick just the most descriptive name to show.
     /// Use `get_name(true)` to get the positional name (replaces `get_pname`)
-    std::string get_name(bool positional = false,  ///< Show the positional name
-                         bool all_options = false  ///< Show every option
-                         ) const {
-        if(get_group().empty())
-            return {};  // Hidden
-
-        if(all_options) {
-
-            std::vector<std::string> name_list;
-
-            /// The all list will never include a positional unless asked or that's the only name.
-            if((positional && (!pname_.empty())) || (snames_.empty() && lnames_.empty())) {
-                name_list.push_back(pname_);
-            }
-            if((get_items_expected() == 0) && (!fnames_.empty())) {
-                for(const std::string &sname : snames_) {
-                    name_list.push_back("-" + sname);
-                    if(check_fname(sname)) {
-                        name_list.back() += "{" + get_flag_value(sname, "") + "}";
-                    }
-                }
-
-                for(const std::string &lname : lnames_) {
-                    name_list.push_back("--" + lname);
-                    if(check_fname(lname)) {
-                        name_list.back() += "{" + get_flag_value(lname, "") + "}";
-                    }
-                }
-            } else {
-                for(const std::string &sname : snames_)
-                    name_list.push_back("-" + sname);
-
-                for(const std::string &lname : lnames_)
-                    name_list.push_back("--" + lname);
-            }
-
-            return detail::join(name_list);
-        }
-
-        // This returns the positional name no matter what
-        if(positional)
-            return pname_;
-
-        // Prefer long name
-        if(!lnames_.empty())
-            return std::string(2, '-') + lnames_[0];
-
-        // Or short name if no long name
-        if(!snames_.empty())
-            return std::string(1, '-') + snames_[0];
-
-        // If positional is the only name, it's okay to use that
-        return pname_;
-    }
+    CLI11_NODISCARD std::string get_name(bool positional = false,  ///< Show the positional name
+                                         bool all_options = false  ///< Show every option
+    ) const;
 
     ///@}
     /// @name Parser tools
     ///@{
 
     /// Process the callback
-    void run_callback() {
-
-        if(current_option_state_ == option_state::parsing) {
-            _validate_results(results_);
-            current_option_state_ = option_state::validated;
-        }
-
-        if(current_option_state_ < option_state::reduced) {
-            _reduce_results(proc_results_, results_);
-            current_option_state_ = option_state::reduced;
-        }
-        if(current_option_state_ >= option_state::reduced) {
-            current_option_state_ = option_state::callback_run;
-            if(!(callback_)) {
-                return;
-            }
-            const results_t &send_results = proc_results_.empty() ? results_ : proc_results_;
-            bool local_result = callback_(send_results);
-
-            if(!local_result)
-                throw ConversionError(get_name(), results_);
-        }
-    }
+    void run_callback();
 
     /// If options share any of the same names, find it
-    const std::string &matching_name(const Option &other) const {
-        static const std::string estring;
-        for(const std::string &sname : snames_)
-            if(other.check_sname(sname))
-                return sname;
-        for(const std::string &lname : lnames_)
-            if(other.check_lname(lname))
-                return lname;
+    CLI11_NODISCARD const std::string &matching_name(const Option &other) const;
 
-        if(ignore_case_ ||
-           ignore_underscore_) {  // We need to do the inverse, in case we are ignore_case or ignore underscore
-            for(const std::string &sname : other.snames_)
-                if(check_sname(sname))
-                    return sname;
-            for(const std::string &lname : other.lnames_)
-                if(check_lname(lname))
-                    return lname;
-        }
-        return estring;
-    }
     /// If options share any of the same names, they are equal (not counting positional)
     bool operator==(const Option &other) const { return !matching_name(other).empty(); }
 
     /// Check a name. Requires "-" or "--" for short / long, supports positional name
-    bool check_name(const std::string &name) const {
-
-        if(name.length() > 2 && name[0] == '-' && name[1] == '-')
-            return check_lname(name.substr(2));
-        if(name.length() > 1 && name.front() == '-')
-            return check_sname(name.substr(1));
-        if(!pname_.empty()) {
-            std::string local_pname = pname_;
-            std::string local_name = name;
-            if(ignore_underscore_) {
-                local_pname = detail::remove_underscore(local_pname);
-                local_name = detail::remove_underscore(local_name);
-            }
-            if(ignore_case_) {
-                local_pname = detail::to_lower(local_pname);
-                local_name = detail::to_lower(local_name);
-            }
-            if(local_name == local_pname) {
-                return true;
-            }
-        }
-
-        if(!envname_.empty()) {
-            // this needs to be the original since envname_ shouldn't match on case insensitivity
-            return (name == envname_);
-        }
-        return false;
-    }
+    CLI11_NODISCARD bool check_name(const std::string &name) const;
 
     /// Requires "-" to be removed from string
-    bool check_sname(std::string name) const {
+    CLI11_NODISCARD bool check_sname(std::string name) const {
         return (detail::find_member(std::move(name), snames_, ignore_case_) >= 0);
     }
 
     /// Requires "--" to be removed from string
-    bool check_lname(std::string name) const {
+    CLI11_NODISCARD bool check_lname(std::string name) const {
         return (detail::find_member(std::move(name), lnames_, ignore_case_, ignore_underscore_) >= 0);
     }
 
     /// Requires "--" to be removed from string
-    bool check_fname(std::string name) const {
+    CLI11_NODISCARD bool check_fname(std::string name) const {
         if(fnames_.empty()) {
             return false;
         }
         return (detail::find_member(std::move(name), fnames_, ignore_case_, ignore_underscore_) >= 0);
     }
 
     /// Get the value that goes for a flag, nominally gets the default value but allows for overrides if not
     /// disabled
-    std::string get_flag_value(const std::string &name, std::string input_value) const {
-        static const std::string trueString{"true"};
-        static const std::string falseString{"false"};
-        static const std::string emptyString{"{}"};
-        // check for disable flag override_
-        if(disable_flag_override_) {
-            if(!((input_value.empty()) || (input_value == emptyString))) {
-                auto default_ind = detail::find_member(name, fnames_, ignore_case_, ignore_underscore_);
-                if(default_ind >= 0) {
-                    // We can static cast this to std::size_t because it is more than 0 in this block
-                    if(default_flag_values_[static_cast<std::size_t>(default_ind)].second != input_value) {
-                        throw(ArgumentMismatch::FlagOverride(name));
-                    }
-                } else {
-                    if(input_value != trueString) {
-                        throw(ArgumentMismatch::FlagOverride(name));
-                    }
-                }
-            }
-        }
-        auto ind = detail::find_member(name, fnames_, ignore_case_, ignore_underscore_);
-        if((input_value.empty()) || (input_value == emptyString)) {
-            if(flag_like_) {
-                return (ind < 0) ? trueString : default_flag_values_[static_cast<std::size_t>(ind)].second;
-            } else {
-                return (ind < 0) ? default_str_ : default_flag_values_[static_cast<std::size_t>(ind)].second;
-            }
-        }
-        if(ind < 0) {
-            return input_value;
-        }
-        if(default_flag_values_[static_cast<std::size_t>(ind)].second == falseString) {
-            try {
-                auto val = detail::to_flag_value(input_value);
-                return (val == 1) ? falseString : (val == (-1) ? trueString : std::to_string(-val));
-            } catch(const std::invalid_argument &) {
-                return input_value;
-            }
-        } else {
-            return input_value;
-        }
-    }
+    CLI11_NODISCARD std::string get_flag_value(const std::string &name, std::string input_value) const;
 
     /// Puts a result at the end
-    Option *add_result(std::string s) {
-        _add_result(std::move(s), results_);
-        current_option_state_ = option_state::parsing;
-        return this;
-    }
+    Option *add_result(std::string s);
 
     /// Puts a result at the end and get a count of the number of arguments actually added
-    Option *add_result(std::string s, int &results_added) {
-        results_added = _add_result(std::move(s), results_);
-        current_option_state_ = option_state::parsing;
-        return this;
-    }
+    Option *add_result(std::string s, int &results_added);
 
     /// Puts a result at the end
-    Option *add_result(std::vector<std::string> s) {
-        for(auto &str : s) {
-            _add_result(std::move(str), results_);
-        }
-        current_option_state_ = option_state::parsing;
-        return this;
-    }
+    Option *add_result(std::vector<std::string> s);
 
     /// Get the current complete results set
-    const results_t &results() const { return results_; }
+    CLI11_NODISCARD const results_t &results() const { return results_; }
 
     /// Get a copy of the results
-    results_t reduced_results() const {
-        results_t res = proc_results_.empty() ? results_ : proc_results_;
-        if(current_option_state_ < option_state::reduced) {
-            if(current_option_state_ == option_state::parsing) {
-                res = results_;
-                _validate_results(res);
-            }
-            if(!res.empty()) {
-                results_t extra;
-                _reduce_results(extra, res);
-                if(!extra.empty()) {
-                    res = std::move(extra);
-                }
-            }
-        }
-        return res;
-    }
+    CLI11_NODISCARD results_t reduced_results() const;
 
     /// Get the results as a specified type
     template <typename T> void results(T &output) const {
-        bool retval;
+        bool retval = false;
         if(current_option_state_ >= option_state::reduced || (results_.size() == 1 && validators_.empty())) {
             const results_t &res = (proc_results_.empty()) ? results_ : proc_results_;
             retval = detail::lexical_conversion<T, T>(res, output);
         } else {
             results_t res;
             if(results_.empty()) {
                 if(!default_str_.empty()) {
@@ -4887,22 +4828,22 @@
         }
         if(!retval) {
             throw ConversionError(get_name(), results_);
         }
     }
 
     /// Return the results as the specified type
-    template <typename T> T as() const {
+    template <typename T> CLI11_NODISCARD T as() const {
         T output;
         results(output);
         return output;
     }
 
     /// See if the callback has been run already
-    bool get_callback_run() const { return (current_option_state_ == option_state::callback_run); }
+    CLI11_NODISCARD bool get_callback_run() const { return (current_option_state_ == option_state::callback_run); }
 
     ///@}
     /// @name Custom options
     ///@{
 
     /// Set the type function to run when displayed on this option
     Option *type_name_fn(std::function<std::string()> typefun) {
@@ -4913,56 +4854,18 @@
     /// Set a custom option typestring
     Option *type_name(std::string typeval) {
         type_name_fn([typeval]() { return typeval; });
         return this;
     }
 
     /// Set a custom option size
-    Option *type_size(int option_type_size) {
-        if(option_type_size < 0) {
-            // this section is included for backwards compatibility
-            type_size_max_ = -option_type_size;
-            type_size_min_ = -option_type_size;
-            expected_max_ = detail::expected_max_vector_size;
-        } else {
-            type_size_max_ = option_type_size;
-            if(type_size_max_ < detail::expected_max_vector_size) {
-                type_size_min_ = option_type_size;
-            } else {
-                inject_separator_ = true;
-            }
-            if(type_size_max_ == 0)
-                required_ = false;
-        }
-        return this;
-    }
-    /// Set a custom option type size range
-    Option *type_size(int option_type_size_min, int option_type_size_max) {
-        if(option_type_size_min < 0 || option_type_size_max < 0) {
-            // this section is included for backwards compatibility
-            expected_max_ = detail::expected_max_vector_size;
-            option_type_size_min = (std::abs)(option_type_size_min);
-            option_type_size_max = (std::abs)(option_type_size_max);
-        }
+    Option *type_size(int option_type_size);
 
-        if(option_type_size_min > option_type_size_max) {
-            type_size_max_ = option_type_size_min;
-            type_size_min_ = option_type_size_max;
-        } else {
-            type_size_min_ = option_type_size_min;
-            type_size_max_ = option_type_size_max;
-        }
-        if(type_size_max_ == 0) {
-            required_ = false;
-        }
-        if(type_size_max_ >= detail::expected_max_vector_size) {
-            inject_separator_ = true;
-        }
-        return this;
-    }
+    /// Set a custom option type size range
+    Option *type_size(int option_type_size_min, int option_type_size_max);
 
     /// Set the value of the separator injection flag
     void inject_separator(bool value = true) { inject_separator_ = value; }
 
     /// Set a capture function for the default. Mostly used by App.
     Option *default_function(const std::function<std::string()> &func) {
         default_function_ = func;
@@ -4988,16 +4891,17 @@
     template <typename X> Option *default_val(const X &val) {
         std::string val_str = detail::to_string(val);
         auto old_option_state = current_option_state_;
         results_t old_results{std::move(results_)};
         results_.clear();
         try {
             add_result(val_str);
-            if(run_callback_for_default_) {
-                run_callback();  // run callback sets the state we need to reset it again
+            // if trigger_on_result_ is set the callback already ran
+            if(run_callback_for_default_ && !trigger_on_result_) {
+                run_callback();  // run callback sets the state, we need to reset it again
                 current_option_state_ = option_state::parsing;
             } else {
                 _validate_results(results_);
                 current_option_state_ = old_option_state;
             }
         } catch(const CLI::Error &) {
             // this should be done
@@ -5007,178 +4911,665 @@
         }
         results_ = std::move(old_results);
         default_str_ = std::move(val_str);
         return this;
     }
 
     /// Get the full typename for this option
-    std::string get_type_name() const {
-        std::string full_type_name = type_name_();
-        if(!validators_.empty()) {
-            for(auto &Validator : validators_) {
-                std::string vtype = Validator.get_description();
-                if(!vtype.empty()) {
-                    full_type_name += ":" + vtype;
-                }
+    CLI11_NODISCARD std::string get_type_name() const;
+
+  private:
+    /// Run the results through the Validators
+    void _validate_results(results_t &res) const;
+
+    /** reduce the results in accordance with the MultiOptionPolicy
+    @param[out] out results are assigned to res if there if they are different
+    */
+    void _reduce_results(results_t &out, const results_t &original) const;
+
+    // Run a result through the Validators
+    std::string _validate(std::string &result, int index) const;
+
+    /// Add a single result to the result set, taking into account delimiters
+    int _add_result(std::string &&result, std::vector<std::string> &res) const;
+};
+
+
+
+
+template <typename CRTP> template <typename T> void OptionBase<CRTP>::copy_to(T *other) const {
+    other->group(group_);
+    other->required(required_);
+    other->ignore_case(ignore_case_);
+    other->ignore_underscore(ignore_underscore_);
+    other->configurable(configurable_);
+    other->disable_flag_override(disable_flag_override_);
+    other->delimiter(delimiter_);
+    other->always_capture_default(always_capture_default_);
+    other->multi_option_policy(multi_option_policy_);
+}
+
+CLI11_INLINE Option *Option::expected(int value) {
+    if(value < 0) {
+        expected_min_ = -value;
+        if(expected_max_ < expected_min_) {
+            expected_max_ = expected_min_;
+        }
+        allow_extra_args_ = true;
+        flag_like_ = false;
+    } else if(value == detail::expected_max_vector_size) {
+        expected_min_ = 1;
+        expected_max_ = detail::expected_max_vector_size;
+        allow_extra_args_ = true;
+        flag_like_ = false;
+    } else {
+        expected_min_ = value;
+        expected_max_ = value;
+        flag_like_ = (expected_min_ == 0);
+    }
+    return this;
+}
+
+CLI11_INLINE Option *Option::expected(int value_min, int value_max) {
+    if(value_min < 0) {
+        value_min = -value_min;
+    }
+
+    if(value_max < 0) {
+        value_max = detail::expected_max_vector_size;
+    }
+    if(value_max < value_min) {
+        expected_min_ = value_max;
+        expected_max_ = value_min;
+    } else {
+        expected_max_ = value_max;
+        expected_min_ = value_min;
+    }
+
+    return this;
+}
+
+CLI11_INLINE Option *Option::check(Validator validator, const std::string &validator_name) {
+    validator.non_modifying();
+    validators_.push_back(std::move(validator));
+    if(!validator_name.empty())
+        validators_.back().name(validator_name);
+    return this;
+}
+
+CLI11_INLINE Option *Option::check(std::function<std::string(const std::string &)> Validator,
+                                   std::string Validator_description,
+                                   std::string Validator_name) {
+    validators_.emplace_back(Validator, std::move(Validator_description), std::move(Validator_name));
+    validators_.back().non_modifying();
+    return this;
+}
+
+CLI11_INLINE Option *Option::transform(Validator Validator, const std::string &Validator_name) {
+    validators_.insert(validators_.begin(), std::move(Validator));
+    if(!Validator_name.empty())
+        validators_.front().name(Validator_name);
+    return this;
+}
+
+CLI11_INLINE Option *Option::transform(const std::function<std::string(std::string)> &func,
+                                       std::string transform_description,
+                                       std::string transform_name) {
+    validators_.insert(validators_.begin(),
+                       Validator(
+                           [func](std::string &val) {
+                               val = func(val);
+                               return std::string{};
+                           },
+                           std::move(transform_description),
+                           std::move(transform_name)));
+
+    return this;
+}
+
+CLI11_INLINE Option *Option::each(const std::function<void(std::string)> &func) {
+    validators_.emplace_back(
+        [func](std::string &inout) {
+            func(inout);
+            return std::string{};
+        },
+        std::string{});
+    return this;
+}
+
+CLI11_INLINE Validator *Option::get_validator(const std::string &Validator_name) {
+    for(auto &Validator : validators_) {
+        if(Validator_name == Validator.get_name()) {
+            return &Validator;
+        }
+    }
+    if((Validator_name.empty()) && (!validators_.empty())) {
+        return &(validators_.front());
+    }
+    throw OptionNotFound(std::string{"Validator "} + Validator_name + " Not Found");
+}
+
+CLI11_INLINE Validator *Option::get_validator(int index) {
+    // This is an signed int so that it is not equivalent to a pointer.
+    if(index >= 0 && index < static_cast<int>(validators_.size())) {
+        return &(validators_[static_cast<decltype(validators_)::size_type>(index)]);
+    }
+    throw OptionNotFound("Validator index is not valid");
+}
+
+CLI11_INLINE bool Option::remove_needs(Option *opt) {
+    auto iterator = std::find(std::begin(needs_), std::end(needs_), opt);
+
+    if(iterator == std::end(needs_)) {
+        return false;
+    }
+    needs_.erase(iterator);
+    return true;
+}
+
+CLI11_INLINE Option *Option::excludes(Option *opt) {
+    if(opt == this) {
+        throw(IncorrectConstruction("and option cannot exclude itself"));
+    }
+    excludes_.insert(opt);
+
+    // Help text should be symmetric - excluding a should exclude b
+    opt->excludes_.insert(this);
+
+    // Ignoring the insert return value, excluding twice is now allowed.
+    // (Mostly to allow both directions to be excluded by user, even though the library does it for you.)
+
+    return this;
+}
+
+CLI11_INLINE bool Option::remove_excludes(Option *opt) {
+    auto iterator = std::find(std::begin(excludes_), std::end(excludes_), opt);
+
+    if(iterator == std::end(excludes_)) {
+        return false;
+    }
+    excludes_.erase(iterator);
+    return true;
+}
+
+template <typename T> Option *Option::ignore_case(bool value) {
+    if(!ignore_case_ && value) {
+        ignore_case_ = value;
+        auto *parent = static_cast<T *>(parent_);
+        for(const Option_p &opt : parent->options_) {
+            if(opt.get() == this) {
+                continue;
+            }
+            const auto &omatch = opt->matching_name(*this);
+            if(!omatch.empty()) {
+                ignore_case_ = false;
+                throw OptionAlreadyAdded("adding ignore case caused a name conflict with " + omatch);
             }
         }
-        return full_type_name;
+    } else {
+        ignore_case_ = value;
     }
+    return this;
+}
 
-  private:
-    /// Run the results through the Validators
-    void _validate_results(results_t &res) const {
-        // Run the Validators (can change the string)
-        if(!validators_.empty()) {
-            if(type_size_max_ > 1) {  // in this context index refers to the index in the type
-                int index = 0;
-                if(get_items_expected_max() < static_cast<int>(res.size()) &&
-                   multi_option_policy_ == CLI::MultiOptionPolicy::TakeLast) {
-                    // create a negative index for the earliest ones
-                    index = get_items_expected_max() - static_cast<int>(res.size());
+template <typename T> Option *Option::ignore_underscore(bool value) {
+
+    if(!ignore_underscore_ && value) {
+        ignore_underscore_ = value;
+        auto *parent = static_cast<T *>(parent_);
+        for(const Option_p &opt : parent->options_) {
+            if(opt.get() == this) {
+                continue;
+            }
+            const auto &omatch = opt->matching_name(*this);
+            if(!omatch.empty()) {
+                ignore_underscore_ = false;
+                throw OptionAlreadyAdded("adding ignore underscore caused a name conflict with " + omatch);
+            }
+        }
+    } else {
+        ignore_underscore_ = value;
+    }
+    return this;
+}
+
+CLI11_INLINE Option *Option::multi_option_policy(MultiOptionPolicy value) {
+    if(value != multi_option_policy_) {
+        if(multi_option_policy_ == MultiOptionPolicy::Throw && expected_max_ == detail::expected_max_vector_size &&
+           expected_min_ > 1) {  // this bizarre condition is to maintain backwards compatibility
+                                 // with the previous behavior of expected_ with vectors
+            expected_max_ = expected_min_;
+        }
+        multi_option_policy_ = value;
+        current_option_state_ = option_state::parsing;
+    }
+    return this;
+}
+
+CLI11_NODISCARD CLI11_INLINE std::string Option::get_name(bool positional, bool all_options) const {
+    if(get_group().empty())
+        return {};  // Hidden
+
+    if(all_options) {
+
+        std::vector<std::string> name_list;
+
+        /// The all list will never include a positional unless asked or that's the only name.
+        if((positional && (!pname_.empty())) || (snames_.empty() && lnames_.empty())) {
+            name_list.push_back(pname_);
+        }
+        if((get_items_expected() == 0) && (!fnames_.empty())) {
+            for(const std::string &sname : snames_) {
+                name_list.push_back("-" + sname);
+                if(check_fname(sname)) {
+                    name_list.back() += "{" + get_flag_value(sname, "") + "}";
                 }
+            }
 
-                for(std::string &result : res) {
-                    if(detail::is_separator(result) && type_size_max_ != type_size_min_ && index >= 0) {
-                        index = 0;  // reset index for variable size chunks
-                        continue;
-                    }
-                    auto err_msg = _validate(result, (index >= 0) ? (index % type_size_max_) : index);
-                    if(!err_msg.empty())
-                        throw ValidationError(get_name(), err_msg);
-                    ++index;
+            for(const std::string &lname : lnames_) {
+                name_list.push_back("--" + lname);
+                if(check_fname(lname)) {
+                    name_list.back() += "{" + get_flag_value(lname, "") + "}";
+                }
+            }
+        } else {
+            for(const std::string &sname : snames_)
+                name_list.push_back("-" + sname);
+
+            for(const std::string &lname : lnames_)
+                name_list.push_back("--" + lname);
+        }
+
+        return detail::join(name_list);
+    }
+
+    // This returns the positional name no matter what
+    if(positional)
+        return pname_;
+
+    // Prefer long name
+    if(!lnames_.empty())
+        return std::string(2, '-') + lnames_[0];
+
+    // Or short name if no long name
+    if(!snames_.empty())
+        return std::string(1, '-') + snames_[0];
+
+    // If positional is the only name, it's okay to use that
+    return pname_;
+}
+
+CLI11_INLINE void Option::run_callback() {
+    if(force_callback_ && results_.empty()) {
+        add_result(default_str_);
+    }
+    if(current_option_state_ == option_state::parsing) {
+        _validate_results(results_);
+        current_option_state_ = option_state::validated;
+    }
+
+    if(current_option_state_ < option_state::reduced) {
+        _reduce_results(proc_results_, results_);
+        current_option_state_ = option_state::reduced;
+    }
+    if(current_option_state_ >= option_state::reduced) {
+        current_option_state_ = option_state::callback_run;
+        if(!(callback_)) {
+            return;
+        }
+        const results_t &send_results = proc_results_.empty() ? results_ : proc_results_;
+        bool local_result = callback_(send_results);
+
+        if(!local_result)
+            throw ConversionError(get_name(), results_);
+    }
+}
+
+CLI11_NODISCARD CLI11_INLINE const std::string &Option::matching_name(const Option &other) const {
+    static const std::string estring;
+    for(const std::string &sname : snames_)
+        if(other.check_sname(sname))
+            return sname;
+    for(const std::string &lname : lnames_)
+        if(other.check_lname(lname))
+            return lname;
+
+    if(ignore_case_ ||
+       ignore_underscore_) {  // We need to do the inverse, in case we are ignore_case or ignore underscore
+        for(const std::string &sname : other.snames_)
+            if(check_sname(sname))
+                return sname;
+        for(const std::string &lname : other.lnames_)
+            if(check_lname(lname))
+                return lname;
+    }
+    return estring;
+}
+
+CLI11_NODISCARD CLI11_INLINE bool Option::check_name(const std::string &name) const {
+
+    if(name.length() > 2 && name[0] == '-' && name[1] == '-')
+        return check_lname(name.substr(2));
+    if(name.length() > 1 && name.front() == '-')
+        return check_sname(name.substr(1));
+    if(!pname_.empty()) {
+        std::string local_pname = pname_;
+        std::string local_name = name;
+        if(ignore_underscore_) {
+            local_pname = detail::remove_underscore(local_pname);
+            local_name = detail::remove_underscore(local_name);
+        }
+        if(ignore_case_) {
+            local_pname = detail::to_lower(local_pname);
+            local_name = detail::to_lower(local_name);
+        }
+        if(local_name == local_pname) {
+            return true;
+        }
+    }
+
+    if(!envname_.empty()) {
+        // this needs to be the original since envname_ shouldn't match on case insensitivity
+        return (name == envname_);
+    }
+    return false;
+}
+
+CLI11_NODISCARD CLI11_INLINE std::string Option::get_flag_value(const std::string &name,
+                                                                std::string input_value) const {
+    static const std::string trueString{"true"};
+    static const std::string falseString{"false"};
+    static const std::string emptyString{"{}"};
+    // check for disable flag override_
+    if(disable_flag_override_) {
+        if(!((input_value.empty()) || (input_value == emptyString))) {
+            auto default_ind = detail::find_member(name, fnames_, ignore_case_, ignore_underscore_);
+            if(default_ind >= 0) {
+                // We can static cast this to std::size_t because it is more than 0 in this block
+                if(default_flag_values_[static_cast<std::size_t>(default_ind)].second != input_value) {
+                    throw(ArgumentMismatch::FlagOverride(name));
                 }
             } else {
-                int index = 0;
-                if(expected_max_ < static_cast<int>(res.size()) &&
-                   multi_option_policy_ == CLI::MultiOptionPolicy::TakeLast) {
-                    // create a negative index for the earliest ones
-                    index = expected_max_ - static_cast<int>(res.size());
-                }
-                for(std::string &result : res) {
-                    auto err_msg = _validate(result, index);
-                    ++index;
-                    if(!err_msg.empty())
-                        throw ValidationError(get_name(), err_msg);
+                if(input_value != trueString) {
+                    throw(ArgumentMismatch::FlagOverride(name));
                 }
             }
         }
     }
+    auto ind = detail::find_member(name, fnames_, ignore_case_, ignore_underscore_);
+    if((input_value.empty()) || (input_value == emptyString)) {
+        if(flag_like_) {
+            return (ind < 0) ? trueString : default_flag_values_[static_cast<std::size_t>(ind)].second;
+        }
+        return (ind < 0) ? default_str_ : default_flag_values_[static_cast<std::size_t>(ind)].second;
+    }
+    if(ind < 0) {
+        return input_value;
+    }
+    if(default_flag_values_[static_cast<std::size_t>(ind)].second == falseString) {
+        try {
+            auto val = detail::to_flag_value(input_value);
+            return (val == 1) ? falseString : (val == (-1) ? trueString : std::to_string(-val));
+        } catch(const std::invalid_argument &) {
+            return input_value;
+        }
+    } else {
+        return input_value;
+    }
+}
 
-    /** reduce the results in accordance with the MultiOptionPolicy
-    @param[out] res results are assigned to res if there if they are different
-    */
-    void _reduce_results(results_t &res, const results_t &original) const {
+CLI11_INLINE Option *Option::add_result(std::string s) {
+    _add_result(std::move(s), results_);
+    current_option_state_ = option_state::parsing;
+    return this;
+}
 
-        // max num items expected or length of vector, always at least 1
-        // Only valid for a trimming policy
+CLI11_INLINE Option *Option::add_result(std::string s, int &results_added) {
+    results_added = _add_result(std::move(s), results_);
+    current_option_state_ = option_state::parsing;
+    return this;
+}
 
-        res.clear();
-        // Operation depends on the policy setting
-        switch(multi_option_policy_) {
-        case MultiOptionPolicy::TakeAll:
-            break;
-        case MultiOptionPolicy::TakeLast: {
-            // Allow multi-option sizes (including 0)
-            std::size_t trim_size = std::min<std::size_t>(
-                static_cast<std::size_t>(std::max<int>(get_items_expected_max(), 1)), original.size());
-            if(original.size() != trim_size) {
-                res.assign(original.end() - static_cast<results_t::difference_type>(trim_size), original.end());
-            }
-        } break;
-        case MultiOptionPolicy::TakeFirst: {
-            std::size_t trim_size = std::min<std::size_t>(
-                static_cast<std::size_t>(std::max<int>(get_items_expected_max(), 1)), original.size());
-            if(original.size() != trim_size) {
-                res.assign(original.begin(), original.begin() + static_cast<results_t::difference_type>(trim_size));
-            }
-        } break;
-        case MultiOptionPolicy::Join:
-            if(results_.size() > 1) {
-                res.push_back(detail::join(original, std::string(1, (delimiter_ == '\0') ? '\n' : delimiter_)));
-            }
-            break;
-        case MultiOptionPolicy::Throw:
-        default: {
-            auto num_min = static_cast<std::size_t>(get_items_expected_min());
-            auto num_max = static_cast<std::size_t>(get_items_expected_max());
-            if(num_min == 0) {
-                num_min = 1;
-            }
-            if(num_max == 0) {
-                num_max = 1;
-            }
-            if(original.size() < num_min) {
-                throw ArgumentMismatch::AtLeast(get_name(), static_cast<int>(num_min), original.size());
-            }
-            if(original.size() > num_max) {
-                throw ArgumentMismatch::AtMost(get_name(), static_cast<int>(num_max), original.size());
+CLI11_INLINE Option *Option::add_result(std::vector<std::string> s) {
+    current_option_state_ = option_state::parsing;
+    for(auto &str : s) {
+        _add_result(std::move(str), results_);
+    }
+    return this;
+}
+
+CLI11_NODISCARD CLI11_INLINE results_t Option::reduced_results() const {
+    results_t res = proc_results_.empty() ? results_ : proc_results_;
+    if(current_option_state_ < option_state::reduced) {
+        if(current_option_state_ == option_state::parsing) {
+            res = results_;
+            _validate_results(res);
+        }
+        if(!res.empty()) {
+            results_t extra;
+            _reduce_results(extra, res);
+            if(!extra.empty()) {
+                res = std::move(extra);
             }
-            break;
         }
+    }
+    return res;
+}
+
+CLI11_INLINE Option *Option::type_size(int option_type_size) {
+    if(option_type_size < 0) {
+        // this section is included for backwards compatibility
+        type_size_max_ = -option_type_size;
+        type_size_min_ = -option_type_size;
+        expected_max_ = detail::expected_max_vector_size;
+    } else {
+        type_size_max_ = option_type_size;
+        if(type_size_max_ < detail::expected_max_vector_size) {
+            type_size_min_ = option_type_size;
+        } else {
+            inject_separator_ = true;
+        }
+        if(type_size_max_ == 0)
+            required_ = false;
+    }
+    return this;
+}
+
+CLI11_INLINE Option *Option::type_size(int option_type_size_min, int option_type_size_max) {
+    if(option_type_size_min < 0 || option_type_size_max < 0) {
+        // this section is included for backwards compatibility
+        expected_max_ = detail::expected_max_vector_size;
+        option_type_size_min = (std::abs)(option_type_size_min);
+        option_type_size_max = (std::abs)(option_type_size_max);
+    }
+
+    if(option_type_size_min > option_type_size_max) {
+        type_size_max_ = option_type_size_min;
+        type_size_min_ = option_type_size_max;
+    } else {
+        type_size_min_ = option_type_size_min;
+        type_size_max_ = option_type_size_max;
+    }
+    if(type_size_max_ == 0) {
+        required_ = false;
+    }
+    if(type_size_max_ >= detail::expected_max_vector_size) {
+        inject_separator_ = true;
+    }
+    return this;
+}
+
+CLI11_NODISCARD CLI11_INLINE std::string Option::get_type_name() const {
+    std::string full_type_name = type_name_();
+    if(!validators_.empty()) {
+        for(const auto &Validator : validators_) {
+            std::string vtype = Validator.get_description();
+            if(!vtype.empty()) {
+                full_type_name += ":" + vtype;
+            }
         }
     }
+    return full_type_name;
+}
 
-    // Run a result through the Validators
-    std::string _validate(std::string &result, int index) const {
-        std::string err_msg;
-        if(result.empty() && expected_min_ == 0) {
-            // an empty with nothing expected is allowed
-            return err_msg;
-        }
-        for(const auto &vali : validators_) {
-            auto v = vali.get_application_index();
-            if(v == -1 || v == index) {
-                try {
-                    err_msg = vali(result);
-                } catch(const ValidationError &err) {
-                    err_msg = err.what();
+CLI11_INLINE void Option::_validate_results(results_t &res) const {
+    // Run the Validators (can change the string)
+    if(!validators_.empty()) {
+        if(type_size_max_ > 1) {  // in this context index refers to the index in the type
+            int index = 0;
+            if(get_items_expected_max() < static_cast<int>(res.size()) &&
+               multi_option_policy_ == CLI::MultiOptionPolicy::TakeLast) {
+                // create a negative index for the earliest ones
+                index = get_items_expected_max() - static_cast<int>(res.size());
+            }
+
+            for(std::string &result : res) {
+                if(detail::is_separator(result) && type_size_max_ != type_size_min_ && index >= 0) {
+                    index = 0;  // reset index for variable size chunks
+                    continue;
                 }
+                auto err_msg = _validate(result, (index >= 0) ? (index % type_size_max_) : index);
                 if(!err_msg.empty())
-                    break;
+                    throw ValidationError(get_name(), err_msg);
+                ++index;
+            }
+        } else {
+            int index = 0;
+            if(expected_max_ < static_cast<int>(res.size()) &&
+               multi_option_policy_ == CLI::MultiOptionPolicy::TakeLast) {
+                // create a negative index for the earliest ones
+                index = expected_max_ - static_cast<int>(res.size());
+            }
+            for(std::string &result : res) {
+                auto err_msg = _validate(result, index);
+                ++index;
+                if(!err_msg.empty())
+                    throw ValidationError(get_name(), err_msg);
             }
         }
+    }
+}
+
+CLI11_INLINE void Option::_reduce_results(results_t &out, const results_t &original) const {
+
+    // max num items expected or length of vector, always at least 1
+    // Only valid for a trimming policy
 
+    out.clear();
+    // Operation depends on the policy setting
+    switch(multi_option_policy_) {
+    case MultiOptionPolicy::TakeAll:
+        break;
+    case MultiOptionPolicy::TakeLast: {
+        // Allow multi-option sizes (including 0)
+        std::size_t trim_size = std::min<std::size_t>(
+            static_cast<std::size_t>(std::max<int>(get_items_expected_max(), 1)), original.size());
+        if(original.size() != trim_size) {
+            out.assign(original.end() - static_cast<results_t::difference_type>(trim_size), original.end());
+        }
+    } break;
+    case MultiOptionPolicy::TakeFirst: {
+        std::size_t trim_size = std::min<std::size_t>(
+            static_cast<std::size_t>(std::max<int>(get_items_expected_max(), 1)), original.size());
+        if(original.size() != trim_size) {
+            out.assign(original.begin(), original.begin() + static_cast<results_t::difference_type>(trim_size));
+        }
+    } break;
+    case MultiOptionPolicy::Join:
+        if(results_.size() > 1) {
+            out.push_back(detail::join(original, std::string(1, (delimiter_ == '\0') ? '\n' : delimiter_)));
+        }
+        break;
+    case MultiOptionPolicy::Sum:
+        out.push_back(detail::sum_string_vector(original));
+        break;
+    case MultiOptionPolicy::Throw:
+    default: {
+        auto num_min = static_cast<std::size_t>(get_items_expected_min());
+        auto num_max = static_cast<std::size_t>(get_items_expected_max());
+        if(num_min == 0) {
+            num_min = 1;
+        }
+        if(num_max == 0) {
+            num_max = 1;
+        }
+        if(original.size() < num_min) {
+            throw ArgumentMismatch::AtLeast(get_name(), static_cast<int>(num_min), original.size());
+        }
+        if(original.size() > num_max) {
+            throw ArgumentMismatch::AtMost(get_name(), static_cast<int>(num_max), original.size());
+        }
+        break;
+    }
+    }
+    // this check is to allow an empty vector in certain circumstances but not if expected is not zero.
+    // {} is the indicator for an empty container
+    if(out.empty()) {
+        if(original.size() == 1 && original[0] == "{}" && get_items_expected_min() > 0) {
+            out.push_back("{}");
+            out.push_back("%%");
+        }
+    } else if(out.size() == 1 && out[0] == "{}" && get_items_expected_min() > 0) {
+        out.push_back("%%");
+    }
+}
+
+CLI11_INLINE std::string Option::_validate(std::string &result, int index) const {
+    std::string err_msg;
+    if(result.empty() && expected_min_ == 0) {
+        // an empty with nothing expected is allowed
         return err_msg;
     }
+    for(const auto &vali : validators_) {
+        auto v = vali.get_application_index();
+        if(v == -1 || v == index) {
+            try {
+                err_msg = vali(result);
+            } catch(const ValidationError &err) {
+                err_msg = err.what();
+            }
+            if(!err_msg.empty())
+                break;
+        }
+    }
 
-    /// Add a single result to the result set, taking into account delimiters
-    int _add_result(std::string &&result, std::vector<std::string> &res) const {
-        int result_count = 0;
-        if(allow_extra_args_ && !result.empty() && result.front() == '[' &&
-           result.back() == ']') {  // this is now a vector string likely from the default or user entry
-            result.pop_back();
+    return err_msg;
+}
 
-            for(auto &var : CLI::detail::split(result.substr(1), ',')) {
+CLI11_INLINE int Option::_add_result(std::string &&result, std::vector<std::string> &res) const {
+    int result_count = 0;
+    if(allow_extra_args_ && !result.empty() && result.front() == '[' &&
+       result.back() == ']') {  // this is now a vector string likely from the default or user entry
+        result.pop_back();
+
+        for(auto &var : CLI::detail::split(result.substr(1), ',')) {
+            if(!var.empty()) {
+                result_count += _add_result(std::move(var), res);
+            }
+        }
+        return result_count;
+    }
+    if(delimiter_ == '\0') {
+        res.push_back(std::move(result));
+        ++result_count;
+    } else {
+        if((result.find_first_of(delimiter_) != std::string::npos)) {
+            for(const auto &var : CLI::detail::split(result, delimiter_)) {
                 if(!var.empty()) {
-                    result_count += _add_result(std::move(var), res);
+                    res.push_back(var);
+                    ++result_count;
                 }
             }
-            return result_count;
-        }
-        if(delimiter_ == '\0') {
+        } else {
             res.push_back(std::move(result));
             ++result_count;
-        } else {
-            if((result.find_first_of(delimiter_) != std::string::npos)) {
-                for(const auto &var : CLI::detail::split(result, delimiter_)) {
-                    if(!var.empty()) {
-                        res.push_back(var);
-                        ++result_count;
-                    }
-                }
-            } else {
-                res.push_back(std::move(result));
-                ++result_count;
-            }
         }
-        return result_count;
     }
-};  // namespace CLI
-
+    return result_count;
+}
 
 
 
 #ifndef CLI11_PARSE
 #define CLI11_PARSE(app, argc, argv)                                                                                   \
     try {                                                                                                              \
         (app).parse((argc), (argv));                                                                                   \
@@ -5189,26 +5580,45 @@
 
 namespace detail {
 enum class Classifier { NONE, POSITIONAL_MARK, SHORT, LONG, WINDOWS_STYLE, SUBCOMMAND, SUBCOMMAND_TERMINATOR };
 struct AppFriend;
 }  // namespace detail
 
 namespace FailureMessage {
-std::string simple(const App *app, const Error &e);
-std::string help(const App *app, const Error &e);
+/// Printout a clean, simple message on error (the default in CLI11 1.5+)
+CLI11_INLINE std::string simple(const App *app, const Error &e);
+
+/// Printout the full help string on error (if this fn is set, the old default for CLI11)
+CLI11_INLINE std::string help(const App *app, const Error &e);
 }  // namespace FailureMessage
 
 /// enumeration of modes of how to deal with extras in config files
 
-enum class config_extras_mode : char { error = 0, ignore, capture };
+enum class config_extras_mode : char { error = 0, ignore, ignore_all, capture };
 
 class App;
 
 using App_p = std::shared_ptr<App>;
 
+namespace detail {
+/// helper functions for adding in appropriate flag modifiers for add_flag
+
+template <typename T, enable_if_t<!std::is_integral<T>::value || (sizeof(T) <= 1U), detail::enabler> = detail::dummy>
+Option *default_flag_modifiers(Option *opt) {
+    return opt->always_capture_default();
+}
+
+/// summing modifiers
+template <typename T, enable_if_t<std::is_integral<T>::value && (sizeof(T) > 1U), detail::enabler> = detail::dummy>
+Option *default_flag_modifiers(Option *opt) {
+    return opt->multi_option_policy(MultiOptionPolicy::Sum)->default_str("0")->force_callback();
+}
+
+}  // namespace detail
+
 class Option_group;
 /// Creates a command line program, with very few defaults.
 /** To use, create a new `Program()` instance with `argc`, `argv`, and a help description. The templated
  *  add_option methods make it easy to prepare options. Remember to call `.start` before starting your
  * program, so that the options can be evaluated and the help option doesn't accidentally run your program. */
 class App {
     friend Option;
@@ -5362,14 +5772,17 @@
 
     /// if set to true the subcommand can be triggered via configuration files INHERITABLE
     bool configurable_{false};
 
     /// If set to true positional options are validated before assigning INHERITABLE
     bool validate_positionals_{false};
 
+    /// If set to true optional vector arguments are validated before assigning INHERITABLE
+    bool validate_optional_arguments_{false};
+
     /// indicator that the subcommand is silent and won't show up in subcommands list
     /// This is potentially useful as a modifier subcommand
     bool silent_{false};
 
     /// Counts the number of times this command/subcommand was parsed
     std::uint32_t parsed_{0U};
 
@@ -5403,46 +5816,15 @@
 
     /// This is the formatter for help printing. Default provided. INHERITABLE (same pointer)
     std::shared_ptr<Config> config_formatter_{new ConfigTOML()};
 
     ///@}
 
     /// Special private constructor for subcommand
-    App(std::string app_description, std::string app_name, App *parent)
-        : name_(std::move(app_name)), description_(std::move(app_description)), parent_(parent) {
-        // Inherit if not from a nullptr
-        if(parent_ != nullptr) {
-            if(parent_->help_ptr_ != nullptr)
-                set_help_flag(parent_->help_ptr_->get_name(false, true), parent_->help_ptr_->get_description());
-            if(parent_->help_all_ptr_ != nullptr)
-                set_help_all_flag(parent_->help_all_ptr_->get_name(false, true),
-                                  parent_->help_all_ptr_->get_description());
-
-            /// OptionDefaults
-            option_defaults_ = parent_->option_defaults_;
-
-            // INHERITABLE
-            failure_message_ = parent_->failure_message_;
-            allow_extras_ = parent_->allow_extras_;
-            allow_config_extras_ = parent_->allow_config_extras_;
-            prefix_command_ = parent_->prefix_command_;
-            immediate_callback_ = parent_->immediate_callback_;
-            ignore_case_ = parent_->ignore_case_;
-            ignore_underscore_ = parent_->ignore_underscore_;
-            fallthrough_ = parent_->fallthrough_;
-            validate_positionals_ = parent_->validate_positionals_;
-            configurable_ = parent_->configurable_;
-            allow_windows_style_options_ = parent_->allow_windows_style_options_;
-            group_ = parent_->group_;
-            footer_ = parent_->footer_;
-            formatter_ = parent_->formatter_;
-            config_formatter_ = parent_->config_formatter_;
-            require_subcommand_max_ = parent_->require_subcommand_max_;
-        }
-    }
+    App(std::string app_description, std::string app_name, App *parent);
 
   public:
     /// @name Basic
     ///@{
 
     /// Create a new program. Pass in the same arguments as main(), along with a help string.
     explicit App(std::string app_description = "", std::string app_name = "")
@@ -5489,63 +5871,18 @@
     ///
     App *preparse_callback(std::function<void(std::size_t)> pp_callback) {
         pre_parse_callback_ = std::move(pp_callback);
         return this;
     }
 
     /// Set a name for the app (empty will use parser to set the name)
-    App *name(std::string app_name = "") {
-
-        if(parent_ != nullptr) {
-            auto oname = name_;
-            name_ = app_name;
-            auto &res = _compare_subcommand_names(*this, *_get_fallthrough_parent());
-            if(!res.empty()) {
-                name_ = oname;
-                throw(OptionAlreadyAdded(app_name + " conflicts with existing subcommand names"));
-            }
-        } else {
-            name_ = app_name;
-        }
-        has_automatic_name_ = false;
-        return this;
-    }
+    App *name(std::string app_name = "");
 
     /// Set an alias for the app
-    App *alias(std::string app_name) {
-        if(!detail::valid_name_string(app_name)) {
-            if(app_name.empty()) {
-                throw IncorrectConstruction("Empty aliases are not allowed");
-            }
-            if(!detail::valid_first_char(app_name[0])) {
-                throw IncorrectConstruction(
-                    "Alias starts with invalid character, allowed characters are [a-zA-z0-9]+'_','?','@' ");
-            }
-            for(auto c : app_name) {
-                if(!detail::valid_later_char(c)) {
-                    throw IncorrectConstruction(std::string("Alias contains invalid character ('") + c +
-                                                "'), allowed characters are "
-                                                "[a-zA-z0-9]+'_','?','@','.','-' ");
-                }
-            }
-        }
-
-        if(parent_ != nullptr) {
-            aliases_.push_back(app_name);
-            auto &res = _compare_subcommand_names(*this, *_get_fallthrough_parent());
-            if(!res.empty()) {
-                aliases_.pop_back();
-                throw(OptionAlreadyAdded("alias already matches an existing subcommand: " + app_name));
-            }
-        } else {
-            aliases_.push_back(app_name);
-        }
-
-        return this;
-    }
+    App *alias(std::string app_name);
 
     /// Remove the error when extras are left over on the command line.
     App *allow_extras(bool allow = true) {
         allow_extras_ = allow;
         return this;
     }
 
@@ -5586,32 +5923,28 @@
             default_startup =
                 (default_startup == startup_mode::disabled) ? startup_mode::disabled : startup_mode::stable;
         }
         return this;
     }
 
     /// Set the subcommand callback to be executed immediately on subcommand completion
-    App *immediate_callback(bool immediate = true) {
-        immediate_callback_ = immediate;
-        if(immediate_callback_) {
-            if(final_callback_ && !(parse_complete_callback_)) {
-                std::swap(final_callback_, parse_complete_callback_);
-            }
-        } else if(!(final_callback_) && parse_complete_callback_) {
-            std::swap(final_callback_, parse_complete_callback_);
-        }
-        return this;
-    }
+    App *immediate_callback(bool immediate = true);
 
     /// Set the subcommand to validate positional arguments before assigning
     App *validate_positionals(bool validate = true) {
         validate_positionals_ = validate;
         return this;
     }
 
+    /// Set the subcommand to validate optional vector arguments before assigning
+    App *validate_optional_arguments(bool validate = true) {
+        validate_optional_arguments_ = validate;
+        return this;
+    }
+
     /// ignore extras in config files
     App *allow_config_extras(bool allow = true) {
         if(allow) {
             allow_config_extras_ = config_extras_mode::capture;
             allow_extras_ = true;
         } else {
             allow_config_extras_ = config_extras_mode::error;
@@ -5628,27 +5961,15 @@
     /// Do not parse anything after the first unrecognized option and return
     App *prefix_command(bool allow = true) {
         prefix_command_ = allow;
         return this;
     }
 
     /// Ignore case. Subcommands inherit value.
-    App *ignore_case(bool value = true) {
-        if(value && !ignore_case_) {
-            ignore_case_ = true;
-            auto *p = (parent_ != nullptr) ? _get_fallthrough_parent() : this;
-            auto &match = _compare_subcommand_names(*this, *p);
-            if(!match.empty()) {
-                ignore_case_ = false;  // we are throwing so need to be exception invariant
-                throw OptionAlreadyAdded("ignore case would cause subcommand name conflicts: " + match);
-            }
-        }
-        ignore_case_ = value;
-        return this;
-    }
+    App *ignore_case(bool value = true);
 
     /// Allow windows style options, such as `/opt`. First matching short or long name used. Subcommands inherit
     /// value.
     App *allow_windows_style_options(bool value = true) {
         allow_windows_style_options_ = value;
         return this;
     }
@@ -5662,27 +5983,15 @@
     /// Specify that the subcommand can be triggered by a config file
     App *configurable(bool value = true) {
         configurable_ = value;
         return this;
     }
 
     /// Ignore underscore. Subcommands inherit value.
-    App *ignore_underscore(bool value = true) {
-        if(value && !ignore_underscore_) {
-            ignore_underscore_ = true;
-            auto *p = (parent_ != nullptr) ? _get_fallthrough_parent() : this;
-            auto &match = _compare_subcommand_names(*this, *p);
-            if(!match.empty()) {
-                ignore_underscore_ = false;
-                throw OptionAlreadyAdded("ignore underscore would cause subcommand name conflicts: " + match);
-            }
-        }
-        ignore_underscore_ = value;
-        return this;
-    }
+    App *ignore_underscore(bool value = true);
 
     /// Set the help formatter
     App *formatter(std::shared_ptr<FormatterBase> fmt) {
         formatter_ = fmt;
         return this;
     }
 
@@ -5695,15 +6004,15 @@
     /// Set the config formatter
     App *config_formatter(std::shared_ptr<Config> fmt) {
         config_formatter_ = fmt;
         return this;
     }
 
     /// Check to see if this subcommand was parsed, true only if received on command line.
-    bool parsed() const { return parsed_ > 0; }
+    CLI11_NODISCARD bool parsed() const { return parsed_ > 0; }
 
     /// Get the OptionDefault object, to set option defaults
     OptionDefaults *option_defaults() { return &option_defaults_; }
 
     ///@}
     /// @name Adding options
     ///@{
@@ -5722,50 +6031,15 @@
     ///     std::string filename;
     ///     program.add_option("filename", filename, "description of filename");
     ///
     Option *add_option(std::string option_name,
                        callback_t option_callback,
                        std::string option_description = "",
                        bool defaulted = false,
-                       std::function<std::string()> func = {}) {
-        Option myopt{option_name, option_description, option_callback, this};
-
-        if(std::find_if(std::begin(options_), std::end(options_), [&myopt](const Option_p &v) {
-               return *v == myopt;
-           }) == std::end(options_)) {
-            options_.emplace_back();
-            Option_p &option = options_.back();
-            option.reset(new Option(option_name, option_description, option_callback, this));
-
-            // Set the default string capture function
-            option->default_function(func);
-
-            // For compatibility with CLI11 1.7 and before, capture the default string here
-            if(defaulted)
-                option->capture_default_str();
-
-            // Transfer defaults to the new option
-            option_defaults_.copy_to(option.get());
-
-            // Don't bother to capture if we already did
-            if(!defaulted && option->get_always_capture_default())
-                option->capture_default_str();
-
-            return option.get();
-        }
-        // we know something matches now find what it is so we can produce more error information
-        for(auto &opt : options_) {
-            auto &matchname = opt->matching_name(myopt);
-            if(!matchname.empty()) {
-                throw(OptionAlreadyAdded("added option matched existing option name: " + matchname));
-            }
-        }
-        // this line should not be reached the above loop should trigger the throw
-        throw(OptionAlreadyAdded("added option matched existing option name"));  // LCOV_EXCL_LINE
-    }
+                       std::function<std::string()> func = {});
 
     /// Add option for assigning to a variable
     template <typename AssignTo,
               typename ConvertTo = AssignTo,
               enable_if_t<!std::is_const<ConvertTo>::value, detail::enabler> = detail::dummy>
     Option *add_option(std::string option_name,
                        AssignTo &variable,  ///< The variable to set
@@ -5839,111 +6113,32 @@
               enable_if_t<std::is_const<T>::value && std::is_constructible<std::string, T>::value, detail::enabler> =
                   detail::dummy>
     Option *add_option(std::string option_name, T &option_description) {
         return add_option(option_name, CLI::callback_t(), option_description, false);
     }
 
     /// Set a help flag, replace the existing one if present
-    Option *set_help_flag(std::string flag_name = "", const std::string &help_description = "") {
-        // take flag_description by const reference otherwise add_flag tries to assign to help_description
-        if(help_ptr_ != nullptr) {
-            remove_option(help_ptr_);
-            help_ptr_ = nullptr;
-        }
-
-        // Empty name will simply remove the help flag
-        if(!flag_name.empty()) {
-            help_ptr_ = add_flag(flag_name, help_description);
-            help_ptr_->configurable(false);
-        }
-
-        return help_ptr_;
-    }
+    Option *set_help_flag(std::string flag_name = "", const std::string &help_description = "");
 
     /// Set a help all flag, replaced the existing one if present
-    Option *set_help_all_flag(std::string help_name = "", const std::string &help_description = "") {
-        // take flag_description by const reference otherwise add_flag tries to assign to flag_description
-        if(help_all_ptr_ != nullptr) {
-            remove_option(help_all_ptr_);
-            help_all_ptr_ = nullptr;
-        }
-
-        // Empty name will simply remove the help all flag
-        if(!help_name.empty()) {
-            help_all_ptr_ = add_flag(help_name, help_description);
-            help_all_ptr_->configurable(false);
-        }
-
-        return help_all_ptr_;
-    }
+    Option *set_help_all_flag(std::string help_name = "", const std::string &help_description = "");
 
     /// Set a version flag and version display string, replace the existing one if present
     Option *set_version_flag(std::string flag_name = "",
                              const std::string &versionString = "",
-                             const std::string &version_help = "Display program version information and exit") {
-        // take flag_description by const reference otherwise add_flag tries to assign to version_description
-        if(version_ptr_ != nullptr) {
-            remove_option(version_ptr_);
-            version_ptr_ = nullptr;
-        }
+                             const std::string &version_help = "Display program version information and exit");
 
-        // Empty name will simply remove the version flag
-        if(!flag_name.empty()) {
-            version_ptr_ = add_flag_callback(
-                flag_name, [versionString]() { throw(CLI::CallForVersion(versionString, 0)); }, version_help);
-            version_ptr_->configurable(false);
-        }
-
-        return version_ptr_;
-    }
     /// Generate the version string through a callback function
     Option *set_version_flag(std::string flag_name,
                              std::function<std::string()> vfunc,
-                             const std::string &version_help = "Display program version information and exit") {
-        if(version_ptr_ != nullptr) {
-            remove_option(version_ptr_);
-            version_ptr_ = nullptr;
-        }
-
-        // Empty name will simply remove the version flag
-        if(!flag_name.empty()) {
-            version_ptr_ = add_flag_callback(
-                flag_name, [vfunc]() { throw(CLI::CallForVersion(vfunc(), 0)); }, version_help);
-            version_ptr_->configurable(false);
-        }
-
-        return version_ptr_;
-    }
+                             const std::string &version_help = "Display program version information and exit");
 
   private:
     /// Internal function for adding a flag
-    Option *_add_flag_internal(std::string flag_name, CLI::callback_t fun, std::string flag_description) {
-        Option *opt;
-        if(detail::has_default_flag_values(flag_name)) {
-            // check for default values and if it has them
-            auto flag_defaults = detail::get_default_flag_values(flag_name);
-            detail::remove_default_flag_values(flag_name);
-            opt = add_option(std::move(flag_name), std::move(fun), std::move(flag_description), false);
-            for(const auto &fname : flag_defaults)
-                opt->fnames_.push_back(fname.first);
-            opt->default_flag_values_ = std::move(flag_defaults);
-        } else {
-            opt = add_option(std::move(flag_name), std::move(fun), std::move(flag_description), false);
-        }
-        // flags cannot have positional values
-        if(opt->get_positional()) {
-            auto pos_name = opt->get_name(true);
-            remove_option(opt);
-            throw IncorrectConstruction::PositionalFlag(pos_name);
-        }
-        opt->multi_option_policy(MultiOptionPolicy::TakeLast);
-        opt->expected(0);
-        opt->required(false);
-        return opt;
-    }
+    Option *_add_flag_internal(std::string flag_name, CLI::callback_t fun, std::string flag_description);
 
   public:
     /// Add a flag with no description or variable assignment
     Option *add_flag(std::string flag_name) { return _add_flag_internal(flag_name, CLI::callback_t(), std::string{}); }
 
     /// Add flag with description but with no variable assignment or callback
     /// takes a constant string,  if a variable string is passed that variable will be assigned the results from the
@@ -5951,311 +6146,138 @@
     template <typename T,
               enable_if_t<std::is_const<T>::value && std::is_constructible<std::string, T>::value, detail::enabler> =
                   detail::dummy>
     Option *add_flag(std::string flag_name, T &flag_description) {
         return _add_flag_internal(flag_name, CLI::callback_t(), flag_description);
     }
 
-    /// Add option for flag with integer result - defaults to allowing multiple passings, but can be forced to one
-    /// if `multi_option_policy(CLI::MultiOptionPolicy::Throw)` is used.
-    template <typename T,
-              enable_if_t<std::is_constructible<T, std::int64_t>::value && !is_bool<T>::value, detail::enabler> =
-                  detail::dummy>
-    Option *add_flag(std::string flag_name,
-                     T &flag_count,  ///< A variable holding the count
-                     std::string flag_description = "") {
-        flag_count = 0;
-        CLI::callback_t fun = [&flag_count](const CLI::results_t &res) {
-            try {
-                detail::sum_flag_vector(res, flag_count);
-            } catch(const std::invalid_argument &) {
-                return false;
-            }
-            return true;
-        };
-        return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description))
-            ->multi_option_policy(MultiOptionPolicy::TakeAll);
-    }
-
     /// Other type version accepts all other types that are not vectors such as bool, enum, string or other classes
     /// that can be converted from a string
     template <typename T,
               enable_if_t<!detail::is_mutable_container<T>::value && !std::is_const<T>::value &&
-                              (!std::is_constructible<T, std::int64_t>::value || is_bool<T>::value) &&
                               !std::is_constructible<std::function<void(int)>, T>::value,
                           detail::enabler> = detail::dummy>
     Option *add_flag(std::string flag_name,
-                     T &flag_result,  ///< A variable holding true if passed
+                     T &flag_result,  ///< A variable holding the flag result
                      std::string flag_description = "") {
 
         CLI::callback_t fun = [&flag_result](const CLI::results_t &res) {
-            return CLI::detail::lexical_cast(res[0], flag_result);
+            using CLI::detail::lexical_cast;
+            return lexical_cast(res[0], flag_result);
         };
-        return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description))->run_callback_for_default();
+        auto *opt = _add_flag_internal(flag_name, std::move(fun), std::move(flag_description));
+        return detail::default_flag_modifiers<T>(opt);
     }
 
     /// Vector version to capture multiple flags.
     template <typename T,
               enable_if_t<!std::is_assignable<std::function<void(std::int64_t)> &, T>::value, detail::enabler> =
                   detail::dummy>
     Option *add_flag(std::string flag_name,
                      std::vector<T> &flag_results,  ///< A vector of values with the flag results
                      std::string flag_description = "") {
         CLI::callback_t fun = [&flag_results](const CLI::results_t &res) {
             bool retval = true;
             for(const auto &elem : res) {
+                using CLI::detail::lexical_cast;
                 flag_results.emplace_back();
-                retval &= detail::lexical_cast(elem, flag_results.back());
+                retval &= lexical_cast(elem, flag_results.back());
             }
             return retval;
         };
         return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description))
             ->multi_option_policy(MultiOptionPolicy::TakeAll)
             ->run_callback_for_default();
     }
 
     /// Add option for callback that is triggered with a true flag and takes no arguments
     Option *add_flag_callback(std::string flag_name,
                               std::function<void(void)> function,  ///< A function to call, void(void)
-                              std::string flag_description = "") {
-
-        CLI::callback_t fun = [function](const CLI::results_t &res) {
-            bool trigger{false};
-            auto result = CLI::detail::lexical_cast(res[0], trigger);
-            if(result && trigger) {
-                function();
-            }
-            return result;
-        };
-        return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description));
-    }
+                              std::string flag_description = "");
 
     /// Add option for callback with an integer value
     Option *add_flag_function(std::string flag_name,
                               std::function<void(std::int64_t)> function,  ///< A function to call, void(int)
-                              std::string flag_description = "") {
-
-        CLI::callback_t fun = [function](const CLI::results_t &res) {
-            std::int64_t flag_count = 0;
-            detail::sum_flag_vector(res, flag_count);
-            function(flag_count);
-            return true;
-        };
-        return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description))
-            ->multi_option_policy(MultiOptionPolicy::TakeAll);
-    }
+                              std::string flag_description = "");
 
 #ifdef CLI11_CPP14
     /// Add option for callback (C++14 or better only)
     Option *add_flag(std::string flag_name,
                      std::function<void(std::int64_t)> function,  ///< A function to call, void(std::int64_t)
                      std::string flag_description = "") {
         return add_flag_function(std::move(flag_name), std::move(function), std::move(flag_description));
     }
 #endif
 
     /// Set a configuration ini file option, or clear it if no name passed
     Option *set_config(std::string option_name = "",
                        std::string default_filename = "",
                        const std::string &help_message = "Read an ini file",
-                       bool config_required = false) {
-
-        // Remove existing config if present
-        if(config_ptr_ != nullptr) {
-            remove_option(config_ptr_);
-            config_ptr_ = nullptr;  // need to remove the config_ptr completely
-        }
-
-        // Only add config if option passed
-        if(!option_name.empty()) {
-            config_ptr_ = add_option(option_name, help_message);
-            if(config_required) {
-                config_ptr_->required();
-            }
-            if(!default_filename.empty()) {
-                config_ptr_->default_str(std::move(default_filename));
-            }
-            config_ptr_->configurable(false);
-        }
-
-        return config_ptr_;
-    }
+                       bool config_required = false);
 
     /// Removes an option from the App. Takes an option pointer. Returns true if found and removed.
-    bool remove_option(Option *opt) {
-        // Make sure no links exist
-        for(Option_p &op : options_) {
-            op->remove_needs(opt);
-            op->remove_excludes(opt);
-        }
-
-        if(help_ptr_ == opt)
-            help_ptr_ = nullptr;
-        if(help_all_ptr_ == opt)
-            help_all_ptr_ = nullptr;
-
-        auto iterator =
-            std::find_if(std::begin(options_), std::end(options_), [opt](const Option_p &v) { return v.get() == opt; });
-        if(iterator != std::end(options_)) {
-            options_.erase(iterator);
-            return true;
-        }
-        return false;
-    }
+    bool remove_option(Option *opt);
 
     /// creates an option group as part of the given app
     template <typename T = Option_group>
     T *add_option_group(std::string group_name, std::string group_description = "") {
+        if(!detail::valid_alias_name_string(group_name)) {
+            throw IncorrectConstruction("option group names may not contain newlines or null characters");
+        }
         auto option_group = std::make_shared<T>(std::move(group_description), group_name, this);
-        auto ptr = option_group.get();
+        auto *ptr = option_group.get();
         // move to App_p for overload resolution on older gcc versions
         App_p app_ptr = std::dynamic_pointer_cast<App>(option_group);
         add_subcommand(std::move(app_ptr));
         return ptr;
     }
 
     ///@}
     /// @name Subcommands
     ///@{
 
     /// Add a subcommand. Inherits INHERITABLE and OptionDefaults, and help flag
-    App *add_subcommand(std::string subcommand_name = "", std::string subcommand_description = "") {
-        if(!subcommand_name.empty() && !detail::valid_name_string(subcommand_name)) {
-            if(!detail::valid_first_char(subcommand_name[0])) {
-                throw IncorrectConstruction(
-                    "Subcommand name starts with invalid character, allowed characters are [a-zA-z0-9]+'_','?','@' ");
-            }
-            for(auto c : subcommand_name) {
-                if(!detail::valid_later_char(c)) {
-                    throw IncorrectConstruction(std::string("Subcommand name contains invalid character ('") + c +
-                                                "'), allowed characters are "
-                                                "[a-zA-z0-9]+'_','?','@','.','-' ");
-                }
-            }
-        }
-        CLI::App_p subcom = std::shared_ptr<App>(new App(std::move(subcommand_description), subcommand_name, this));
-        return add_subcommand(std::move(subcom));
-    }
+    App *add_subcommand(std::string subcommand_name = "", std::string subcommand_description = "");
 
     /// Add a previously created app as a subcommand
-    App *add_subcommand(CLI::App_p subcom) {
-        if(!subcom)
-            throw IncorrectConstruction("passed App is not valid");
-        auto ckapp = (name_.empty() && parent_ != nullptr) ? _get_fallthrough_parent() : this;
-        auto &mstrg = _compare_subcommand_names(*subcom, *ckapp);
-        if(!mstrg.empty()) {
-            throw(OptionAlreadyAdded("subcommand name or alias matches existing subcommand: " + mstrg));
-        }
-        subcom->parent_ = this;
-        subcommands_.push_back(std::move(subcom));
-        return subcommands_.back().get();
-    }
+    App *add_subcommand(CLI::App_p subcom);
 
     /// Removes a subcommand from the App. Takes a subcommand pointer. Returns true if found and removed.
-    bool remove_subcommand(App *subcom) {
-        // Make sure no links exist
-        for(App_p &sub : subcommands_) {
-            sub->remove_excludes(subcom);
-            sub->remove_needs(subcom);
-        }
+    bool remove_subcommand(App *subcom);
 
-        auto iterator = std::find_if(
-            std::begin(subcommands_), std::end(subcommands_), [subcom](const App_p &v) { return v.get() == subcom; });
-        if(iterator != std::end(subcommands_)) {
-            subcommands_.erase(iterator);
-            return true;
-        }
-        return false;
-    }
     /// Check to see if a subcommand is part of this command (doesn't have to be in command line)
     /// returns the first subcommand if passed a nullptr
-    App *get_subcommand(const App *subcom) const {
-        if(subcom == nullptr)
-            throw OptionNotFound("nullptr passed");
-        for(const App_p &subcomptr : subcommands_)
-            if(subcomptr.get() == subcom)
-                return subcomptr.get();
-        throw OptionNotFound(subcom->get_name());
-    }
+    App *get_subcommand(const App *subcom) const;
 
     /// Check to see if a subcommand is part of this command (text version)
-    App *get_subcommand(std::string subcom) const {
-        auto subc = _find_subcommand(subcom, false, false);
-        if(subc == nullptr)
-            throw OptionNotFound(subcom);
-        return subc;
-    }
+    CLI11_NODISCARD App *get_subcommand(std::string subcom) const;
+
     /// Get a pointer to subcommand by index
-    App *get_subcommand(int index = 0) const {
-        if(index >= 0) {
-            auto uindex = static_cast<unsigned>(index);
-            if(uindex < subcommands_.size())
-                return subcommands_[uindex].get();
-        }
-        throw OptionNotFound(std::to_string(index));
-    }
+    CLI11_NODISCARD App *get_subcommand(int index = 0) const;
 
     /// Check to see if a subcommand is part of this command and get a shared_ptr to it
-    CLI::App_p get_subcommand_ptr(App *subcom) const {
-        if(subcom == nullptr)
-            throw OptionNotFound("nullptr passed");
-        for(const App_p &subcomptr : subcommands_)
-            if(subcomptr.get() == subcom)
-                return subcomptr;
-        throw OptionNotFound(subcom->get_name());
-    }
+    CLI::App_p get_subcommand_ptr(App *subcom) const;
 
     /// Check to see if a subcommand is part of this command (text version)
-    CLI::App_p get_subcommand_ptr(std::string subcom) const {
-        for(const App_p &subcomptr : subcommands_)
-            if(subcomptr->check_name(subcom))
-                return subcomptr;
-        throw OptionNotFound(subcom);
-    }
+    CLI11_NODISCARD CLI::App_p get_subcommand_ptr(std::string subcom) const;
 
     /// Get an owning pointer to subcommand by index
-    CLI::App_p get_subcommand_ptr(int index = 0) const {
-        if(index >= 0) {
-            auto uindex = static_cast<unsigned>(index);
-            if(uindex < subcommands_.size())
-                return subcommands_[uindex];
-        }
-        throw OptionNotFound(std::to_string(index));
-    }
+    CLI11_NODISCARD CLI::App_p get_subcommand_ptr(int index = 0) const;
 
     /// Check to see if an option group is part of this App
-    App *get_option_group(std::string group_name) const {
-        for(const App_p &app : subcommands_) {
-            if(app->name_.empty() && app->group_ == group_name) {
-                return app.get();
-            }
-        }
-        throw OptionNotFound(group_name);
-    }
+    CLI11_NODISCARD App *get_option_group(std::string group_name) const;
 
     /// No argument version of count counts the number of times this subcommand was
     /// passed in. The main app will return 1. Unnamed subcommands will also return 1 unless
     /// otherwise modified in a callback
-    std::size_t count() const { return parsed_; }
+    CLI11_NODISCARD std::size_t count() const { return parsed_; }
 
     /// Get a count of all the arguments processed in options and subcommands, this excludes arguments which were
     /// treated as extras.
-    std::size_t count_all() const {
-        std::size_t cnt{0};
-        for(auto &opt : options_) {
-            cnt += opt->count();
-        }
-        for(auto &sub : subcommands_) {
-            cnt += sub->count_all();
-        }
-        if(!get_name().empty()) {  // for named subcommands add the number of times the subcommand was called
-            cnt += parsed_;
-        }
-        return cnt;
-    }
+    CLI11_NODISCARD std::size_t count_all() const;
 
     /// Changes the group membership
     App *group(std::string group_name) {
         group_ = group_name;
         return this;
     }
 
@@ -6338,206 +6360,72 @@
     virtual void pre_callback() {}
 
     ///@}
     /// @name Parsing
     ///@{
     //
     /// Reset the parsed data
-    void clear() {
-
-        parsed_ = 0;
-        pre_parse_called_ = false;
-
-        missing_.clear();
-        parsed_subcommands_.clear();
-        for(const Option_p &opt : options_) {
-            opt->clear();
-        }
-        for(const App_p &subc : subcommands_) {
-            subc->clear();
-        }
-    }
+    void clear();
 
     /// Parses the command line - throws errors.
     /// This must be called after the options are in but before the rest of the program.
-    void parse(int argc, const char *const *argv) {
-        // If the name is not set, read from command line
-        if(name_.empty() || has_automatic_name_) {
-            has_automatic_name_ = true;
-            name_ = argv[0];
-        }
-
-        std::vector<std::string> args;
-        args.reserve(static_cast<std::size_t>(argc) - 1);
-        for(int i = argc - 1; i > 0; i--)
-            args.emplace_back(argv[i]);
-        parse(std::move(args));
-    }
+    void parse(int argc, const char *const *argv);
 
     /// Parse a single string as if it contained command line arguments.
     /// This function splits the string into arguments then calls parse(std::vector<std::string> &)
     /// the function takes an optional boolean argument specifying if the programName is included in the string to
     /// process
-    void parse(std::string commandline, bool program_name_included = false) {
-
-        if(program_name_included) {
-            auto nstr = detail::split_program_name(commandline);
-            if((name_.empty()) || (has_automatic_name_)) {
-                has_automatic_name_ = true;
-                name_ = nstr.first;
-            }
-            commandline = std::move(nstr.second);
-        } else {
-            detail::trim(commandline);
-        }
-        // the next section of code is to deal with quoted arguments after an '=' or ':' for windows like operations
-        if(!commandline.empty()) {
-            commandline = detail::find_and_modify(commandline, "=", detail::escape_detect);
-            if(allow_windows_style_options_)
-                commandline = detail::find_and_modify(commandline, ":", detail::escape_detect);
-        }
-
-        auto args = detail::split_up(std::move(commandline));
-        // remove all empty strings
-        args.erase(std::remove(args.begin(), args.end(), std::string{}), args.end());
-        std::reverse(args.begin(), args.end());
-
-        parse(std::move(args));
-    }
+    void parse(std::string commandline, bool program_name_included = false);
 
     /// The real work is done here. Expects a reversed vector.
     /// Changes the vector to the remaining options.
-    void parse(std::vector<std::string> &args) {
-        // Clear if parsed
-        if(parsed_ > 0)
-            clear();
-
-        // parsed_ is incremented in commands/subcommands,
-        // but placed here to make sure this is cleared when
-        // running parse after an error is thrown, even by _validate or _configure.
-        parsed_ = 1;
-        _validate();
-        _configure();
-        // set the parent as nullptr as this object should be the top now
-        parent_ = nullptr;
-        parsed_ = 0;
-
-        _parse(args);
-        run_callback();
-    }
+    void parse(std::vector<std::string> &args);
 
     /// The real work is done here. Expects a reversed vector.
-    void parse(std::vector<std::string> &&args) {
-        // Clear if parsed
-        if(parsed_ > 0)
-            clear();
+    void parse(std::vector<std::string> &&args);
 
-        // parsed_ is incremented in commands/subcommands,
-        // but placed here to make sure this is cleared when
-        // running parse after an error is thrown, even by _validate or _configure.
-        parsed_ = 1;
-        _validate();
-        _configure();
-        // set the parent as nullptr as this object should be the top now
-        parent_ = nullptr;
-        parsed_ = 0;
-
-        _parse(std::move(args));
-        run_callback();
-    }
+    void parse_from_stream(std::istream &input);
 
     /// Provide a function to print a help message. The function gets access to the App pointer and error.
     void failure_message(std::function<std::string(const App *, const Error &e)> function) {
         failure_message_ = function;
     }
 
     /// Print a nice error message and return the exit code
-    int exit(const Error &e, std::ostream &out = std::cout, std::ostream &err = std::cerr) const {
-
-        /// Avoid printing anything if this is a CLI::RuntimeError
-        if(e.get_name() == "RuntimeError")
-            return e.get_exit_code();
-
-        if(e.get_name() == "CallForHelp") {
-            out << help();
-            return e.get_exit_code();
-        }
-
-        if(e.get_name() == "CallForAllHelp") {
-            out << help("", AppFormatMode::All);
-            return e.get_exit_code();
-        }
-
-        if(e.get_name() == "CallForVersion") {
-            out << e.what() << std::endl;
-            return e.get_exit_code();
-        }
-
-        if(e.get_exit_code() != static_cast<int>(ExitCodes::Success)) {
-            if(failure_message_)
-                err << failure_message_(this, e) << std::flush;
-        }
-
-        return e.get_exit_code();
-    }
+    int exit(const Error &e, std::ostream &out = std::cout, std::ostream &err = std::cerr) const;
 
     ///@}
     /// @name Post parsing
     ///@{
 
     /// Counts the number of times the given option was passed.
-    std::size_t count(std::string option_name) const { return get_option(option_name)->count(); }
+    CLI11_NODISCARD std::size_t count(std::string option_name) const { return get_option(option_name)->count(); }
 
     /// Get a subcommand pointer list to the currently selected subcommands (after parsing by default, in command
     /// line order; use parsed = false to get the original definition list.)
-    std::vector<App *> get_subcommands() const { return parsed_subcommands_; }
+    CLI11_NODISCARD std::vector<App *> get_subcommands() const { return parsed_subcommands_; }
 
     /// Get a filtered subcommand pointer list from the original definition list. An empty function will provide all
     /// subcommands (const)
-    std::vector<const App *> get_subcommands(const std::function<bool(const App *)> &filter) const {
-        std::vector<const App *> subcomms(subcommands_.size());
-        std::transform(std::begin(subcommands_), std::end(subcommands_), std::begin(subcomms), [](const App_p &v) {
-            return v.get();
-        });
-
-        if(filter) {
-            subcomms.erase(std::remove_if(std::begin(subcomms),
-                                          std::end(subcomms),
-                                          [&filter](const App *app) { return !filter(app); }),
-                           std::end(subcomms));
-        }
-
-        return subcomms;
-    }
+    std::vector<const App *> get_subcommands(const std::function<bool(const App *)> &filter) const;
 
     /// Get a filtered subcommand pointer list from the original definition list. An empty function will provide all
     /// subcommands
-    std::vector<App *> get_subcommands(const std::function<bool(App *)> &filter) {
-        std::vector<App *> subcomms(subcommands_.size());
-        std::transform(std::begin(subcommands_), std::end(subcommands_), std::begin(subcomms), [](const App_p &v) {
-            return v.get();
-        });
-
-        if(filter) {
-            subcomms.erase(
-                std::remove_if(std::begin(subcomms), std::end(subcomms), [&filter](App *app) { return !filter(app); }),
-                std::end(subcomms));
-        }
-
-        return subcomms;
-    }
+    std::vector<App *> get_subcommands(const std::function<bool(App *)> &filter);
 
     /// Check to see if given subcommand was selected
     bool got_subcommand(const App *subcom) const {
         // get subcom needed to verify that this was a real subcommand
         return get_subcommand(subcom)->parsed_ > 0;
     }
 
     /// Check with name instead of pointer to see if subcommand was selected
-    bool got_subcommand(std::string subcommand_name) const { return get_subcommand(subcommand_name)->parsed_ > 0; }
+    CLI11_NODISCARD bool got_subcommand(std::string subcommand_name) const {
+        return get_subcommand(subcommand_name)->parsed_ > 0;
+    }
 
     /// Sets excluded options for the subcommand
     App *excludes(Option *opt) {
         if(opt == nullptr) {
             throw OptionNotFound("nullptr passed");
         }
         exclude_options_.insert(opt);
@@ -6576,55 +6464,24 @@
             throw OptionNotFound("cannot self reference in needs");
         }
         need_subcommands_.insert(app);
         return this;
     }
 
     /// Removes an option from the excludes list of this subcommand
-    bool remove_excludes(Option *opt) {
-        auto iterator = std::find(std::begin(exclude_options_), std::end(exclude_options_), opt);
-        if(iterator == std::end(exclude_options_)) {
-            return false;
-        }
-        exclude_options_.erase(iterator);
-        return true;
-    }
+    bool remove_excludes(Option *opt);
 
     /// Removes a subcommand from the excludes list of this subcommand
-    bool remove_excludes(App *app) {
-        auto iterator = std::find(std::begin(exclude_subcommands_), std::end(exclude_subcommands_), app);
-        if(iterator == std::end(exclude_subcommands_)) {
-            return false;
-        }
-        auto other_app = *iterator;
-        exclude_subcommands_.erase(iterator);
-        other_app->remove_excludes(this);
-        return true;
-    }
+    bool remove_excludes(App *app);
 
     /// Removes an option from the needs list of this subcommand
-    bool remove_needs(Option *opt) {
-        auto iterator = std::find(std::begin(need_options_), std::end(need_options_), opt);
-        if(iterator == std::end(need_options_)) {
-            return false;
-        }
-        need_options_.erase(iterator);
-        return true;
-    }
+    bool remove_needs(Option *opt);
 
     /// Removes a subcommand from the needs list of this subcommand
-    bool remove_needs(App *app) {
-        auto iterator = std::find(std::begin(need_subcommands_), std::end(need_subcommands_), app);
-        if(iterator == std::end(need_subcommands_)) {
-            return false;
-        }
-        need_subcommands_.erase(iterator);
-        return true;
-    }
-
+    bool remove_needs(App *app);
     ///@}
     /// @name Help
     ///@{
 
     /// Set footer.
     App *footer(std::string footer_string) {
         footer_ = std::move(footer_string);
@@ -6633,1638 +6490,2505 @@
     /// Set footer.
     App *footer(std::function<std::string()> footer_function) {
         footer_callback_ = std::move(footer_function);
         return this;
     }
     /// Produce a string that could be read in as a config of the current values of the App. Set default_also to
     /// include default arguments. write_descriptions will print a description for the App and for each option.
-    std::string config_to_str(bool default_also = false, bool write_description = false) const {
+    CLI11_NODISCARD std::string config_to_str(bool default_also = false, bool write_description = false) const {
         return config_formatter_->to_config(this, default_also, write_description, "");
     }
 
     /// Makes a help message, using the currently configured formatter
     /// Will only do one subcommand at a time
-    std::string help(std::string prev = "", AppFormatMode mode = AppFormatMode::Normal) const {
-        if(prev.empty())
-            prev = get_name();
-        else
-            prev += " " + get_name();
-
-        // Delegate to subcommand if needed
-        auto selected_subcommands = get_subcommands();
-        if(!selected_subcommands.empty()) {
-            return selected_subcommands.at(0)->help(prev, mode);
-        }
-        return formatter_->make_help(this, prev, mode);
-    }
+    CLI11_NODISCARD std::string help(std::string prev = "", AppFormatMode mode = AppFormatMode::Normal) const;
 
     /// Displays a version string
-    std::string version() const {
-        std::string val;
-        if(version_ptr_ != nullptr) {
-            auto rv = version_ptr_->results();
-            version_ptr_->clear();
-            version_ptr_->add_result("true");
-            try {
-                version_ptr_->run_callback();
-            } catch(const CLI::CallForVersion &cfv) {
-                val = cfv.what();
-            }
-            version_ptr_->clear();
-            version_ptr_->add_result(rv);
-        }
-        return val;
-    }
+    CLI11_NODISCARD std::string version() const;
     ///@}
     /// @name Getters
     ///@{
 
     /// Access the formatter
-    std::shared_ptr<FormatterBase> get_formatter() const { return formatter_; }
+    CLI11_NODISCARD std::shared_ptr<FormatterBase> get_formatter() const { return formatter_; }
 
     /// Access the config formatter
-    std::shared_ptr<Config> get_config_formatter() const { return config_formatter_; }
+    CLI11_NODISCARD std::shared_ptr<Config> get_config_formatter() const { return config_formatter_; }
 
     /// Access the config formatter as a configBase pointer
-    std::shared_ptr<ConfigBase> get_config_formatter_base() const {
+    CLI11_NODISCARD std::shared_ptr<ConfigBase> get_config_formatter_base() const {
         // This is safer as a dynamic_cast if we have RTTI, as Config -> ConfigBase
-#if defined(__cpp_rtti) || (defined(__GXX_RTTI) && __GXX_RTTI) || (defined(_HAS_STATIC_RTTI) && (_HAS_STATIC_RTTI == 0))
+#if CLI11_USE_STATIC_RTTI == 0
         return std::dynamic_pointer_cast<ConfigBase>(config_formatter_);
 #else
         return std::static_pointer_cast<ConfigBase>(config_formatter_);
 #endif
     }
 
     /// Get the app or subcommand description
-    std::string get_description() const { return description_; }
+    CLI11_NODISCARD std::string get_description() const { return description_; }
 
     /// Set the description of the app
     App *description(std::string app_description) {
         description_ = std::move(app_description);
         return this;
     }
 
     /// Get the list of options (user facing function, so returns raw pointers), has optional filter function
-    std::vector<const Option *> get_options(const std::function<bool(const Option *)> filter = {}) const {
-        std::vector<const Option *> options(options_.size());
-        std::transform(std::begin(options_), std::end(options_), std::begin(options), [](const Option_p &val) {
-            return val.get();
-        });
-
-        if(filter) {
-            options.erase(std::remove_if(std::begin(options),
-                                         std::end(options),
-                                         [&filter](const Option *opt) { return !filter(opt); }),
-                          std::end(options));
-        }
-
-        return options;
-    }
+    std::vector<const Option *> get_options(const std::function<bool(const Option *)> filter = {}) const;
 
     /// Non-const version of the above
-    std::vector<Option *> get_options(const std::function<bool(Option *)> filter = {}) {
-        std::vector<Option *> options(options_.size());
-        std::transform(std::begin(options_), std::end(options_), std::begin(options), [](const Option_p &val) {
-            return val.get();
-        });
-
-        if(filter) {
-            options.erase(
-                std::remove_if(std::begin(options), std::end(options), [&filter](Option *opt) { return !filter(opt); }),
-                std::end(options));
-        }
-
-        return options;
-    }
+    std::vector<Option *> get_options(const std::function<bool(Option *)> filter = {});
 
     /// Get an option by name (noexcept non-const version)
-    Option *get_option_no_throw(std::string option_name) noexcept {
-        for(Option_p &opt : options_) {
-            if(opt->check_name(option_name)) {
-                return opt.get();
-            }
-        }
-        for(auto &subc : subcommands_) {
-            // also check down into nameless subcommands
-            if(subc->get_name().empty()) {
-                auto opt = subc->get_option_no_throw(option_name);
-                if(opt != nullptr) {
-                    return opt;
-                }
-            }
-        }
-        return nullptr;
-    }
+    Option *get_option_no_throw(std::string option_name) noexcept;
 
     /// Get an option by name (noexcept const version)
-    const Option *get_option_no_throw(std::string option_name) const noexcept {
-        for(const Option_p &opt : options_) {
-            if(opt->check_name(option_name)) {
-                return opt.get();
-            }
-        }
-        for(const auto &subc : subcommands_) {
-            // also check down into nameless subcommands
-            if(subc->get_name().empty()) {
-                auto opt = subc->get_option_no_throw(option_name);
-                if(opt != nullptr) {
-                    return opt;
-                }
-            }
-        }
-        return nullptr;
-    }
+    CLI11_NODISCARD const Option *get_option_no_throw(std::string option_name) const noexcept;
 
     /// Get an option by name
-    const Option *get_option(std::string option_name) const {
-        auto opt = get_option_no_throw(option_name);
+    CLI11_NODISCARD const Option *get_option(std::string option_name) const {
+        const auto *opt = get_option_no_throw(option_name);
         if(opt == nullptr) {
             throw OptionNotFound(option_name);
         }
         return opt;
     }
 
     /// Get an option by name (non-const version)
     Option *get_option(std::string option_name) {
-        auto opt = get_option_no_throw(option_name);
+        auto *opt = get_option_no_throw(option_name);
         if(opt == nullptr) {
             throw OptionNotFound(option_name);
         }
         return opt;
     }
 
     /// Shortcut bracket operator for getting a pointer to an option
     const Option *operator[](const std::string &option_name) const { return get_option(option_name); }
 
     /// Shortcut bracket operator for getting a pointer to an option
     const Option *operator[](const char *option_name) const { return get_option(option_name); }
 
     /// Check the status of ignore_case
-    bool get_ignore_case() const { return ignore_case_; }
+    CLI11_NODISCARD bool get_ignore_case() const { return ignore_case_; }
 
     /// Check the status of ignore_underscore
-    bool get_ignore_underscore() const { return ignore_underscore_; }
+    CLI11_NODISCARD bool get_ignore_underscore() const { return ignore_underscore_; }
 
     /// Check the status of fallthrough
-    bool get_fallthrough() const { return fallthrough_; }
+    CLI11_NODISCARD bool get_fallthrough() const { return fallthrough_; }
 
     /// Check the status of the allow windows style options
-    bool get_allow_windows_style_options() const { return allow_windows_style_options_; }
+    CLI11_NODISCARD bool get_allow_windows_style_options() const { return allow_windows_style_options_; }
 
     /// Check the status of the allow windows style options
-    bool get_positionals_at_end() const { return positionals_at_end_; }
+    CLI11_NODISCARD bool get_positionals_at_end() const { return positionals_at_end_; }
 
     /// Check the status of the allow windows style options
-    bool get_configurable() const { return configurable_; }
+    CLI11_NODISCARD bool get_configurable() const { return configurable_; }
 
     /// Get the group of this subcommand
-    const std::string &get_group() const { return group_; }
+    CLI11_NODISCARD const std::string &get_group() const { return group_; }
 
     /// Generate and return the footer.
-    std::string get_footer() const { return (footer_callback_) ? footer_callback_() + '\n' + footer_ : footer_; }
+    CLI11_NODISCARD std::string get_footer() const {
+        return (footer_callback_) ? footer_callback_() + '\n' + footer_ : footer_;
+    }
 
     /// Get the required min subcommand value
-    std::size_t get_require_subcommand_min() const { return require_subcommand_min_; }
+    CLI11_NODISCARD std::size_t get_require_subcommand_min() const { return require_subcommand_min_; }
 
     /// Get the required max subcommand value
-    std::size_t get_require_subcommand_max() const { return require_subcommand_max_; }
+    CLI11_NODISCARD std::size_t get_require_subcommand_max() const { return require_subcommand_max_; }
 
     /// Get the required min option value
-    std::size_t get_require_option_min() const { return require_option_min_; }
+    CLI11_NODISCARD std::size_t get_require_option_min() const { return require_option_min_; }
 
     /// Get the required max option value
-    std::size_t get_require_option_max() const { return require_option_max_; }
+    CLI11_NODISCARD std::size_t get_require_option_max() const { return require_option_max_; }
 
     /// Get the prefix command status
-    bool get_prefix_command() const { return prefix_command_; }
+    CLI11_NODISCARD bool get_prefix_command() const { return prefix_command_; }
 
     /// Get the status of allow extras
-    bool get_allow_extras() const { return allow_extras_; }
+    CLI11_NODISCARD bool get_allow_extras() const { return allow_extras_; }
 
     /// Get the status of required
-    bool get_required() const { return required_; }
+    CLI11_NODISCARD bool get_required() const { return required_; }
 
     /// Get the status of disabled
-    bool get_disabled() const { return disabled_; }
+    CLI11_NODISCARD bool get_disabled() const { return disabled_; }
 
     /// Get the status of silence
-    bool get_silent() const { return silent_; }
+    CLI11_NODISCARD bool get_silent() const { return silent_; }
 
     /// Get the status of disabled
-    bool get_immediate_callback() const { return immediate_callback_; }
+    CLI11_NODISCARD bool get_immediate_callback() const { return immediate_callback_; }
 
     /// Get the status of disabled by default
-    bool get_disabled_by_default() const { return (default_startup == startup_mode::disabled); }
+    CLI11_NODISCARD bool get_disabled_by_default() const { return (default_startup == startup_mode::disabled); }
 
     /// Get the status of disabled by default
-    bool get_enabled_by_default() const { return (default_startup == startup_mode::enabled); }
+    CLI11_NODISCARD bool get_enabled_by_default() const { return (default_startup == startup_mode::enabled); }
     /// Get the status of validating positionals
-    bool get_validate_positionals() const { return validate_positionals_; }
+    CLI11_NODISCARD bool get_validate_positionals() const { return validate_positionals_; }
+    /// Get the status of validating optional vector arguments
+    CLI11_NODISCARD bool get_validate_optional_arguments() const { return validate_optional_arguments_; }
 
     /// Get the status of allow extras
-    config_extras_mode get_allow_config_extras() const { return allow_config_extras_; }
+    CLI11_NODISCARD config_extras_mode get_allow_config_extras() const { return allow_config_extras_; }
 
     /// Get a pointer to the help flag.
     Option *get_help_ptr() { return help_ptr_; }
 
     /// Get a pointer to the help flag. (const)
-    const Option *get_help_ptr() const { return help_ptr_; }
+    CLI11_NODISCARD const Option *get_help_ptr() const { return help_ptr_; }
 
     /// Get a pointer to the help all flag. (const)
-    const Option *get_help_all_ptr() const { return help_all_ptr_; }
+    CLI11_NODISCARD const Option *get_help_all_ptr() const { return help_all_ptr_; }
 
     /// Get a pointer to the config option.
     Option *get_config_ptr() { return config_ptr_; }
 
     /// Get a pointer to the config option. (const)
-    const Option *get_config_ptr() const { return config_ptr_; }
+    CLI11_NODISCARD const Option *get_config_ptr() const { return config_ptr_; }
 
     /// Get a pointer to the version option.
     Option *get_version_ptr() { return version_ptr_; }
 
     /// Get a pointer to the version option. (const)
-    const Option *get_version_ptr() const { return version_ptr_; }
+    CLI11_NODISCARD const Option *get_version_ptr() const { return version_ptr_; }
 
-    /// Get the parent of this subcommand (or nullptr if master app)
+    /// Get the parent of this subcommand (or nullptr if main app)
     App *get_parent() { return parent_; }
 
-    /// Get the parent of this subcommand (or nullptr if master app) (const version)
-    const App *get_parent() const { return parent_; }
+    /// Get the parent of this subcommand (or nullptr if main app) (const version)
+    CLI11_NODISCARD const App *get_parent() const { return parent_; }
 
     /// Get the name of the current app
-    const std::string &get_name() const { return name_; }
+    CLI11_NODISCARD const std::string &get_name() const { return name_; }
 
     /// Get the aliases of the current app
-    const std::vector<std::string> &get_aliases() const { return aliases_; }
+    CLI11_NODISCARD const std::vector<std::string> &get_aliases() const { return aliases_; }
 
     /// clear all the aliases of the current App
     App *clear_aliases() {
         aliases_.clear();
         return this;
     }
 
     /// Get a display name for an app
-    std::string get_display_name(bool with_aliases = false) const {
-        if(name_.empty()) {
-            return std::string("[Option Group: ") + get_group() + "]";
-        }
-        if(aliases_.empty() || !with_aliases || aliases_.empty()) {
-            return name_;
-        }
-        std::string dispname = name_;
-        for(const auto &lalias : aliases_) {
-            dispname.push_back(',');
-            dispname.push_back(' ');
-            dispname.append(lalias);
+    CLI11_NODISCARD std::string get_display_name(bool with_aliases = false) const;
+
+    /// Check the name, case insensitive and underscore insensitive if set
+    CLI11_NODISCARD bool check_name(std::string name_to_check) const;
+
+    /// Get the groups available directly from this option (in order)
+    CLI11_NODISCARD std::vector<std::string> get_groups() const;
+
+    /// This gets a vector of pointers with the original parse order
+    CLI11_NODISCARD const std::vector<Option *> &parse_order() const { return parse_order_; }
+
+    /// This returns the missing options from the current subcommand
+    CLI11_NODISCARD std::vector<std::string> remaining(bool recurse = false) const;
+
+    /// This returns the missing options in a form ready for processing by another command line program
+    CLI11_NODISCARD std::vector<std::string> remaining_for_passthrough(bool recurse = false) const;
+
+    /// This returns the number of remaining options, minus the -- separator
+    CLI11_NODISCARD std::size_t remaining_size(bool recurse = false) const;
+
+    ///@}
+
+  protected:
+    /// Check the options to make sure there are no conflicts.
+    ///
+    /// Currently checks to see if multiple positionals exist with unlimited args and checks if the min and max options
+    /// are feasible
+    void _validate() const;
+
+    /// configure subcommands to enable parsing through the current object
+    /// set the correct fallthrough and prefix for nameless subcommands and manage the automatic enable or disable
+    /// makes sure parent is set correctly
+    void _configure();
+
+    /// Internal function to run (App) callback, bottom up
+    void run_callback(bool final_mode = false, bool suppress_final_callback = false);
+
+    /// Check to see if a subcommand is valid. Give up immediately if subcommand max has been reached.
+    CLI11_NODISCARD bool _valid_subcommand(const std::string &current, bool ignore_used = true) const;
+
+    /// Selects a Classifier enum based on the type of the current argument
+    CLI11_NODISCARD detail::Classifier _recognize(const std::string &current,
+                                                  bool ignore_used_subcommands = true) const;
+
+    // The parse function is now broken into several parts, and part of process
+
+    /// Read and process a configuration file (main app only)
+    void _process_config_file();
+
+    /// Get envname options if not yet passed. Runs on *all* subcommands.
+    void _process_env();
+
+    /// Process callbacks. Runs on *all* subcommands.
+    void _process_callbacks();
+
+    /// Run help flag processing if any are found.
+    ///
+    /// The flags allow recursive calls to remember if there was a help flag on a parent.
+    void _process_help_flags(bool trigger_help = false, bool trigger_all_help = false) const;
+
+    /// Verify required options and cross requirements. Subcommands too (only if selected).
+    void _process_requirements();
+
+    /// Process callbacks and such.
+    void _process();
+
+    /// Throw an error if anything is left over and should not be.
+    void _process_extras();
+
+    /// Throw an error if anything is left over and should not be.
+    /// Modifies the args to fill in the missing items before throwing.
+    void _process_extras(std::vector<std::string> &args);
+
+    /// Internal function to recursively increment the parsed counter on the current app as well unnamed subcommands
+    void increment_parsed();
+
+    /// Internal parse function
+    void _parse(std::vector<std::string> &args);
+
+    /// Internal parse function
+    void _parse(std::vector<std::string> &&args);
+
+    /// Internal function to parse a stream
+    void _parse_stream(std::istream &input);
+
+    /// Parse one config param, return false if not found in any subcommand, remove if it is
+    ///
+    /// If this has more than one dot.separated.name, go into the subcommand matching it
+    /// Returns true if it managed to find the option, if false you'll need to remove the arg manually.
+    void _parse_config(const std::vector<ConfigItem> &args);
+
+    /// Fill in a single config option
+    bool _parse_single_config(const ConfigItem &item, std::size_t level = 0);
+
+    /// Parse "one" argument (some may eat more than one), delegate to parent if fails, add to missing if missing
+    /// from main return false if the parse has failed and needs to return to parent
+    bool _parse_single(std::vector<std::string> &args, bool &positional_only);
+
+    /// Count the required remaining positional arguments
+    CLI11_NODISCARD std::size_t _count_remaining_positionals(bool required_only = false) const;
+
+    /// Count the required remaining positional arguments
+    CLI11_NODISCARD bool _has_remaining_positionals() const;
+
+    /// Parse a positional, go up the tree to check
+    /// @param haltOnSubcommand if set to true the operation will not process subcommands merely return false
+    /// Return true if the positional was used false otherwise
+    bool _parse_positional(std::vector<std::string> &args, bool haltOnSubcommand);
+
+    /// Locate a subcommand by name with two conditions, should disabled subcommands be ignored, and should used
+    /// subcommands be ignored
+    CLI11_NODISCARD App *
+    _find_subcommand(const std::string &subc_name, bool ignore_disabled, bool ignore_used) const noexcept;
+
+    /// Parse a subcommand, modify args and continue
+    ///
+    /// Unlike the others, this one will always allow fallthrough
+    /// return true if the subcommand was processed false otherwise
+    bool _parse_subcommand(std::vector<std::string> &args);
+
+    /// Parse a short (false) or long (true) argument, must be at the top of the list
+    /// return true if the argument was processed or false if nothing was done
+    bool _parse_arg(std::vector<std::string> &args, detail::Classifier current_type);
+
+    /// Trigger the pre_parse callback if needed
+    void _trigger_pre_parse(std::size_t remaining_args);
+
+    /// Get the appropriate parent to fallthrough to which is the first one that has a name or the main app
+    App *_get_fallthrough_parent();
+
+    /// Helper function to run through all possible comparisons of subcommand names to check there is no overlap
+    CLI11_NODISCARD const std::string &_compare_subcommand_names(const App &subcom, const App &base) const;
+
+    /// Helper function to place extra values in the most appropriate position
+    void _move_to_missing(detail::Classifier val_type, const std::string &val);
+
+  public:
+    /// function that could be used by subclasses of App to shift options around into subcommands
+    void _move_option(Option *opt, App *app);
+};  // namespace CLI
+
+/// Extension of App to better manage groups of options
+class Option_group : public App {
+  public:
+    Option_group(std::string group_description, std::string group_name, App *parent)
+        : App(std::move(group_description), "", parent) {
+        group(group_name);
+        // option groups should have automatic fallthrough
+    }
+    using App::add_option;
+    /// Add an existing option to the Option_group
+    Option *add_option(Option *opt) {
+        if(get_parent() == nullptr) {
+            throw OptionNotFound("Unable to locate the specified option");
         }
-        return dispname;
+        get_parent()->_move_option(opt, this);
+        return opt;
+    }
+    /// Add an existing option to the Option_group
+    void add_options(Option *opt) { add_option(opt); }
+    /// Add a bunch of options to the group
+    template <typename... Args> void add_options(Option *opt, Args... args) {
+        add_option(opt);
+        add_options(args...);
+    }
+    using App::add_subcommand;
+    /// Add an existing subcommand to be a member of an option_group
+    App *add_subcommand(App *subcom) {
+        App_p subc = subcom->get_parent()->get_subcommand_ptr(subcom);
+        subc->get_parent()->remove_subcommand(subcom);
+        add_subcommand(std::move(subc));
+        return subcom;
     }
+};
 
-    /// Check the name, case insensitive and underscore insensitive if set
-    bool check_name(std::string name_to_check) const {
-        std::string local_name = name_;
-        if(ignore_underscore_) {
-            local_name = detail::remove_underscore(name_);
-            name_to_check = detail::remove_underscore(name_to_check);
+/// Helper function to enable one option group/subcommand when another is used
+CLI11_INLINE void TriggerOn(App *trigger_app, App *app_to_enable);
+
+/// Helper function to enable one option group/subcommand when another is used
+CLI11_INLINE void TriggerOn(App *trigger_app, std::vector<App *> apps_to_enable);
+
+/// Helper function to disable one option group/subcommand when another is used
+CLI11_INLINE void TriggerOff(App *trigger_app, App *app_to_enable);
+
+/// Helper function to disable one option group/subcommand when another is used
+CLI11_INLINE void TriggerOff(App *trigger_app, std::vector<App *> apps_to_enable);
+
+/// Helper function to mark an option as deprecated
+CLI11_INLINE void deprecate_option(Option *opt, const std::string &replacement = "");
+
+/// Helper function to mark an option as deprecated
+inline void deprecate_option(App *app, const std::string &option_name, const std::string &replacement = "") {
+    auto *opt = app->get_option(option_name);
+    deprecate_option(opt, replacement);
+}
+
+/// Helper function to mark an option as deprecated
+inline void deprecate_option(App &app, const std::string &option_name, const std::string &replacement = "") {
+    auto *opt = app.get_option(option_name);
+    deprecate_option(opt, replacement);
+}
+
+/// Helper function to mark an option as retired
+CLI11_INLINE void retire_option(App *app, Option *opt);
+
+/// Helper function to mark an option as retired
+CLI11_INLINE void retire_option(App &app, Option *opt);
+
+/// Helper function to mark an option as retired
+CLI11_INLINE void retire_option(App *app, const std::string &option_name);
+
+/// Helper function to mark an option as retired
+CLI11_INLINE void retire_option(App &app, const std::string &option_name);
+
+namespace detail {
+/// This class is simply to allow tests access to App's protected functions
+struct AppFriend {
+#ifdef CLI11_CPP14
+
+    /// Wrap _parse_short, perfectly forward arguments and return
+    template <typename... Args> static decltype(auto) parse_arg(App *app, Args &&...args) {
+        return app->_parse_arg(std::forward<Args>(args)...);
+    }
+
+    /// Wrap _parse_subcommand, perfectly forward arguments and return
+    template <typename... Args> static decltype(auto) parse_subcommand(App *app, Args &&...args) {
+        return app->_parse_subcommand(std::forward<Args>(args)...);
+    }
+#else
+    /// Wrap _parse_short, perfectly forward arguments and return
+    template <typename... Args>
+    static auto parse_arg(App *app, Args &&...args) ->
+        typename std::result_of<decltype (&App::_parse_arg)(App, Args...)>::type {
+        return app->_parse_arg(std::forward<Args>(args)...);
+    }
+
+    /// Wrap _parse_subcommand, perfectly forward arguments and return
+    template <typename... Args>
+    static auto parse_subcommand(App *app, Args &&...args) ->
+        typename std::result_of<decltype (&App::_parse_subcommand)(App, Args...)>::type {
+        return app->_parse_subcommand(std::forward<Args>(args)...);
+    }
+#endif
+    /// Wrap the fallthrough parent function to make sure that is working correctly
+    static App *get_fallthrough_parent(App *app) { return app->_get_fallthrough_parent(); }
+};
+}  // namespace detail
+
+
+
+
+CLI11_INLINE App::App(std::string app_description, std::string app_name, App *parent)
+    : name_(std::move(app_name)), description_(std::move(app_description)), parent_(parent) {
+    // Inherit if not from a nullptr
+    if(parent_ != nullptr) {
+        if(parent_->help_ptr_ != nullptr)
+            set_help_flag(parent_->help_ptr_->get_name(false, true), parent_->help_ptr_->get_description());
+        if(parent_->help_all_ptr_ != nullptr)
+            set_help_all_flag(parent_->help_all_ptr_->get_name(false, true), parent_->help_all_ptr_->get_description());
+
+        /// OptionDefaults
+        option_defaults_ = parent_->option_defaults_;
+
+        // INHERITABLE
+        failure_message_ = parent_->failure_message_;
+        allow_extras_ = parent_->allow_extras_;
+        allow_config_extras_ = parent_->allow_config_extras_;
+        prefix_command_ = parent_->prefix_command_;
+        immediate_callback_ = parent_->immediate_callback_;
+        ignore_case_ = parent_->ignore_case_;
+        ignore_underscore_ = parent_->ignore_underscore_;
+        fallthrough_ = parent_->fallthrough_;
+        validate_positionals_ = parent_->validate_positionals_;
+        validate_optional_arguments_ = parent_->validate_optional_arguments_;
+        configurable_ = parent_->configurable_;
+        allow_windows_style_options_ = parent_->allow_windows_style_options_;
+        group_ = parent_->group_;
+        footer_ = parent_->footer_;
+        formatter_ = parent_->formatter_;
+        config_formatter_ = parent_->config_formatter_;
+        require_subcommand_max_ = parent_->require_subcommand_max_;
+    }
+}
+
+CLI11_INLINE App *App::name(std::string app_name) {
+
+    if(parent_ != nullptr) {
+        auto oname = name_;
+        name_ = app_name;
+        const auto &res = _compare_subcommand_names(*this, *_get_fallthrough_parent());
+        if(!res.empty()) {
+            name_ = oname;
+            throw(OptionAlreadyAdded(app_name + " conflicts with existing subcommand names"));
         }
-        if(ignore_case_) {
-            local_name = detail::to_lower(name_);
-            name_to_check = detail::to_lower(name_to_check);
+    } else {
+        name_ = app_name;
+    }
+    has_automatic_name_ = false;
+    return this;
+}
+
+CLI11_INLINE App *App::alias(std::string app_name) {
+    if(app_name.empty() || !detail::valid_alias_name_string(app_name)) {
+        throw IncorrectConstruction("Aliases may not be empty or contain newlines or null characters");
+    }
+    if(parent_ != nullptr) {
+        aliases_.push_back(app_name);
+        const auto &res = _compare_subcommand_names(*this, *_get_fallthrough_parent());
+        if(!res.empty()) {
+            aliases_.pop_back();
+            throw(OptionAlreadyAdded("alias already matches an existing subcommand: " + app_name));
         }
+    } else {
+        aliases_.push_back(app_name);
+    }
 
-        if(local_name == name_to_check) {
-            return true;
+    return this;
+}
+
+CLI11_INLINE App *App::immediate_callback(bool immediate) {
+    immediate_callback_ = immediate;
+    if(immediate_callback_) {
+        if(final_callback_ && !(parse_complete_callback_)) {
+            std::swap(final_callback_, parse_complete_callback_);
         }
-        for(auto les : aliases_) {
-            if(ignore_underscore_) {
-                les = detail::remove_underscore(les);
-            }
-            if(ignore_case_) {
-                les = detail::to_lower(les);
-            }
-            if(les == name_to_check) {
-                return true;
-            }
+    } else if(!(final_callback_) && parse_complete_callback_) {
+        std::swap(final_callback_, parse_complete_callback_);
+    }
+    return this;
+}
+
+CLI11_INLINE App *App::ignore_case(bool value) {
+    if(value && !ignore_case_) {
+        ignore_case_ = true;
+        auto *p = (parent_ != nullptr) ? _get_fallthrough_parent() : this;
+        const auto &match = _compare_subcommand_names(*this, *p);
+        if(!match.empty()) {
+            ignore_case_ = false;  // we are throwing so need to be exception invariant
+            throw OptionAlreadyAdded("ignore case would cause subcommand name conflicts: " + match);
         }
-        return false;
     }
+    ignore_case_ = value;
+    return this;
+}
 
-    /// Get the groups available directly from this option (in order)
-    std::vector<std::string> get_groups() const {
-        std::vector<std::string> groups;
+CLI11_INLINE App *App::ignore_underscore(bool value) {
+    if(value && !ignore_underscore_) {
+        ignore_underscore_ = true;
+        auto *p = (parent_ != nullptr) ? _get_fallthrough_parent() : this;
+        const auto &match = _compare_subcommand_names(*this, *p);
+        if(!match.empty()) {
+            ignore_underscore_ = false;
+            throw OptionAlreadyAdded("ignore underscore would cause subcommand name conflicts: " + match);
+        }
+    }
+    ignore_underscore_ = value;
+    return this;
+}
 
-        for(const Option_p &opt : options_) {
-            // Add group if it is not already in there
-            if(std::find(groups.begin(), groups.end(), opt->get_group()) == groups.end()) {
-                groups.push_back(opt->get_group());
-            }
+CLI11_INLINE Option *App::add_option(std::string option_name,
+                                     callback_t option_callback,
+                                     std::string option_description,
+                                     bool defaulted,
+                                     std::function<std::string()> func) {
+    Option myopt{option_name, option_description, option_callback, this};
+
+    if(std::find_if(std::begin(options_), std::end(options_), [&myopt](const Option_p &v) { return *v == myopt; }) ==
+       std::end(options_)) {
+        options_.emplace_back();
+        Option_p &option = options_.back();
+        option.reset(new Option(option_name, option_description, option_callback, this));
+
+        // Set the default string capture function
+        option->default_function(func);
+
+        // For compatibility with CLI11 1.7 and before, capture the default string here
+        if(defaulted)
+            option->capture_default_str();
+
+        // Transfer defaults to the new option
+        option_defaults_.copy_to(option.get());
+
+        // Don't bother to capture if we already did
+        if(!defaulted && option->get_always_capture_default())
+            option->capture_default_str();
+
+        return option.get();
+    }
+    // we know something matches now find what it is so we can produce more error information
+    for(auto &opt : options_) {
+        const auto &matchname = opt->matching_name(myopt);
+        if(!matchname.empty()) {
+            throw(OptionAlreadyAdded("added option matched existing option name: " + matchname));
         }
+    }
+    // this line should not be reached the above loop should trigger the throw
+    throw(OptionAlreadyAdded("added option matched existing option name"));  // LCOV_EXCL_LINE
+}
 
-        return groups;
+CLI11_INLINE Option *App::set_help_flag(std::string flag_name, const std::string &help_description) {
+    // take flag_description by const reference otherwise add_flag tries to assign to help_description
+    if(help_ptr_ != nullptr) {
+        remove_option(help_ptr_);
+        help_ptr_ = nullptr;
     }
 
-    /// This gets a vector of pointers with the original parse order
-    const std::vector<Option *> &parse_order() const { return parse_order_; }
+    // Empty name will simply remove the help flag
+    if(!flag_name.empty()) {
+        help_ptr_ = add_flag(flag_name, help_description);
+        help_ptr_->configurable(false);
+    }
 
-    /// This returns the missing options from the current subcommand
-    std::vector<std::string> remaining(bool recurse = false) const {
-        std::vector<std::string> miss_list;
-        for(const std::pair<detail::Classifier, std::string> &miss : missing_) {
-            miss_list.push_back(std::get<1>(miss));
-        }
-        // Get from a subcommand that may allow extras
-        if(recurse) {
-            if(!allow_extras_) {
-                for(const auto &sub : subcommands_) {
-                    if(sub->name_.empty() && !sub->missing_.empty()) {
-                        for(const std::pair<detail::Classifier, std::string> &miss : sub->missing_) {
-                            miss_list.push_back(std::get<1>(miss));
-                        }
-                    }
-                }
-            }
-            // Recurse into subcommands
+    return help_ptr_;
+}
 
-            for(const App *sub : parsed_subcommands_) {
-                std::vector<std::string> output = sub->remaining(recurse);
-                std::copy(std::begin(output), std::end(output), std::back_inserter(miss_list));
-            }
-        }
-        return miss_list;
+CLI11_INLINE Option *App::set_help_all_flag(std::string help_name, const std::string &help_description) {
+    // take flag_description by const reference otherwise add_flag tries to assign to flag_description
+    if(help_all_ptr_ != nullptr) {
+        remove_option(help_all_ptr_);
+        help_all_ptr_ = nullptr;
     }
 
-    /// This returns the missing options in a form ready for processing by another command line program
-    std::vector<std::string> remaining_for_passthrough(bool recurse = false) const {
-        std::vector<std::string> miss_list = remaining(recurse);
-        std::reverse(std::begin(miss_list), std::end(miss_list));
-        return miss_list;
+    // Empty name will simply remove the help all flag
+    if(!help_name.empty()) {
+        help_all_ptr_ = add_flag(help_name, help_description);
+        help_all_ptr_->configurable(false);
     }
 
-    /// This returns the number of remaining options, minus the -- separator
-    std::size_t remaining_size(bool recurse = false) const {
-        auto remaining_options = static_cast<std::size_t>(std::count_if(
-            std::begin(missing_), std::end(missing_), [](const std::pair<detail::Classifier, std::string> &val) {
-                return val.first != detail::Classifier::POSITIONAL_MARK;
-            }));
-
-        if(recurse) {
-            for(const App_p &sub : subcommands_) {
-                remaining_options += sub->remaining_size(recurse);
-            }
-        }
-        return remaining_options;
+    return help_all_ptr_;
+}
+
+CLI11_INLINE Option *
+App::set_version_flag(std::string flag_name, const std::string &versionString, const std::string &version_help) {
+    // take flag_description by const reference otherwise add_flag tries to assign to version_description
+    if(version_ptr_ != nullptr) {
+        remove_option(version_ptr_);
+        version_ptr_ = nullptr;
     }
 
-    ///@}
+    // Empty name will simply remove the version flag
+    if(!flag_name.empty()) {
+        version_ptr_ = add_flag_callback(
+            flag_name, [versionString]() { throw(CLI::CallForVersion(versionString, 0)); }, version_help);
+        version_ptr_->configurable(false);
+    }
 
-  protected:
-    /// Check the options to make sure there are no conflicts.
-    ///
-    /// Currently checks to see if multiple positionals exist with unlimited args and checks if the min and max options
-    /// are feasible
-    void _validate() const {
-        // count the number of positional only args
-        auto pcount = std::count_if(std::begin(options_), std::end(options_), [](const Option_p &opt) {
-            return opt->get_items_expected_max() >= detail::expected_max_vector_size && !opt->nonpositional();
-        });
-        if(pcount > 1) {
-            auto pcount_req = std::count_if(std::begin(options_), std::end(options_), [](const Option_p &opt) {
-                return opt->get_items_expected_max() >= detail::expected_max_vector_size && !opt->nonpositional() &&
-                       opt->get_required();
-            });
-            if(pcount - pcount_req > 1) {
-                throw InvalidError(name_);
-            }
+    return version_ptr_;
+}
+
+CLI11_INLINE Option *
+App::set_version_flag(std::string flag_name, std::function<std::string()> vfunc, const std::string &version_help) {
+    if(version_ptr_ != nullptr) {
+        remove_option(version_ptr_);
+        version_ptr_ = nullptr;
+    }
+
+    // Empty name will simply remove the version flag
+    if(!flag_name.empty()) {
+        version_ptr_ = add_flag_callback(
+            flag_name, [vfunc]() { throw(CLI::CallForVersion(vfunc(), 0)); }, version_help);
+        version_ptr_->configurable(false);
+    }
+
+    return version_ptr_;
+}
+
+CLI11_INLINE Option *App::_add_flag_internal(std::string flag_name, CLI::callback_t fun, std::string flag_description) {
+    Option *opt = nullptr;
+    if(detail::has_default_flag_values(flag_name)) {
+        // check for default values and if it has them
+        auto flag_defaults = detail::get_default_flag_values(flag_name);
+        detail::remove_default_flag_values(flag_name);
+        opt = add_option(std::move(flag_name), std::move(fun), std::move(flag_description), false);
+        for(const auto &fname : flag_defaults)
+            opt->fnames_.push_back(fname.first);
+        opt->default_flag_values_ = std::move(flag_defaults);
+    } else {
+        opt = add_option(std::move(flag_name), std::move(fun), std::move(flag_description), false);
+    }
+    // flags cannot have positional values
+    if(opt->get_positional()) {
+        auto pos_name = opt->get_name(true);
+        remove_option(opt);
+        throw IncorrectConstruction::PositionalFlag(pos_name);
+    }
+    opt->multi_option_policy(MultiOptionPolicy::TakeLast);
+    opt->expected(0);
+    opt->required(false);
+    return opt;
+}
+
+CLI11_INLINE Option *App::add_flag_callback(std::string flag_name,
+                                            std::function<void(void)> function,  ///< A function to call, void(void)
+                                            std::string flag_description) {
+
+    CLI::callback_t fun = [function](const CLI::results_t &res) {
+        using CLI::detail::lexical_cast;
+        bool trigger{false};
+        auto result = lexical_cast(res[0], trigger);
+        if(result && trigger) {
+            function();
         }
+        return result;
+    };
+    return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description));
+}
+
+CLI11_INLINE Option *
+App::add_flag_function(std::string flag_name,
+                       std::function<void(std::int64_t)> function,  ///< A function to call, void(int)
+                       std::string flag_description) {
+
+    CLI::callback_t fun = [function](const CLI::results_t &res) {
+        using CLI::detail::lexical_cast;
+        std::int64_t flag_count{0};
+        lexical_cast(res[0], flag_count);
+        function(flag_count);
+        return true;
+    };
+    return _add_flag_internal(flag_name, std::move(fun), std::move(flag_description))
+        ->multi_option_policy(MultiOptionPolicy::Sum);
+}
+
+CLI11_INLINE Option *App::set_config(std::string option_name,
+                                     std::string default_filename,
+                                     const std::string &help_message,
+                                     bool config_required) {
 
-        std::size_t nameless_subs{0};
-        for(const App_p &app : subcommands_) {
-            app->_validate();
-            if(app->get_name().empty())
-                ++nameless_subs;
+    // Remove existing config if present
+    if(config_ptr_ != nullptr) {
+        remove_option(config_ptr_);
+        config_ptr_ = nullptr;  // need to remove the config_ptr completely
+    }
+
+    // Only add config if option passed
+    if(!option_name.empty()) {
+        config_ptr_ = add_option(option_name, help_message);
+        if(config_required) {
+            config_ptr_->required();
+        }
+        if(!default_filename.empty()) {
+            config_ptr_->default_str(std::move(default_filename));
         }
+        config_ptr_->configurable(false);
+    }
 
-        if(require_option_min_ > 0) {
-            if(require_option_max_ > 0) {
-                if(require_option_max_ < require_option_min_) {
-                    throw(InvalidError("Required min options greater than required max options",
-                                       ExitCodes::InvalidError));
-                }
-            }
-            if(require_option_min_ > (options_.size() + nameless_subs)) {
-                throw(InvalidError("Required min options greater than number of available options",
-                                   ExitCodes::InvalidError));
+    return config_ptr_;
+}
+
+CLI11_INLINE bool App::remove_option(Option *opt) {
+    // Make sure no links exist
+    for(Option_p &op : options_) {
+        op->remove_needs(opt);
+        op->remove_excludes(opt);
+    }
+
+    if(help_ptr_ == opt)
+        help_ptr_ = nullptr;
+    if(help_all_ptr_ == opt)
+        help_all_ptr_ = nullptr;
+
+    auto iterator =
+        std::find_if(std::begin(options_), std::end(options_), [opt](const Option_p &v) { return v.get() == opt; });
+    if(iterator != std::end(options_)) {
+        options_.erase(iterator);
+        return true;
+    }
+    return false;
+}
+
+CLI11_INLINE App *App::add_subcommand(std::string subcommand_name, std::string subcommand_description) {
+    if(!subcommand_name.empty() && !detail::valid_name_string(subcommand_name)) {
+        if(!detail::valid_first_char(subcommand_name[0])) {
+            throw IncorrectConstruction("Subcommand name starts with invalid character, '!' and '-' are not allowed");
+        }
+        for(auto c : subcommand_name) {
+            if(!detail::valid_later_char(c)) {
+                throw IncorrectConstruction(std::string("Subcommand name contains invalid character ('") + c +
+                                            "'), all characters are allowed except"
+                                            "'=',':','{','}', and ' '");
             }
         }
     }
+    CLI::App_p subcom = std::shared_ptr<App>(new App(std::move(subcommand_description), subcommand_name, this));
+    return add_subcommand(std::move(subcom));
+}
 
-    /// configure subcommands to enable parsing through the current object
-    /// set the correct fallthrough and prefix for nameless subcommands and manage the automatic enable or disable
-    /// makes sure parent is set correctly
-    void _configure() {
-        if(default_startup == startup_mode::enabled) {
-            disabled_ = false;
-        } else if(default_startup == startup_mode::disabled) {
-            disabled_ = true;
-        }
-        for(const App_p &app : subcommands_) {
-            if(app->has_automatic_name_) {
-                app->name_.clear();
-            }
-            if(app->name_.empty()) {
-                app->fallthrough_ = false;  // make sure fallthrough_ is false to prevent infinite loop
-                app->prefix_command_ = false;
-            }
-            // make sure the parent is set to be this object in preparation for parse
-            app->parent_ = this;
-            app->_configure();
+CLI11_INLINE App *App::add_subcommand(CLI::App_p subcom) {
+    if(!subcom)
+        throw IncorrectConstruction("passed App is not valid");
+    auto *ckapp = (name_.empty() && parent_ != nullptr) ? _get_fallthrough_parent() : this;
+    const auto &mstrg = _compare_subcommand_names(*subcom, *ckapp);
+    if(!mstrg.empty()) {
+        throw(OptionAlreadyAdded("subcommand name or alias matches existing subcommand: " + mstrg));
+    }
+    subcom->parent_ = this;
+    subcommands_.push_back(std::move(subcom));
+    return subcommands_.back().get();
+}
+
+CLI11_INLINE bool App::remove_subcommand(App *subcom) {
+    // Make sure no links exist
+    for(App_p &sub : subcommands_) {
+        sub->remove_excludes(subcom);
+        sub->remove_needs(subcom);
+    }
+
+    auto iterator = std::find_if(
+        std::begin(subcommands_), std::end(subcommands_), [subcom](const App_p &v) { return v.get() == subcom; });
+    if(iterator != std::end(subcommands_)) {
+        subcommands_.erase(iterator);
+        return true;
+    }
+    return false;
+}
+
+CLI11_INLINE App *App::get_subcommand(const App *subcom) const {
+    if(subcom == nullptr)
+        throw OptionNotFound("nullptr passed");
+    for(const App_p &subcomptr : subcommands_)
+        if(subcomptr.get() == subcom)
+            return subcomptr.get();
+    throw OptionNotFound(subcom->get_name());
+}
+
+CLI11_NODISCARD CLI11_INLINE App *App::get_subcommand(std::string subcom) const {
+    auto *subc = _find_subcommand(subcom, false, false);
+    if(subc == nullptr)
+        throw OptionNotFound(subcom);
+    return subc;
+}
+
+CLI11_NODISCARD CLI11_INLINE App *App::get_subcommand(int index) const {
+    if(index >= 0) {
+        auto uindex = static_cast<unsigned>(index);
+        if(uindex < subcommands_.size())
+            return subcommands_[uindex].get();
+    }
+    throw OptionNotFound(std::to_string(index));
+}
+
+CLI11_INLINE CLI::App_p App::get_subcommand_ptr(App *subcom) const {
+    if(subcom == nullptr)
+        throw OptionNotFound("nullptr passed");
+    for(const App_p &subcomptr : subcommands_)
+        if(subcomptr.get() == subcom)
+            return subcomptr;
+    throw OptionNotFound(subcom->get_name());
+}
+
+CLI11_NODISCARD CLI11_INLINE CLI::App_p App::get_subcommand_ptr(std::string subcom) const {
+    for(const App_p &subcomptr : subcommands_)
+        if(subcomptr->check_name(subcom))
+            return subcomptr;
+    throw OptionNotFound(subcom);
+}
+
+CLI11_NODISCARD CLI11_INLINE CLI::App_p App::get_subcommand_ptr(int index) const {
+    if(index >= 0) {
+        auto uindex = static_cast<unsigned>(index);
+        if(uindex < subcommands_.size())
+            return subcommands_[uindex];
+    }
+    throw OptionNotFound(std::to_string(index));
+}
+
+CLI11_NODISCARD CLI11_INLINE CLI::App *App::get_option_group(std::string group_name) const {
+    for(const App_p &app : subcommands_) {
+        if(app->name_.empty() && app->group_ == group_name) {
+            return app.get();
         }
     }
+    throw OptionNotFound(group_name);
+}
 
-    /// Internal function to run (App) callback, bottom up
-    void run_callback(bool final_mode = false, bool suppress_final_callback = false) {
-        pre_callback();
-        // in the main app if immediate_callback_ is set it runs the main callback before the used subcommands
-        if(!final_mode && parse_complete_callback_) {
-            parse_complete_callback_();
+CLI11_NODISCARD CLI11_INLINE std::size_t App::count_all() const {
+    std::size_t cnt{0};
+    for(const auto &opt : options_) {
+        cnt += opt->count();
+    }
+    for(const auto &sub : subcommands_) {
+        cnt += sub->count_all();
+    }
+    if(!get_name().empty()) {  // for named subcommands add the number of times the subcommand was called
+        cnt += parsed_;
+    }
+    return cnt;
+}
+
+CLI11_INLINE void App::clear() {
+
+    parsed_ = 0;
+    pre_parse_called_ = false;
+
+    missing_.clear();
+    parsed_subcommands_.clear();
+    for(const Option_p &opt : options_) {
+        opt->clear();
+    }
+    for(const App_p &subc : subcommands_) {
+        subc->clear();
+    }
+}
+
+CLI11_INLINE void App::parse(int argc, const char *const *argv) {
+    // If the name is not set, read from command line
+    if(name_.empty() || has_automatic_name_) {
+        has_automatic_name_ = true;
+        name_ = argv[0];
+    }
+
+    std::vector<std::string> args;
+    args.reserve(static_cast<std::size_t>(argc) - 1U);
+    for(auto i = static_cast<std::size_t>(argc) - 1U; i > 0U; --i)
+        args.emplace_back(argv[i]);
+    parse(std::move(args));
+}
+
+CLI11_INLINE void App::parse(std::string commandline, bool program_name_included) {
+
+    if(program_name_included) {
+        auto nstr = detail::split_program_name(commandline);
+        if((name_.empty()) || (has_automatic_name_)) {
+            has_automatic_name_ = true;
+            name_ = nstr.first;
         }
-        // run the callbacks for the received subcommands
-        for(App *subc : get_subcommands()) {
-            subc->run_callback(true, suppress_final_callback);
+        commandline = std::move(nstr.second);
+    } else {
+        detail::trim(commandline);
+    }
+    // the next section of code is to deal with quoted arguments after an '=' or ':' for windows like operations
+    if(!commandline.empty()) {
+        commandline = detail::find_and_modify(commandline, "=", detail::escape_detect);
+        if(allow_windows_style_options_)
+            commandline = detail::find_and_modify(commandline, ":", detail::escape_detect);
+    }
+
+    auto args = detail::split_up(std::move(commandline));
+    // remove all empty strings
+    args.erase(std::remove(args.begin(), args.end(), std::string{}), args.end());
+    std::reverse(args.begin(), args.end());
+
+    parse(std::move(args));
+}
+
+CLI11_INLINE void App::parse(std::vector<std::string> &args) {
+    // Clear if parsed
+    if(parsed_ > 0)
+        clear();
+
+    // parsed_ is incremented in commands/subcommands,
+    // but placed here to make sure this is cleared when
+    // running parse after an error is thrown, even by _validate or _configure.
+    parsed_ = 1;
+    _validate();
+    _configure();
+    // set the parent as nullptr as this object should be the top now
+    parent_ = nullptr;
+    parsed_ = 0;
+
+    _parse(args);
+    run_callback();
+}
+
+CLI11_INLINE void App::parse(std::vector<std::string> &&args) {
+    // Clear if parsed
+    if(parsed_ > 0)
+        clear();
+
+    // parsed_ is incremented in commands/subcommands,
+    // but placed here to make sure this is cleared when
+    // running parse after an error is thrown, even by _validate or _configure.
+    parsed_ = 1;
+    _validate();
+    _configure();
+    // set the parent as nullptr as this object should be the top now
+    parent_ = nullptr;
+    parsed_ = 0;
+
+    _parse(std::move(args));
+    run_callback();
+}
+
+CLI11_INLINE void App::parse_from_stream(std::istream &input) {
+    if(parsed_ == 0) {
+        _validate();
+        _configure();
+        // set the parent as nullptr as this object should be the top now
+    }
+
+    _parse_stream(input);
+    run_callback();
+}
+
+CLI11_INLINE int App::exit(const Error &e, std::ostream &out, std::ostream &err) const {
+
+    /// Avoid printing anything if this is a CLI::RuntimeError
+    if(e.get_name() == "RuntimeError")
+        return e.get_exit_code();
+
+    if(e.get_name() == "CallForHelp") {
+        out << help();
+        return e.get_exit_code();
+    }
+
+    if(e.get_name() == "CallForAllHelp") {
+        out << help("", AppFormatMode::All);
+        return e.get_exit_code();
+    }
+
+    if(e.get_name() == "CallForVersion") {
+        out << e.what() << std::endl;
+        return e.get_exit_code();
+    }
+
+    if(e.get_exit_code() != static_cast<int>(ExitCodes::Success)) {
+        if(failure_message_)
+            err << failure_message_(this, e) << std::flush;
+    }
+
+    return e.get_exit_code();
+}
+
+CLI11_INLINE std::vector<const App *> App::get_subcommands(const std::function<bool(const App *)> &filter) const {
+    std::vector<const App *> subcomms(subcommands_.size());
+    std::transform(
+        std::begin(subcommands_), std::end(subcommands_), std::begin(subcomms), [](const App_p &v) { return v.get(); });
+
+    if(filter) {
+        subcomms.erase(std::remove_if(std::begin(subcomms),
+                                      std::end(subcomms),
+                                      [&filter](const App *app) { return !filter(app); }),
+                       std::end(subcomms));
+    }
+
+    return subcomms;
+}
+
+CLI11_INLINE std::vector<App *> App::get_subcommands(const std::function<bool(App *)> &filter) {
+    std::vector<App *> subcomms(subcommands_.size());
+    std::transform(
+        std::begin(subcommands_), std::end(subcommands_), std::begin(subcomms), [](const App_p &v) { return v.get(); });
+
+    if(filter) {
+        subcomms.erase(
+            std::remove_if(std::begin(subcomms), std::end(subcomms), [&filter](App *app) { return !filter(app); }),
+            std::end(subcomms));
+    }
+
+    return subcomms;
+}
+
+CLI11_INLINE bool App::remove_excludes(Option *opt) {
+    auto iterator = std::find(std::begin(exclude_options_), std::end(exclude_options_), opt);
+    if(iterator == std::end(exclude_options_)) {
+        return false;
+    }
+    exclude_options_.erase(iterator);
+    return true;
+}
+
+CLI11_INLINE bool App::remove_excludes(App *app) {
+    auto iterator = std::find(std::begin(exclude_subcommands_), std::end(exclude_subcommands_), app);
+    if(iterator == std::end(exclude_subcommands_)) {
+        return false;
+    }
+    auto *other_app = *iterator;
+    exclude_subcommands_.erase(iterator);
+    other_app->remove_excludes(this);
+    return true;
+}
+
+CLI11_INLINE bool App::remove_needs(Option *opt) {
+    auto iterator = std::find(std::begin(need_options_), std::end(need_options_), opt);
+    if(iterator == std::end(need_options_)) {
+        return false;
+    }
+    need_options_.erase(iterator);
+    return true;
+}
+
+CLI11_INLINE bool App::remove_needs(App *app) {
+    auto iterator = std::find(std::begin(need_subcommands_), std::end(need_subcommands_), app);
+    if(iterator == std::end(need_subcommands_)) {
+        return false;
+    }
+    need_subcommands_.erase(iterator);
+    return true;
+}
+
+CLI11_NODISCARD CLI11_INLINE std::string App::help(std::string prev, AppFormatMode mode) const {
+    if(prev.empty())
+        prev = get_name();
+    else
+        prev += " " + get_name();
+
+    // Delegate to subcommand if needed
+    auto selected_subcommands = get_subcommands();
+    if(!selected_subcommands.empty()) {
+        return selected_subcommands.back()->help(prev, mode);
+    }
+    return formatter_->make_help(this, prev, mode);
+}
+
+CLI11_NODISCARD CLI11_INLINE std::string App::version() const {
+    std::string val;
+    if(version_ptr_ != nullptr) {
+        auto rv = version_ptr_->results();
+        version_ptr_->clear();
+        version_ptr_->add_result("true");
+        try {
+            version_ptr_->run_callback();
+        } catch(const CLI::CallForVersion &cfv) {
+            val = cfv.what();
         }
-        // now run callbacks for option_groups
-        for(auto &subc : subcommands_) {
-            if(subc->name_.empty() && subc->count_all() > 0) {
-                subc->run_callback(true, suppress_final_callback);
+        version_ptr_->clear();
+        version_ptr_->add_result(rv);
+    }
+    return val;
+}
+
+CLI11_INLINE std::vector<const Option *> App::get_options(const std::function<bool(const Option *)> filter) const {
+    std::vector<const Option *> options(options_.size());
+    std::transform(
+        std::begin(options_), std::end(options_), std::begin(options), [](const Option_p &val) { return val.get(); });
+
+    if(filter) {
+        options.erase(std::remove_if(std::begin(options),
+                                     std::end(options),
+                                     [&filter](const Option *opt) { return !filter(opt); }),
+                      std::end(options));
+    }
+
+    return options;
+}
+
+CLI11_INLINE std::vector<Option *> App::get_options(const std::function<bool(Option *)> filter) {
+    std::vector<Option *> options(options_.size());
+    std::transform(
+        std::begin(options_), std::end(options_), std::begin(options), [](const Option_p &val) { return val.get(); });
+
+    if(filter) {
+        options.erase(
+            std::remove_if(std::begin(options), std::end(options), [&filter](Option *opt) { return !filter(opt); }),
+            std::end(options));
+    }
+
+    return options;
+}
+
+CLI11_INLINE Option *App::get_option_no_throw(std::string option_name) noexcept {
+    for(Option_p &opt : options_) {
+        if(opt->check_name(option_name)) {
+            return opt.get();
+        }
+    }
+    for(auto &subc : subcommands_) {
+        // also check down into nameless subcommands
+        if(subc->get_name().empty()) {
+            auto *opt = subc->get_option_no_throw(option_name);
+            if(opt != nullptr) {
+                return opt;
             }
         }
+    }
+    return nullptr;
+}
 
-        // finally run the main callback
-        if(final_callback_ && (parsed_ > 0) && (!suppress_final_callback)) {
-            if(!name_.empty() || count_all() > 0 || parent_ == nullptr) {
-                final_callback_();
+CLI11_NODISCARD CLI11_INLINE const Option *App::get_option_no_throw(std::string option_name) const noexcept {
+    for(const Option_p &opt : options_) {
+        if(opt->check_name(option_name)) {
+            return opt.get();
+        }
+    }
+    for(const auto &subc : subcommands_) {
+        // also check down into nameless subcommands
+        if(subc->get_name().empty()) {
+            auto *opt = subc->get_option_no_throw(option_name);
+            if(opt != nullptr) {
+                return opt;
             }
         }
     }
+    return nullptr;
+}
 
-    /// Check to see if a subcommand is valid. Give up immediately if subcommand max has been reached.
-    bool _valid_subcommand(const std::string &current, bool ignore_used = true) const {
-        // Don't match if max has been reached - but still check parents
-        if(require_subcommand_max_ != 0 && parsed_subcommands_.size() >= require_subcommand_max_) {
-            return parent_ != nullptr && parent_->_valid_subcommand(current, ignore_used);
+CLI11_NODISCARD CLI11_INLINE std::string App::get_display_name(bool with_aliases) const {
+    if(name_.empty()) {
+        return std::string("[Option Group: ") + get_group() + "]";
+    }
+    if(aliases_.empty() || !with_aliases) {
+        return name_;
+    }
+    std::string dispname = name_;
+    for(const auto &lalias : aliases_) {
+        dispname.push_back(',');
+        dispname.push_back(' ');
+        dispname.append(lalias);
+    }
+    return dispname;
+}
+
+CLI11_NODISCARD CLI11_INLINE bool App::check_name(std::string name_to_check) const {
+    std::string local_name = name_;
+    if(ignore_underscore_) {
+        local_name = detail::remove_underscore(name_);
+        name_to_check = detail::remove_underscore(name_to_check);
+    }
+    if(ignore_case_) {
+        local_name = detail::to_lower(name_);
+        name_to_check = detail::to_lower(name_to_check);
+    }
+
+    if(local_name == name_to_check) {
+        return true;
+    }
+    for(auto les : aliases_) {  // NOLINT(performance-for-range-copy)
+        if(ignore_underscore_) {
+            les = detail::remove_underscore(les);
+        }
+        if(ignore_case_) {
+            les = detail::to_lower(les);
         }
-        auto com = _find_subcommand(current, true, ignore_used);
-        if(com != nullptr) {
+        if(les == name_to_check) {
             return true;
         }
-        // Check parent if exists, else return false
-        return parent_ != nullptr && parent_->_valid_subcommand(current, ignore_used);
     }
+    return false;
+}
 
-    /// Selects a Classifier enum based on the type of the current argument
-    detail::Classifier _recognize(const std::string &current, bool ignore_used_subcommands = true) const {
-        std::string dummy1, dummy2;
+CLI11_NODISCARD CLI11_INLINE std::vector<std::string> App::get_groups() const {
+    std::vector<std::string> groups;
 
-        if(current == "--")
-            return detail::Classifier::POSITIONAL_MARK;
-        if(_valid_subcommand(current, ignore_used_subcommands))
-            return detail::Classifier::SUBCOMMAND;
-        if(detail::split_long(current, dummy1, dummy2))
-            return detail::Classifier::LONG;
-        if(detail::split_short(current, dummy1, dummy2)) {
-            if(dummy1[0] >= '0' && dummy1[0] <= '9') {
-                if(get_option_no_throw(std::string{'-', dummy1[0]}) == nullptr) {
-                    return detail::Classifier::NONE;
-                }
-            }
-            return detail::Classifier::SHORT;
-        }
-        if((allow_windows_style_options_) && (detail::split_windows_style(current, dummy1, dummy2)))
-            return detail::Classifier::WINDOWS_STYLE;
-        if((current == "++") && !name_.empty() && parent_ != nullptr)
-            return detail::Classifier::SUBCOMMAND_TERMINATOR;
-        return detail::Classifier::NONE;
+    for(const Option_p &opt : options_) {
+        // Add group if it is not already in there
+        if(std::find(groups.begin(), groups.end(), opt->get_group()) == groups.end()) {
+            groups.push_back(opt->get_group());
+        }
     }
 
-    // The parse function is now broken into several parts, and part of process
+    return groups;
+}
 
-    /// Read and process a configuration file (main app only)
-    void _process_config_file() {
-        if(config_ptr_ != nullptr) {
-            bool config_required = config_ptr_->get_required();
-            auto file_given = config_ptr_->count() > 0;
-            auto config_files = config_ptr_->as<std::vector<std::string>>();
-            if(config_files.empty() || config_files.front().empty()) {
-                if(config_required) {
-                    throw FileError::Missing("no specified config file");
-                }
-                return;
-            }
-            for(auto rit = config_files.rbegin(); rit != config_files.rend(); ++rit) {
-                const auto &config_file = *rit;
-                auto path_result = detail::check_path(config_file.c_str());
-                if(path_result == detail::path_type::file) {
-                    try {
-                        std::vector<ConfigItem> values = config_formatter_->from_file(config_file);
-                        _parse_config(values);
-                        if(!file_given) {
-                            config_ptr_->add_result(config_file);
-                        }
-                    } catch(const FileError &) {
-                        if(config_required || file_given)
-                            throw;
+CLI11_NODISCARD CLI11_INLINE std::vector<std::string> App::remaining(bool recurse) const {
+    std::vector<std::string> miss_list;
+    for(const std::pair<detail::Classifier, std::string> &miss : missing_) {
+        miss_list.push_back(std::get<1>(miss));
+    }
+    // Get from a subcommand that may allow extras
+    if(recurse) {
+        if(!allow_extras_) {
+            for(const auto &sub : subcommands_) {
+                if(sub->name_.empty() && !sub->missing_.empty()) {
+                    for(const std::pair<detail::Classifier, std::string> &miss : sub->missing_) {
+                        miss_list.push_back(std::get<1>(miss));
                     }
-                } else if(config_required || file_given) {
-                    throw FileError::Missing(config_file);
                 }
             }
         }
+        // Recurse into subcommands
+
+        for(const App *sub : parsed_subcommands_) {
+            std::vector<std::string> output = sub->remaining(recurse);
+            std::copy(std::begin(output), std::end(output), std::back_inserter(miss_list));
+        }
     }
+    return miss_list;
+}
 
-    /// Get envname options if not yet passed. Runs on *all* subcommands.
-    void _process_env() {
-        for(const Option_p &opt : options_) {
-            if(opt->count() == 0 && !opt->envname_.empty()) {
-                char *buffer = nullptr;
-                std::string ename_string;
+CLI11_NODISCARD CLI11_INLINE std::vector<std::string> App::remaining_for_passthrough(bool recurse) const {
+    std::vector<std::string> miss_list = remaining(recurse);
+    std::reverse(std::begin(miss_list), std::end(miss_list));
+    return miss_list;
+}
 
-#ifdef _MSC_VER
-                // Windows version
-                std::size_t sz = 0;
-                if(_dupenv_s(&buffer, &sz, opt->envname_.c_str()) == 0 && buffer != nullptr) {
-                    ename_string = std::string(buffer);
-                    free(buffer);
-                }
-#else
-                // This also works on Windows, but gives a warning
-                buffer = std::getenv(opt->envname_.c_str());
-                if(buffer != nullptr)
-                    ename_string = std::string(buffer);
-#endif
+CLI11_NODISCARD CLI11_INLINE std::size_t App::remaining_size(bool recurse) const {
+    auto remaining_options = static_cast<std::size_t>(std::count_if(
+        std::begin(missing_), std::end(missing_), [](const std::pair<detail::Classifier, std::string> &val) {
+            return val.first != detail::Classifier::POSITIONAL_MARK;
+        }));
 
-                if(!ename_string.empty()) {
-                    opt->add_result(ename_string);
-                }
-            }
+    if(recurse) {
+        for(const App_p &sub : subcommands_) {
+            remaining_options += sub->remaining_size(recurse);
         }
+    }
+    return remaining_options;
+}
 
-        for(App_p &sub : subcommands_) {
-            if(sub->get_name().empty() || !sub->parse_complete_callback_)
-                sub->_process_env();
+CLI11_INLINE void App::_validate() const {
+    // count the number of positional only args
+    auto pcount = std::count_if(std::begin(options_), std::end(options_), [](const Option_p &opt) {
+        return opt->get_items_expected_max() >= detail::expected_max_vector_size && !opt->nonpositional();
+    });
+    if(pcount > 1) {
+        auto pcount_req = std::count_if(std::begin(options_), std::end(options_), [](const Option_p &opt) {
+            return opt->get_items_expected_max() >= detail::expected_max_vector_size && !opt->nonpositional() &&
+                   opt->get_required();
+        });
+        if(pcount - pcount_req > 1) {
+            throw InvalidError(name_);
         }
     }
 
-    /// Process callbacks. Runs on *all* subcommands.
-    void _process_callbacks() {
+    std::size_t nameless_subs{0};
+    for(const App_p &app : subcommands_) {
+        app->_validate();
+        if(app->get_name().empty())
+            ++nameless_subs;
+    }
 
-        for(App_p &sub : subcommands_) {
-            // process the priority option_groups first
-            if(sub->get_name().empty() && sub->parse_complete_callback_) {
-                if(sub->count_all() > 0) {
-                    sub->_process_callbacks();
-                    sub->run_callback();
-                }
+    if(require_option_min_ > 0) {
+        if(require_option_max_ > 0) {
+            if(require_option_max_ < require_option_min_) {
+                throw(InvalidError("Required min options greater than required max options", ExitCodes::InvalidError));
             }
         }
+        if(require_option_min_ > (options_.size() + nameless_subs)) {
+            throw(
+                InvalidError("Required min options greater than number of available options", ExitCodes::InvalidError));
+        }
+    }
+}
 
-        for(const Option_p &opt : options_) {
-            if(opt->count() > 0 && !opt->get_callback_run()) {
-                opt->run_callback();
-            }
+CLI11_INLINE void App::_configure() {
+    if(default_startup == startup_mode::enabled) {
+        disabled_ = false;
+    } else if(default_startup == startup_mode::disabled) {
+        disabled_ = true;
+    }
+    for(const App_p &app : subcommands_) {
+        if(app->has_automatic_name_) {
+            app->name_.clear();
         }
-        for(App_p &sub : subcommands_) {
-            if(!sub->parse_complete_callback_) {
-                sub->_process_callbacks();
-            }
+        if(app->name_.empty()) {
+            app->fallthrough_ = false;  // make sure fallthrough_ is false to prevent infinite loop
+            app->prefix_command_ = false;
         }
+        // make sure the parent is set to be this object in preparation for parse
+        app->parent_ = this;
+        app->_configure();
     }
+}
 
-    /// Run help flag processing if any are found.
-    ///
-    /// The flags allow recursive calls to remember if there was a help flag on a parent.
-    void _process_help_flags(bool trigger_help = false, bool trigger_all_help = false) const {
-        const Option *help_ptr = get_help_ptr();
-        const Option *help_all_ptr = get_help_all_ptr();
-
-        if(help_ptr != nullptr && help_ptr->count() > 0)
-            trigger_help = true;
-        if(help_all_ptr != nullptr && help_all_ptr->count() > 0)
-            trigger_all_help = true;
-
-        // If there were parsed subcommands, call those. First subcommand wins if there are multiple ones.
-        if(!parsed_subcommands_.empty()) {
-            for(const App *sub : parsed_subcommands_)
-                sub->_process_help_flags(trigger_help, trigger_all_help);
-
-            // Only the final subcommand should call for help. All help wins over help.
-        } else if(trigger_all_help) {
-            throw CallForAllHelp();
-        } else if(trigger_help) {
-            throw CallForHelp();
+CLI11_INLINE void App::run_callback(bool final_mode, bool suppress_final_callback) {
+    pre_callback();
+    // in the main app if immediate_callback_ is set it runs the main callback before the used subcommands
+    if(!final_mode && parse_complete_callback_) {
+        parse_complete_callback_();
+    }
+    // run the callbacks for the received subcommands
+    for(App *subc : get_subcommands()) {
+        if(subc->parent_ == this) {
+            subc->run_callback(true, suppress_final_callback);
+        }
+    }
+    // now run callbacks for option_groups
+    for(auto &subc : subcommands_) {
+        if(subc->name_.empty() && subc->count_all() > 0) {
+            subc->run_callback(true, suppress_final_callback);
         }
     }
 
-    /// Verify required options and cross requirements. Subcommands too (only if selected).
-    void _process_requirements() {
-        // check excludes
-        bool excluded{false};
-        std::string excluder;
-        for(auto &opt : exclude_options_) {
-            if(opt->count() > 0) {
-                excluded = true;
-                excluder = opt->get_name();
-            }
-        }
-        for(auto &subc : exclude_subcommands_) {
-            if(subc->count_all() > 0) {
-                excluded = true;
-                excluder = subc->get_display_name();
-            }
-        }
-        if(excluded) {
-            if(count_all() > 0) {
-                throw ExcludesError(get_display_name(), excluder);
-            }
-            // if we are excluded but didn't receive anything, just return
-            return;
+    // finally run the main callback
+    if(final_callback_ && (parsed_ > 0) && (!suppress_final_callback)) {
+        if(!name_.empty() || count_all() > 0 || parent_ == nullptr) {
+            final_callback_();
         }
+    }
+}
+
+CLI11_NODISCARD CLI11_INLINE bool App::_valid_subcommand(const std::string &current, bool ignore_used) const {
+    // Don't match if max has been reached - but still check parents
+    if(require_subcommand_max_ != 0 && parsed_subcommands_.size() >= require_subcommand_max_) {
+        return parent_ != nullptr && parent_->_valid_subcommand(current, ignore_used);
+    }
+    auto *com = _find_subcommand(current, true, ignore_used);
+    if(com != nullptr) {
+        return true;
+    }
+    // Check parent if exists, else return false
+    return parent_ != nullptr && parent_->_valid_subcommand(current, ignore_used);
+}
 
-        // check excludes
-        bool missing_needed{false};
-        std::string missing_need;
-        for(auto &opt : need_options_) {
-            if(opt->count() == 0) {
-                missing_needed = true;
-                missing_need = opt->get_name();
-            }
-        }
-        for(auto &subc : need_subcommands_) {
-            if(subc->count_all() == 0) {
-                missing_needed = true;
-                missing_need = subc->get_display_name();
-            }
-        }
-        if(missing_needed) {
-            if(count_all() > 0) {
-                throw RequiresError(get_display_name(), missing_need);
+CLI11_NODISCARD CLI11_INLINE detail::Classifier App::_recognize(const std::string &current,
+                                                                bool ignore_used_subcommands) const {
+    std::string dummy1, dummy2;
+
+    if(current == "--")
+        return detail::Classifier::POSITIONAL_MARK;
+    if(_valid_subcommand(current, ignore_used_subcommands))
+        return detail::Classifier::SUBCOMMAND;
+    if(detail::split_long(current, dummy1, dummy2))
+        return detail::Classifier::LONG;
+    if(detail::split_short(current, dummy1, dummy2)) {
+        if(dummy1[0] >= '0' && dummy1[0] <= '9') {
+            if(get_option_no_throw(std::string{'-', dummy1[0]}) == nullptr) {
+                return detail::Classifier::NONE;
+            }
+        }
+        return detail::Classifier::SHORT;
+    }
+    if((allow_windows_style_options_) && (detail::split_windows_style(current, dummy1, dummy2)))
+        return detail::Classifier::WINDOWS_STYLE;
+    if((current == "++") && !name_.empty() && parent_ != nullptr)
+        return detail::Classifier::SUBCOMMAND_TERMINATOR;
+    return detail::Classifier::NONE;
+}
+
+CLI11_INLINE void App::_process_config_file() {
+    if(config_ptr_ != nullptr) {
+        bool config_required = config_ptr_->get_required();
+        auto file_given = config_ptr_->count() > 0;
+        auto config_files = config_ptr_->as<std::vector<std::string>>();
+        if(config_files.empty() || config_files.front().empty()) {
+            if(config_required) {
+                throw FileError::Missing("no specified config file");
             }
-            // if we missing something but didn't have any options, just return
             return;
         }
+        for(auto rit = config_files.rbegin(); rit != config_files.rend(); ++rit) {
+            const auto &config_file = *rit;
+            auto path_result = detail::check_path(config_file.c_str());
+            if(path_result == detail::path_type::file) {
+                try {
+                    std::vector<ConfigItem> values = config_formatter_->from_file(config_file);
+                    _parse_config(values);
+                    if(!file_given) {
+                        config_ptr_->add_result(config_file);
+                    }
+                } catch(const FileError &) {
+                    if(config_required || file_given)
+                        throw;
+                }
+            } else if(config_required || file_given) {
+                throw FileError::Missing(config_file);
+            }
+        }
+    }
+}
 
-        std::size_t used_options = 0;
-        for(const Option_p &opt : options_) {
+CLI11_INLINE void App::_process_env() {
+    for(const Option_p &opt : options_) {
+        if(opt->count() == 0 && !opt->envname_.empty()) {
+            char *buffer = nullptr;
+            std::string ename_string;
 
-            if(opt->count() != 0) {
-                ++used_options;
+#ifdef _MSC_VER
+            // Windows version
+            std::size_t sz = 0;
+            if(_dupenv_s(&buffer, &sz, opt->envname_.c_str()) == 0 && buffer != nullptr) {
+                ename_string = std::string(buffer);
+                free(buffer);
             }
-            // Required but empty
-            if(opt->get_required() && opt->count() == 0) {
-                throw RequiredError(opt->get_name());
-            }
-            // Requires
-            for(const Option *opt_req : opt->needs_)
-                if(opt->count() > 0 && opt_req->count() == 0)
-                    throw RequiresError(opt->get_name(), opt_req->get_name());
-            // Excludes
-            for(const Option *opt_ex : opt->excludes_)
-                if(opt->count() > 0 && opt_ex->count() != 0)
-                    throw ExcludesError(opt->get_name(), opt_ex->get_name());
-        }
-        // check for the required number of subcommands
-        if(require_subcommand_min_ > 0) {
-            auto selected_subcommands = get_subcommands();
-            if(require_subcommand_min_ > selected_subcommands.size())
-                throw RequiredError::Subcommand(require_subcommand_min_);
-        }
-
-        // Max error cannot occur, the extra subcommand will parse as an ExtrasError or a remaining item.
-
-        // run this loop to check how many unnamed subcommands were actually used since they are considered options
-        // from the perspective of an App
-        for(App_p &sub : subcommands_) {
-            if(sub->disabled_)
-                continue;
-            if(sub->name_.empty() && sub->count_all() > 0) {
-                ++used_options;
+#else
+            // This also works on Windows, but gives a warning
+            buffer = std::getenv(opt->envname_.c_str());
+            if(buffer != nullptr)
+                ename_string = std::string(buffer);
+#endif
+
+            if(!ename_string.empty()) {
+                opt->add_result(ename_string);
             }
         }
+    }
 
-        if(require_option_min_ > used_options || (require_option_max_ > 0 && require_option_max_ < used_options)) {
-            auto option_list = detail::join(options_, [this](const Option_p &ptr) {
-                if(ptr.get() == help_ptr_ || ptr.get() == help_all_ptr_) {
-                    return std::string{};
-                }
-                return ptr->get_name(false, true);
-            });
+    for(App_p &sub : subcommands_) {
+        if(sub->get_name().empty() || !sub->parse_complete_callback_)
+            sub->_process_env();
+    }
+}
 
-            auto subc_list = get_subcommands([](App *app) { return ((app->get_name().empty()) && (!app->disabled_)); });
-            if(!subc_list.empty()) {
-                option_list += "," + detail::join(subc_list, [](const App *app) { return app->get_display_name(); });
+CLI11_INLINE void App::_process_callbacks() {
+
+    for(App_p &sub : subcommands_) {
+        // process the priority option_groups first
+        if(sub->get_name().empty() && sub->parse_complete_callback_) {
+            if(sub->count_all() > 0) {
+                sub->_process_callbacks();
+                sub->run_callback();
             }
-            throw RequiredError::Option(require_option_min_, require_option_max_, used_options, option_list);
         }
+    }
 
-        // now process the requirements for subcommands if needed
-        for(App_p &sub : subcommands_) {
-            if(sub->disabled_)
-                continue;
-            if(sub->name_.empty() && sub->required_ == false) {
-                if(sub->count_all() == 0) {
-                    if(require_option_min_ > 0 && require_option_min_ <= used_options) {
-                        continue;
-                        // if we have met the requirement and there is nothing in this option group skip checking
-                        // requirements
-                    }
-                    if(require_option_max_ > 0 && used_options >= require_option_min_) {
-                        continue;
-                        // if we have met the requirement and there is nothing in this option group skip checking
-                        // requirements
-                    }
-                }
-            }
-            if(sub->count() > 0 || sub->name_.empty()) {
-                sub->_process_requirements();
-            }
+    for(const Option_p &opt : options_) {
+        if((*opt) && !opt->get_callback_run()) {
+            opt->run_callback();
+        }
+    }
+    for(App_p &sub : subcommands_) {
+        if(!sub->parse_complete_callback_) {
+            sub->_process_callbacks();
+        }
+    }
+}
 
-            if(sub->required_ && sub->count_all() == 0) {
-                throw(CLI::RequiredError(sub->get_display_name()));
-            }
+CLI11_INLINE void App::_process_help_flags(bool trigger_help, bool trigger_all_help) const {
+    const Option *help_ptr = get_help_ptr();
+    const Option *help_all_ptr = get_help_all_ptr();
+
+    if(help_ptr != nullptr && help_ptr->count() > 0)
+        trigger_help = true;
+    if(help_all_ptr != nullptr && help_all_ptr->count() > 0)
+        trigger_all_help = true;
+
+    // If there were parsed subcommands, call those. First subcommand wins if there are multiple ones.
+    if(!parsed_subcommands_.empty()) {
+        for(const App *sub : parsed_subcommands_)
+            sub->_process_help_flags(trigger_help, trigger_all_help);
+
+        // Only the final subcommand should call for help. All help wins over help.
+    } else if(trigger_all_help) {
+        throw CallForAllHelp();
+    } else if(trigger_help) {
+        throw CallForHelp();
+    }
+}
+
+CLI11_INLINE void App::_process_requirements() {
+    // check excludes
+    bool excluded{false};
+    std::string excluder;
+    for(const auto &opt : exclude_options_) {
+        if(opt->count() > 0) {
+            excluded = true;
+            excluder = opt->get_name();
+        }
+    }
+    for(const auto &subc : exclude_subcommands_) {
+        if(subc->count_all() > 0) {
+            excluded = true;
+            excluder = subc->get_display_name();
         }
     }
+    if(excluded) {
+        if(count_all() > 0) {
+            throw ExcludesError(get_display_name(), excluder);
+        }
+        // if we are excluded but didn't receive anything, just return
+        return;
+    }
 
-    /// Process callbacks and such.
-    void _process() {
-        CLI::FileError fe("ne");
-        bool caught_error{false};
-        try {
-            // the config file might generate a FileError but that should not be processed until later in the process
-            // to allow for help, version and other errors to generate first.
-            _process_config_file();
-            // process env shouldn't throw but no reason to process it if config generated an error
-            _process_env();
-        } catch(const CLI::FileError &fe2) {
-            fe = fe2;
-            caught_error = true;
+    // check excludes
+    bool missing_needed{false};
+    std::string missing_need;
+    for(const auto &opt : need_options_) {
+        if(opt->count() == 0) {
+            missing_needed = true;
+            missing_need = opt->get_name();
+        }
+    }
+    for(const auto &subc : need_subcommands_) {
+        if(subc->count_all() == 0) {
+            missing_needed = true;
+            missing_need = subc->get_display_name();
+        }
+    }
+    if(missing_needed) {
+        if(count_all() > 0) {
+            throw RequiresError(get_display_name(), missing_need);
         }
-        // callbacks and help_flags can generate exceptions which should take priority over the config file error if one
-        // exists
-        _process_callbacks();
-        _process_help_flags();
+        // if we missing something but didn't have any options, just return
+        return;
+    }
 
-        if(caught_error) {
-            throw CLI::FileError(std::move(fe));
+    std::size_t used_options = 0;
+    for(const Option_p &opt : options_) {
+
+        if(opt->count() != 0) {
+            ++used_options;
         }
+        // Required but empty
+        if(opt->get_required() && opt->count() == 0) {
+            throw RequiredError(opt->get_name());
+        }
+        // Requires
+        for(const Option *opt_req : opt->needs_)
+            if(opt->count() > 0 && opt_req->count() == 0)
+                throw RequiresError(opt->get_name(), opt_req->get_name());
+        // Excludes
+        for(const Option *opt_ex : opt->excludes_)
+            if(opt->count() > 0 && opt_ex->count() != 0)
+                throw ExcludesError(opt->get_name(), opt_ex->get_name());
+    }
+    // check for the required number of subcommands
+    if(require_subcommand_min_ > 0) {
+        auto selected_subcommands = get_subcommands();
+        if(require_subcommand_min_ > selected_subcommands.size())
+            throw RequiredError::Subcommand(require_subcommand_min_);
+    }
 
-        _process_requirements();
+    // Max error cannot occur, the extra subcommand will parse as an ExtrasError or a remaining item.
+
+    // run this loop to check how many unnamed subcommands were actually used since they are considered options
+    // from the perspective of an App
+    for(App_p &sub : subcommands_) {
+        if(sub->disabled_)
+            continue;
+        if(sub->name_.empty() && sub->count_all() > 0) {
+            ++used_options;
+        }
     }
 
-    /// Throw an error if anything is left over and should not be.
-    void _process_extras() {
-        if(!(allow_extras_ || prefix_command_)) {
-            std::size_t num_left_over = remaining_size();
-            if(num_left_over > 0) {
-                throw ExtrasError(name_, remaining(false));
+    if(require_option_min_ > used_options || (require_option_max_ > 0 && require_option_max_ < used_options)) {
+        auto option_list = detail::join(options_, [this](const Option_p &ptr) {
+            if(ptr.get() == help_ptr_ || ptr.get() == help_all_ptr_) {
+                return std::string{};
             }
-        }
+            return ptr->get_name(false, true);
+        });
 
-        for(App_p &sub : subcommands_) {
-            if(sub->count() > 0)
-                sub->_process_extras();
+        auto subc_list = get_subcommands([](App *app) { return ((app->get_name().empty()) && (!app->disabled_)); });
+        if(!subc_list.empty()) {
+            option_list += "," + detail::join(subc_list, [](const App *app) { return app->get_display_name(); });
         }
+        throw RequiredError::Option(require_option_min_, require_option_max_, used_options, option_list);
     }
 
-    /// Throw an error if anything is left over and should not be.
-    /// Modifies the args to fill in the missing items before throwing.
-    void _process_extras(std::vector<std::string> &args) {
-        if(!(allow_extras_ || prefix_command_)) {
-            std::size_t num_left_over = remaining_size();
-            if(num_left_over > 0) {
-                args = remaining(false);
-                throw ExtrasError(name_, args);
+    // now process the requirements for subcommands if needed
+    for(App_p &sub : subcommands_) {
+        if(sub->disabled_)
+            continue;
+        if(sub->name_.empty() && sub->required_ == false) {
+            if(sub->count_all() == 0) {
+                if(require_option_min_ > 0 && require_option_min_ <= used_options) {
+                    continue;
+                    // if we have met the requirement and there is nothing in this option group skip checking
+                    // requirements
+                }
+                if(require_option_max_ > 0 && used_options >= require_option_min_) {
+                    continue;
+                    // if we have met the requirement and there is nothing in this option group skip checking
+                    // requirements
+                }
             }
         }
+        if(sub->count() > 0 || sub->name_.empty()) {
+            sub->_process_requirements();
+        }
 
-        for(App_p &sub : subcommands_) {
-            if(sub->count() > 0)
-                sub->_process_extras(args);
+        if(sub->required_ && sub->count_all() == 0) {
+            throw(CLI::RequiredError(sub->get_display_name()));
         }
     }
+}
 
-    /// Internal function to recursively increment the parsed counter on the current app as well unnamed subcommands
-    void increment_parsed() {
-        ++parsed_;
-        for(App_p &sub : subcommands_) {
-            if(sub->get_name().empty())
-                sub->increment_parsed();
-        }
+CLI11_INLINE void App::_process() {
+    try {
+        // the config file might generate a FileError but that should not be processed until later in the process
+        // to allow for help, version and other errors to generate first.
+        _process_config_file();
+
+        // process env shouldn't throw but no reason to process it if config generated an error
+        _process_env();
+    } catch(const CLI::FileError &) {
+        // callbacks and help_flags can generate exceptions which should take priority
+        // over the config file error if one exists.
+        _process_callbacks();
+        _process_help_flags();
+        throw;
     }
-    /// Internal parse function
-    void _parse(std::vector<std::string> &args) {
-        increment_parsed();
-        _trigger_pre_parse(args.size());
-        bool positional_only = false;
 
-        while(!args.empty()) {
-            if(!_parse_single(args, positional_only)) {
-                break;
-            }
-        }
+    _process_callbacks();
+    _process_help_flags();
+
+    _process_requirements();
+}
 
-        if(parent_ == nullptr) {
-            _process();
+CLI11_INLINE void App::_process_extras() {
+    if(!(allow_extras_ || prefix_command_)) {
+        std::size_t num_left_over = remaining_size();
+        if(num_left_over > 0) {
+            throw ExtrasError(name_, remaining(false));
+        }
+    }
 
-            // Throw error if any items are left over (depending on settings)
-            _process_extras(args);
+    for(App_p &sub : subcommands_) {
+        if(sub->count() > 0)
+            sub->_process_extras();
+    }
+}
 
-            // Convert missing (pairs) to extras (string only) ready for processing in another app
-            args = remaining_for_passthrough(false);
-        } else if(parse_complete_callback_) {
-            _process_env();
-            _process_callbacks();
-            _process_help_flags();
-            _process_requirements();
-            run_callback(false, true);
+CLI11_INLINE void App::_process_extras(std::vector<std::string> &args) {
+    if(!(allow_extras_ || prefix_command_)) {
+        std::size_t num_left_over = remaining_size();
+        if(num_left_over > 0) {
+            args = remaining(false);
+            throw ExtrasError(name_, args);
         }
     }
 
-    /// Internal parse function
-    void _parse(std::vector<std::string> &&args) {
-        // this can only be called by the top level in which case parent == nullptr by definition
-        // operation is simplified
-        increment_parsed();
-        _trigger_pre_parse(args.size());
-        bool positional_only = false;
+    for(App_p &sub : subcommands_) {
+        if(sub->count() > 0)
+            sub->_process_extras(args);
+    }
+}
 
-        while(!args.empty()) {
-            _parse_single(args, positional_only);
+CLI11_INLINE void App::increment_parsed() {
+    ++parsed_;
+    for(App_p &sub : subcommands_) {
+        if(sub->get_name().empty())
+            sub->increment_parsed();
+    }
+}
+
+CLI11_INLINE void App::_parse(std::vector<std::string> &args) {
+    increment_parsed();
+    _trigger_pre_parse(args.size());
+    bool positional_only = false;
+
+    while(!args.empty()) {
+        if(!_parse_single(args, positional_only)) {
+            break;
         }
+    }
+
+    if(parent_ == nullptr) {
         _process();
 
         // Throw error if any items are left over (depending on settings)
-        _process_extras();
+        _process_extras(args);
+
+        // Convert missing (pairs) to extras (string only) ready for processing in another app
+        args = remaining_for_passthrough(false);
+    } else if(parse_complete_callback_) {
+        _process_env();
+        _process_callbacks();
+        _process_help_flags();
+        _process_requirements();
+        run_callback(false, true);
     }
+}
 
-    /// Parse one config param, return false if not found in any subcommand, remove if it is
-    ///
-    /// If this has more than one dot.separated.name, go into the subcommand matching it
-    /// Returns true if it managed to find the option, if false you'll need to remove the arg manually.
-    void _parse_config(const std::vector<ConfigItem> &args) {
-        for(const ConfigItem &item : args) {
-            if(!_parse_single_config(item) && allow_config_extras_ == config_extras_mode::error)
-                throw ConfigError::Extras(item.fullname());
-        }
+CLI11_INLINE void App::_parse(std::vector<std::string> &&args) {
+    // this can only be called by the top level in which case parent == nullptr by definition
+    // operation is simplified
+    increment_parsed();
+    _trigger_pre_parse(args.size());
+    bool positional_only = false;
+
+    while(!args.empty()) {
+        _parse_single(args, positional_only);
     }
+    _process();
 
-    /// Fill in a single config option
-    bool _parse_single_config(const ConfigItem &item, std::size_t level = 0) {
-        if(level < item.parents.size()) {
-            try {
-                auto subcom = get_subcommand(item.parents.at(level));
-                auto result = subcom->_parse_single_config(item, level + 1);
+    // Throw error if any items are left over (depending on settings)
+    _process_extras();
+}
 
-                return result;
-            } catch(const OptionNotFound &) {
-                return false;
-            }
+CLI11_INLINE void App::_parse_stream(std::istream &input) {
+    auto values = config_formatter_->from_config(input);
+    _parse_config(values);
+    increment_parsed();
+    _trigger_pre_parse(values.size());
+    _process();
+
+    // Throw error if any items are left over (depending on settings)
+    _process_extras();
+}
+
+CLI11_INLINE void App::_parse_config(const std::vector<ConfigItem> &args) {
+    for(const ConfigItem &item : args) {
+        if(!_parse_single_config(item) && allow_config_extras_ == config_extras_mode::error)
+            throw ConfigError::Extras(item.fullname());
+    }
+}
+
+CLI11_INLINE bool App::_parse_single_config(const ConfigItem &item, std::size_t level) {
+    if(level < item.parents.size()) {
+        try {
+            auto *subcom = get_subcommand(item.parents.at(level));
+            auto result = subcom->_parse_single_config(item, level + 1);
+
+            return result;
+        } catch(const OptionNotFound &) {
+            return false;
         }
-        // check for section open
-        if(item.name == "++") {
-            if(configurable_) {
-                increment_parsed();
-                _trigger_pre_parse(2);
-                if(parent_ != nullptr) {
-                    parent_->parsed_subcommands_.push_back(this);
-                }
+    }
+    // check for section open
+    if(item.name == "++") {
+        if(configurable_) {
+            increment_parsed();
+            _trigger_pre_parse(2);
+            if(parent_ != nullptr) {
+                parent_->parsed_subcommands_.push_back(this);
             }
-            return true;
         }
-        // check for section close
-        if(item.name == "--") {
-            if(configurable_) {
-                _process_callbacks();
-                _process_requirements();
-                run_callback();
-            }
-            return true;
+        return true;
+    }
+    // check for section close
+    if(item.name == "--") {
+        if(configurable_ && parse_complete_callback_) {
+            _process_callbacks();
+            _process_requirements();
+            run_callback();
         }
-        Option *op = get_option_no_throw("--" + item.name);
-        if(op == nullptr) {
-            if(item.name.size() == 1) {
-                op = get_option_no_throw("-" + item.name);
-            }
+        return true;
+    }
+    Option *op = get_option_no_throw("--" + item.name);
+    if(op == nullptr) {
+        if(item.name.size() == 1) {
+            op = get_option_no_throw("-" + item.name);
         }
-        if(op == nullptr) {
-            op = get_option_no_throw(item.name);
-        }
-        if(op == nullptr) {
-            // If the option was not present
-            if(get_allow_config_extras() == config_extras_mode::capture)
-                // Should we worry about classifying the extras properly?
-                missing_.emplace_back(detail::Classifier::NONE, item.fullname());
+    }
+    if(op == nullptr) {
+        op = get_option_no_throw(item.name);
+    }
+    if(op == nullptr) {
+        // If the option was not present
+        if(get_allow_config_extras() == config_extras_mode::capture)
+            // Should we worry about classifying the extras properly?
+            missing_.emplace_back(detail::Classifier::NONE, item.fullname());
+        return false;
+    }
+
+    if(!op->get_configurable()) {
+        if(get_allow_config_extras() == config_extras_mode::ignore_all) {
             return false;
         }
+        throw ConfigError::NotConfigurable(item.fullname());
+    }
 
-        if(!op->get_configurable())
-            throw ConfigError::NotConfigurable(item.fullname());
+    if(op->empty()) {
 
-        if(op->empty()) {
-            // Flag parsing
-            if(op->get_expected_min() == 0) {
+        if(op->get_expected_min() == 0) {
+            if(item.inputs.size() <= 1) {
+                // Flag parsing
                 auto res = config_formatter_->to_flag(item);
-                res = op->get_flag_value(item.name, res);
+                bool converted{false};
+                if(op->get_disable_flag_override()) {
 
-                op->add_result(res);
+                    try {
+                        auto val = detail::to_flag_value(res);
+                        if(val == 1) {
+                            res = op->get_flag_value(item.name, "{}");
+                            converted = true;
+                        }
+                    } catch(...) {
+                    }
+                }
 
-            } else {
-                op->add_result(item.inputs);
-                op->run_callback();
+                if(!converted) {
+                    res = op->get_flag_value(item.name, res);
+                }
+
+                op->add_result(res);
+                return true;
+            }
+            if(static_cast<int>(item.inputs.size()) > op->get_items_expected_max()) {
+                if(op->get_items_expected_max() > 1) {
+                    throw ArgumentMismatch::AtMost(item.fullname(), op->get_items_expected_max(), item.inputs.size());
+                }
+                throw ConversionError::TooManyInputsFlag(item.fullname());
             }
         }
-
-        return true;
+        op->add_result(item.inputs);
+        op->run_callback();
     }
 
-    /// Parse "one" argument (some may eat more than one), delegate to parent if fails, add to missing if missing
-    /// from master return false if the parse has failed and needs to return to parent
-    bool _parse_single(std::vector<std::string> &args, bool &positional_only) {
-        bool retval = true;
-        detail::Classifier classifier = positional_only ? detail::Classifier::NONE : _recognize(args.back());
-        switch(classifier) {
-        case detail::Classifier::POSITIONAL_MARK:
-            args.pop_back();
-            positional_only = true;
-            if((!_has_remaining_positionals()) && (parent_ != nullptr)) {
-                retval = false;
-            } else {
-                _move_to_missing(classifier, "--");
-            }
-            break;
-        case detail::Classifier::SUBCOMMAND_TERMINATOR:
-            // treat this like a positional mark if in the parent app
-            args.pop_back();
+    return true;
+}
+
+CLI11_INLINE bool App::_parse_single(std::vector<std::string> &args, bool &positional_only) {
+    bool retval = true;
+    detail::Classifier classifier = positional_only ? detail::Classifier::NONE : _recognize(args.back());
+    switch(classifier) {
+    case detail::Classifier::POSITIONAL_MARK:
+        args.pop_back();
+        positional_only = true;
+        if((!_has_remaining_positionals()) && (parent_ != nullptr)) {
             retval = false;
-            break;
-        case detail::Classifier::SUBCOMMAND:
-            retval = _parse_subcommand(args);
-            break;
-        case detail::Classifier::LONG:
-        case detail::Classifier::SHORT:
-        case detail::Classifier::WINDOWS_STYLE:
-            // If already parsed a subcommand, don't accept options_
-            _parse_arg(args, classifier);
-            break;
-        case detail::Classifier::NONE:
-            // Probably a positional or something for a parent (sub)command
-            retval = _parse_positional(args, false);
-            if(retval && positionals_at_end_) {
-                positional_only = true;
-            }
-            break;
-            // LCOV_EXCL_START
-        default:
-            throw HorribleError("unrecognized classifier (you should not see this!)");
-            // LCOV_EXCL_STOP
+        } else {
+            _move_to_missing(classifier, "--");
         }
-        return retval;
+        break;
+    case detail::Classifier::SUBCOMMAND_TERMINATOR:
+        // treat this like a positional mark if in the parent app
+        args.pop_back();
+        retval = false;
+        break;
+    case detail::Classifier::SUBCOMMAND:
+        retval = _parse_subcommand(args);
+        break;
+    case detail::Classifier::LONG:
+    case detail::Classifier::SHORT:
+    case detail::Classifier::WINDOWS_STYLE:
+        // If already parsed a subcommand, don't accept options_
+        _parse_arg(args, classifier);
+        break;
+    case detail::Classifier::NONE:
+        // Probably a positional or something for a parent (sub)command
+        retval = _parse_positional(args, false);
+        if(retval && positionals_at_end_) {
+            positional_only = true;
+        }
+        break;
+        // LCOV_EXCL_START
+    default:
+        throw HorribleError("unrecognized classifier (you should not see this!)");
+        // LCOV_EXCL_STOP
     }
+    return retval;
+}
 
-    /// Count the required remaining positional arguments
-    std::size_t _count_remaining_positionals(bool required_only = false) const {
-        std::size_t retval = 0;
-        for(const Option_p &opt : options_) {
-            if(opt->get_positional() && (!required_only || opt->get_required())) {
-                if(opt->get_items_expected_min() > 0 &&
-                   static_cast<int>(opt->count()) < opt->get_items_expected_min()) {
-                    retval += static_cast<std::size_t>(opt->get_items_expected_min()) - opt->count();
-                }
+CLI11_NODISCARD CLI11_INLINE std::size_t App::_count_remaining_positionals(bool required_only) const {
+    std::size_t retval = 0;
+    for(const Option_p &opt : options_) {
+        if(opt->get_positional() && (!required_only || opt->get_required())) {
+            if(opt->get_items_expected_min() > 0 && static_cast<int>(opt->count()) < opt->get_items_expected_min()) {
+                retval += static_cast<std::size_t>(opt->get_items_expected_min()) - opt->count();
             }
         }
-        return retval;
     }
+    return retval;
+}
 
-    /// Count the required remaining positional arguments
-    bool _has_remaining_positionals() const {
-        for(const Option_p &opt : options_) {
-            if(opt->get_positional() && ((static_cast<int>(opt->count()) < opt->get_items_expected_min()))) {
-                return true;
-            }
+CLI11_NODISCARD CLI11_INLINE bool App::_has_remaining_positionals() const {
+    for(const Option_p &opt : options_) {
+        if(opt->get_positional() && ((static_cast<int>(opt->count()) < opt->get_items_expected_min()))) {
+            return true;
         }
-
-        return false;
     }
 
-    /// Parse a positional, go up the tree to check
-    /// @param haltOnSubcommand if set to true the operation will not process subcommands merely return false
-    /// Return true if the positional was used false otherwise
-    bool _parse_positional(std::vector<std::string> &args, bool haltOnSubcommand) {
+    return false;
+}
 
-        const std::string &positional = args.back();
+CLI11_INLINE bool App::_parse_positional(std::vector<std::string> &args, bool haltOnSubcommand) {
 
-        if(positionals_at_end_) {
-            // deal with the case of required arguments at the end which should take precedence over other arguments
-            auto arg_rem = args.size();
-            auto remreq = _count_remaining_positionals(true);
-            if(arg_rem <= remreq) {
-                for(const Option_p &opt : options_) {
-                    if(opt->get_positional() && opt->required_) {
-                        if(static_cast<int>(opt->count()) < opt->get_items_expected_min()) {
-                            if(validate_positionals_) {
-                                std::string pos = positional;
-                                pos = opt->_validate(pos, 0);
-                                if(!pos.empty()) {
-                                    continue;
-                                }
+    const std::string &positional = args.back();
+
+    if(positionals_at_end_) {
+        // deal with the case of required arguments at the end which should take precedence over other arguments
+        auto arg_rem = args.size();
+        auto remreq = _count_remaining_positionals(true);
+        if(arg_rem <= remreq) {
+            for(const Option_p &opt : options_) {
+                if(opt->get_positional() && opt->required_) {
+                    if(static_cast<int>(opt->count()) < opt->get_items_expected_min()) {
+                        if(validate_positionals_) {
+                            std::string pos = positional;
+                            pos = opt->_validate(pos, 0);
+                            if(!pos.empty()) {
+                                continue;
                             }
-                            opt->add_result(positional);
-                            parse_order_.push_back(opt.get());
-                            args.pop_back();
-                            return true;
                         }
+
+                        parse_order_.push_back(opt.get());
+                        /// if we require a separator add it here
+                        if(opt->get_inject_separator()) {
+                            if(!opt->results().empty() && !opt->results().back().empty()) {
+                                opt->add_result(std::string{});
+                            }
+                        }
+                        if(opt->get_trigger_on_parse() &&
+                           opt->current_option_state_ == Option::option_state::callback_run) {
+                            opt->clear();
+                        }
+                        opt->add_result(positional);
+                        if(opt->get_trigger_on_parse()) {
+                            opt->run_callback();
+                        }
+                        args.pop_back();
+                        return true;
                     }
                 }
             }
         }
-        for(const Option_p &opt : options_) {
-            // Eat options, one by one, until done
-            if(opt->get_positional() &&
-               (static_cast<int>(opt->count()) < opt->get_items_expected_min() || opt->get_allow_extra_args())) {
-                if(validate_positionals_) {
-                    std::string pos = positional;
-                    pos = opt->_validate(pos, 0);
-                    if(!pos.empty()) {
-                        continue;
-                    }
+    }
+    for(const Option_p &opt : options_) {
+        // Eat options, one by one, until done
+        if(opt->get_positional() &&
+           (static_cast<int>(opt->count()) < opt->get_items_expected_min() || opt->get_allow_extra_args())) {
+            if(validate_positionals_) {
+                std::string pos = positional;
+                pos = opt->_validate(pos, 0);
+                if(!pos.empty()) {
+                    continue;
                 }
-                opt->add_result(positional);
-                parse_order_.push_back(opt.get());
-                args.pop_back();
-                return true;
             }
-        }
-
-        for(auto &subc : subcommands_) {
-            if((subc->name_.empty()) && (!subc->disabled_)) {
-                if(subc->_parse_positional(args, false)) {
-                    if(!subc->pre_parse_called_) {
-                        subc->_trigger_pre_parse(args.size());
-                    }
-                    return true;
+            if(opt->get_inject_separator()) {
+                if(!opt->results().empty() && !opt->results().back().empty()) {
+                    opt->add_result(std::string{});
                 }
             }
-        }
-        // let the parent deal with it if possible
-        if(parent_ != nullptr && fallthrough_)
-            return _get_fallthrough_parent()->_parse_positional(args, static_cast<bool>(parse_complete_callback_));
-
-        /// Try to find a local subcommand that is repeated
-        auto com = _find_subcommand(args.back(), true, false);
-        if(com != nullptr && (require_subcommand_max_ == 0 || require_subcommand_max_ > parsed_subcommands_.size())) {
-            if(haltOnSubcommand) {
-                return false;
+            if(opt->get_trigger_on_parse() && opt->current_option_state_ == Option::option_state::callback_run) {
+                opt->clear();
             }
+            opt->add_result(positional);
+            if(opt->get_trigger_on_parse()) {
+                opt->run_callback();
+            }
+            parse_order_.push_back(opt.get());
             args.pop_back();
-            com->_parse(args);
             return true;
         }
-        /// now try one last gasp at subcommands that have been executed before, go to root app and try to find a
-        /// subcommand in a broader way, if one exists let the parent deal with it
-        auto parent_app = (parent_ != nullptr) ? _get_fallthrough_parent() : this;
-        com = parent_app->_find_subcommand(args.back(), true, false);
-        if(com != nullptr && (com->parent_->require_subcommand_max_ == 0 ||
-                              com->parent_->require_subcommand_max_ > com->parent_->parsed_subcommands_.size())) {
-            return false;
-        }
+    }
 
-        if(positionals_at_end_) {
-            throw CLI::ExtrasError(name_, args);
+    for(auto &subc : subcommands_) {
+        if((subc->name_.empty()) && (!subc->disabled_)) {
+            if(subc->_parse_positional(args, false)) {
+                if(!subc->pre_parse_called_) {
+                    subc->_trigger_pre_parse(args.size());
+                }
+                return true;
+            }
         }
-        /// If this is an option group don't deal with it
-        if(parent_ != nullptr && name_.empty()) {
+    }
+    // let the parent deal with it if possible
+    if(parent_ != nullptr && fallthrough_)
+        return _get_fallthrough_parent()->_parse_positional(args, static_cast<bool>(parse_complete_callback_));
+
+    /// Try to find a local subcommand that is repeated
+    auto *com = _find_subcommand(args.back(), true, false);
+    if(com != nullptr && (require_subcommand_max_ == 0 || require_subcommand_max_ > parsed_subcommands_.size())) {
+        if(haltOnSubcommand) {
             return false;
         }
-        /// We are out of other options this goes to missing
-        _move_to_missing(detail::Classifier::NONE, positional);
         args.pop_back();
-        if(prefix_command_) {
-            while(!args.empty()) {
-                _move_to_missing(detail::Classifier::NONE, args.back());
-                args.pop_back();
-            }
-        }
-
+        com->_parse(args);
         return true;
     }
+    /// now try one last gasp at subcommands that have been executed before, go to root app and try to find a
+    /// subcommand in a broader way, if one exists let the parent deal with it
+    auto *parent_app = (parent_ != nullptr) ? _get_fallthrough_parent() : this;
+    com = parent_app->_find_subcommand(args.back(), true, false);
+    if(com != nullptr && (com->parent_->require_subcommand_max_ == 0 ||
+                          com->parent_->require_subcommand_max_ > com->parent_->parsed_subcommands_.size())) {
+        return false;
+    }
 
-    /// Locate a subcommand by name with two conditions, should disabled subcommands be ignored, and should used
-    /// subcommands be ignored
-    App *_find_subcommand(const std::string &subc_name, bool ignore_disabled, bool ignore_used) const noexcept {
-        for(const App_p &com : subcommands_) {
-            if(com->disabled_ && ignore_disabled)
-                continue;
-            if(com->get_name().empty()) {
-                auto subc = com->_find_subcommand(subc_name, ignore_disabled, ignore_used);
-                if(subc != nullptr) {
-                    return subc;
-                }
-            }
-            if(com->check_name(subc_name)) {
-                if((!*com) || !ignore_used)
-                    return com.get();
+    if(positionals_at_end_) {
+        throw CLI::ExtrasError(name_, args);
+    }
+    /// If this is an option group don't deal with it
+    if(parent_ != nullptr && name_.empty()) {
+        return false;
+    }
+    /// We are out of other options this goes to missing
+    _move_to_missing(detail::Classifier::NONE, positional);
+    args.pop_back();
+    if(prefix_command_) {
+        while(!args.empty()) {
+            _move_to_missing(detail::Classifier::NONE, args.back());
+            args.pop_back();
+        }
+    }
+
+    return true;
+}
+
+CLI11_NODISCARD CLI11_INLINE App *
+App::_find_subcommand(const std::string &subc_name, bool ignore_disabled, bool ignore_used) const noexcept {
+    for(const App_p &com : subcommands_) {
+        if(com->disabled_ && ignore_disabled)
+            continue;
+        if(com->get_name().empty()) {
+            auto *subc = com->_find_subcommand(subc_name, ignore_disabled, ignore_used);
+            if(subc != nullptr) {
+                return subc;
             }
         }
-        return nullptr;
+        if(com->check_name(subc_name)) {
+            if((!*com) || !ignore_used)
+                return com.get();
+        }
     }
+    return nullptr;
+}
 
-    /// Parse a subcommand, modify args and continue
-    ///
-    /// Unlike the others, this one will always allow fallthrough
-    /// return true if the subcommand was processed false otherwise
-    bool _parse_subcommand(std::vector<std::string> &args) {
-        if(_count_remaining_positionals(/* required */ true) > 0) {
-            _parse_positional(args, false);
-            return true;
+CLI11_INLINE bool App::_parse_subcommand(std::vector<std::string> &args) {
+    if(_count_remaining_positionals(/* required */ true) > 0) {
+        _parse_positional(args, false);
+        return true;
+    }
+    auto *com = _find_subcommand(args.back(), true, true);
+    if(com != nullptr) {
+        args.pop_back();
+        if(!com->silent_) {
+            parsed_subcommands_.push_back(com);
         }
-        auto com = _find_subcommand(args.back(), true, true);
-        if(com != nullptr) {
-            args.pop_back();
+        com->_parse(args);
+        auto *parent_app = com->parent_;
+        while(parent_app != this) {
+            parent_app->_trigger_pre_parse(args.size());
             if(!com->silent_) {
-                parsed_subcommands_.push_back(com);
+                parent_app->parsed_subcommands_.push_back(com);
             }
-            com->_parse(args);
-            auto parent_app = com->parent_;
-            while(parent_app != this) {
-                parent_app->_trigger_pre_parse(args.size());
-                if(!com->silent_) {
-                    parent_app->parsed_subcommands_.push_back(com);
-                }
-                parent_app = parent_app->parent_;
-            }
-            return true;
+            parent_app = parent_app->parent_;
         }
-
-        if(parent_ == nullptr)
-            throw HorribleError("Subcommand " + args.back() + " missing");
-        return false;
+        return true;
     }
 
-    /// Parse a short (false) or long (true) argument, must be at the top of the list
-    /// return true if the argument was processed or false if nothing was done
-    bool _parse_arg(std::vector<std::string> &args, detail::Classifier current_type) {
+    if(parent_ == nullptr)
+        throw HorribleError("Subcommand " + args.back() + " missing");
+    return false;
+}
 
-        std::string current = args.back();
+CLI11_INLINE bool App::_parse_arg(std::vector<std::string> &args, detail::Classifier current_type) {
 
-        std::string arg_name;
-        std::string value;
-        std::string rest;
-
-        switch(current_type) {
-        case detail::Classifier::LONG:
-            if(!detail::split_long(current, arg_name, value))
-                throw HorribleError("Long parsed but missing (you should not see this):" + args.back());
-            break;
-        case detail::Classifier::SHORT:
-            if(!detail::split_short(current, arg_name, rest))
-                throw HorribleError("Short parsed but missing! You should not see this");
-            break;
-        case detail::Classifier::WINDOWS_STYLE:
-            if(!detail::split_windows_style(current, arg_name, value))
-                throw HorribleError("windows option parsed but missing! You should not see this");
-            break;
-        case detail::Classifier::SUBCOMMAND:
-        case detail::Classifier::SUBCOMMAND_TERMINATOR:
-        case detail::Classifier::POSITIONAL_MARK:
-        case detail::Classifier::NONE:
-        default:
-            throw HorribleError("parsing got called with invalid option! You should not see this");
-        }
+    std::string current = args.back();
 
-        auto op_ptr =
-            std::find_if(std::begin(options_), std::end(options_), [arg_name, current_type](const Option_p &opt) {
-                if(current_type == detail::Classifier::LONG)
-                    return opt->check_lname(arg_name);
-                if(current_type == detail::Classifier::SHORT)
-                    return opt->check_sname(arg_name);
-                // this will only get called for detail::Classifier::WINDOWS_STYLE
-                return opt->check_lname(arg_name) || opt->check_sname(arg_name);
-            });
+    std::string arg_name;
+    std::string value;
+    std::string rest;
+
+    switch(current_type) {
+    case detail::Classifier::LONG:
+        if(!detail::split_long(current, arg_name, value))
+            throw HorribleError("Long parsed but missing (you should not see this):" + args.back());
+        break;
+    case detail::Classifier::SHORT:
+        if(!detail::split_short(current, arg_name, rest))
+            throw HorribleError("Short parsed but missing! You should not see this");
+        break;
+    case detail::Classifier::WINDOWS_STYLE:
+        if(!detail::split_windows_style(current, arg_name, value))
+            throw HorribleError("windows option parsed but missing! You should not see this");
+        break;
+    case detail::Classifier::SUBCOMMAND:
+    case detail::Classifier::SUBCOMMAND_TERMINATOR:
+    case detail::Classifier::POSITIONAL_MARK:
+    case detail::Classifier::NONE:
+    default:
+        throw HorribleError("parsing got called with invalid option! You should not see this");
+    }
 
-        // Option not found
-        if(op_ptr == std::end(options_)) {
-            for(auto &subc : subcommands_) {
-                if(subc->name_.empty() && !subc->disabled_) {
-                    if(subc->_parse_arg(args, current_type)) {
-                        if(!subc->pre_parse_called_) {
-                            subc->_trigger_pre_parse(args.size());
-                        }
-                        return true;
+    auto op_ptr = std::find_if(std::begin(options_), std::end(options_), [arg_name, current_type](const Option_p &opt) {
+        if(current_type == detail::Classifier::LONG)
+            return opt->check_lname(arg_name);
+        if(current_type == detail::Classifier::SHORT)
+            return opt->check_sname(arg_name);
+        // this will only get called for detail::Classifier::WINDOWS_STYLE
+        return opt->check_lname(arg_name) || opt->check_sname(arg_name);
+    });
+
+    // Option not found
+    if(op_ptr == std::end(options_)) {
+        for(auto &subc : subcommands_) {
+            if(subc->name_.empty() && !subc->disabled_) {
+                if(subc->_parse_arg(args, current_type)) {
+                    if(!subc->pre_parse_called_) {
+                        subc->_trigger_pre_parse(args.size());
                     }
+                    return true;
                 }
             }
-            // If a subcommand, try the master command
-            if(parent_ != nullptr && fallthrough_)
-                return _get_fallthrough_parent()->_parse_arg(args, current_type);
-            // don't capture missing if this is a nameless subcommand
-            if(parent_ != nullptr && name_.empty()) {
-                return false;
-            }
-            // Otherwise, add to missing
-            args.pop_back();
-            _move_to_missing(current_type, current);
-            return true;
         }
 
-        args.pop_back();
-
-        // Get a reference to the pointer to make syntax bearable
-        Option_p &op = *op_ptr;
-        /// if we require a separator add it here
-        if(op->get_inject_separator()) {
-            if(!op->results().empty() && !op->results().back().empty()) {
-                op->add_result(std::string{});
-            }
-        }
-        int min_num = (std::min)(op->get_type_size_min(), op->get_items_expected_min());
-        int max_num = op->get_items_expected_max();
-        // check container like options to limit the argument size to a single type if the allow_extra_flags argument is
-        // set. 16 is somewhat arbitrary (needs to be at least 4)
-        if(max_num >= detail::expected_max_vector_size / 16 && !op->get_allow_extra_args()) {
-            auto tmax = op->get_type_size_max();
-            max_num = detail::checked_multiply(tmax, op->get_expected_min()) ? tmax : detail::expected_max_vector_size;
-        }
-        // Make sure we always eat the minimum for unlimited vectors
-        int collected = 0;     // total number of arguments collected
-        int result_count = 0;  // local variable for number of results in a single arg string
-        // deal with purely flag like things
-        if(max_num == 0) {
-            auto res = op->get_flag_value(arg_name, value);
-            op->add_result(res);
-            parse_order_.push_back(op.get());
-        } else if(!value.empty()) {  // --this=value
-            op->add_result(value, result_count);
-            parse_order_.push_back(op.get());
-            collected += result_count;
-            // -Trest
-        } else if(!rest.empty()) {
-            op->add_result(rest, result_count);
-            parse_order_.push_back(op.get());
-            rest = "";
-            collected += result_count;
+        // don't capture missing if this is a nameless subcommand and nameless subcommands can't fallthrough
+        if(parent_ != nullptr && name_.empty()) {
+            return false;
         }
 
-        // gather the minimum number of arguments
-        while(min_num > collected && !args.empty()) {
-            std::string current_ = args.back();
-            args.pop_back();
-            op->add_result(current_, result_count);
-            parse_order_.push_back(op.get());
-            collected += result_count;
-        }
+        // If a subcommand, try the main command
+        if(parent_ != nullptr && fallthrough_)
+            return _get_fallthrough_parent()->_parse_arg(args, current_type);
 
-        if(min_num > collected) {  // if we have run out of arguments and the minimum was not met
-            throw ArgumentMismatch::TypedAtLeast(op->get_name(), min_num, op->get_type_name());
-        }
+        // Otherwise, add to missing
+        args.pop_back();
+        _move_to_missing(current_type, current);
+        return true;
+    }
 
-        if(max_num > collected || op->get_allow_extra_args()) {  // we allow optional arguments
-            auto remreqpos = _count_remaining_positionals(true);
-            // we have met the minimum now optionally check up to the maximum
-            while((collected < max_num || op->get_allow_extra_args()) && !args.empty() &&
-                  _recognize(args.back(), false) == detail::Classifier::NONE) {
-                // If any required positionals remain, don't keep eating
-                if(remreqpos >= args.size()) {
-                    break;
-                }
+    args.pop_back();
 
-                op->add_result(args.back(), result_count);
-                parse_order_.push_back(op.get());
-                args.pop_back();
-                collected += result_count;
+    // Get a reference to the pointer to make syntax bearable
+    Option_p &op = *op_ptr;
+    /// if we require a separator add it here
+    if(op->get_inject_separator()) {
+        if(!op->results().empty() && !op->results().back().empty()) {
+            op->add_result(std::string{});
+        }
+    }
+    if(op->get_trigger_on_parse() && op->current_option_state_ == Option::option_state::callback_run) {
+        op->clear();
+    }
+    int min_num = (std::min)(op->get_type_size_min(), op->get_items_expected_min());
+    int max_num = op->get_items_expected_max();
+    // check container like options to limit the argument size to a single type if the allow_extra_flags argument is
+    // set. 16 is somewhat arbitrary (needs to be at least 4)
+    if(max_num >= detail::expected_max_vector_size / 16 && !op->get_allow_extra_args()) {
+        auto tmax = op->get_type_size_max();
+        max_num = detail::checked_multiply(tmax, op->get_expected_min()) ? tmax : detail::expected_max_vector_size;
+    }
+    // Make sure we always eat the minimum for unlimited vectors
+    int collected = 0;     // total number of arguments collected
+    int result_count = 0;  // local variable for number of results in a single arg string
+    // deal with purely flag like things
+    if(max_num == 0) {
+        auto res = op->get_flag_value(arg_name, value);
+        op->add_result(res);
+        parse_order_.push_back(op.get());
+    } else if(!value.empty()) {  // --this=value
+        op->add_result(value, result_count);
+        parse_order_.push_back(op.get());
+        collected += result_count;
+        // -Trest
+    } else if(!rest.empty()) {
+        op->add_result(rest, result_count);
+        parse_order_.push_back(op.get());
+        rest = "";
+        collected += result_count;
+    }
+
+    // gather the minimum number of arguments
+    while(min_num > collected && !args.empty()) {
+        std::string current_ = args.back();
+        args.pop_back();
+        op->add_result(current_, result_count);
+        parse_order_.push_back(op.get());
+        collected += result_count;
+    }
+
+    if(min_num > collected) {  // if we have run out of arguments and the minimum was not met
+        throw ArgumentMismatch::TypedAtLeast(op->get_name(), min_num, op->get_type_name());
+    }
+
+    // now check for optional arguments
+    if(max_num > collected || op->get_allow_extra_args()) {  // we allow optional arguments
+        auto remreqpos = _count_remaining_positionals(true);
+        // we have met the minimum now optionally check up to the maximum
+        while((collected < max_num || op->get_allow_extra_args()) && !args.empty() &&
+              _recognize(args.back(), false) == detail::Classifier::NONE) {
+            // If any required positionals remain, don't keep eating
+            if(remreqpos >= args.size()) {
+                break;
             }
-
-            // Allow -- to end an unlimited list and "eat" it
-            if(!args.empty() && _recognize(args.back()) == detail::Classifier::POSITIONAL_MARK)
-                args.pop_back();
-            // optional flag that didn't receive anything now get the default value
-            if(min_num == 0 && max_num > 0 && collected == 0) {
-                auto res = op->get_flag_value(arg_name, std::string{});
-                op->add_result(res);
-                parse_order_.push_back(op.get());
+            if(validate_optional_arguments_) {
+                std::string arg = args.back();
+                arg = op->_validate(arg, 0);
+                if(!arg.empty()) {
+                    break;
+                }
             }
+            op->add_result(args.back(), result_count);
+            parse_order_.push_back(op.get());
+            args.pop_back();
+            collected += result_count;
         }
 
-        // if we only partially completed a type then add an empty string for later processing
-        if(min_num > 0 && op->get_type_size_max() != min_num && (collected % op->get_type_size_max()) != 0) {
-            op->add_result(std::string{});
+        // Allow -- to end an unlimited list and "eat" it
+        if(!args.empty() && _recognize(args.back()) == detail::Classifier::POSITIONAL_MARK)
+            args.pop_back();
+        // optional flag that didn't receive anything now get the default value
+        if(min_num == 0 && max_num > 0 && collected == 0) {
+            auto res = op->get_flag_value(arg_name, std::string{});
+            op->add_result(res);
+            parse_order_.push_back(op.get());
         }
-
-        if(!rest.empty()) {
-            rest = "-" + rest;
-            args.push_back(rest);
+    }
+    // if we only partially completed a type then add an empty string if allowed for later processing
+    if(min_num > 0 && (collected % op->get_type_size_max()) != 0) {
+        if(op->get_type_size_max() != op->get_type_size_min()) {
+            op->add_result(std::string{});
+        } else {
+            throw ArgumentMismatch::PartialType(op->get_name(), op->get_type_size_min(), op->get_type_name());
         }
-        return true;
     }
+    if(op->get_trigger_on_parse()) {
+        op->run_callback();
+    }
+    if(!rest.empty()) {
+        rest = "-" + rest;
+        args.push_back(rest);
+    }
+    return true;
+}
 
-    /// Trigger the pre_parse callback if needed
-    void _trigger_pre_parse(std::size_t remaining_args) {
-        if(!pre_parse_called_) {
+CLI11_INLINE void App::_trigger_pre_parse(std::size_t remaining_args) {
+    if(!pre_parse_called_) {
+        pre_parse_called_ = true;
+        if(pre_parse_callback_) {
+            pre_parse_callback_(remaining_args);
+        }
+    } else if(immediate_callback_) {
+        if(!name_.empty()) {
+            auto pcnt = parsed_;
+            auto extras = std::move(missing_);
+            clear();
+            parsed_ = pcnt;
             pre_parse_called_ = true;
-            if(pre_parse_callback_) {
-                pre_parse_callback_(remaining_args);
-            }
-        } else if(immediate_callback_) {
-            if(!name_.empty()) {
-                auto pcnt = parsed_;
-                auto extras = std::move(missing_);
-                clear();
-                parsed_ = pcnt;
-                pre_parse_called_ = true;
-                missing_ = std::move(extras);
-            }
+            missing_ = std::move(extras);
         }
     }
+}
 
-    /// Get the appropriate parent to fallthrough to which is the first one that has a name or the main app
-    App *_get_fallthrough_parent() {
-        if(parent_ == nullptr) {
-            throw(HorribleError("No Valid parent"));
-        }
-        auto fallthrough_parent = parent_;
-        while((fallthrough_parent->parent_ != nullptr) && (fallthrough_parent->get_name().empty())) {
-            fallthrough_parent = fallthrough_parent->parent_;
-        }
-        return fallthrough_parent;
+CLI11_INLINE App *App::_get_fallthrough_parent() {
+    if(parent_ == nullptr) {
+        throw(HorribleError("No Valid parent"));
     }
+    auto *fallthrough_parent = parent_;
+    while((fallthrough_parent->parent_ != nullptr) && (fallthrough_parent->get_name().empty())) {
+        fallthrough_parent = fallthrough_parent->parent_;
+    }
+    return fallthrough_parent;
+}
 
-    /// Helper function to run through all possible comparisons of subcommand names to check there is no overlap
-    const std::string &_compare_subcommand_names(const App &subcom, const App &base) const {
-        static const std::string estring;
-        if(subcom.disabled_) {
-            return estring;
-        }
-        for(auto &subc : base.subcommands_) {
-            if(subc.get() != &subcom) {
-                if(subc->disabled_) {
-                    continue;
-                }
-                if(!subcom.get_name().empty()) {
-                    if(subc->check_name(subcom.get_name())) {
-                        return subcom.get_name();
-                    }
+CLI11_NODISCARD CLI11_INLINE const std::string &App::_compare_subcommand_names(const App &subcom,
+                                                                               const App &base) const {
+    static const std::string estring;
+    if(subcom.disabled_) {
+        return estring;
+    }
+    for(const auto &subc : base.subcommands_) {
+        if(subc.get() != &subcom) {
+            if(subc->disabled_) {
+                continue;
+            }
+            if(!subcom.get_name().empty()) {
+                if(subc->check_name(subcom.get_name())) {
+                    return subcom.get_name();
                 }
-                if(!subc->get_name().empty()) {
-                    if(subcom.check_name(subc->get_name())) {
-                        return subc->get_name();
-                    }
+            }
+            if(!subc->get_name().empty()) {
+                if(subcom.check_name(subc->get_name())) {
+                    return subc->get_name();
                 }
-                for(const auto &les : subcom.aliases_) {
-                    if(subc->check_name(les)) {
-                        return les;
-                    }
+            }
+            for(const auto &les : subcom.aliases_) {
+                if(subc->check_name(les)) {
+                    return les;
                 }
-                // this loop is needed in case of ignore_underscore or ignore_case on one but not the other
-                for(const auto &les : subc->aliases_) {
-                    if(subcom.check_name(les)) {
-                        return les;
-                    }
+            }
+            // this loop is needed in case of ignore_underscore or ignore_case on one but not the other
+            for(const auto &les : subc->aliases_) {
+                if(subcom.check_name(les)) {
+                    return les;
                 }
-                // if the subcommand is an option group we need to check deeper
-                if(subc->get_name().empty()) {
-                    auto &cmpres = _compare_subcommand_names(subcom, *subc);
-                    if(!cmpres.empty()) {
-                        return cmpres;
-                    }
+            }
+            // if the subcommand is an option group we need to check deeper
+            if(subc->get_name().empty()) {
+                const auto &cmpres = _compare_subcommand_names(subcom, *subc);
+                if(!cmpres.empty()) {
+                    return cmpres;
                 }
-                // if the test subcommand is an option group we need to check deeper
-                if(subcom.get_name().empty()) {
-                    auto &cmpres = _compare_subcommand_names(*subc, subcom);
-                    if(!cmpres.empty()) {
-                        return cmpres;
-                    }
+            }
+            // if the test subcommand is an option group we need to check deeper
+            if(subcom.get_name().empty()) {
+                const auto &cmpres = _compare_subcommand_names(*subc, subcom);
+                if(!cmpres.empty()) {
+                    return cmpres;
                 }
             }
         }
-        return estring;
     }
-    /// Helper function to place extra values in the most appropriate position
-    void _move_to_missing(detail::Classifier val_type, const std::string &val) {
-        if(allow_extras_ || subcommands_.empty()) {
-            missing_.emplace_back(val_type, val);
-            return;
-        }
-        // allow extra arguments to be places in an option group if it is allowed there
-        for(auto &subc : subcommands_) {
-            if(subc->name_.empty() && subc->allow_extras_) {
-                subc->missing_.emplace_back(val_type, val);
-                return;
-            }
-        }
-        // if we haven't found any place to put them yet put them in missing
+    return estring;
+}
+
+CLI11_INLINE void App::_move_to_missing(detail::Classifier val_type, const std::string &val) {
+    if(allow_extras_ || subcommands_.empty()) {
         missing_.emplace_back(val_type, val);
+        return;
     }
-
-  public:
-    /// function that could be used by subclasses of App to shift options around into subcommands
-    void _move_option(Option *opt, App *app) {
-        if(opt == nullptr) {
-            throw OptionNotFound("the option is NULL");
-        }
-        // verify that the give app is actually a subcommand
-        bool found = false;
-        for(auto &subc : subcommands_) {
-            if(app == subc.get()) {
-                found = true;
-            }
-        }
-        if(!found) {
-            throw OptionNotFound("The Given app is not a subcommand");
-        }
-
-        if((help_ptr_ == opt) || (help_all_ptr_ == opt))
-            throw OptionAlreadyAdded("cannot move help options");
-
-        if(config_ptr_ == opt)
-            throw OptionAlreadyAdded("cannot move config file options");
-
-        auto iterator =
-            std::find_if(std::begin(options_), std::end(options_), [opt](const Option_p &v) { return v.get() == opt; });
-        if(iterator != std::end(options_)) {
-            const auto &opt_p = *iterator;
-            if(std::find_if(std::begin(app->options_), std::end(app->options_), [&opt_p](const Option_p &v) {
-                   return (*v == *opt_p);
-               }) == std::end(app->options_)) {
-                // only erase after the insertion was successful
-                app->options_.push_back(std::move(*iterator));
-                options_.erase(iterator);
-            } else {
-                throw OptionAlreadyAdded("option was not located: " + opt->get_name());
-            }
-        } else {
-            throw OptionNotFound("could not locate the given Option");
+    // allow extra arguments to be places in an option group if it is allowed there
+    for(auto &subc : subcommands_) {
+        if(subc->name_.empty() && subc->allow_extras_) {
+            subc->missing_.emplace_back(val_type, val);
+            return;
         }
     }
-};  // namespace CLI
+    // if we haven't found any place to put them yet put them in missing
+    missing_.emplace_back(val_type, val);
+}
 
-/// Extension of App to better manage groups of options
-class Option_group : public App {
-  public:
-    Option_group(std::string group_description, std::string group_name, App *parent)
-        : App(std::move(group_description), "", parent) {
-        group(group_name);
-        // option groups should have automatic fallthrough
+CLI11_INLINE void App::_move_option(Option *opt, App *app) {
+    if(opt == nullptr) {
+        throw OptionNotFound("the option is NULL");
     }
-    using App::add_option;
-    /// Add an existing option to the Option_group
-    Option *add_option(Option *opt) {
-        if(get_parent() == nullptr) {
-            throw OptionNotFound("Unable to locate the specified option");
+    // verify that the give app is actually a subcommand
+    bool found = false;
+    for(auto &subc : subcommands_) {
+        if(app == subc.get()) {
+            found = true;
         }
-        get_parent()->_move_option(opt, this);
-        return opt;
     }
-    /// Add an existing option to the Option_group
-    void add_options(Option *opt) { add_option(opt); }
-    /// Add a bunch of options to the group
-    template <typename... Args> void add_options(Option *opt, Args... args) {
-        add_option(opt);
-        add_options(args...);
+    if(!found) {
+        throw OptionNotFound("The Given app is not a subcommand");
     }
-    using App::add_subcommand;
-    /// Add an existing subcommand to be a member of an option_group
-    App *add_subcommand(App *subcom) {
-        App_p subc = subcom->get_parent()->get_subcommand_ptr(subcom);
-        subc->get_parent()->remove_subcommand(subcom);
-        add_subcommand(std::move(subc));
-        return subcom;
+
+    if((help_ptr_ == opt) || (help_all_ptr_ == opt))
+        throw OptionAlreadyAdded("cannot move help options");
+
+    if(config_ptr_ == opt)
+        throw OptionAlreadyAdded("cannot move config file options");
+
+    auto iterator =
+        std::find_if(std::begin(options_), std::end(options_), [opt](const Option_p &v) { return v.get() == opt; });
+    if(iterator != std::end(options_)) {
+        const auto &opt_p = *iterator;
+        if(std::find_if(std::begin(app->options_), std::end(app->options_), [&opt_p](const Option_p &v) {
+               return (*v == *opt_p);
+           }) == std::end(app->options_)) {
+            // only erase after the insertion was successful
+            app->options_.push_back(std::move(*iterator));
+            options_.erase(iterator);
+        } else {
+            throw OptionAlreadyAdded("option was not located: " + opt->get_name());
+        }
+    } else {
+        throw OptionNotFound("could not locate the given Option");
     }
-};
-/// Helper function to enable one option group/subcommand when another is used
-inline void TriggerOn(App *trigger_app, App *app_to_enable) {
+}
+
+CLI11_INLINE void TriggerOn(App *trigger_app, App *app_to_enable) {
     app_to_enable->enabled_by_default(false);
     app_to_enable->disabled_by_default();
     trigger_app->preparse_callback([app_to_enable](std::size_t) { app_to_enable->disabled(false); });
 }
 
-/// Helper function to enable one option group/subcommand when another is used
-inline void TriggerOn(App *trigger_app, std::vector<App *> apps_to_enable) {
+CLI11_INLINE void TriggerOn(App *trigger_app, std::vector<App *> apps_to_enable) {
     for(auto &app : apps_to_enable) {
         app->enabled_by_default(false);
         app->disabled_by_default();
     }
 
     trigger_app->preparse_callback([apps_to_enable](std::size_t) {
-        for(auto &app : apps_to_enable) {
+        for(const auto &app : apps_to_enable) {
             app->disabled(false);
         }
     });
 }
 
-/// Helper function to disable one option group/subcommand when another is used
-inline void TriggerOff(App *trigger_app, App *app_to_enable) {
+CLI11_INLINE void TriggerOff(App *trigger_app, App *app_to_enable) {
     app_to_enable->disabled_by_default(false);
     app_to_enable->enabled_by_default();
     trigger_app->preparse_callback([app_to_enable](std::size_t) { app_to_enable->disabled(); });
 }
 
-/// Helper function to disable one option group/subcommand when another is used
-inline void TriggerOff(App *trigger_app, std::vector<App *> apps_to_enable) {
+CLI11_INLINE void TriggerOff(App *trigger_app, std::vector<App *> apps_to_enable) {
     for(auto &app : apps_to_enable) {
         app->disabled_by_default(false);
         app->enabled_by_default();
     }
 
     trigger_app->preparse_callback([apps_to_enable](std::size_t) {
-        for(auto &app : apps_to_enable) {
+        for(const auto &app : apps_to_enable) {
             app->disabled();
         }
     });
 }
 
-/// Helper function to mark an option as deprecated
-inline void deprecate_option(Option *opt, const std::string &replacement = "") {
+CLI11_INLINE void deprecate_option(Option *opt, const std::string &replacement) {
     Validator deprecate_warning{[opt, replacement](std::string &) {
                                     std::cout << opt->get_name() << " is deprecated please use '" << replacement
                                               << "' instead\n";
                                     return std::string();
                                 },
                                 "DEPRECATED"};
     deprecate_warning.application_index(0);
     opt->check(deprecate_warning);
     if(!replacement.empty()) {
         opt->description(opt->get_description() + " DEPRECATED: please use '" + replacement + "' instead");
     }
 }
 
-/// Helper function to mark an option as deprecated
-inline void deprecate_option(App *app, const std::string &option_name, const std::string &replacement = "") {
-    auto opt = app->get_option(option_name);
-    deprecate_option(opt, replacement);
-}
-
-/// Helper function to mark an option as deprecated
-inline void deprecate_option(App &app, const std::string &option_name, const std::string &replacement = "") {
-    auto opt = app.get_option(option_name);
-    deprecate_option(opt, replacement);
-}
-
-/// Helper function to mark an option as retired
-inline void retire_option(App *app, Option *opt) {
+CLI11_INLINE void retire_option(App *app, Option *opt) {
     App temp;
-    auto option_copy = temp.add_option(opt->get_name(false, true))
-                           ->type_size(opt->get_type_size_min(), opt->get_type_size_max())
-                           ->expected(opt->get_expected_min(), opt->get_expected_max())
-                           ->allow_extra_args(opt->get_allow_extra_args());
+    auto *option_copy = temp.add_option(opt->get_name(false, true))
+                            ->type_size(opt->get_type_size_min(), opt->get_type_size_max())
+                            ->expected(opt->get_expected_min(), opt->get_expected_max())
+                            ->allow_extra_args(opt->get_allow_extra_args());
 
     app->remove_option(opt);
-    auto opt2 = app->add_option(option_copy->get_name(false, true), "option has been retired and has no effect")
-                    ->type_name("RETIRED")
-                    ->default_str("RETIRED")
-                    ->type_size(option_copy->get_type_size_min(), option_copy->get_type_size_max())
-                    ->expected(option_copy->get_expected_min(), option_copy->get_expected_max())
-                    ->allow_extra_args(option_copy->get_allow_extra_args());
+    auto *opt2 = app->add_option(option_copy->get_name(false, true), "option has been retired and has no effect")
+                     ->type_name("RETIRED")
+                     ->default_str("RETIRED")
+                     ->type_size(option_copy->get_type_size_min(), option_copy->get_type_size_max())
+                     ->expected(option_copy->get_expected_min(), option_copy->get_expected_max())
+                     ->allow_extra_args(option_copy->get_allow_extra_args());
 
     Validator retired_warning{[opt2](std::string &) {
                                   std::cout << "WARNING " << opt2->get_name() << " is retired and has no effect\n";
                                   return std::string();
                               },
                               ""};
     retired_warning.application_index(0);
     opt2->check(retired_warning);
 }
 
-/// Helper function to mark an option as retired
-inline void retire_option(App &app, Option *opt) { retire_option(&app, opt); }
+CLI11_INLINE void retire_option(App &app, Option *opt) { retire_option(&app, opt); }
 
-/// Helper function to mark an option as retired
-inline void retire_option(App *app, const std::string &option_name) {
+CLI11_INLINE void retire_option(App *app, const std::string &option_name) {
 
-    auto opt = app->get_option_no_throw(option_name);
+    auto *opt = app->get_option_no_throw(option_name);
     if(opt != nullptr) {
         retire_option(app, opt);
         return;
     }
-    auto opt2 = app->add_option(option_name, "option has been retired and has no effect")
-                    ->type_name("RETIRED")
-                    ->expected(0, 1)
-                    ->default_str("RETIRED");
+    auto *opt2 = app->add_option(option_name, "option has been retired and has no effect")
+                     ->type_name("RETIRED")
+                     ->expected(0, 1)
+                     ->default_str("RETIRED");
     Validator retired_warning{[opt2](std::string &) {
                                   std::cout << "WARNING " << opt2->get_name() << " is retired and has no effect\n";
                                   return std::string();
                               },
                               ""};
     retired_warning.application_index(0);
     opt2->check(retired_warning);
 }
 
-/// Helper function to mark an option as retired
-inline void retire_option(App &app, const std::string &option_name) { retire_option(&app, option_name); }
+CLI11_INLINE void retire_option(App &app, const std::string &option_name) { retire_option(&app, option_name); }
 
 namespace FailureMessage {
 
-/// Printout a clean, simple message on error (the default in CLI11 1.5+)
-inline std::string simple(const App *app, const Error &e) {
+CLI11_INLINE std::string simple(const App *app, const Error &e) {
     std::string header = std::string(e.what()) + "\n";
     std::vector<std::string> names;
 
     // Collect names
     if(app->get_help_ptr() != nullptr)
         names.push_back(app->get_help_ptr()->get_name());
 
@@ -8274,74 +8998,61 @@
     // If any names found, suggest those
     if(!names.empty())
         header += "Run with " + detail::join(names, " or ") + " for more information.\n";
 
     return header;
 }
 
-/// Printout the full help string on error (if this fn is set, the old default for CLI11)
-inline std::string help(const App *app, const Error &e) {
+CLI11_INLINE std::string help(const App *app, const Error &e) {
     std::string header = std::string("ERROR: ") + e.get_name() + ": " + e.what() + "\n";
     header += app->help();
     return header;
 }
 
 }  // namespace FailureMessage
 
+
+
+
 namespace detail {
-/// This class is simply to allow tests access to App's protected functions
-struct AppFriend {
-#ifdef CLI11_CPP14
 
-    /// Wrap _parse_short, perfectly forward arguments and return
-    template <typename... Args> static decltype(auto) parse_arg(App *app, Args &&... args) {
-        return app->_parse_arg(std::forward<Args>(args)...);
-    }
+std::string convert_arg_for_ini(const std::string &arg, char stringQuote = '"', char characterQuote = '\'');
 
-    /// Wrap _parse_subcommand, perfectly forward arguments and return
-    template <typename... Args> static decltype(auto) parse_subcommand(App *app, Args &&... args) {
-        return app->_parse_subcommand(std::forward<Args>(args)...);
-    }
-#else
-    /// Wrap _parse_short, perfectly forward arguments and return
-    template <typename... Args>
-    static auto parse_arg(App *app, Args &&... args) ->
-        typename std::result_of<decltype (&App::_parse_arg)(App, Args...)>::type {
-        return app->_parse_arg(std::forward<Args>(args)...);
-    }
+/// Comma separated join, adds quotes if needed
+std::string ini_join(const std::vector<std::string> &args,
+                     char sepChar = ',',
+                     char arrayStart = '[',
+                     char arrayEnd = ']',
+                     char stringQuote = '"',
+                     char characterQuote = '\'');
 
-    /// Wrap _parse_subcommand, perfectly forward arguments and return
-    template <typename... Args>
-    static auto parse_subcommand(App *app, Args &&... args) ->
-        typename std::result_of<decltype (&App::_parse_subcommand)(App, Args...)>::type {
-        return app->_parse_subcommand(std::forward<Args>(args)...);
-    }
-#endif
-    /// Wrap the fallthrough parent function to make sure that is working correctly
-    static App *get_fallthrough_parent(App *app) { return app->_get_fallthrough_parent(); }
-};
+std::vector<std::string> generate_parents(const std::string &section, std::string &name, char parentSeparator);
+
+/// assuming non default segments do a check on the close and open of the segments in a configItem structure
+void checkParentSegments(std::vector<ConfigItem> &output, const std::string &currentSection, char parentSeparator);
 }  // namespace detail
 
 
 
 
 namespace detail {
 
-inline std::string convert_arg_for_ini(const std::string &arg, char stringQuote = '"', char characterQuote = '\'') {
+CLI11_INLINE std::string convert_arg_for_ini(const std::string &arg, char stringQuote, char characterQuote) {
     if(arg.empty()) {
         return std::string(2, stringQuote);
     }
     // some specifically supported strings
     if(arg == "true" || arg == "false" || arg == "nan" || arg == "inf") {
         return arg;
     }
     // floating point conversion can convert some hex codes, but don't try that here
     if(arg.compare(0, 2, "0x") != 0 && arg.compare(0, 2, "0X") != 0) {
-        double val;
-        if(detail::lexical_cast(arg, val)) {
+        using CLI::detail::lexical_cast;
+        double val = 0.0;
+        if(lexical_cast(arg, val)) {
             return arg;
         }
     }
     // just quote a single non numeric character
     if(arg.size() == 1) {
         return std::string(1, characterQuote) + arg + characterQuote;
     }
@@ -8361,75 +9072,74 @@
             if(std::all_of(arg.begin() + 2, arg.end(), [](char x) { return (x == '0' || x == '1'); })) {
                 return arg;
             }
         }
     }
     if(arg.find_first_of(stringQuote) == std::string::npos) {
         return std::string(1, stringQuote) + arg + stringQuote;
-    } else {
-        return characterQuote + arg + characterQuote;
     }
+    return characterQuote + arg + characterQuote;
 }
 
-/// Comma separated join, adds quotes if needed
-inline std::string ini_join(const std::vector<std::string> &args,
-                            char sepChar = ',',
-                            char arrayStart = '[',
-                            char arrayEnd = ']',
-                            char stringQuote = '"',
-                            char characterQuote = '\'') {
+CLI11_INLINE std::string ini_join(const std::vector<std::string> &args,
+                                  char sepChar,
+                                  char arrayStart,
+                                  char arrayEnd,
+                                  char stringQuote,
+                                  char characterQuote) {
     std::string joined;
     if(args.size() > 1 && arrayStart != '\0') {
         joined.push_back(arrayStart);
     }
     std::size_t start = 0;
     for(const auto &arg : args) {
         if(start++ > 0) {
             joined.push_back(sepChar);
-            if(isspace(sepChar) == 0) {
+            if(!std::isspace<char>(sepChar, std::locale())) {
                 joined.push_back(' ');
             }
         }
         joined.append(convert_arg_for_ini(arg, stringQuote, characterQuote));
     }
     if(args.size() > 1 && arrayEnd != '\0') {
         joined.push_back(arrayEnd);
     }
     return joined;
 }
 
-inline std::vector<std::string> generate_parents(const std::string &section, std::string &name) {
+CLI11_INLINE std::vector<std::string>
+generate_parents(const std::string &section, std::string &name, char parentSeparator) {
     std::vector<std::string> parents;
     if(detail::to_lower(section) != "default") {
-        if(section.find('.') != std::string::npos) {
-            parents = detail::split(section, '.');
+        if(section.find(parentSeparator) != std::string::npos) {
+            parents = detail::split(section, parentSeparator);
         } else {
             parents = {section};
         }
     }
-    if(name.find('.') != std::string::npos) {
-        std::vector<std::string> plist = detail::split(name, '.');
+    if(name.find(parentSeparator) != std::string::npos) {
+        std::vector<std::string> plist = detail::split(name, parentSeparator);
         name = plist.back();
         detail::remove_quotes(name);
         plist.pop_back();
         parents.insert(parents.end(), plist.begin(), plist.end());
     }
 
     // clean up quotes on the parents
     for(auto &parent : parents) {
         detail::remove_quotes(parent);
     }
     return parents;
 }
 
-/// assuming non default segments do a check on the close and open of the segments in a configItem structure
-inline void checkParentSegments(std::vector<ConfigItem> &output, const std::string &currentSection) {
+CLI11_INLINE void
+checkParentSegments(std::vector<ConfigItem> &output, const std::string &currentSection, char parentSeparator) {
 
     std::string estring;
-    auto parents = detail::generate_parents(currentSection, estring);
+    auto parents = detail::generate_parents(currentSection, estring, parentSeparator);
     if(!output.empty() && output.back().name == "--") {
         std::size_t msize = (parents.size() > 1U) ? parents.size() : 2;
         while(output.back().parents.size() >= msize) {
             output.push_back(output.back());
             output.back().parents.pop_back();
         }
 
@@ -8469,61 +9179,76 @@
     output.back().parents = std::move(parents);
     output.back().name = "++";
 }
 }  // namespace detail
 
 inline std::vector<ConfigItem> ConfigBase::from_config(std::istream &input) const {
     std::string line;
-    std::string section = "default";
-
+    std::string currentSection = "default";
+    std::string previousSection = "default";
     std::vector<ConfigItem> output;
     bool isDefaultArray = (arrayStart == '[' && arrayEnd == ']' && arraySeparator == ',');
     bool isINIArray = (arrayStart == '\0' || arrayStart == ' ') && arrayStart == arrayEnd;
+    bool inSection{false};
     char aStart = (isINIArray) ? '[' : arrayStart;
     char aEnd = (isINIArray) ? ']' : arrayEnd;
     char aSep = (isINIArray && arraySeparator == ' ') ? ',' : arraySeparator;
-
+    int currentSectionIndex{0};
     while(getline(input, line)) {
         std::vector<std::string> items_buffer;
         std::string name;
 
         detail::trim(line);
         std::size_t len = line.length();
-        if(len > 1 && line.front() == '[' && line.back() == ']') {
-            if(section != "default") {
+        // lines have to be at least 3 characters to have any meaning to CLI just skip the rest
+        if(len < 3) {
+            continue;
+        }
+        if(line.front() == '[' && line.back() == ']') {
+            if(currentSection != "default") {
                 // insert a section end which is just an empty items_buffer
                 output.emplace_back();
-                output.back().parents = detail::generate_parents(section, name);
+                output.back().parents = detail::generate_parents(currentSection, name, parentSeparatorChar);
                 output.back().name = "--";
             }
-            section = line.substr(1, len - 2);
+            currentSection = line.substr(1, len - 2);
             // deal with double brackets for TOML
-            if(section.size() > 1 && section.front() == '[' && section.back() == ']') {
-                section = section.substr(1, section.size() - 2);
+            if(currentSection.size() > 1 && currentSection.front() == '[' && currentSection.back() == ']') {
+                currentSection = currentSection.substr(1, currentSection.size() - 2);
             }
-            if(detail::to_lower(section) == "default") {
-                section = "default";
+            if(detail::to_lower(currentSection) == "default") {
+                currentSection = "default";
             } else {
-                detail::checkParentSegments(output, section);
+                detail::checkParentSegments(output, currentSection, parentSeparatorChar);
+            }
+            inSection = false;
+            if(currentSection == previousSection) {
+                ++currentSectionIndex;
+            } else {
+                currentSectionIndex = 0;
+                previousSection = currentSection;
             }
             continue;
         }
-        if(len == 0) {
-            continue;
-        }
+
         // comment lines
         if(line.front() == ';' || line.front() == '#' || line.front() == commentChar) {
             continue;
         }
 
         // Find = in string, split and recombine
         auto pos = line.find(valueDelimiter);
         if(pos != std::string::npos) {
             name = detail::trim_copy(line.substr(0, pos));
             std::string item = detail::trim_copy(line.substr(pos + 1));
+            auto cloc = item.find(commentChar);
+            if(cloc != std::string::npos) {
+                item.erase(cloc, std::string::npos);  // NOLINT(readability-suspicious-call-argument)
+                detail::trim(item);
+            }
             if(item.size() > 1 && item.front() == aStart) {
                 for(std::string multiline; item.back() != aEnd && std::getline(input, multiline);) {
                     detail::trim(multiline);
                     item += multiline;
                 }
                 items_buffer = detail::split_up(item.substr(1, item.length() - 2), aSep);
             } else if((isDefaultArray || isINIArray) && item.find_first_of(aSep) != std::string::npos) {
@@ -8531,50 +9256,68 @@
             } else if((isDefaultArray || isINIArray) && item.find_first_of(' ') != std::string::npos) {
                 items_buffer = detail::split_up(item);
             } else {
                 items_buffer = {item};
             }
         } else {
             name = detail::trim_copy(line);
+            auto cloc = name.find(commentChar);
+            if(cloc != std::string::npos) {
+                name.erase(cloc, std::string::npos);  // NOLINT(readability-suspicious-call-argument)
+                detail::trim(name);
+            }
+
             items_buffer = {"true"};
         }
-        if(name.find('.') == std::string::npos) {
+        if(name.find(parentSeparatorChar) == std::string::npos) {
             detail::remove_quotes(name);
         }
         // clean up quotes on the items
         for(auto &it : items_buffer) {
             detail::remove_quotes(it);
         }
 
-        std::vector<std::string> parents = detail::generate_parents(section, name);
-
+        std::vector<std::string> parents = detail::generate_parents(currentSection, name, parentSeparatorChar);
+        if(parents.size() > maximumLayers) {
+            continue;
+        }
+        if(!configSection.empty() && !inSection) {
+            if(parents.empty() || parents.front() != configSection) {
+                continue;
+            }
+            if(configIndex >= 0 && currentSectionIndex != configIndex) {
+                continue;
+            }
+            parents.erase(parents.begin());
+            inSection = true;
+        }
         if(!output.empty() && name == output.back().name && parents == output.back().parents) {
             output.back().inputs.insert(output.back().inputs.end(), items_buffer.begin(), items_buffer.end());
         } else {
             output.emplace_back();
             output.back().parents = std::move(parents);
             output.back().name = std::move(name);
             output.back().inputs = std::move(items_buffer);
         }
     }
-    if(section != "default") {
+    if(currentSection != "default") {
         // insert a section end which is just an empty items_buffer
         std::string ename;
         output.emplace_back();
-        output.back().parents = detail::generate_parents(section, ename);
+        output.back().parents = detail::generate_parents(currentSection, ename, parentSeparatorChar);
         output.back().name = "--";
         while(output.back().parents.size() > 1) {
             output.push_back(output.back());
             output.back().parents.pop_back();
         }
     }
     return output;
 }
 
-inline std::string
+CLI11_INLINE std::string
 ConfigBase::to_config(const App *app, bool default_also, bool write_description, std::string prefix) const {
     std::stringstream out;
     std::string commentLead;
     commentLead.push_back(commentChar);
     commentLead.push_back(' ');
 
     std::vector<std::string> groups = app->get_groups();
@@ -8613,14 +9356,17 @@
                         value = "false";
                     } else if(opt->get_run_callback_for_default()) {
                         value = "\"\"";  // empty string default value
                     }
                 }
 
                 if(!value.empty()) {
+                    if(!opt->get_fnames().empty()) {
+                        value = opt->get_flag_value(name, value);
+                    }
                     if(write_description && opt->has_description()) {
                         out << '\n';
                         out << commentLead << detail::fix_newlines(commentLead, opt->get_description()) << '\n';
                     }
                     out << name << valueDelimiter << value << '\n';
                 }
             }
@@ -8638,58 +9384,61 @@
 
     for(const App *subcom : subcommands) {
         if(!subcom->get_name().empty()) {
             if(subcom->get_configurable() && app->got_subcommand(subcom)) {
                 if(!prefix.empty() || app->get_parent() == nullptr) {
                     out << '[' << prefix << subcom->get_name() << "]\n";
                 } else {
-                    std::string subname = app->get_name() + "." + subcom->get_name();
-                    auto p = app->get_parent();
+                    std::string subname = app->get_name() + parentSeparatorChar + subcom->get_name();
+                    const auto *p = app->get_parent();
                     while(p->get_parent() != nullptr) {
-                        subname = p->get_name() + "." + subname;
+                        subname = p->get_name() + parentSeparatorChar + subname;
                         p = p->get_parent();
                     }
                     out << '[' << subname << "]\n";
                 }
                 out << to_config(subcom, default_also, write_description, "");
             } else {
-                out << to_config(subcom, default_also, write_description, prefix + subcom->get_name() + ".");
+                out << to_config(
+                    subcom, default_also, write_description, prefix + subcom->get_name() + parentSeparatorChar);
             }
         }
     }
 
     return out.str();
 }
 
 
 
 
-inline std::string
+
+
+CLI11_INLINE std::string
 Formatter::make_group(std::string group, bool is_positional, std::vector<const Option *> opts) const {
     std::stringstream out;
 
     out << "\n" << group << ":\n";
     for(const Option *opt : opts) {
         out << make_option(opt, is_positional);
     }
 
     return out.str();
 }
 
-inline std::string Formatter::make_positionals(const App *app) const {
+CLI11_INLINE std::string Formatter::make_positionals(const App *app) const {
     std::vector<const Option *> opts =
         app->get_options([](const Option *opt) { return !opt->get_group().empty() && opt->get_positional(); });
 
     if(opts.empty())
-        return std::string();
+        return {};
 
     return make_group(get_label("Positionals"), true, opts);
 }
 
-inline std::string Formatter::make_groups(const App *app, AppFormatMode mode) const {
+CLI11_INLINE std::string Formatter::make_groups(const App *app, AppFormatMode mode) const {
     std::stringstream out;
     std::vector<std::string> groups = app->get_groups();
 
     // Options
     for(const std::string &group : groups) {
         std::vector<const Option *> opts = app->get_options([app, mode, &group](const Option *opt) {
             return opt->get_group() == group                     // Must be in the right group
@@ -8705,41 +9454,41 @@
                 out << "\n";
         }
     }
 
     return out.str();
 }
 
-inline std::string Formatter::make_description(const App *app) const {
+CLI11_INLINE std::string Formatter::make_description(const App *app) const {
     std::string desc = app->get_description();
     auto min_options = app->get_require_option_min();
     auto max_options = app->get_require_option_max();
     if(app->get_required()) {
         desc += " REQUIRED ";
     }
     if((max_options == min_options) && (min_options > 0)) {
         if(min_options == 1) {
             desc += " \n[Exactly 1 of the following options is required]";
         } else {
-            desc += " \n[Exactly " + std::to_string(min_options) + "options from the following list are required]";
+            desc += " \n[Exactly " + std::to_string(min_options) + " options from the following list are required]";
         }
     } else if(max_options > 0) {
         if(min_options > 0) {
             desc += " \n[Between " + std::to_string(min_options) + " and " + std::to_string(max_options) +
                     " of the follow options are required]";
         } else {
             desc += " \n[At most " + std::to_string(max_options) + " of the following options are allowed]";
         }
     } else if(min_options > 0) {
         desc += " \n[At least " + std::to_string(min_options) + " of the following options are required]";
     }
     return (!desc.empty()) ? desc + "\n" : std::string{};
 }
 
-inline std::string Formatter::make_usage(const App *app, std::string name) const {
+CLI11_INLINE std::string Formatter::make_usage(const App *app, std::string name) const {
     std::stringstream out;
 
     out << get_label("Usage") << ":" << (name.empty() ? "" : " ") << name;
 
     std::vector<std::string> groups = app->get_groups();
 
     // Print an Options badge if any options exist
@@ -8773,23 +9522,23 @@
     }
 
     out << std::endl;
 
     return out.str();
 }
 
-inline std::string Formatter::make_footer(const App *app) const {
+CLI11_INLINE std::string Formatter::make_footer(const App *app) const {
     std::string footer = app->get_footer();
     if(footer.empty()) {
         return std::string{};
     }
-    return footer + "\n";
+    return "\n" + footer + "\n";
 }
 
-inline std::string Formatter::make_help(const App *app, std::string name, AppFormatMode mode) const {
+CLI11_INLINE std::string Formatter::make_help(const App *app, std::string name, AppFormatMode mode) const {
 
     // This immediately forwards to the make_expanded method. This is done this way so that subcommands can
     // have overridden formatters
     if(mode == AppFormatMode::Sub)
         return make_expanded(app);
 
     std::stringstream out;
@@ -8800,20 +9549,20 @@
     }
 
     out << make_description(app);
     out << make_usage(app, name);
     out << make_positionals(app);
     out << make_groups(app, mode);
     out << make_subcommands(app, mode);
-    out << '\n' << make_footer(app);
+    out << make_footer(app);
 
     return out.str();
 }
 
-inline std::string Formatter::make_subcommands(const App *app, AppFormatMode mode) const {
+CLI11_INLINE std::string Formatter::make_subcommands(const App *app, AppFormatMode mode) const {
     std::stringstream out;
 
     std::vector<const App *> subcommands = app->get_subcommands({});
 
     // Make a list in definition order of the groups seen
     std::vector<std::string> subcmd_groups_seen;
     for(const App *com : subcommands) {
@@ -8847,21 +9596,21 @@
             }
         }
     }
 
     return out.str();
 }
 
-inline std::string Formatter::make_subcommand(const App *sub) const {
+CLI11_INLINE std::string Formatter::make_subcommand(const App *sub) const {
     std::stringstream out;
     detail::format_help(out, sub->get_display_name(true), sub->get_description(), column_width_);
     return out.str();
 }
 
-inline std::string Formatter::make_expanded(const App *sub) const {
+CLI11_INLINE std::string Formatter::make_expanded(const App *sub) const {
     std::stringstream out;
     out << sub->get_display_name(true) << "\n";
 
     out << make_description(sub);
     if(sub->get_name().empty() && !sub->get_aliases().empty()) {
         detail::format_aliases(out, sub->get_aliases(), column_width_ + 2);
     }
@@ -8873,32 +9622,32 @@
     std::string tmp = detail::find_and_replace(out.str(), "\n\n", "\n");
     tmp = tmp.substr(0, tmp.size() - 1);  // Remove the final '\n'
 
     // Indent all but the first line (the name)
     return detail::find_and_replace(tmp, "\n", "\n  ") + "\n";
 }
 
-inline std::string Formatter::make_option_name(const Option *opt, bool is_positional) const {
+CLI11_INLINE std::string Formatter::make_option_name(const Option *opt, bool is_positional) const {
     if(is_positional)
         return opt->get_name(true, false);
 
     return opt->get_name(false, true);
 }
 
-inline std::string Formatter::make_option_opts(const Option *opt) const {
+CLI11_INLINE std::string Formatter::make_option_opts(const Option *opt) const {
     std::stringstream out;
 
     if(!opt->get_option_text().empty()) {
         out << " " << opt->get_option_text();
     } else {
         if(opt->get_type_size() != 0) {
             if(!opt->get_type_name().empty())
                 out << " " << get_label(opt->get_type_name());
             if(!opt->get_default_str().empty())
-                out << "=" << opt->get_default_str();
+                out << " [" << opt->get_default_str() << "] ";
             if(opt->get_expected_max() == detail::expected_max_vector_size)
                 out << " ...";
             else if(opt->get_expected_min() > 1)
                 out << " x " << opt->get_expected();
 
             if(opt->get_required())
                 out << " " << get_label("REQUIRED");
@@ -8915,24 +9664,23 @@
             for(const Option *op : opt->get_excludes())
                 out << " " << op->get_name();
         }
     }
     return out.str();
 }
 
-inline std::string Formatter::make_option_desc(const Option *opt) const { return opt->get_description(); }
+CLI11_INLINE std::string Formatter::make_option_desc(const Option *opt) const { return opt->get_description(); }
 
-inline std::string Formatter::make_option_usage(const Option *opt) const {
+CLI11_INLINE std::string Formatter::make_option_usage(const Option *opt) const {
     // Note that these are positionals usages
     std::stringstream out;
     out << make_option_name(opt, true);
     if(opt->get_expected_max() >= detail::expected_max_vector_size)
         out << "...";
     else if(opt->get_expected_max() > 1)
         out << "(" << opt->get_expected() << "x)";
 
     return opt->get_required() ? out.str() : "[" + out.str() + "]";
 }
 
 
-
 } // namespace CLI
```

### Comparing `aestream-0.5.1/include/CPM.cmake` & `aestream-0.6.0/include/CPM.cmake`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/include/rapidxml.hpp` & `aestream-0.6.0/include/rapidxml.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/setup.py` & `aestream-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,25 +24,25 @@
         ]
 except:
     pass
 
 # Setuptools entrypoint
 setup(
     name="aestream",
-    version="0.5.1",
-    author="Jens E. Pedersen, Christian Pehle",
-    author_email="jens@jepedersen.dk, christian.pehle@gmail.com",
-    url="https://github.com/norse/aestream",
+    version="0.6.0",
+    author="Jens E. Pedersen",
+    author_email="jens@jepedersen.dk",
+    url="https://github.com/aestream/aestream",
     description="Streaming library for Address-Event Representation (AER) data",
     license="MIT",
     long_description=readme_text,
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
     packages=["aestream"],
-    install_requires=["numpy"],
+    install_requires=["numpy", "pysdl2-dll"],
     extras_require={"torch": ["torch"]},
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: C++",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Hardware :: Universal Serial Bus (USB)",
```

### Comparing `aestream-0.5.1/src/CMakeLists.txt` & `aestream-0.6.0/src/CMakeLists.txt`

 * *Files 27% similar despite different names*

```diff
@@ -22,13 +22,35 @@
 
 if (USE_PYTHON)
   # AEStream Python
   add_subdirectory(pybind)
 endif() 
 
 # AEStream executable
-add_executable(aestream aestream.cpp)
+set(aestream_sources "")
+set(aestream_link_libraries "")
+find_package(SDL2 CONFIG COMPONENTS SDL2 QUIET)
+if (SDL2_FOUND)
+  message(STATUS "SDL2 found")
+  set(WITH_SDL ON)
+  list(APPEND aestream_sources viewer/viewer.cpp viewer/viewer.hpp)
+  list(APPEND aestream_link_libraries SDL2)
+  add_compile_definitions(WITH_SDL)
+else()
+  message(STATUS "SDL2 not found, cannot compile viewer")
+endif()
+add_executable(aestream aestream.cpp ${aestream_sources})
 target_include_directories(aestream PRIVATE ${CMAKE_INSTALL_LIBDIR})
-target_link_libraries(aestream PRIVATE aer aestream_file aestream_input aestream_output)
+target_link_libraries(aestream PRIVATE aer aestream_file aestream_input aestream_output ${aestream_link_libraries})
 
 # Install targets
-install(IMPORTED_RUNTIME_ARTIFACTS aestream DESTINATION ${CMAKE_INSTALL_BINDIR})
+if (${USE_CAMERA})
+  set(aestream_drivers "")
+  if (${WITH_CAER})
+    list(APPEND aestream_drivers "libcaer")
+  endif()
+  if (${WITH_METAVISION})
+    list(APPEND aestream_drivers "MetavisionSDK::core MetavisionSDK::driver")
+  endif()
+endif()
+install(TARGETS aer aestream_file aestream_input aestream_output EXPORT aestream DESTINATION ${CMAKE_INSTALL_LIBDIR})
+install(TARGETS aestream DESTINATION ${CMAKE_INSTALL_BINDIR})
```

### Comparing `aestream-0.5.1/src/aestream.cpp` & `aestream-0.6.0/src/aestream.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,24 @@
 #include "input/file.hpp"
 #ifdef WITH_CAER
 #include "input/inivation.hpp"
 #endif
 #ifdef WITH_METAVISION
 #include "input/prophesee.hpp"
 #endif
+#ifdef WITH_ZMQ
+#include "input/zmq.hpp"
+#endif
 
 // Output
 #include "output/dvs_to_file.hpp"
 #include "output/dvs_to_udp.hpp"
+#ifdef WITH_SDL
+#include "viewer/viewer.hpp"
+#endif
 
 // Interrupt
 auto runFlag = std::atomic<bool>(true);
 void signalHandler(int signum) { runFlag.store(false); }
 
 // Main
 int main(int argc, char *argv[]) {
@@ -47,15 +53,15 @@
   // Inivation cameras
   auto app_input_inivation = app_input->add_subcommand(
       "inivation", "DVS input source for inivation cameras");
   app_input_inivation->add_option("id", deviceId, "Hardware ID");
   app_input_inivation->add_option("address", deviceAddress, "Hardware address");
   app_input_inivation->add_option("camera", camera,
                                   "Type of camera; davis or dvx");
-  uint64_t timeLimitMs;
+  int64_t timeLimitMs;
   app_input_inivation
       ->add_option("timeout", timeLimitMs,
                    "Time limit of the stream in ms. Defaults to infinity")
       ->default_val(-1);
   // Prophesee cameras
   auto app_input_prophesee = app_input->add_subcommand(
       "prophesee", "DVS input source for prophesee cameras");
@@ -68,14 +74,20 @@
   auto app_input_file = app_input->add_subcommand("file", "AEDAT4 input file");
   app_input_file
       ->add_option("file", input_filename, "Path to .aedat or .aedat4 file")
       ->required();
   // app_input_file->add_flag(
   //     "--ignore-time", input_ignore_time,
   //     "Playback in real-time (false, default) or ignore timestamps (true).");
+  // - ZMQ
+  std::string input_zmq_socket = "tcp://0.0.0.0:40001";
+  auto app_input_zmq =
+      app_input->add_subcommand("speck", "SynSense Speck input");
+  app_input_zmq->add_option("sock", input_zmq_socket,
+                            "ZMQ socket. Defaults to tcp://0.0.0.0:40001");
 
   //
   // Output
   //
   auto app_output =
       app.add_subcommand("output", "Output target. Defaults to stdout");
   // - STDOUT
@@ -99,15 +111,34 @@
       "Number of events in a single UDP packet. Defaults to 128");
   app_output_udp->add_option("--include-timestamp", include_timestamp,
                              "Include timestamp in events");
   // - FILE
   std::string output_filename;
   auto app_output_file = app_output->add_subcommand("file", "File output");
   app_output_file->add_option("output-filename", output_filename,
-                              "Output Filename. Supports .txt or .aedat4");
+                              "Output Filename. Supports .csv or .aedat4");
+  // - VIEWER
+#ifdef WITH_SDL
+  size_t viewer_width = 1280;
+  size_t viewer_height = 720;
+  size_t viewer_frame_duration = 20;
+  bool viewer_quiet = false;
+  auto app_output_viewer =
+      app_output->add_subcommand("view", "View event stream on-screen");
+  app_output_viewer->add_option(
+      "--width", viewer_width, "Width of viewport in pixels. Defaults to 1280");
+  app_output_viewer->add_option(
+      "--height", viewer_height,
+      "Height of viewport in pixels. Defaults to 720");
+  app_output_viewer->add_option(
+      "--frame_duration", viewer_frame_duration,
+      "Duration of one rendered frame in ms. Defaults to 20");
+  app_output_viewer->add_flag("--quiet,-q", viewer_quiet,
+                              "Prevent the viewer from printing");
+#endif
 
   //
   // Generate options
   //
   std::int64_t maxPackets = -1;
   app.add_option("--max-packets", maxPackets,
                  "Maximum number of packets to read before stopping. Defaults "
@@ -138,41 +169,53 @@
     throw std::invalid_argument(
         "Prophesee cameras unavailable: please recompile with MetavisionSDK");
 #endif
   } else if (app_input_file->parsed()) {
     file_handle = open_event_file(input_filename);
     input_generator = file_handle->stream();
   }
+#ifdef WITH_ZMQ
+  else if (app_input_zmq->parsed()) {
+    input_generator = open_zmq(input_zmq_socket, runFlag);
+  }
+#endif
 
   //
   // Handle output
   //
   try {
     if (app_output_udp->parsed()) {
       std::cout << "Sending events to: " << ipAddress << " on port: " << port
                 << std::endl;
       DVSToUDP<AER::Event> client(bufferSize, port, ipAddress);
       client.stream(input_generator, include_timestamp);
     } else if (app_output_file->parsed()) {
       std::cout << "Sending events to file " << output_filename << std::endl;
-      if (output_filename.ends_with(".txt")) {
-        dvs_to_file_txt(input_generator, output_filename);
+      if (output_filename.ends_with(".csv")) {
+        dvs_to_file_csv(input_generator, output_filename);
       } else if (output_filename.ends_with(".aedat4")) {
         dvs_to_file_aedat(input_generator, output_filename);
       } else {
         std::stringstream error;
         error << "Unsupported file ending" << output_filename;
         throw std::invalid_argument(error.str());
       }
-    } else { // Default to STDOUT
+    }
+#ifdef WITH_SDL
+    else if (app_output_viewer->parsed()) {
+      view_stream(input_generator, viewer_width, viewer_height,
+                  viewer_frame_duration, viewer_quiet);
+    }
+#endif
+    else { // Default to STDOUT
       uint64_t count = 0;
       for (AER::Event event : input_generator) {
         count += 1;
-        std::cout << event.x << "," << event.y << ","
-                  << std::to_string(event.timestamp) << std::endl;
+        std::cout << std::to_string(event.timestamp) << "," << event.x << ","
+                  << event.y << "," << event.polarity << std::endl;
       }
       std::cout << "Sent a total of " << count << " events" << std::endl;
     }
   } catch (const std::exception &e) {
     std::cout << "Failure while streaming events: " << e.what() << "\n";
   }
 }
```

### Comparing `aestream-0.5.1/src/dvs_gesture.hpp` & `aestream-0.6.0/src/dvs_gesture.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/file/CMakeLists.txt` & `aestream-0.6.0/src/file/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 set(input_definitions "")
-set(input_sources aedat.hpp aedat4.hpp dat.hpp utils.hpp )
+set(input_sources aedat.hpp aedat4.hpp evt3.hpp csv.hpp dat.hpp utils.hpp )
 set(input_libraries aer)
 set(input_include_directories "")
 
 # Include flatbuffers and generate headers
 find_package(flatbuffers CONFIG NAMES flatbuffers Flatbuffers FlatBuffers QUIET)
 set(FLATBUFFERS_BUILD_TESTS OFF)
 if (flatbuffers_FOUND AND FLATBUFFERS_SOURCE_DIR) # Add flatbuffers from source dir (set in flake.nix)
```

### Comparing `aestream-0.5.1/src/file/aedat.hpp` & `aestream-0.6.0/src/file/aedat.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/file/aedat4.hpp` & `aestream-0.6.0/src/file/aedat4.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -160,18 +160,20 @@
     auto packetHeader = PacketHeader(0, size);
     stream.write((char *)&packetHeader, 8);
 
     // Write events
     stream.write(compressed, size);
   }
 
-  std::tuple<AER::Event *, size_t> read_events(const int64_t n_events = -1) {
+  std::tuple<std::vector<AER::Event>, size_t>
+  read_events(const int64_t n_events = -1) {
     int64_t byte_count =
         (n_events > 0 ? n_events : total_number_of_events) * sizeof(AER::Event);
-    AER::Event *events = (AER::Event *)malloc(byte_count);
+    std::vector<AER::Event> events{};
+    events.resize(n_events > 0 ? n_events : total_number_of_events);
 
     int64_t count = 0;
     while (get_packet()) {
       for (; packet_events_read < event_vector->size(); ++packet_events_read) {
         const Event *event = event_vector->Get(packet_events_read);
         if (n_events > 0 && n_events - count <= 0) {
           return {events, count};
@@ -238,45 +240,45 @@
       attributes[name] = value;
     }
     return attributes;
   }
 
   void read_file_header() {
     static const uint32_t VERSION_STRING_SIZE = 14;
-    char data[BUFFER_SIZE];
-    size_t dst_size = dst_buffer.size();
+    std::vector<char> data_buffer(BUFFER_SIZE);
 
     struct stat stat_info;
     if (fstat(fileno(fp.get()), &stat_info)) {
       throw std::runtime_error("Failed to stat file");
     }
 
-    auto header_ret = fread(data, 1, dst_size, fp.get());
+    auto header_ret = fread(data_buffer.data(), 1, dst_buffer.size(), fp.get());
     if (header_ret <= 0) {
       throw std::runtime_error("Failed to read file version number");
     }
 
-    auto header = std::string(data, VERSION_STRING_SIZE);
+    auto header = std::string(data_buffer.data(), VERSION_STRING_SIZE);
     if (header != "#!AER-DAT4.0\r\n") {
       throw std::runtime_error("Invalid AEDAT version");
     }
 
     // find size of IOHeader (it is variable)
     flatbuffers::uoffset_t ioheader_offset =
-        *reinterpret_cast<flatbuffers::uoffset_t *>(data + VERSION_STRING_SIZE);
+        *reinterpret_cast<flatbuffers::uoffset_t *>(data_buffer.data() +
+                                                    VERSION_STRING_SIZE);
     const IOHeader *ioheader =
-        GetSizePrefixedIOHeader(data + VERSION_STRING_SIZE);
+        GetSizePrefixedIOHeader(data_buffer.data() + VERSION_STRING_SIZE);
 
     // TODO: We currently only support LZ4 compression
     if (ioheader->compression() != CompressionType_LZ4 &&
         ioheader->compression() != CompressionType_LZ4_HIGH) {
       throw std::runtime_error("Only LZ4 compression is supported");
     }
 
-    const auto data_table_position = ioheader->data_table_position();
+    const size_t data_table_position = ioheader->data_table_position();
     if (data_table_position < 0) {
       throw std::runtime_error(
           "AEDAT files without datatables are currently not supported");
     }
 
     // rapidxml::xml_document<> doc;
     // doc.parse<0>((char *)(ioheader->info_node()->str().c_str()));
@@ -335,34 +337,45 @@
     if (LZ4F_isError(lz4_error)) {
       const auto message = "Error creating LZ4 decompression context: " +
                            std::string(LZ4F_getErrorName(lz4_error));
       throw std::runtime_error(message);
     }
 
     // Load data table
-    fseek(fp.get(), data_table_position, SEEK_SET);
+    if (fseek(fp.get(), data_table_position, SEEK_SET) != 0) {
+      throw std::runtime_error("Failed to locate AEDAT4 data table");
+    }
     size_t data_table_size = stat_info.st_size - data_table_position;
-    size_t table_ret = fread(data, 1, data_table_size, fp.get());
-    if (table_ret != data_table_size) {
+    // Ensure buffer is large enough
+    if (data_buffer.size() < data_table_size) {
+      data_buffer.resize(data_table_size);
+      dst_buffer.resize(data_table_size * 2); // Ensure sufficient capacity
+    }
+    if (fread(data_buffer.data(), sizeof(char), data_table_size, fp.get()) !=
+        data_table_size) {
       throw std::runtime_error("Failed to read AEDAT4 data table");
     }
-    auto ret = LZ4F_decompress(ctx, &dst_buffer[0], &dst_size, data,
-                               &data_table_size, nullptr);
+    size_t dst_capacity = dst_buffer.capacity();
+    int ret = LZ4F_decompress(ctx, dst_buffer.data(), &dst_capacity,
+                              data_buffer.data(), &data_table_size, nullptr);
     if (LZ4F_isError(ret)) {
       std::string message = "Error decompressing AEDAT4 DataTable:" +
                             std::string(LZ4F_getErrorName(ret));
       throw std::runtime_error(message);
     }
-    const auto table = GetSizePrefixedFileDataTable(&dst_buffer[0]);
+    auto root = GetSizePrefixedFileDataTable(dst_buffer.data());
 
     // Record offsets of event packets
     // TODO: add IMU + frames
-    auto packets = table->table();
+    auto packets = root->table();
     for (size_t i = 0; i < packets->size(); ++i) {
-      const auto *definition = packets->Get(i);
+      auto definition = packets->Get(i);
+      if (definition->num_elements() == 0) {
+        continue;
+      }
       const auto stream_id = definition->packet_info()->stream_id();
       const size_t offset = definition->byte_offset();
       switch (stream_id) {
       case 0: {
         event_packet_offsets.push_back(offset - 8); // Include 8 byte header
         total_number_of_events += definition->num_elements();
       }
@@ -424,17 +437,17 @@
     // Read packet bytes
     auto packet_ret = fread(&packet_buffer[0], 1, size, fp.get());
     if (packet_ret == 0) { // Error or EOF
       return false;
     }
 
     // Decompress packet
-    size_t dst_size = dst_buffer.size();
     size_t decomp_size = size;
-    auto ret = LZ4F_decompress(ctx, &dst_buffer[0], &dst_size,
+    size_t dst_capacity = dst_buffer.capacity();
+    auto ret = LZ4F_decompress(ctx, &dst_buffer[0], &dst_capacity,
                                &packet_buffer[0], &decomp_size, nullptr);
     if (LZ4F_isError(ret)) {
       printf("Decompression package error: %s\n", LZ4F_getErrorName(ret));
       return false;
     }
     const auto events = GetSizePrefixedEventPacket(&dst_buffer[0]);
     event_vector = events->elements();
```

### Comparing `aestream-0.5.1/src/file/dat.hpp` & `aestream-0.6.0/src/file/dat.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -39,56 +39,63 @@
           event.timestamp = (overflows << 32) | event.timestamp;
         }
         co_yield event;
       }
     } while (size > 0);
   }
 
-  std::tuple<AER::Event *, size_t> read_events(const int64_t n_events = -1) {
+  std::tuple<std::vector<AER::Event>, size_t>
+  read_events(const int64_t n_events = -1) {
     static const size_t READ_BUFFER_SIZE = 4096;
     const size_t buffer_size = n_events > 0 ? n_events : READ_BUFFER_SIZE;
     const size_t event_array_size =
         n_events > 0 ? n_events : total_number_of_events;
 
-    uint64_t *buffer = (uint64_t *)malloc(buffer_size * sizeof(uint64_t));
-    AER::Event *events =
-        (AER::Event *)malloc(event_array_size * sizeof(AER::Event));
+    std::vector<uint64_t> buffer_vector = std::vector<uint64_t>();
+    buffer_vector.resize(buffer_size);
+    uint64_t *buffer = buffer_vector.data();
+    std::vector<AER::Event> events{};
+    events.reserve(event_array_size);
     size_t timestep = 0, overflows = 0, index = 0, size = 0;
     do {
       size = fread(buffer, sizeof(uint64_t), buffer_size, fp.get());
 
       if (size == 0 && !feof(fp.get())) {
         throw std::runtime_error("Error when processing .dat file");
       }
 
       if (size > n_events - index) {
+        fseek(fp.get(), size - (n_events - index), SEEK_CUR); // Re-align file
         size = n_events - index;
       }
 
       for (size_t i = 0; i < size; ++i) {
         AER::Event event = dat_decode_event(buffer[i], overflows);
         if (event.timestamp < timestep) { // Timestep overflow occurred
           overflows++;
           event.timestamp = (overflows << 32) | event.timestamp;
         }
-        events[index + i] = event;
+        events.push_back(event);
       }
       index += size;
     } while (size > 0 && n_events - index > 0);
     return {events, index};
   }
 
   explicit DAT(const std::string &filename) : DAT(open_file(filename)) {}
   explicit DAT(file_t &&fp)
       : fp(std::move(fp)), total_number_of_events{dat_read_header()} {}
 
 private:
   const file_t fp;
   const size_t total_number_of_events;
 
+  static constexpr char HEADER_END = 0x0A;   // \n
+  static constexpr char HEADER_START = 0x25; // %
+
   size_t dat_read_header() {
     size_t bytes_read = 0;
     uint8_t c, header_begins;
 
     do {
       header_begins = 1;
       do {
```

### Comparing `aestream-0.5.1/src/file/utils.hpp` & `aestream-0.6.0/src/file/utils.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,54 @@
 #include <memory>
 #include <queue>
 #include <string>
 
 #include "../aer.hpp"
 #include "../generator.hpp"
 
-#define HEADER_START 0x25
-#define HEADER_END 0x0A
 #define BUFFER_SIZE 4096
 
-static void close_file(FILE *fp) {
-  if (fp) {
+static void close_file(FILE *fp)
+{
+  if (fp)
+  {
     fclose(fp);
   }
 }
 
 typedef std::unique_ptr<FILE, decltype(&close_file)> file_t;
 
 // Thanks to https://stackoverflow.com/a/2072890/999865
-static bool ends_with(std::string const &value, std::string const &ending) {
+static bool ends_with(std::string const &value, std::string const &ending)
+{
   if (ending.size() > value.size())
     return false;
   return std::equal(ending.rbegin(), ending.rend(), value.rbegin());
 }
 
-static file_t open_file(const std::string &filename) {
+static file_t open_file(const std::string &filename)
+{
   file_t fp(fopen(filename.c_str(), "rb"), &close_file);
 
-  if (fp.get() == NULL) {
+  if (fp.get() == NULL)
+  {
     throw std::invalid_argument("Cannot open file " +
                                 filename); // throw std::runtime_error("");
   }
   return fp;
 }
 
+static long file_size(FILE *fp) {
+  auto origin = ftell(fp);
+  fseek(fp, 0, SEEK_END);
+  auto size = ftell(fp);
+  fseek(fp, origin, SEEK_SET);
+  return size;
+}
 
-struct FileBase {
+struct FileBase
+{
   virtual ~FileBase() = default;
   virtual Generator<AER::Event> stream(const int64_t n_events = -1) = 0;
-  virtual std::tuple<AER::Event *, size_t>
+  virtual std::tuple<std::vector<AER::Event>, size_t>
   read_events(const int64_t n_events = -1) = 0;
 };
```

### Comparing `aestream-0.5.1/src/generator.hpp` & `aestream-0.6.0/src/generator.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/input/inivation.cpp` & `aestream-0.6.0/src/input/inivation.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/input/inivation.hpp` & `aestream-0.6.0/src/input/inivation.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -25,23 +25,29 @@
 class CAERUSBConnection {
   uint32_t containerInterval = 128;
   uint32_t bufferSize = 1024;
   libcaer::devices::device *handle;
 
   //   static void signalHandler(int signal) { close(); }
   static void shutdownHandler(void *ptr) {
-    // Unused
+    // close();
   }
 
 public:
   CAERUSBConnection(std::optional<InivationDeviceAddress> deviceAddress);
   ~CAERUSBConnection() { close(); }
 
   std::unique_ptr<libcaer::events::EventPacketContainer> getPacket() {
     return handle->dataGet();
   }
-  void close() { handle->dataStop(); }
+  void close() { 
+    try {
+      handle->dataStop();
+    } catch (const std::runtime_error &e) {
+      // Ignore exceptions
+    }
+  }
 };
 
 Generator<AER::Event>
 inivation_event_generator(std::optional<InivationDeviceAddress> device_address,
                           const std::atomic<bool> &runFlag);
```

### Comparing `aestream-0.5.1/src/input/prophesee.cpp` & `aestream-0.6.0/src/input/prophesee.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/output/CMakeLists.txt` & `aestream-0.6.0/src/output/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 set(output_definitions "")
-set(output_sources dvs_to_udp.hpp dvs_to_udp.cpp dvs_to_file.hpp dvs_to_file.cpp )
+set(output_sources dvs_to_udp.hpp dvs_to_udp.cpp dvs_to_file.hpp dvs_to_file.cpp)
 set(output_libraries aer aestream_file)
 
 # Create the output library
 add_library(aestream_output SHARED ${output_sources})
 target_compile_definitions(aestream_output PUBLIC ${output_definitions})
 target_compile_features(aestream_output PUBLIC cxx_std_20)
 target_include_directories(aestream_output PRIVATE "${TORCH_INCLUDE_DIRS}" ${CMAKE_INSTALL_LIBDIR})
```

### Comparing `aestream-0.5.1/src/output/dvs_to_file.cpp` & `aestream-0.6.0/src/output/dvs_to_file.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 
   // Footer
   AEDAT4::save_footer(fileOutput, headerOffset, timeStart, timeEnd, sum);
   fileOutput.flush();
   fileOutput.close();
 }
 
-void dvs_to_file_txt(Generator<AER::Event> &input_generator,
+void dvs_to_file_csv(Generator<AER::Event> &input_generator,
                      const std::string &filename) {
   std::fstream fileOutput;
   fileOutput.open(filename, std::fstream::app);
 
   for (AER::Event event : input_generator) {
-    fileOutput << event.timestamp << " " << event.x << " "
-               << event.y << " " << event.polarity << std::endl;
+    fileOutput << event.timestamp << "," << event.x << ","
+               << event.y << "," << event.polarity << std::endl;
   }
 
   fileOutput.close();
 }
```

### Comparing `aestream-0.5.1/src/output/dvs_to_tensor.cpp` & `aestream-0.6.0/src/output/dvs_to_tensor.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/output/dvs_to_tensor.hpp` & `aestream-0.6.0/src/output/dvs_to_tensor.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/output/dvs_to_udp.cpp` & `aestream-0.6.0/src/output/dvs_to_udp.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/output/dvs_to_udp.hpp` & `aestream-0.6.0/src/output/dvs_to_udp.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/CMakeLists.txt` & `aestream-0.6.0/src/pybind/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,26 +6,33 @@
 if (USE_CUDA)
   if(NOT DEFINED ${CMAKE_CUDA_ARCHITECTURES})
     set(CMAKE_CUDA_ARCHITECTURES 50 52 60 61 70 75 80 86)
   endif()
   find_package(CUDAToolkit REQUIRED)
 
   enable_language(CUDA)
-  set(module_source_files "${module_source_files}" tensor_buffer_kernel.cu)
-  set(module_link_libraries CUDA::cudart)
-  set(module_compile_definitions USE_CUDA)
+  list(APPEND module_source_files "${module_source_files}" tensor_buffer_kernel.cu)
+  list(APPEND module_link_libraries CUDA::cudart)
+  list(APPEND module_compile_definitions USE_CUDA)
 endif()
 
 # Configure Inivation
-if (libcaer_FOUND) 
-  set(module_compile_definitions WITH_CAER)
-  set(module_source_files "${module_source_files}" usb.cpp)
+if (WITH_CAER) 
+  list(APPEND module_compile_definitions WITH_CAER)
+  list(APPEND module_source_files "${module_source_files}" usb.cpp)
 endif()
 
-# find_library(MetavisionSDK NAMES metavision_sdk_core REQUIRED)
+# Configure ZMQ
+if (WITH_ZMQ)
+  list(APPEND module_compile_definitions WITH_ZMQ)
+  list(APPEND module_source_files "${module_source_files}" zmq.cpp)
+endif()
+
+# Configure Python extension
+find_package(PythonExtensions REQUIRED)
 
 # Thanks to https://github.com/wjakob/nanobind_example/blob/master/CMakeLists.txt
 # Create CMake targets for all Python components needed by nanobind
 if (CMAKE_VERSION VERSION_GREATER_EQUAL 3.26)
   find_package(Python 3.8 COMPONENTS Interpreter Development.Module Development.SABIModule REQUIRED)
 else()
   find_package(Python 3.8 COMPONENTS Interpreter Development.Module REQUIRED)
@@ -71,11 +78,11 @@
 else()
   set_target_properties(aestream_ext PROPERTIES
     INSTALL_RPATH "\$ORIGIN"
     INSTALL_RPATH_USE_LINK_PATH TRUE
   )
 endif()
 target_compile_definitions(aestream_ext PRIVATE ${module_compile_definitions})
-target_include_directories(aestream_ext PRIVATE "${CMAKE_INSTALL_LIBDIR}" "${CUDA_INCLUDE_DIRS}" "${CudaToolkitLibDir}" "${PYTHON_SITE_PACKAGES_DIR}/aestream")
+target_include_directories(aestream_ext PRIVATE "${CMAKE_INSTALL_LIBDIR}" "${CUDA_INCLUDE_DIRS}" "${CudaToolkitLibDir}" "${PYTHON_SITE_PACKAGES_DIR}")
 target_link_libraries(aestream_ext PRIVATE ${module_link_libraries} aer aestream_file aestream_input aestream_output)
 
 install(TARGETS aestream_ext LIBRARY DESTINATION aestream)
```

### Comparing `aestream-0.5.1/src/pybind/convert.cpp` & `aestream-0.6.0/src/pybind/convert.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/convert.hpp` & `aestream-0.6.0/src/pybind/convert.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/file.cpp` & `aestream-0.6.0/src/pybind/file.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -23,31 +23,39 @@
 }
 
 FileInput::FileInput(const std::string &filename, py_size_t shape,
                      const std::string &device, bool ignore_time)
     : buffer(shape, device, EVENT_BUFFER_SIZE), ignore_time(ignore_time),
       shape(shape), filename(filename), file(open_event_file(filename)){};
 
-BufferPointer FileInput::read() {
+std::unique_ptr<BufferPointer> FileInput::read() {
   auto tmp = buffer.read();
   is_nonempty.store(false);
-  return tmp;
+  return std::unique_ptr<BufferPointer>(std::move(tmp));
 }
 
 Generator<AER::Event>::Iter FileInput::begin() { return generator.begin(); }
 std::default_sentinel_t FileInput::end() { return generator.end(); }
 
 bool FileInput::get_is_streaming() {
   return is_streaming.load() || is_nonempty.load();
 }
 
 nb::ndarray<nb::numpy, uint8_t, nb::shape<1, nb::any>> FileInput::load() {
+  struct Container {
+    std::vector<AER::Event> events;
+  };
   auto [arr, n_read] = file->read_events(-1);
+  Container *c = new Container();
+  c->events = std::move(arr);
+  nb::capsule deleter(c, [](void *p) noexcept {
+    delete (Container *) p;
+  });
   const size_t shape[1] = {n_read * sizeof(AER::Event)};
-  return nb::ndarray<nb::numpy, uint8_t, nb::shape<1, nb::any>>(arr, 1, shape);
+  return nb::ndarray<nb::numpy, uint8_t, nb::shape<1, nb::any>>(c->events.data(), 1, shape, deleter);
 }
 
 // py::array_t<AER::Event> FileInput::events_co() {
 //   AER::Event *event_array = (AER::Event *)malloc(n_events *
 //   sizeof(AER::Event)); size_t index = 0; for (auto event : generator) {
 //     event_array[index] = event;
 //     index++;
```

### Comparing `aestream-0.5.1/src/pybind/file.hpp` & `aestream-0.6.0/src/pybind/file.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #pragma once
-#include <algorithm>
 
 #include "../aer.hpp"
-#include "../file/aedat4.hpp"
 #include "../generator.hpp"
 #include "../input/file.hpp"
 
 #include "tensor_buffer.hpp"
 #include "tensor_iterator.hpp"
 
 class FileInput {
@@ -32,16 +30,16 @@
   const std::unique_ptr<FileBase> file;
   Generator<AER::Event> generator;
   const std::string filename;
 
   FileInput(const std::string &filename, py_size_t shape,
             const std::string &device, bool ignore_time = false);
 
-  BufferPointer read();
-
+  std::unique_ptr<BufferPointer> read();
+  void read_genn(uint32_t *bitmask, size_t size){ buffer.read_genn(bitmask, size); }
   Generator<AER::Event>::Iter begin();
   std::default_sentinel_t end();
 
   bool get_is_streaming();
 
   nb::ndarray<nb::numpy, uint8_t, nb::shape<1, nb::any>> load();
```

### Comparing `aestream-0.5.1/src/pybind/iterator.cpp` & `aestream-0.6.0/src/pybind/iterator.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/tensor_buffer.hpp` & `aestream-0.6.0/src/pybind/tensor_buffer.hpp`

 * *Files 23% similar despite different names*

```diff
@@ -19,50 +19,65 @@
 void free_memory_cuda(void *cuda_device_pointer);
 #endif
 template <typename scalar_t> struct BufferDeleter {
   void operator()(scalar_t *ptr) {
 #ifdef USE_CUDA
     free_memory_cuda(static_cast<void *>(ptr));
 #else
-    delete ptr;
+    delete[] ptr;
 #endif
   }
 };
 
 using tensor_numpy = nb::ndarray<nb::numpy, float, nb::shape<2, nb::any>>;
 using tensor_torch = nb::ndarray<nb::pytorch, float, nb::shape<2, nb::any>>;
 using buffer_t = std::unique_ptr<float[], BufferDeleter<float>>;
 using index_t = std::unique_ptr<int[], BufferDeleter<int>>;
 
 struct BufferPointer {
-  BufferPointer(buffer_t data, const std::vector<int64_t> &shape,
-                std::string device);
+  BufferPointer(buffer_t data, const std::vector<size_t> &shape,
+                const std::string& device);
   tensor_numpy to_numpy();
   tensor_torch to_torch();
+  const std::string& device;
 
 private:
-  std::string device;
-  const std::vector<int64_t> &shape;
+  const std::vector<size_t> &shape;
   buffer_t data;
 };
 
 class TensorBuffer {
 private:
-  const std::vector<int64_t> shape;
   uint64_t current_timestamp = 0;
   std::string device;
 
   std::mutex buffer_lock;
   buffer_t buffer1;
   buffer_t buffer2;
 #ifdef USE_CUDA
   std::vector<int> offset_buffer;
   index_t cuda_buffer;
 #endif
+  std::vector<uint32_t> genn_events;
+
+  void set_genn_event(int x, int y, bool polarity)
+  {
+    if(shape.size() == 2 || shape[2] == 1) {
+      const int idx = x + (y * shape[0]);
+      genn_events[idx / 32] |= (1 << (idx % 32));
+    }
+    else {
+      const int idx = (polarity ? 1 : 0) + (x * shape[2]) + (y * shape[0] * shape[2]);
+      genn_events[idx / 32] |= (1 << (idx % 32));
+    }
+  }
+
 public:
-  TensorBuffer(py_size_t size, std::string device, size_t buffer_size);
-  ~TensorBuffer();
+  TensorBuffer(std::vector<size_t> size, std::string device, size_t buffer_size);
+  const std::vector<size_t> shape;
+
   template <typename R> void assign_event(R *array, int16_t x, int16_t y);
   void set_buffer(uint16_t data[], int numbytes);
   void set_vector(std::vector<AER::Event> events);
-  BufferPointer read();
-};
+  std::unique_ptr<BufferPointer> read();
+  void read_genn(uint32_t *bitmask, size_t size);
+};
```

### Comparing `aestream-0.5.1/src/pybind/tensor_buffer_kernel.cu` & `aestream-0.6.0/src/pybind/tensor_buffer_kernel.cu`

 * *Files 20% similar despite different names*

```diff
@@ -11,22 +11,22 @@
       atomicAdd((array + offsets[index]), val);
     }
 }
 
 void index_increment_cuda(float *array, int *offset_pointer, size_t indices, int* event_device_pointer) {
   const size_t buffer_size = indices * sizeof(int);
 
-  cudaMemcpyAsync(event_device_pointer, offset_pointer, buffer_size, cudaMemcpyHostToDevice, 0);
+  cudaMemcpyAsync(event_device_pointer, offset_pointer, buffer_size, cudaMemcpyHostToDevice, cudaStreamPerThread);
   cuda_increment_kernel<float><<<1, indices>>>(array, event_device_pointer, indices);
 }
 
 void* alloc_memory_cuda(size_t buffer_size, size_t bytes) {
   void *cuda_device_pointer;
   const size_t size = buffer_size * bytes;
-  cudaMallocAsync(&cuda_device_pointer, size, 0);
-  cudaMemsetAsync(&cuda_device_pointer, 0, size, 0);
+  cudaMalloc(&cuda_device_pointer, size);
+  cudaMemset(&cuda_device_pointer, 0, size);
   return cuda_device_pointer;
 }
 
 void free_memory_cuda(void* cuda_device_pointer) {
   cudaFreeAsync(cuda_device_pointer, 0);
 }
```

### Comparing `aestream-0.5.1/src/pybind/tensor_iterator.cpp` & `aestream-0.6.0/src/pybind/tensor_iterator.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/tensor_iterator.hpp` & `aestream-0.6.0/src/pybind/tensor_iterator.hpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/test/test_file.py` & `aestream-0.6.0/src/pybind/test/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,8 +93,8 @@
                 break
             frame = stream.read()
             assert isinstance(frame, torch.Tensor)
             assert frame.device.type == "cuda"
             events += frame.sum()
             time.sleep(0.1)
         events += stream.read().sum()
-    assert events == 539136
+    assert events == 539481
```

### Comparing `aestream-0.5.1/src/pybind/test/test_udp.py` & `aestream-0.6.0/src/pybind/test/test_udp.py`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/udp.cpp` & `aestream-0.6.0/src/pybind/udp.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
   UDPInput *start_stream() {
     std::thread socket_thread(&UDPInput::serve_synchronous, this);
     socket_thread.detach();
     return this;
   }
 
-  BufferPointer read() { return buffer.read(); }
-
+  std::unique_ptr<BufferPointer> read() { return buffer.read(); }
+  void read_genn(uint32_t *bitmask, size_t size){ buffer.read_genn(bitmask, size); }
   void serve_synchronous() {
     int sockfd;
     int numbytes;
     uint16_t int_buf[max_events_per_packet];
 
     // Connect to socket
     struct sockaddr_storage their_addr;
```

### Comparing `aestream-0.5.1/src/pybind/udp_client.cpp` & `aestream-0.6.0/src/pybind/udp_client.cpp`

 * *Files identical despite different names*

### Comparing `aestream-0.5.1/src/pybind/usb.cpp` & `aestream-0.6.0/src/pybind/usb.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #include "../aer.hpp"
 #include "../generator.hpp"
 #include "../input/inivation.hpp"
 
 #include "types.hpp"
-
 #include "tensor_buffer.hpp"
 
 class USBInput {
 
 private:
   Generator<AER::Event> generator;
   std::thread socket_thread;
-  static const uint32_t EVENT_BUFFER_SIZE = 128;
+  static const uint32_t EVENT_BUFFER_SIZE = 64;
   TensorBuffer buffer;
   std::atomic<bool> is_streaming = {true};
+  std::atomic<bool> done_streaming = {false};
 
   void stream_synchronous() {
     while (is_streaming.load()) {
       // We add a local buffer to avoid overusing the atomic lock in the actual
       // buffer
       std::vector<AER::Event> local_buffer = {};
       for (auto event : generator) {
@@ -25,14 +25,15 @@
 
         if (local_buffer.size() >= EVENT_BUFFER_SIZE) {
           buffer.set_vector(local_buffer);
           local_buffer.clear();
         }
       }
     }
+    done_streaming.store(true);
   };
 
 public:
   USBInput(py_size_t shape, const std::string& device, uint16_t deviceId,
            uint16_t deviceAddress)
       : buffer(shape, device, EVENT_BUFFER_SIZE) {
     if (deviceId > 0) {
@@ -44,20 +45,25 @@
         generator = inivation_event_generator(address, is_streaming);
       }
     } else {
       generator = inivation_event_generator({}, is_streaming);
     }
   }
 
-  tensor_t read() { return buffer.read(); }
+  std::unique_ptr<BufferPointer> read() { 
+    return buffer.read(); 
+  }
+  void read_genn(uint32_t *bitmask, size_t size){ buffer.read_genn(bitmask, size); }
 
   USBInput *start_stream() {
     std::thread socket_thread(&USBInput::stream_synchronous, this);
     socket_thread.detach();
     return this;
   }
 
   void stop_stream() {
     is_streaming.store(false);
-    socket_thread.join();
+    while (!done_streaming.load()) {
+      // Wait until the thread is done streaming to avoid freeing memory too early
+    }
   }
 };
```

