# Comparing `tmp/pulumi_opsgenie-1.3.0a1689314769.tar.gz` & `tmp/pulumi_opsgenie-1.3.0a1689370468.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.3.0a1689314769.tar", last modified: Fri Jul 14 06:12:49 2023, max compression
+gzip compressed data, was "pulumi_opsgenie-1.3.0a1689370468.tar", last modified: Fri Jul 14 21:38:21 2023, max compression
```

## Comparing `pulumi_opsgenie-1.3.0a1689314769.tar` & `pulumi_opsgenie-1.3.0a1689370468.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:12:49.375823 pulumi_opsgenie-1.3.0a1689314769/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 06:12:49.375823 pulumi_opsgenie-1.3.0a1689314769/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:12:49.371823 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179600 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:12:49.375823 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   160301 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:12:49.375823 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:12:49.375823 pulumi_opsgenie-1.3.0a1689314769/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 06:12:49.000000 pulumi_opsgenie-1.3.0a1689314769/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:38:21.123930 pulumi_opsgenie-1.3.0a1689370468/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 21:38:21.123930 pulumi_opsgenie-1.3.0a1689370468/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:38:21.123930 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179652 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58074 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33658 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:38:21.123930 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160353 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:38:21.123930 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 21:38:21.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-14 21:38:21.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:38:21.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:38:21.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 21:38:21.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 21:38:21.000000 pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:38:21.123930 pulumi_opsgenie-1.3.0a1689370468/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 21:38:20.000000 pulumi_opsgenie-1.3.0a1689370468/setup.py
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/PKG-INFO` & `pulumi_opsgenie-1.3.0a1689370468/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.3.0a1689314769
+Version: 1.3.0a1689370468
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/README.md` & `pulumi_opsgenie-1.3.0a1689370468/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     def __init__(__self__, *,
                  id: pulumi.Input[str],
                  type: pulumi.Input[str],
                  name: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] id: ID of the responder
-        :param pulumi.Input[str] type: Type of responder. Acceptable values are: `user` or `team`
+        :param pulumi.Input[str] type: Type of responder. Acceptable values are: `user`, `team`, `escalation` or `schedule`
         :param pulumi.Input[str] name: Name of the responder
         :param pulumi.Input[str] username: Username of the responder
         """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "type", type)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -256,15 +256,15 @@
     def id(self, value: pulumi.Input[str]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        Type of responder. Acceptable values are: `user` or `team`
+        Type of responder. Acceptable values are: `user`, `team`, `escalation` or `schedule`
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/alert_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         :param pulumi.Input[bool] ignore_original_actions: If set to `true`, policy will ignore the original actions of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_details: If set to `true`, policy will ignore the original details of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_responders: If set to `true`, policy will ignore the original responders of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_tags: If set to `true`, policy will ignore the original tags of the alert. Default: `false`
         :param pulumi.Input[str] name: Name of the alert policy
         :param pulumi.Input[str] policy_description: Description of the policy. This can be max 512 characters.
         :param pulumi.Input[str] priority: Priority of the alert. Should be one of `P1`, `P2`, `P3`, `P4`, or `P5`
-        :param pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        :param pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         :param pulumi.Input[str] source: Source field of the alert. You can use `{{source}}` to refer to the original source. Default: `{{source}}`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags to add to the alerts original tags value as a list of strings. If `ignore_original_responders` field is set to `true`, this will replace the original responders.
         :param pulumi.Input[str] team_id: Id of team that this policy belongs to.
         :param pulumi.Input[Sequence[pulumi.Input['AlertPolicyTimeRestrictionArgs']]] time_restrictions: Time restrictions specified in this field must be met for this policy to work. This is a block, structure is documented below.
         """
         pulumi.set(__self__, "message", message)
         if actions is not None:
@@ -279,15 +279,15 @@
     def priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
     def responders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]]]:
         """
-        Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         """
         return pulumi.get(self, "responders")
 
     @responders.setter
     def responders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]]]):
         pulumi.set(self, "responders", value)
 
