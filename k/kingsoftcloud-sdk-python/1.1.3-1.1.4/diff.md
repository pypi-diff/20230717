# Comparing `tmp/kingsoftcloud-sdk-python-1.1.3.tar.gz` & `tmp/kingsoftcloud-sdk-python-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingsoftcloud-sdk-python-1.1.3.tar", last modified: Fri Jul 14 08:50:49 2023, max compression
+gzip compressed data, was "kingsoftcloud-sdk-python-1.1.4.tar", last modified: Mon Jul 17 06:44:14 2023, max compression
```

## Comparing `kingsoftcloud-sdk-python-1.1.3.tar` & `kingsoftcloud-sdk-python-1.1.4.tar`

### file list

```diff
@@ -1,159 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.809237 kingsoftcloud-sdk-python-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 08:50:49.809237 kingsoftcloud-sdk-python-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.777237 kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-14 08:50:49.000000 kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-14 08:50:49.000000 kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:50:49.000000 kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 08:50:49.000000 kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 08:50:49.000000 kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.777237 kingsoftcloud-sdk-python-1.1.3/ksyun/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/v20190401/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/v20190401/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/v20190401/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/v20190401/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/v20180601/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/v20180601/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/v20180601/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/v20180601/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.781237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.785237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20211209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20211209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20211209/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20211209/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.785237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.785237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.785237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.785237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.785237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.789237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/v20161122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/v20161122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/v20161122/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/v20161122/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.793237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.793237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/v20200101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/v20200101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/v20200101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/v20200101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.793237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.793237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   124863 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.793237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.793237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/v20170101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/v20170101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/v20170101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/v20170101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.797237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.797237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/v20210320/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/v20210320/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/v20210320/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/v20210320/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.797237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.797237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.797237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.797237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20171210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20171210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20171210/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20171210/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/v20151101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/v20151101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/v20151101/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/v20151101/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/v20200901/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/v20200901/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/v20200901/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/v20200901/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.801237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200114/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200114/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.805237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200831/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200831/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200831/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200831/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.805237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.805237 kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/v20160304/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/v20160304/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/v20160304/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/v20160304/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.805237 kingsoftcloud-sdk-python-1.1.3/ksyun/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.809237 kingsoftcloud-sdk-python-1.1.3/ksyun/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/exception/ksyun_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.809237 kingsoftcloud-sdk-python-1.1.3/ksyun/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:49.809237 kingsoftcloud-sdk-python-1.1.3/ksyun/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/ksyun/common/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 08:50:49.809237 kingsoftcloud-sdk-python-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-14 08:50:38.000000 kingsoftcloud-sdk-python-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 06:44:14.000000 kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/ksyun/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.698917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16760 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21288 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48112 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58267 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.702917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49208 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42904 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85700 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124863 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/kls/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36775 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.706917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43349 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59990 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.710917 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72970 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76572 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/ksyun_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/ksyun/common/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 06:44:14.714918 kingsoftcloud-sdk-python-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-17 06:44:03.000000 kingsoftcloud-sdk-python-1.1.4/setup.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.3/LICENSE` & `kingsoftcloud-sdk-python-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.3
+Version: 1.1.4
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.3/README.rst` & `kingsoftcloud-sdk-python-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/PKG-INFO` & `kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingsoftcloud-sdk-python
-Version: 1.1.3
+Version: 1.1.4
 Summary: Kingsoft Cloud SDK for Python
 Home-page: https://github.com/ksyun/ksyun-sdk-python
 Author: Kingsoft Cloud
 Maintainer-email: liuhuicheng1@kingsoft.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kingsoftcloud-sdk-python-1.1.3/kingsoftcloud_sdk_python.egg-info/SOURCES.txt` & `kingsoftcloud-sdk-python-1.1.4/kingsoftcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 ksyun/client/kead/v20200101/__init__.py
 ksyun/client/kead/v20200101/client.py
 ksyun/client/kead/v20200101/models.py
 ksyun/client/kec/__init__.py
 ksyun/client/kec/v20160304/__init__.py
 ksyun/client/kec/v20160304/client.py
 ksyun/client/kec/v20160304/models.py
+ksyun/client/kls/__init__.py
+ksyun/client/kls/v20170101/__init__.py
+ksyun/client/kls/v20170101/client.py
+ksyun/client/kls/v20170101/models.py
 ksyun/client/mongodb/__init__.py
 ksyun/client/mongodb/v20170101/__init__.py
 ksyun/client/mongodb/v20170101/client.py
 ksyun/client/mongodb/v20170101/models.py
 ksyun/client/resourcemanager/__init__.py
 ksyun/client/resourcemanager/v20210320/__init__.py
 ksyun/client/resourcemanager/v20210320/client.py
```

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/__init__.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '1.1.3'
+__version__ = '1.1.4'
```

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/v20190401/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/actiontrail/v20190401/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/actiontrail/v20190401/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/v20180601/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill/v20180601/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill/v20180601/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20211209/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bill_union/v20211209/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bill_union/v20211209/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/bws/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/bws/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/ebs/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/ebs/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/eip/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/eip/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/epc/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/epc/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/iam/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/iam/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/v20161122/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/kad/v20161122/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kad/v20161122/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/v20200101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/kead/v20200101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kead/v20200101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/kec/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/kec/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/v20170101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/mongodb/v20170101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/mongodb/v20170101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/v20210320/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/resourcemanager/v20210320/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/resourcemanager/v20210320/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/sks/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sks/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20171210/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/slb/v20171210/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/slb/v20171210/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/v20151101/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/sts/v20151101/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/sts/v20151101/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/v20200901/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/tagv2/v20200901/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/tagv2/v20200901/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200114/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200114/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200831/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/trade/v20200831/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/trade/v20200831/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/v20160304/client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/client/vpc/v20160304/models.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/client/vpc/v20160304/models.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/abstract_client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/abstract_model.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/common_client.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/common_client.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/credential.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/credential.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/exception/__init__.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/exception/ksyun_sdk_exception.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/exception/ksyun_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/http/request.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/http/request.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/profile/client_profile.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/profile/http_profile.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/ksyun/common/sign.py` & `kingsoftcloud-sdk-python-1.1.4/ksyun/common/sign.py`

 * *Files identical despite different names*

### Comparing `kingsoftcloud-sdk-python-1.1.3/setup.py` & `kingsoftcloud-sdk-python-1.1.4/setup.py`

 * *Files identical despite different names*

