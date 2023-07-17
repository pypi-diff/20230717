# Comparing `tmp/bizlogic-0.1.0.tar.gz` & `tmp/bizlogic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.1.0.tar", max compression
+gzip compressed data, was "bizlogic-0.1.1.tar", max compression
```

## Comparing `bizlogic-0.1.0.tar` & `bizlogic-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.0/LICENSE
--rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.0/README.md
--rw-r--r--   0        0        0      341 2023-07-16 23:12:36.783630 bizlogic-0.1.0/bizlogic/__init__.py
--rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.0/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.0/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     6047 2023-07-08 02:24:36.315409 bizlogic-0.1.0/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.0/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1475 2023-05-15 17:30:35.538502 bizlogic-0.1.0/bizlogic/loan/status.py
--rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.0/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.0/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.0/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.0/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.0/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     3337 2023-05-15 17:30:35.539448 bizlogic-0.1.0/bizlogic/utils.py
--rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.0/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-07-16 23:12:25.550160 bizlogic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.1/README.md
+-rw-r--r--   0        0        0      341 2023-07-17 01:19:59.935715 bizlogic-0.1.1/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.1/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.1/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     6047 2023-07-08 02:24:36.315409 bizlogic-0.1.1/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.1/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1561 2023-07-17 01:14:36.341880 bizlogic-0.1.1/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.1/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.1/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.1/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.1/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.1/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3337 2023-05-15 17:30:35.539448 bizlogic-0.1.1/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.1/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-17 01:19:53.335965 bizlogic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.1/PKG-INFO
```

### Comparing `bizlogic-0.1.0/LICENSE` & `bizlogic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/README.md` & `bizlogic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/application.py` & `bizlogic-0.1.1/bizlogic/application.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/loan/reader.py` & `bizlogic-0.1.1/bizlogic/loan/reader.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/loan/repayment.py` & `bizlogic-0.1.1/bizlogic/loan/repayment.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/loan/status.py` & `bizlogic-0.1.1/bizlogic/loan/status.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,20 +40,17 @@
 
         Returns:
             LoanStatusType: the status of the loan
         """
         now = datetime.now()
         expiry = LoanStatus._timestamp_to_datetime(loan.offer_expiry)
 
-        if expiry <= now and not loan.accepted:
+        if expiry > now and not loan.accepted:  # if the loan has not expired and is not accepted
             return LoanStatusType.PENDING_ACCEPTANCE
 
-        elif expiry > now and not loan.accepted:
+        elif expiry <= now and not loan.accepted:  # if the loan has expired and is not accepted
             return LoanStatusType.EXPIRED_UNACCEPTED
 
-        elif expiry <= now and loan.accepted:
+        elif loan.accepted:  # if the loan is accepted, regardless of expiry
             return LoanStatusType.ACCEPTED
 
-        elif expiry > now and loan.accepted:
-            return LoanStatusType.ACCEPTED
-
-        raise
+        raise ValueError("Unable to determine loan status")
```

### Comparing `bizlogic-0.1.0/bizlogic/loan/writer.py` & `bizlogic-0.1.1/bizlogic/loan/writer.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.1.1/bizlogic/protoc/loan_application_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.1.1/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.1.1/bizlogic/protoc/vouch_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/utils.py` & `bizlogic-0.1.1/bizlogic/utils.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/bizlogic/vouch.py` & `bizlogic-0.1.1/bizlogic/vouch.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.1.0/PKG-INFO` & `bizlogic-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.1.0
+Version: 0.1.1
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
```

