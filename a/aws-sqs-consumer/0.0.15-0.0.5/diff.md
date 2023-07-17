# Comparing `tmp/aws_sqs_consumer-0.0.15.tar.gz` & `tmp/aws_sqs_consumer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_sqs_consumer-0.0.15.tar", max compression
+gzip compressed data, was "aws_sqs_consumer-0.0.5.tar", last modified: Tue Dec 21 14:42:45 2021, max compression
```

## Comparing `aws_sqs_consumer-0.0.15.tar` & `aws_sqs_consumer-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-07-17 14:14:16.384477 aws_sqs_consumer-0.0.15/LICENSE
--rw-r--r--   0        0        0     1341 2023-07-17 14:14:16.384477 aws_sqs_consumer-0.0.15/README.md
--rw-r--r--   0        0        0      321 2023-07-17 14:14:16.384477 aws_sqs_consumer-0.0.15/aws_sqs_consumer/__init__.py
--rw-r--r--   0        0        0     6183 2023-07-17 14:14:16.384477 aws_sqs_consumer-0.0.15/aws_sqs_consumer/consumer.py
--rw-r--r--   0        0        0      123 2023-07-17 14:14:16.384477 aws_sqs_consumer-0.0.15/aws_sqs_consumer/error.py
--rw-r--r--   0        0        0     1293 2023-07-17 14:14:16.384477 aws_sqs_consumer-0.0.15/aws_sqs_consumer/message.py
--rw-r--r--   0        0        0      994 2023-07-17 14:14:16.392477 aws_sqs_consumer-0.0.15/pyproject.toml
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 aws_sqs_consumer-0.0.15/PKG-INFO
+drwxr-xr-x   0 nowke      (501) staff       (20)        0 2021-12-21 14:42:45.080522 aws_sqs_consumer-0.0.5/
+-rw-r--r--   0 nowke      (501) staff       (20)     1071 2021-12-19 17:42:08.000000 aws_sqs_consumer-0.0.5/LICENSE
+-rw-r--r--   0 nowke      (501) staff       (20)      381 2021-12-21 14:42:45.080335 aws_sqs_consumer-0.0.5/PKG-INFO
+-rw-r--r--   0 nowke      (501) staff       (20)      566 2021-12-21 03:13:31.000000 aws_sqs_consumer-0.0.5/README.md
+drwxr-xr-x   0 nowke      (501) staff       (20)        0 2021-12-21 14:42:45.079392 aws_sqs_consumer-0.0.5/aws_sqs_consumer/
+-rw-r--r--   0 nowke      (501) staff       (20)       62 2021-12-21 03:12:46.000000 aws_sqs_consumer-0.0.5/aws_sqs_consumer/__init__.py
+-rw-r--r--   0 nowke      (501) staff       (20)     1625 2021-12-21 03:08:27.000000 aws_sqs_consumer-0.0.5/aws_sqs_consumer/aws_sqs_consumer.py
+drwxr-xr-x   0 nowke      (501) staff       (20)        0 2021-12-21 14:42:45.080037 aws_sqs_consumer-0.0.5/aws_sqs_consumer.egg-info/
+-rw-r--r--   0 nowke      (501) staff       (20)      381 2021-12-21 14:42:45.000000 aws_sqs_consumer-0.0.5/aws_sqs_consumer.egg-info/PKG-INFO
+-rw-r--r--   0 nowke      (501) staff       (20)      267 2021-12-21 14:42:45.000000 aws_sqs_consumer-0.0.5/aws_sqs_consumer.egg-info/SOURCES.txt
+-rw-r--r--   0 nowke      (501) staff       (20)        1 2021-12-21 14:42:45.000000 aws_sqs_consumer-0.0.5/aws_sqs_consumer.egg-info/dependency_links.txt
+-rw-r--r--   0 nowke      (501) staff       (20)       17 2021-12-21 14:42:45.000000 aws_sqs_consumer-0.0.5/aws_sqs_consumer.egg-info/top_level.txt
+-rw-r--r--   0 nowke      (501) staff       (20)      103 2021-12-19 17:36:00.000000 aws_sqs_consumer-0.0.5/pyproject.toml
+-rw-r--r--   0 nowke      (501) staff       (20)       38 2021-12-21 14:42:45.080577 aws_sqs_consumer-0.0.5/setup.cfg
+-rw-r--r--   0 nowke      (501) staff       (20)      449 2021-12-21 03:12:51.000000 aws_sqs_consumer-0.0.5/setup.py
```

### Comparing `aws_sqs_consumer-0.0.15/LICENSE` & `aws_sqs_consumer-0.0.5/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Hexmos Technology
+Copyright (c) 2022 Navaneesh Kumar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