@@ -376,15 +376,15 @@
         :param pulumi.Input[bool] ignore_original_details: If set to `true`, policy will ignore the original details of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_responders: If set to `true`, policy will ignore the original responders of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_tags: If set to `true`, policy will ignore the original tags of the alert. Default: `false`
         :param pulumi.Input[str] message: Message of the alerts
         :param pulumi.Input[str] name: Name of the alert policy
         :param pulumi.Input[str] policy_description: Description of the policy. This can be max 512 characters.
         :param pulumi.Input[str] priority: Priority of the alert. Should be one of `P1`, `P2`, `P3`, `P4`, or `P5`
-        :param pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        :param pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         :param pulumi.Input[str] source: Source field of the alert. You can use `{{source}}` to refer to the original source. Default: `{{source}}`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags to add to the alerts original tags value as a list of strings. If `ignore_original_responders` field is set to `true`, this will replace the original responders.
         :param pulumi.Input[str] team_id: Id of team that this policy belongs to.
         :param pulumi.Input[Sequence[pulumi.Input['AlertPolicyTimeRestrictionArgs']]] time_restrictions: Time restrictions specified in this field must be met for this policy to work. This is a block, structure is documented below.
         """
         if actions is not None:
             pulumi.set(__self__, "actions", actions)
@@ -607,15 +607,15 @@
     def priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
     def responders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]]]:
         """
-        Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         """
         return pulumi.get(self, "responders")
 
     @responders.setter
     def responders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['AlertPolicyResponderArgs']]]]):
         pulumi.set(self, "responders", value)
 
@@ -759,15 +759,15 @@
         :param pulumi.Input[bool] ignore_original_details: If set to `true`, policy will ignore the original details of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_responders: If set to `true`, policy will ignore the original responders of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_tags: If set to `true`, policy will ignore the original tags of the alert. Default: `false`
         :param pulumi.Input[str] message: Message of the alerts
         :param pulumi.Input[str] name: Name of the alert policy
         :param pulumi.Input[str] policy_description: Description of the policy. This can be max 512 characters.
         :param pulumi.Input[str] priority: Priority of the alert. Should be one of `P1`, `P2`, `P3`, `P4`, or `P5`
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyResponderArgs']]]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyResponderArgs']]]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         :param pulumi.Input[str] source: Source field of the alert. You can use `{{source}}` to refer to the original source. Default: `{{source}}`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags to add to the alerts original tags value as a list of strings. If `ignore_original_responders` field is set to `true`, this will replace the original responders.
         :param pulumi.Input[str] team_id: Id of team that this policy belongs to.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyTimeRestrictionArgs']]]] time_restrictions: Time restrictions specified in this field must be met for this policy to work. This is a block, structure is documented below.
         """
         ...
     @overload
@@ -941,15 +941,15 @@
         :param pulumi.Input[bool] ignore_original_details: If set to `true`, policy will ignore the original details of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_responders: If set to `true`, policy will ignore the original responders of the alert. Default: `false`
         :param pulumi.Input[bool] ignore_original_tags: If set to `true`, policy will ignore the original tags of the alert. Default: `false`
         :param pulumi.Input[str] message: Message of the alerts
         :param pulumi.Input[str] name: Name of the alert policy
         :param pulumi.Input[str] policy_description: Description of the policy. This can be max 512 characters.
         :param pulumi.Input[str] priority: Priority of the alert. Should be one of `P1`, `P2`, `P3`, `P4`, or `P5`
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyResponderArgs']]]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyResponderArgs']]]] responders: Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         :param pulumi.Input[str] source: Source field of the alert. You can use `{{source}}` to refer to the original source. Default: `{{source}}`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags to add to the alerts original tags value as a list of strings. If `ignore_original_responders` field is set to `true`, this will replace the original responders.
         :param pulumi.Input[str] team_id: Id of team that this policy belongs to.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyTimeRestrictionArgs']]]] time_restrictions: Time restrictions specified in this field must be met for this policy to work. This is a block, structure is documented below.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -1097,15 +1097,15 @@
         """
         return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter
     def responders(self) -> pulumi.Output[Optional[Sequence['outputs.AlertPolicyResponder']]]:
         """
