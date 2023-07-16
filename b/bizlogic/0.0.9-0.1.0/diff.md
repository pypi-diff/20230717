# Comparing `tmp/bizlogic-0.0.9.tar.gz` & `tmp/bizlogic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bizlogic-0.0.9.tar", max compression
+gzip compressed data, was "bizlogic-0.1.0.tar", max compression
```

## Comparing `bizlogic-0.0.9.tar` & `bizlogic-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.0.9/LICENSE
--rw-r--r--   0        0        0     2000 2023-04-23 01:27:25.257694 bizlogic-0.0.9/README.md
--rw-r--r--   0        0        0      393 2023-04-23 19:20:59.434581 bizlogic-0.0.9/bizlogic/__init__.py
--rw-r--r--   0        0        0     3433 2023-04-23 19:19:35.197027 bizlogic-0.0.9/bizlogic/application.py
--rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.0.9/bizlogic/loan/__init__.py
--rw-r--r--   0        0        0     2230 2023-04-23 19:20:38.910227 bizlogic-0.0.9/bizlogic/loan/reader.py
--rw-r--r--   0        0        0     1600 2023-04-23 15:41:28.932012 bizlogic-0.0.9/bizlogic/loan/repayment.py
--rw-r--r--   0        0        0     1074 2023-04-23 15:39:56.859849 bizlogic-0.0.9/bizlogic/loan/status.py
--rw-r--r--   0        0        0     3231 2023-04-23 01:29:12.085631 bizlogic-0.0.9/bizlogic/loan/writer.py
--rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.0.9/bizlogic/protoc/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-23 15:31:58.337652 bizlogic-0.0.9/bizlogic/protoc/loan_application_pb2.py
--rw-r--r--   0        0        0     1709 2023-04-23 15:31:58.338431 bizlogic-0.0.9/bizlogic/protoc/loan_pb2.py
--rw-r--r--   0        0        0      942 2023-04-23 15:31:58.338641 bizlogic-0.0.9/bizlogic/protoc/vouch_pb2.py
--rw-r--r--   0        0        0     2128 2023-04-23 19:20:08.408812 bizlogic-0.0.9/bizlogic/vouch.py
--rw-r--r--   0        0        0      451 2023-04-23 19:20:51.434045 bizlogic-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bizlogic-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-20 00:41:45.427991 bizlogic-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2182 2023-05-15 17:30:35.537449 bizlogic-0.1.0/README.md
+-rw-r--r--   0        0        0      341 2023-07-16 23:12:36.783630 bizlogic-0.1.0/bizlogic/__init__.py
+-rw-r--r--   0        0        0     5923 2023-05-15 17:30:35.537815 bizlogic-0.1.0/bizlogic/application.py
+-rw-r--r--   0        0        0       61 2023-04-23 15:36:06.068712 bizlogic-0.1.0/bizlogic/loan/__init__.py
+-rw-r--r--   0        0        0     6047 2023-07-08 02:24:36.315409 bizlogic-0.1.0/bizlogic/loan/reader.py
+-rw-r--r--   0        0        0     2742 2023-07-16 23:08:16.349583 bizlogic-0.1.0/bizlogic/loan/repayment.py
+-rw-r--r--   0        0        0     1475 2023-05-15 17:30:35.538502 bizlogic-0.1.0/bizlogic/loan/status.py
+-rw-r--r--   0        0        0     4269 2023-05-15 17:30:35.538679 bizlogic-0.1.0/bizlogic/loan/writer.py
+-rw-r--r--   0        0        0       48 2023-04-23 15:35:52.968443 bizlogic-0.1.0/bizlogic/protoc/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-15 17:30:35.538935 bizlogic-0.1.0/bizlogic/protoc/loan_application_pb2.py
+-rw-r--r--   0        0        0     1709 2023-05-14 16:41:31.172854 bizlogic-0.1.0/bizlogic/protoc/loan_pb2.py
+-rw-r--r--   0        0        0      952 2023-05-15 17:30:35.539315 bizlogic-0.1.0/bizlogic/protoc/vouch_pb2.py
+-rw-r--r--   0        0        0     3337 2023-05-15 17:30:35.539448 bizlogic-0.1.0/bizlogic/utils.py
+-rw-r--r--   0        0        0     4165 2023-05-15 17:30:35.539612 bizlogic-0.1.0/bizlogic/vouch.py
+-rw-r--r--   0        0        0      451 2023-07-16 23:12:25.550160 bizlogic-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 bizlogic-0.1.0/PKG-INFO
```

### Comparing `bizlogic-0.0.9/LICENSE` & `bizlogic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.9/README.md` & `bizlogic-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 https://bizlogic.readthedocs.io/
 
 ### Build docs locally
 `mkdocs serve`
 
 ## Tests
