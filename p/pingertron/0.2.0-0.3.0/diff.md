# Comparing `tmp/pingertron-0.2.0.tar.gz` & `tmp/pingertron-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingertron-0.2.0.tar", max compression
+gzip compressed data, was "pingertron-0.3.0.tar", max compression
```

## Comparing `pingertron-0.2.0.tar` & `pingertron-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-22 15:17:56.890459 pingertron-0.2.0/LICENSE
--rw-r--r--   0        0        0     1597 2023-05-22 18:14:44.481413 pingertron-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-19 20:54:31.460873 pingertron-0.2.0/pingertron/__init__.py
--rw-r--r--   0        0        0     5295 2023-05-24 16:09:11.792797 pingertron-0.2.0/pingertron/main.py
--rw-r--r--   0        0        0     1594 2023-05-22 14:45:31.372782 pingertron-0.2.0/pingertron/metrics.py
--rw-r--r--   0        0        0      531 2023-05-22 15:52:21.557725 pingertron-0.2.0/pingertron/probes_config.py
--rw-r--r--   0        0        0      884 2023-05-24 17:47:03.276720 pingertron-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 pingertron-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-24 08:50:30.300557 pingertron-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1597 2023-05-26 11:06:50.058224 pingertron-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 08:50:30.301382 pingertron-0.3.0/pingertron/__init__.py
+-rw-r--r--   0        0        0     3016 2023-07-17 13:53:53.255590 pingertron-0.3.0/pingertron/main.py
+-rw-r--r--   0        0        0     1594 2023-05-24 08:50:30.301650 pingertron-0.3.0/pingertron/metrics.py
+-rw-r--r--   0        0        0     3181 2023-07-17 13:53:53.256056 pingertron-0.3.0/pingertron/probes.py
+-rw-r--r--   0        0        0      829 2023-07-17 13:53:53.256601 pingertron-0.3.0/pingertron/probes_config.py
+-rw-r--r--   0        0        0     1016 2023-07-17 15:20:45.542811 pingertron-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 pingertron-0.3.0/PKG-INFO
```

### Comparing `pingertron-0.2.0/LICENSE` & `pingertron-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pingertron-0.2.0/README.md` & `pingertron-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pingertron-0.2.0/pingertron/metrics.py` & `pingertron-0.3.0/pingertron/metrics.py`

 * *Files identical despite different names*

### Comparing `pingertron-0.2.0/pingertron/probes_config.py` & `pingertron-0.3.0/pingertron/probes_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pydantic
 
 
 class Protocol(enum.StrEnum):
     http = "http"
     icmp = "icmp"
+    failing = "failing"
 
 
 class HTTPProbe(pydantic.BaseModel):
     protocol: Protocol = Protocol.http
     description: str | None
     url: str
     method: str = "GET"
@@ -18,13 +19,25 @@
 
 class ICMPProbe(pydantic.BaseModel):
     protocol: Protocol = Protocol.icmp
     description: str | None
     hostname: str
 
 
-Probe = HTTPProbe | ICMPProbe
+class FailureMode(enum.StrEnum):
+    exception = "exception"
+    timeout = "timeout"
+
+
+class FailingProbe(pydantic.BaseModel):
+    protocol: Protocol = Protocol.failing
+    description: str | None
+    failure_rate: float = 0.8
+    failure_mode: FailureMode
+
+
+Probe = HTTPProbe | ICMPProbe | FailingProbe
 
 
 class ProbesConfig(pydantic.BaseModel):
     interval_seconds: float = 60
     probes: list[Probe]
```

### Comparing `pingertron-0.2.0/PKG-INFO` & `pingertron-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pingertron
-Version: 0.2.0
+Version: 0.3.0
 Summary: Ping Hosts and URLs and keep stats on successes and failures
+Home-page: https://github.com/micktwomey/pingertron
 License: MIT
 Author: Michael Twomey
 Author-email: mick@twomeylee.name
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +15,15 @@
 Requires-Dist: prometheus-client (>=0.16.0,<0.17.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pydantic-yaml (>=1.0.0a2,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/micktwomey/pingertron
 Description-Content-Type: text/markdown
 
 # Ping Hosts and URLs and keep stats on successes and failures
 
 Run this as a daemon on your box and check in to see if there are problems.
 
 Intended to be a slightly different approach to blackbox_exporter.
```