-        Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`. This is a block, structure is documented below.
+        Responders to add to the alerts original responders value as a list of teams, users or the reserved word none or all. If `ignore_original_responders` field is set to `true`, this will replace the original responders. The possible values for responders are: `user`, `team`, `escalation`, `schedule`. This is a block, structure is documented below.
         """
         return pulumi.get(self, "responders")
 
     @property
     @pulumi.getter
     def source(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/api_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  webhook_url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ApiIntegration resource.
         :param pulumi.Input[bool] allow_write_access: This parameter is for configuring the write access of integration. If write access is restricted, the integration will not be authorized to write within any domain. Default: `true`.
         :param pulumi.Input[bool] enabled: This parameter is for specifying whether the integration will be enabled or not. Default: `true`
         :param pulumi.Input[bool] ignore_responders_from_payload: If enabled, the integration will ignore recipients sent in request payloads. Default: `false`.
         :param pulumi.Input[str] name: Name of the integration. Name must be unique for each integration.
-        :param pulumi.Input[str] owner_team_id: Owner team id of the integration.
+        :param pulumi.Input[str] owner_team_id: Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         :param pulumi.Input[Sequence[pulumi.Input['ApiIntegrationResponderArgs']]] responders: User, schedule, teams or escalation names to calculate which users will receive the notifications of the alert.
         :param pulumi.Input[bool] suppress_notifications: If enabled, notifications that come from alerts will be suppressed. Default: `false`.
         :param pulumi.Input[str] type: Type of the integration (API, Marid, Prometheus, etc). The full list of options can be found [here](https://docs.opsgenie.com/docs/integration-types-to-use-with-api).
         :param pulumi.Input[str] webhook_url: It is required if type is `Webhook`. This is the url Opsgenie will be sending request to.
         """
         if allow_write_access is not None:
             pulumi.set(__self__, "allow_write_access", allow_write_access)
@@ -116,15 +116,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerTeamId")
     def owner_team_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Owner team id of the integration.
+        Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         """
         return pulumi.get(self, "owner_team_id")
 
     @owner_team_id.setter
     def owner_team_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "owner_team_id", value)
 
@@ -194,15 +194,15 @@
         """
         Input properties used for looking up and filtering ApiIntegration resources.
         :param pulumi.Input[bool] allow_write_access: This parameter is for configuring the write access of integration. If write access is restricted, the integration will not be authorized to write within any domain. Default: `true`.
         :param pulumi.Input[str] api_key: (Computed) API key of the created integration
         :param pulumi.Input[bool] enabled: This parameter is for specifying whether the integration will be enabled or not. Default: `true`
         :param pulumi.Input[bool] ignore_responders_from_payload: If enabled, the integration will ignore recipients sent in request payloads. Default: `false`.
         :param pulumi.Input[str] name: Name of the integration. Name must be unique for each integration.
-        :param pulumi.Input[str] owner_team_id: Owner team id of the integration.
+        :param pulumi.Input[str] owner_team_id: Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         :param pulumi.Input[Sequence[pulumi.Input['ApiIntegrationResponderArgs']]] responders: User, schedule, teams or escalation names to calculate which users will receive the notifications of the alert.
         :param pulumi.Input[bool] suppress_notifications: If enabled, notifications that come from alerts will be suppressed. Default: `false`.
         :param pulumi.Input[str] type: Type of the integration (API, Marid, Prometheus, etc). The full list of options can be found [here](https://docs.opsgenie.com/docs/integration-types-to-use-with-api).
         :param pulumi.Input[str] webhook_url: It is required if type is `Webhook`. This is the url Opsgenie will be sending request to.
         """
         if allow_write_access is not None:
             pulumi.set(__self__, "allow_write_access", allow_write_access)
@@ -296,15 +296,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="ownerTeamId")
     def owner_team_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Owner team id of the integration.
+        Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         """
         return pulumi.get(self, "owner_team_id")
 
     @owner_team_id.setter
     def owner_team_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "owner_team_id", value)
 
@@ -430,15 +430,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_write_access: This parameter is for configuring the write access of integration. If write access is restricted, the integration will not be authorized to write within any domain. Default: `true`.
         :param pulumi.Input[bool] enabled: This parameter is for specifying whether the integration will be enabled or not. Default: `true`
         :param pulumi.Input[bool] ignore_responders_from_payload: If enabled, the integration will ignore recipients sent in request payloads. Default: `false`.
         :param pulumi.Input[str] name: Name of the integration. Name must be unique for each integration.
-        :param pulumi.Input[str] owner_team_id: Owner team id of the integration.
+        :param pulumi.Input[str] owner_team_id: Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ApiIntegrationResponderArgs']]]] responders: User, schedule, teams or escalation names to calculate which users will receive the notifications of the alert.
         :param pulumi.Input[bool] suppress_notifications: If enabled, notifications that come from alerts will be suppressed. Default: `false`.
         :param pulumi.Input[str] type: Type of the integration (API, Marid, Prometheus, etc). The full list of options can be found [here](https://docs.opsgenie.com/docs/integration-types-to-use-with-api).
         :param pulumi.Input[str] webhook_url: It is required if type is `Webhook`. This is the url Opsgenie will be sending request to.
         """
         ...
     @overload
@@ -577,15 +577,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_write_access: This parameter is for configuring the write access of integration. If write access is restricted, the integration will not be authorized to write within any domain. Default: `true`.
         :param pulumi.Input[str] api_key: (Computed) API key of the created integration
         :param pulumi.Input[bool] enabled: This parameter is for specifying whether the integration will be enabled or not. Default: `true`
         :param pulumi.Input[bool] ignore_responders_from_payload: If enabled, the integration will ignore recipients sent in request payloads. Default: `false`.
         :param pulumi.Input[str] name: Name of the integration. Name must be unique for each integration.
-        :param pulumi.Input[str] owner_team_id: Owner team id of the integration.
+        :param pulumi.Input[str] owner_team_id: Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ApiIntegrationResponderArgs']]]] responders: User, schedule, teams or escalation names to calculate which users will receive the notifications of the alert.
         :param pulumi.Input[bool] suppress_notifications: If enabled, notifications that come from alerts will be suppressed. Default: `false`.
         :param pulumi.Input[str] type: Type of the integration (API, Marid, Prometheus, etc). The full list of options can be found [here](https://docs.opsgenie.com/docs/integration-types-to-use-with-api).
         :param pulumi.Input[str] webhook_url: It is required if type is `Webhook`. This is the url Opsgenie will be sending request to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -649,15 +649,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="ownerTeamId")
     def owner_team_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Owner team id of the integration.
+        Owner team id of the integration. If changed, this will recreate a new API integration, which will probably have a different API key.
         """
         return pulumi.get(self, "owner_team_id")
 
     @property
     @pulumi.getter
     def responders(self) -> pulumi.Output[Optional[Sequence['outputs.ApiIntegrationResponder']]]:
         """
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/email_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/incident_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/integration_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     def __init__(__self__, *,
                  id: str,
                  type: str,
                  name: Optional[str] = None,
                  username: Optional[str] = None):
         """
         :param str id: ID of the responder
-        :param str type: Type of responder. Acceptable values are: `user` or `team`
+        :param str type: Type of responder. Acceptable values are: `user`, `team`, `escalation` or `schedule`
         :param str name: Name of the responder
         :param str username: Username of the responder
         """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "type", type)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -240,15 +240,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Type of responder. Acceptable values are: `user` or `team`
+        Type of responder. Acceptable values are: `user`, `team`, `escalation` or `schedule`
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/schedule_rotation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opsgenie
-Version: 1.3.0a1689314769
+Version: 1.3.0a1689370468
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_opsgenie-1.3.0a1689314769/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.3.0a1689370468/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1689314769/setup.py` & `pulumi_opsgenie-1.3.0a1689370468/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1689314769"
-PLUGIN_VERSION = "1.3.0-alpha.1689314769+b3cb8b6a"
+VERSION = "1.3.0a1689370468"
+PLUGIN_VERSION = "1.3.0-alpha.1689370468+35c050a8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opsgenie', PLUGIN_VERSION])
         except OSError as error:
```