-To only run tests: `pytest`  
+To only run tests: `pytest --cov=bizlogic --log-cli-level=debug`  
+To only run lints: `flake8 bizlogic --docstring-convention google --ignore=D100,D104 --exclude=loan_pb2.py,vouch_pb2.py,loan_application_pb2.py`
 To run all checks: `nox`
 
 ### Before running tests:
 
 #### Regenerate pb2.py files 
 ```
 protoc --python_out=bizlogic/protoc --proto_path=protobuf protobuf/*.proto
```

### Comparing `bizlogic-0.0.9/bizlogic/loan/repayment.py` & `bizlogic-0.1.0/bizlogic/loan/repayment.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,77 @@
 import datetime
-from typing import List
-from google.protobuf.timestamp_pb2 import Timestamp
 import uuid
+from typing import List
+import math
 
 from bizlogic.protoc.loan_pb2 import LoanPayment
 
+from google.protobuf.timestamp_pb2 import Timestamp
 
-class PaymentSchedule():
 
-    @staticmethod
+class PaymentSchedule():
+    """Payment Schedule Utilities."""
     @staticmethod
     def create_payment_schedule(
-            amount: int,
+            principal: int,
             interest_rate: float,
-            total_duration: datetime.timedelta,
+            start_date: datetime.datetime,
+            end_date: datetime.datetime,
             number_of_payments: int) -> List[LoanPayment]:
-        """
-        Generate a list of loan payment objects based on some initial loan parameters
+        """Generate a list of loan payment objects.
+
+        This method will create a schedule of uniformly distributed payments
+        from start_date to end_date inclusive.
 
         Args:
-            amount (int): The amount of the loan (before interest)
-            interest_rate (float): The interest rate of the loan in decimal (ex: 1.05 is 5%)
-            total_duration (datetime.timedelta): The time that the borrower has to finish all repayments
-            number_of_payments (int): The number of payments to break up the loan into
+            principal (int): The amount of the loan (before interest)
+            interest_rate (float): The interest rate of the loan in decimal
+                (ex: 0.05 is 5%)
+            start_date (datetime.datetime): Date when the first payment is due.
+            end_date (datetime.datetime): Date when the last payment is due.
+            number_of_payments (int): The total number of payments to break up
+                the loan into. Must be greater than 2.
+
+        Returns:
+            List[LoanPayment]: A list of loan payment objects
+
+        Raises:
+            ValueError: If the number of payments is not greater than 2.
         """
-        assert interest_rate > 1
+        if number_of_payments <= 2:
+            raise ValueError("Number of payments must be greater than 2")
 
         # calculate the payment terms
-        total_amount_due = amount * interest_rate
-        amount_due_each_payment = int(total_amount_due / number_of_payments)
-        first_payment = datetime.datetime.now()
+        total_amount_due = principal * (1 + interest_rate)
+        amount_due_each_payment = int(
+            math.ceil(
+                total_amount_due / number_of_payments
+            )
+        )
+
+        # calculate the duration between each payment
+        total_duration = end_date - start_date
+        payment_duration = total_duration / (number_of_payments - 1)
 
         result = []
         for payment_interval in range(number_of_payments):
-            timestamp = Timestamp()
-            timestamp.FromDatetime(first_payment + payment_interval * total_duration)
+            # calculate the due date
+            due_date = Timestamp()
+            if payment_interval == number_of_payments - 1:
+                # Set the due_date for the last payment to the end_date
+                # (to avoid rounding errors)
+                due_date.FromDatetime(end_date)
+            else:
+                # calculate the due_date for the other payments
+                due_date.FromDatetime(
+                    start_date + payment_duration * payment_interval
+                )
+
             # format the data
-            loan_payment = LoanPayment(
-                payment_id=str(uuid.uuid4()),
-                amount_due=amount_due_each_payment,
-                due_date=timestamp
-            )
+            loan_payment = LoanPayment()
+            loan_payment.payment_id = str(uuid.uuid4())
+            loan_payment.amount_due = amount_due_each_payment
+            loan_payment.due_date.CopyFrom(due_date)
+
             result.append(loan_payment)
+
+        return result
```

### Comparing `bizlogic-0.0.9/bizlogic/loan/writer.py` & `bizlogic-0.1.0/bizlogic/loan/writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 
 import datetime
 import time
 import uuid
 from typing import List, Self
 
-from ipfskvs.store import Store
-from ipfsclient.ipfs import Ipfs
-from ipfskvs.index import Index
-
-from bizlogic.protoc.loan_pb2 import Loan, LoanPayment
 from bizlogic.loan import PREFIX
+from bizlogic.protoc.loan_pb2 import Loan, LoanPayment
 
+from google.protobuf.timestamp_pb2 import Timestamp
 
-# ipfs filename:
-#   loan/borrower_<id>.lender_<id>.loan_<id>/created_<timestamp>
+from ipfsclient.ipfs import Ipfs
 
+from ipfskvs.index import Index
+from ipfskvs.store import Store
 
 
 class LoanWriter():
+    """Loan Writer.
+
+    ipfs filename:
+        loan/borrower_<id>.lender_<id>.loan_<id>/created_<timestamp>
+    """
+
     loan_id: str
     borrower: str
     lender: str
     index: Index
     data: Loan
     ipfsclient: Ipfs
 
@@ -29,86 +33,117 @@
             self: Self,
             ipfs: Ipfs,
             borrower: str,
             lender: str,
             principal_amount: int,
             repayment_schedule: List[LoanPayment],
             offer_expiry: datetime.date) -> None:
-        """Construct a new unaccepted loan and write it."""
+        """Construct a new unaccepted loan and write it.
+
+        The loan is not accepted until the borrower signs it.
+
+        Args:
+            ipfs: the ipfs client
+            borrower: the borrower id
+            lender: the lender id
+            principal_amount: the principal amount of the loan
+            repayment_schedule: the repayment schedule of the loan
+            offer_expiry: the expiry date of the loan offer
+        """
         self.loan_id = str(uuid.uuid4())
         self.borrower = borrower
         self.lender = lender
         self.ipfsclient = ipfs
+        timestamp = Timestamp()
+        timestamp.FromDatetime(offer_expiry)
         self.data = Loan(
             principal_amount=principal_amount,
             repayment_schedule=repayment_schedule,
-            offer_expiry=offer_expiry,
+            offer_expiry=timestamp,
             accepted=False
         )
 
     @staticmethod
-    def from_data(ipfs: Ipfs, data: Store):
+    def from_data(ipfs: Ipfs, data: Store) -> Self:
+        """Construct a loan from data.
+
+        Args:
+            ipfs: the ipfs client
+            data: the data to construct the loan from
+
+        Returns:
+            LoanWriter: the constructed loan
+        """
         return LoanWriter(
             ipfs=ipfs,
             borrower=data.index["borrower"],
             lender=data.index["lender"],
             principal_amount=data.reader.principal_amount,
             repayment_schedule=data.reader.repayment_schedule,
             offer_expiry=data.reader.offer_expiry
         )
 
-    def write(self):
+    def write(self: Self) -> None:
+        """Write the loan to IPFS."""
         self._generate_index()
 
         store = Store(
             index=self.index,
             ipfs=self.ipfsclient,
             writer=self.data
         )
 
         store.add()
-    
-    def _generate_index(self):
+
+    def _generate_index(self: Self) -> None:
+        """Generate the index for the loan."""
         self.index = Index(
             prefix=PREFIX,
             index={
                 "borrower": self.borrower,
                 "lender": self.lender,
                 "loan": self.loan_id
             },
             subindex=Index(
-                subindex=Index(
-                    index={
-                        "created": str(time.time_ns())
-                    }
-                )
+                index={
+                    "created": str(time.time_ns())
+                }
             )
         )
 
-    def accept_terms(self: Self):
+    def accept_terms(self: Self) -> None:
+        """Accept the loan terms."""
         self.data = Loan(
             principal_amount=self.data.principal_amount,
             repayment_schedule=self.data.repayment_schedule,
             offer_expiry=self.data.offer_expiry,
             accepted=True
         )
 
-    def register_payment(self: Self, payment_id: str, transaction: str):
+    def register_payment(
+            self: Self,
+            payment_id: str,
+            transaction: str) -> None:
+        """Register a payment.
+
+        Args:
+            payment_id: the payment id
+            transaction: the transaction id
+        """
         new_repayment_schedule = []
         for payment in self.data.repayment_schedule:
             if payment.payment_id == payment_id:
                 new_repayment_schedule.append(LoanPayment(
                     payment_id=payment_id,
                     amount_due=payment.amount_due_each_payment,
                     due_date=payment.timestamp,
                     transaction=transaction
                 ))
             else:
                 new_repayment_schedule.append(payment)
-        
+
         self.data = Loan(
             principal_amount=self.data.principal_amount,
             repayment_schedule=self.data.repayment_schedule,
             offer_expiry=self.data.offer_expiry,
             accepted=self.data.accepted
         )
-
```

### Comparing `bizlogic-0.0.9/bizlogic/protoc/loan_application_pb2.py` & `bizlogic-0.1.0/bizlogic/protoc/loan_application_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16loan_application.proto\x12\x10nanoswap.message\"8\n\x0fLoanApplication\x12\x15\n\ramount_asking\x18\x01 \x01(\x03\x12\x0e\n\x06\x63losed\x18\x03 \x01(\x08\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16loan_application.proto\x12\x10nanoswap.message\"8\n\x0fLoanApplication\x12\x15\n\ramount_asking\x18\x01 \x01(\x03\x12\x0e\n\x06\x63losed\x18\x02 \x01(\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'loan_application_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _LOANAPPLICATION._serialized_start=44
```

### Comparing `bizlogic-0.0.9/bizlogic/protoc/loan_pb2.py` & `bizlogic-0.1.0/bizlogic/protoc/loan_pb2.py`

 * *Files identical despite different names*

### Comparing `bizlogic-0.0.9/bizlogic/protoc/vouch_pb2.py` & `bizlogic-0.1.0/bizlogic/protoc/vouch_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bvouch.proto\x12\x10nanoswap.message\"\x18\n\x05Vouch\x12\x0f\n\x07voucher\x18\x01 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bvouch.proto\x12\x10nanoswap.message\"\x17\n\x05Vouch\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'vouch_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _VOUCH._serialized_start=33
-  _VOUCH._serialized_end=57
+  _VOUCH._serialized_end=56
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bizlogic-0.0.9/PKG-INFO` & `bizlogic-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bizlogic
-Version: 0.0.9
+Version: 0.1.0
 Summary: web3 lending platform business logic
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (==0.0.7)
@@ -43,15 +43,16 @@
 
 https://bizlogic.readthedocs.io/
 
 ### Build docs locally
 `mkdocs serve`
 
 ## Tests
-To only run tests: `pytest`  
+To only run tests: `pytest --cov=bizlogic --log-cli-level=debug`  
+To only run lints: `flake8 bizlogic --docstring-convention google --ignore=D100,D104 --exclude=loan_pb2.py,vouch_pb2.py,loan_application_pb2.py`
 To run all checks: `nox`
 
 ### Before running tests:
 
 #### Regenerate pb2.py files 
 ```
 protoc --python_out=bizlogic/protoc --proto_path=protobuf protobuf/*.proto
```

