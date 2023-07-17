# Comparing `tmp/atro_pylog-0.2.1.tar.gz` & `tmp/atro_pylog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_pylog-0.2.1.tar", max compression
+gzip compressed data, was "atro_pylog-0.3.0.tar", max compression
```

## Comparing `atro_pylog-0.2.1.tar` & `atro_pylog-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1717 2023-07-11 20:05:26.775535 atro_pylog-0.2.1/atro_pylog/__init__.py
--rw-r--r--   0        0        0     1050 2023-07-11 19:45:01.356569 atro_pylog-0.2.1/atro_pylog/level.py
--rw-r--r--   0        0        0      363 2023-07-11 19:45:01.356569 atro_pylog-0.2.1/atro_pylog/logger_type.py
--rw-r--r--   0        0        0     1096 2023-07-11 19:59:20.704545 atro_pylog-0.2.1/atro_pylog/opentelemetry_setup.py
--rw-r--r--   0        0        0      127 2023-07-11 19:45:01.356569 atro_pylog-0.2.1/atro_pylog/rich_setup.py
--rw-r--r--   0        0        0      865 2023-07-16 20:46:20.949079 atro_pylog-0.2.1/atro_pylog/settings.py
--rw-r--r--   0        0        0      636 2023-07-16 20:46:28.832573 atro_pylog-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 atro_pylog-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1604 2023-07-17 21:36:09.801670 atro_pylog-0.3.0/atro_pylog/__init__.py
+-rw-r--r--   0        0        0     1050 2023-07-11 19:45:01.356569 atro_pylog-0.3.0/atro_pylog/level.py
+-rw-r--r--   0        0        0      363 2023-07-11 19:45:01.356569 atro_pylog-0.3.0/atro_pylog/logger_type.py
+-rw-r--r--   0        0        0     1007 2023-07-17 21:35:20.624005 atro_pylog-0.3.0/atro_pylog/opentelemetry_setup.py
+-rw-r--r--   0        0        0      127 2023-07-11 19:45:01.356569 atro_pylog-0.3.0/atro_pylog/rich_setup.py
+-rw-r--r--   0        0        0      606 2023-07-17 21:36:10.838358 atro_pylog-0.3.0/atro_pylog/settings.py
+-rw-r--r--   0        0        0      636 2023-07-17 21:42:27.142670 atro_pylog-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 atro_pylog-0.3.0/PKG-INFO
```

### Comparing `atro_pylog-0.2.1/atro_pylog/__init__.py` & `atro_pylog-0.3.0/atro_pylog/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 sys.path.append(Path(__file__).resolve().parent.parent.as_posix())
 
 from atro_pylog.level import level_to_str, str_to_level  # noqa E402
 from atro_pylog.logger_type import LoggerType  # noqa E402
 from atro_pylog.logger_type import str_to_logger_type  # noqa E402
 from atro_pylog.opentelemetry_setup import open_telemetry_logger_setup  # noqa E402
 from atro_pylog.rich_setup import rich_handler  # noqa E402
-from atro_pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings  # noqa E402
+from atro_pylog.settings import LoggerSettings  # noqa E402
 
 logger = logging.getLogger(__name__)
 
 
 def exception_handler(exc_type, exc_value, exc_traceback):
     logger.critical(stackprinter.format(exc_value))
 
 
-def set_logger(base_settings: BaseLoggerSettings = BaseLoggerSettings(), open_telemetry_settings: OpenTelemetryLoggerSettings = OpenTelemetryLoggerSettings()):
+def set_logger(settings: LoggerSettings = LoggerSettings()):
     sys.excepthook = exception_handler
     handlers = []
 
-    types = [str_to_logger_type(type.strip()) for type in base_settings.type.split(";")]
+    types = [str_to_logger_type(type.strip()) for type in settings.type.split(";")]
     for tp in types:
         match tp:
             case LoggerType.RICH:
-                handlers.append(rich_handler(str_to_level(base_settings.level)))
+                handlers.append(rich_handler(str_to_level(settings.level)))
             case LoggerType.OPENTELEMETRY:
-                handlers.append(open_telemetry_logger_setup(str_to_level(base_settings.level), open_telemetry_settings))
+                handlers.append(open_telemetry_logger_setup(str_to_level(settings.level), settings.otel_service_name, settings.otel_instance_id, settings.otel_endpoint))
             case _:
                 raise Exception(f"Unknown logger type: {tp}")
-    logger = logging.getLogger(base_settings.name)
+    logger = logging.getLogger(settings.name)
     if logger.hasHandlers():
         logger.handlers.clear()
 
-    logging.basicConfig(level=level_to_str(base_settings.level), format=base_settings.msg_format, datefmt=base_settings.date_format, handlers=handlers)
+    logging.basicConfig(level=level_to_str(settings.level), format=settings.msg_format, datefmt=settings.date_format, handlers=handlers)
 
     return logger
```

### Comparing `atro_pylog-0.2.1/atro_pylog/level.py` & `atro_pylog-0.3.0/atro_pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro_pylog-0.2.1/atro_pylog/opentelemetry_setup.py` & `atro_pylog-0.3.0/atro_pylog/opentelemetry_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 
-from atro_pylog.settings import OpenTelemetryLoggerSettings
 
 
-def open_telemetry_logger_setup(level: int, settings: OpenTelemetryLoggerSettings):
+def open_telemetry_logger_setup(level: int, service_name, instance_id, endpoint):
     trace.set_tracer_provider(TracerProvider())
     logger_provider = LoggerProvider(  # type: ignore
         resource=Resource.create(
             {
-                "service.name": settings.service_name,
-                "service.instance.id": settings.instance_id,
+                "service.name": service_name,
+                "service.instance.id": instance_id,
             },
         ),
     )
     set_logger_provider(logger_provider)
-    exporter = OTLPLogExporter(endpoint=settings.endpoint)
+    exporter = OTLPLogExporter(endpoint=endpoint)
     logger_provider.add_log_record_processor(BatchLogRecordProcessor(exporter))
     return LoggingHandler(level=level, logger_provider=logger_provider)
```

### Comparing `atro_pylog-0.2.1/pyproject.toml` & `atro_pylog-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "atro-pylog"
-version = "0.2.1"
+version = "0.3.0"
 description = "A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging)."
 authors = ["Atropos <pypi.rising@atro.xyz>"]
 packages = [{ include = "atro_pylog" }]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 rich = "*"
```

### Comparing `atro_pylog-0.2.1/PKG-INFO` & `atro_pylog-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.2.1
+Version: 0.3.0
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

