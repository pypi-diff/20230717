# Comparing `tmp/landingzone_organization-0.6.1.tar.gz` & `tmp/landingzone_organization-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingzone_organization-0.6.1.tar", max compression
+gzip compressed data, was "landingzone_organization-0.6.2.tar", max compression
```

## Comparing `landingzone_organization-0.6.1.tar` & `landingzone_organization-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      981 2023-07-16 14:31:58.411204 landingzone_organization-0.6.1/README.md
--rw-r--r--   0        0        0      636 2023-07-16 14:31:59.271248 landingzone_organization-0.6.1/landingzone_organization/__init__.py
--rw-r--r--   0        0        0      525 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/account.py
--rw-r--r--   0        0        0       75 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/adapters/__init__.py
--rw-r--r--   0        0        0     3248 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/adapters/aws_organization.py
--rw-r--r--   0        0        0      509 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/account.py
--rw-r--r--   0        0        0      558 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/organization.py
--rw-r--r--   0        0        0     2096 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/profiles.py
--rw-r--r--   0        0        0      707 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/commands/workload.py
--rw-r--r--   0        0        0     1517 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/context.py
--rw-r--r--   0        0        0      744 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/cli/handler.py
--rw-r--r--   0        0        0      955 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/filtering.py
--rw-r--r--   0        0        0     1035 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/group.py
--rw-r--r--   0        0        0      929 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/groups.py
--rw-r--r--   0        0        0     3220 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/organization.py
--rw-r--r--   0        0        0      938 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/organization_unit.py
--rw-r--r--   0        0        0      917 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/profile.py
--rw-r--r--   0        0        0     1164 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/profiles.py
--rw-r--r--   0        0        0      906 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/workload.py
--rw-r--r--   0        0        0     1559 2023-07-16 14:31:58.415204 landingzone_organization-0.6.1/landingzone_organization/workloads.py
--rw-r--r--   0        0        0     1386 2023-07-16 14:31:59.271248 landingzone_organization-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      981 2023-07-17 09:06:15.822490 landingzone_organization-0.6.2/README.md
+-rw-r--r--   0        0        0      777 2023-07-17 09:06:16.734505 landingzone_organization-0.6.2/landingzone_organization/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/account.py
+-rw-r--r--   0        0        0       75 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/adapters/__init__.py
+-rw-r--r--   0        0        0     3248 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/adapters/aws_organization.py
+-rw-r--r--   0        0        0      509 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/commands/account.py
+-rw-r--r--   0        0        0      558 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/commands/organization.py
+-rw-r--r--   0        0        0     2096 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/commands/profiles.py
+-rw-r--r--   0        0        0      707 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/commands/workload.py
+-rw-r--r--   0        0        0     1517 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/context.py
+-rw-r--r--   0        0        0      744 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/cli/handler.py
+-rw-r--r--   0        0        0      955 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/filtering.py
+-rw-r--r--   0        0        0     1035 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/group.py
+-rw-r--r--   0        0        0      929 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/groups.py
+-rw-r--r--   0        0        0     3220 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/organization.py
+-rw-r--r--   0        0        0      938 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/organization_unit.py
+-rw-r--r--   0        0        0      917 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/profile.py
+-rw-r--r--   0        0        0     1164 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/profiles.py
+-rw-r--r--   0        0        0      906 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/workload.py
+-rw-r--r--   0        0        0     1559 2023-07-17 09:06:15.826490 landingzone_organization-0.6.2/landingzone_organization/workloads.py
+-rw-r--r--   0        0        0     1386 2023-07-17 09:06:16.734505 landingzone_organization-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.6.2/PKG-INFO
```

### Comparing `landingzone_organization-0.6.1/README.md` & `landingzone_organization-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/__init__.py` & `landingzone_organization-0.6.2/landingzone_organization/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from landingzone_organization.adapters.aws_organization import AWSOrganization
 from landingzone_organization.organization import Organization
 from landingzone_organization.organization_unit import OrganizationUnit
+from landingzone_organization.workloads import Workloads
+from landingzone_organization.workload import Workload
 from landingzone_organization.account import Account
 from landingzone_organization.groups import Groups
 from landingzone_organization.group import Group
 from landingzone_organization.profile import Profile
 from landingzone_organization.profiles import Profiles
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 __all__ = [
     AWSOrganization,
     Organization,
     OrganizationUnit,
+    Workloads,
+    Workload,
     Account,
     Groups,
     Group,
     Profile,
     Profiles,
 ]
```

### Comparing `landingzone_organization-0.6.1/landingzone_organization/account.py` & `landingzone_organization-0.6.2/landingzone_organization/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
     @property
     def environment(self) -> Optional[str]:
         return resolve_account_environment(self.name)
 
     @property
     def weight(self) -> int:
-        return resolve_account_weight(self.name)
+        return resolve_account_weight(self.environment)
```

### Comparing `landingzone_organization-0.6.1/landingzone_organization/adapters/aws_organization.py` & `landingzone_organization-0.6.2/landingzone_organization/adapters/aws_organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/cli/commands/account.py` & `landingzone_organization-0.6.2/landingzone_organization/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/cli/commands/organization.py` & `landingzone_organization-0.6.2/landingzone_organization/cli/commands/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/cli/commands/profiles.py` & `landingzone_organization-0.6.2/landingzone_organization/cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/cli/commands/workload.py` & `landingzone_organization-0.6.2/landingzone_organization/cli/commands/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/cli/context.py` & `landingzone_organization-0.6.2/landingzone_organization/cli/context.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/cli/handler.py` & `landingzone_organization-0.6.2/landingzone_organization/cli/handler.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/filtering.py` & `landingzone_organization-0.6.2/landingzone_organization/filtering.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/group.py` & `landingzone_organization-0.6.2/landingzone_organization/group.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/groups.py` & `landingzone_organization-0.6.2/landingzone_organization/groups.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/organization.py` & `landingzone_organization-0.6.2/landingzone_organization/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/organization_unit.py` & `landingzone_organization-0.6.2/landingzone_organization/organization_unit.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/profile.py` & `landingzone_organization-0.6.2/landingzone_organization/profile.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/profiles.py` & `landingzone_organization-0.6.2/landingzone_organization/profiles.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/workload.py` & `landingzone_organization-0.6.2/landingzone_organization/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/landingzone_organization/workloads.py` & `landingzone_organization-0.6.2/landingzone_organization/workloads.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.6.1/pyproject.toml` & `landingzone_organization-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "landingzone-organization"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 readme = "README.md"
 homepage = "https://binxio.github.io/landingzone-organization/"
 documentation = "https://binxio.github.io/landingzone-organization/3-user-documentation/"
 repository = "https://github.com/binxio/landingzone-organization"
 packages = [{include = "landingzone_organization"}]
```

### Comparing `landingzone_organization-0.6.1/PKG-INFO` & `landingzone_organization-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingzone-organization
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Home-page: https://binxio.github.io/landingzone-organization/
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

