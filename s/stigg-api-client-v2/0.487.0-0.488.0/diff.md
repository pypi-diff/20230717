# Comparing `tmp/stigg_api_client_v2-0.487.0.tar.gz` & `tmp/stigg_api_client_v2-0.488.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.487.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.488.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.487.0.tar` & `stigg_api_client_v2-0.488.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-16 07:56:46.819877 stigg_api_client_v2-0.487.0/README.md
--rw-r--r--   0        0        0      432 2023-07-16 07:57:31.388798 stigg_api_client_v2-0.487.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-16 07:56:46.819877 stigg_api_client_v2-0.487.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-16 07:56:46.819877 stigg_api_client_v2-0.487.0/stigg/client.py
--rw-r--r--   0        0        0    39986 2023-07-16 07:57:29.704763 stigg_api_client_v2-0.487.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-16 07:57:28.460736 stigg_api_client_v2-0.487.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-16 07:57:29.328755 stigg_api_client_v2-0.487.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    67443 2023-07-16 07:57:29.548759 stigg_api_client_v2-0.487.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-16 07:57:24.256650 stigg_api_client_v2-0.487.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-16 07:57:29.328755 stigg_api_client_v2-0.487.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-16 07:57:28.404735 stigg_api_client_v2-0.487.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-16 07:57:28.420736 stigg_api_client_v2-0.487.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67016 2023-07-16 07:57:24.476654 stigg_api_client_v2-0.487.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-16 07:57:28.448736 stigg_api_client_v2-0.487.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24302 2023-07-16 07:57:26.048686 stigg_api_client_v2-0.487.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-16 07:57:28.412736 stigg_api_client_v2-0.487.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-16 07:57:28.416736 stigg_api_client_v2-0.487.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-16 07:57:29.328755 stigg_api_client_v2-0.487.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    54916 2023-07-16 07:57:29.328755 stigg_api_client_v2-0.487.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-16 07:57:28.472737 stigg_api_client_v2-0.487.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-16 07:57:28.480737 stigg_api_client_v2-0.487.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-16 07:57:28.464737 stigg_api_client_v2-0.487.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-16 07:57:28.520738 stigg_api_client_v2-0.487.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-16 07:57:28.496737 stigg_api_client_v2-0.487.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-16 07:57:28.492737 stigg_api_client_v2-0.487.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-16 07:57:28.528738 stigg_api_client_v2-0.487.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-16 07:57:28.484737 stigg_api_client_v2-0.487.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-16 07:57:28.504737 stigg_api_client_v2-0.487.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-16 07:57:28.512738 stigg_api_client_v2-0.487.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-16 07:57:28.372735 stigg_api_client_v2-0.487.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-16 07:57:28.364735 stigg_api_client_v2-0.487.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-16 07:57:28.392735 stigg_api_client_v2-0.487.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   127035 2023-07-16 07:57:28.348734 stigg_api_client_v2-0.487.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-16 07:57:28.452736 stigg_api_client_v2-0.487.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-16 07:57:28.360734 stigg_api_client_v2-0.487.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-16 07:57:28.388735 stigg_api_client_v2-0.487.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-16 07:57:28.440736 stigg_api_client_v2-0.487.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-16 07:57:28.436736 stigg_api_client_v2-0.487.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-16 07:57:28.432736 stigg_api_client_v2-0.487.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-16 07:57:29.332755 stigg_api_client_v2-0.487.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-16 07:57:28.376735 stigg_api_client_v2-0.487.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-16 07:57:28.400735 stigg_api_client_v2-0.487.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-16 07:57:28.536738 stigg_api_client_v2-0.487.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.487.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-16 12:17:05.903545 stigg_api_client_v2-0.488.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-16 12:17:52.536578 stigg_api_client_v2-0.488.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-16 12:17:05.903545 stigg_api_client_v2-0.488.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-16 12:17:05.903545 stigg_api_client_v2-0.488.0/stigg/client.py
+-rw-r--r--   0        0        0    39986 2023-07-16 12:17:50.804542 stigg_api_client_v2-0.488.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-16 12:17:49.556516 stigg_api_client_v2-0.488.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-16 12:17:50.420534 stigg_api_client_v2-0.488.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    67443 2023-07-16 12:17:50.648538 stigg_api_client_v2-0.488.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-16 12:17:45.384427 stigg_api_client_v2-0.488.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-16 12:17:50.420534 stigg_api_client_v2-0.488.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-16 12:17:49.500515 stigg_api_client_v2-0.488.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-16 12:17:49.520515 stigg_api_client_v2-0.488.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67016 2023-07-16 12:17:45.600432 stigg_api_client_v2-0.488.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-16 12:17:49.544515 stigg_api_client_v2-0.488.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24352 2023-07-16 12:17:47.176466 stigg_api_client_v2-0.488.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-16 12:17:49.508515 stigg_api_client_v2-0.488.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-16 12:17:49.516515 stigg_api_client_v2-0.488.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-16 12:17:50.420534 stigg_api_client_v2-0.488.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    54916 2023-07-16 12:17:50.420534 stigg_api_client_v2-0.488.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-16 12:17:49.568516 stigg_api_client_v2-0.488.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-16 12:17:49.580516 stigg_api_client_v2-0.488.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-16 12:17:49.564516 stigg_api_client_v2-0.488.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-16 12:17:49.616517 stigg_api_client_v2-0.488.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-16 12:17:49.592517 stigg_api_client_v2-0.488.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-16 12:17:49.588516 stigg_api_client_v2-0.488.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-16 12:17:49.624517 stigg_api_client_v2-0.488.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-16 12:17:49.584516 stigg_api_client_v2-0.488.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-16 12:17:49.600517 stigg_api_client_v2-0.488.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-16 12:17:49.612517 stigg_api_client_v2-0.488.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-16 12:17:49.468514 stigg_api_client_v2-0.488.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-16 12:17:49.460514 stigg_api_client_v2-0.488.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-16 12:17:49.488514 stigg_api_client_v2-0.488.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   127063 2023-07-16 12:17:49.444513 stigg_api_client_v2-0.488.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-16 12:17:49.552516 stigg_api_client_v2-0.488.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-16 12:17:49.456514 stigg_api_client_v2-0.488.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-16 12:17:49.484514 stigg_api_client_v2-0.488.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-16 12:17:49.536515 stigg_api_client_v2-0.488.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-16 12:17:49.532515 stigg_api_client_v2-0.488.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-16 12:17:49.528515 stigg_api_client_v2-0.488.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-16 12:17:50.424534 stigg_api_client_v2-0.488.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-16 12:17:49.472514 stigg_api_client_v2-0.488.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-16 12:17:49.496514 stigg_api_client_v2-0.488.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-16 12:17:49.632517 stigg_api_client_v2-0.488.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.488.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.487.0/README.md` & `stigg_api_client_v2-0.488.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.487.0/stigg/client.py` & `stigg_api_client_v2-0.488.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.488.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.488.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.488.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.488.0/stigg/generated/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.488.0/stigg/generated/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.488.0/stigg/generated/cancel_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/client.py` & `stigg_api_client_v2-0.488.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.488.0/stigg/generated/update_subscription.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
 
 
-class CreateSubscription(BaseModel):
-    create_subscription: "CreateSubscriptionCreateSubscription" = Field(
-        alias="createSubscription"
+class UpdateSubscription(BaseModel):
+    update_subscription: "UpdateSubscriptionUpdateSubscription" = Field(
+        alias="updateSubscription"
     )
 
 
-class CreateSubscriptionCreateSubscription(SlimSubscriptionFragment):
+class UpdateSubscriptionUpdateSubscription(SlimSubscriptionFragment):
     pass
 
 
-CreateSubscription.update_forward_refs()
-CreateSubscriptionCreateSubscription.update_forward_refs()
+UpdateSubscription.update_forward_refs()
+UpdateSubscriptionUpdateSubscription.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.488.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -372,14 +372,15 @@
     IntegrationNotFound = "IntegrationNotFound"
     IntegrityViolation = "IntegrityViolation"
     InvalidAddressError = "InvalidAddressError"
     InvalidArgumentError = "InvalidArgumentError"
     InvalidCancellationDate = "InvalidCancellationDate"
     InvalidEntitlementResetPeriod = "InvalidEntitlementResetPeriod"
     InvalidMemberDelete = "InvalidMemberDelete"
+    InvalidMetadataError = "InvalidMetadataError"
     InvalidQuantity = "InvalidQuantity"
     InvalidSubscriptionStatus = "InvalidSubscriptionStatus"
     InvalidUpdatePriceUnitAmountError = "InvalidUpdatePriceUnitAmountError"
     MemberInvitationError = "MemberInvitationError"
     MemberNotFound = "MemberNotFound"
     MeterDoesNotBelongToTheEntitlementFeature = (
         "MeterDoesNotBelongToTheEntitlementFeature"
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.488.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.488.0/stigg/generated/estimate_subscription_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.488.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.488.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -55,36 +77,14 @@
 class PriceFragmentFeature(BaseModel):
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -124,25 +124,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -157,14 +146,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,34 +328,14 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -419,14 +399,21 @@
     id: str
     ref_id: str = Field(alias="refId")
     display_name: str = Field(alias="displayName")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -504,14 +491,27 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -1311,28 +1311,28 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1346,37 +1346,37 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerResourceFragment.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.488.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.488.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.488.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.488.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.488.0/stigg/generated/get_products.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.488.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.488.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -436,14 +436,15 @@
 
 class CustomerBillingInfo(BaseModel):
     billing_address: Optional["Address"] = Field(alias="billingAddress")
     currency: Optional[Currency] = Currency.USD
     customer_name: Optional[str] = Field(alias="customerName")
     invoice_custom_fields: Optional[Any] = Field(alias="invoiceCustomFields")
     language: Optional[str]
+    metadata: Optional[Any]
     payment_method_id: Optional[str] = Field(alias="paymentMethodId")
     shipping_address: Optional["Address"] = Field(alias="shippingAddress")
     tax_ids: Optional[List["TaxExempt"]] = Field(alias="taxIds")
     timezone: Optional[str]
 
 
 class CustomerFilter(BaseModel):
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.488.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.488.0/stigg/generated/provision_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.488.0/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.488.0/stigg/generated/report_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-16 07:57
+# Generated by ariadne-codegen on 2023-07-16 12:17
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.487.0/PKG-INFO` & `stigg_api_client_v2-0.488.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.487.0
+Version: 0.488.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

