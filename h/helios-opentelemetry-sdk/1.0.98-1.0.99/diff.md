# Comparing `tmp/helios-opentelemetry-sdk-1.0.98.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.98.tar", last modified: Mon Jul 10 16:06:51 2023, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.99.tar", last modified: Mon Jul 17 06:14:22 2023, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.98.tar` & `helios-opentelemetry-sdk-1.0.99.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/
--rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/base_data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/redis_data_obfuscator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/span_attribute_dropper/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/span_attribute_dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.943584 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/eventbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/confluent_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.947584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 16:06:51.000000 helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/hstest/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 16:06:51.951584 helios-opentelemetry-sdk-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-10 16:06:34.000000 helios-opentelemetry-sdk-1.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/base_data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/redis_data_obfuscator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/base/span_attribute_dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/span_attribute_dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.982102 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/eventbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/confluent_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.986102 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-17 06:14:22.000000 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-17 06:14:22.000000 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 06:14:22.000000 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 06:14:22.000000 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 06:14:22.000000 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 06:14:22.000000 helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/hstest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 06:14:22.990101 helios-opentelemetry-sdk-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-17 06:14:03.000000 helios-opentelemetry-sdk-1.0.99/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.98/LICENSE` & `helios-opentelemetry-sdk-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/PKG-INFO` & `helios-opentelemetry-sdk-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.98
+Version: 1.0.99
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.98/README.md` & `helios-opentelemetry-sdk-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/base_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/base_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/data_obfuscator/redis_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/data_obfuscator/redis_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/span_attribute_dropper/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/span_attribute_dropper/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.99/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/helios.py` & `helios-opentelemetry-sdk-1.0.99/helios/helios.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.99/helios/helios_test_trace.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aio_pika.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aio_pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/aws_lambda.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/base.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/base_http_instrumentor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/eventbridge.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/eventbridge.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/s3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/confluent_kafka.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/confluent_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/django.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
         self.tracer_provider = tracer_provider
         self.excluded_urls = kwargs.get('excluded_urls')
         self.custom_attributes_hook = kwargs.get('fastapi_custom_attributes_hook')
 
-        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.fastapi', '_get_route_details', HeliosAsgiMiddleware.get_span_details_wrapper)
+        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.fastapi', '_get_default_span_details', HeliosAsgiMiddleware.get_span_details_wrapper)
         wrapt.wrap_function_wrapper('fastapi', 'FastAPI.__init__', self.fastapi_instrument_and_init)
 
     def uninstrument(self):
         if self.get_instrumentor() is None:
             return
 
         for app in self.instrumented_apps:
@@ -44,15 +44,15 @@
             if instance not in self.instrumented_apps:
                 self.instrumented_apps.add(instance)
                 self.get_instrumentor().instrument_app(
                     instance,
                     tracer_provider=self.tracer_provider,
                     excluded_urls=self.excluded_urls
                 )
-                get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_route_details')
+                get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_default_span_details')
                 attributes_hook = self.custom_attributes_hook
                 if callable(attributes_hook):
                     @instance.middleware('http')
                     async def custom_span_middleware_hook(request, call_next):
                         try:
                             attributes = attributes_hook(request)
                             from helios import create_custom_span
```

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/grpc.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/grpc.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/helios_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/httpx.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/redis.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/redis.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/requests.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/starlette.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
 
         self.tracer_provider = tracer_provider
         self.excluded_urls = kwargs.get('excluded_urls')
 
-        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.starlette', '_get_route_details', HeliosAsgiMiddleware.get_span_details_wrapper)
+        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.starlette', '_get_default_span_details', HeliosAsgiMiddleware.get_span_details_wrapper)
         wrapt.wrap_function_wrapper('starlette.applications', 'Starlette.__init__', self.starlette_instrument_and_run)
 
     def uninstrument(self):
         if self.get_instrumentor() is None:
             return
 
         for app in self.instrumented_apps:
@@ -51,15 +51,15 @@
                 self.get_instrumentor().instrument_app(
                     instance,
                     # server_request_hook=self.server_request_hook,
                     # client_request_hook=self.client_request_hook,
                     # client_response_hook=self.client_response_hook,
                     tracer_provider=self.tracer_provider
                 )
-                get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_route_details')
+                get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_default_span_details')
                 instance.add_middleware(
                     HeliosAsgiMiddleware,
                     tracer=self.tracer_provider.get_tracer(self.MODULE_NAME),
                     excluded_urls=self.excluded_urls,
                     get_span_details=get_span_details
                 )
         except Exception as error:
```

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/instrumentation/urllib3.py` & `helios-opentelemetry-sdk-1.0.99/helios/instrumentation/urllib3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.99/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.99/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.99/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.99/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios/utils.py` & `helios-opentelemetry-sdk-1.0.99/helios/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.98
+Version: 1.0.99
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.99/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 autowrapt==1.0
 jsonpath-ng==1.5.3
-opentelemetry-api==1.18.0
-opentelemetry-exporter-otlp-proto-http==1.18.0
-opentelemetry-instrumentation-aio-pika==0.39b0
-opentelemetry-instrumentation-aiohttp-client==0.39b0
-opentelemetry-instrumentation-aiopg==0.39b0
-opentelemetry-instrumentation-asyncpg==0.39b0
-opentelemetry-instrumentation-aws-lambda==0.39b0
-opentelemetry-instrumentation-boto==0.39b0
-opentelemetry-instrumentation-botocore==0.39b0
-opentelemetry-instrumentation-celery==0.39b0
-opentelemetry-instrumentation-confluent-kafka==0.39b0
-opentelemetry-instrumentation-django==0.39b0
-opentelemetry-instrumentation-elasticsearch==0.39b0
-opentelemetry-instrumentation-fastapi==0.39b0
-opentelemetry-instrumentation-flask==0.39b0
-opentelemetry-instrumentation-grpc==0.39b0
-opentelemetry-instrumentation-httpx==0.39b0
-opentelemetry-instrumentation-logging==0.39b0
-opentelemetry-instrumentation-mysql==0.39b0
-opentelemetry-instrumentation-pika==0.39b0
-opentelemetry-instrumentation-psycopg2==0.39b0
-opentelemetry-instrumentation-pymemcache==0.39b0
-opentelemetry-instrumentation-pymongo==0.39b0
-opentelemetry-instrumentation-pymysql==0.39b0
-opentelemetry-instrumentation-redis==0.39b0
-opentelemetry-instrumentation-requests==0.39b0
-opentelemetry-instrumentation-sqlalchemy==0.39b0
-opentelemetry-instrumentation-sqlite3==0.39b0
-opentelemetry-instrumentation-starlette==0.39b0
-opentelemetry-instrumentation-tornado==0.39b0
-opentelemetry-instrumentation-urllib==0.39b0
-opentelemetry-instrumentation-urllib3==0.39b0
-opentelemetry-instrumentation-system-metrics==0.39b0
-opentelemetry-instrumentation==0.39b0
-opentelemetry-sdk==1.18.0
+opentelemetry-api==1.19.0
+opentelemetry-exporter-otlp-proto-http==1.19.0
+opentelemetry-instrumentation-aio-pika==0.40b0
+opentelemetry-instrumentation-aiohttp-client==0.40b0
+opentelemetry-instrumentation-aiopg==0.40b0
+opentelemetry-instrumentation-asyncpg==0.40b0
+opentelemetry-instrumentation-aws-lambda==0.40b0
+opentelemetry-instrumentation-boto==0.40b0
+opentelemetry-instrumentation-botocore==0.40b0
+opentelemetry-instrumentation-celery==0.40b0
+opentelemetry-instrumentation-confluent-kafka==0.40b0
+opentelemetry-instrumentation-django==0.40b0
+opentelemetry-instrumentation-elasticsearch==0.40b0
+opentelemetry-instrumentation-fastapi==0.40b0
+opentelemetry-instrumentation-flask==0.40b0
+opentelemetry-instrumentation-grpc==0.40b0
+opentelemetry-instrumentation-httpx==0.40b0
+opentelemetry-instrumentation-logging==0.40b0
+opentelemetry-instrumentation-mysql==0.40b0
+opentelemetry-instrumentation-pika==0.40b0
+opentelemetry-instrumentation-psycopg2==0.40b0
+opentelemetry-instrumentation-pymemcache==0.40b0
+opentelemetry-instrumentation-pymongo==0.40b0
+opentelemetry-instrumentation-pymysql==0.40b0
+opentelemetry-instrumentation-redis==0.40b0
+opentelemetry-instrumentation-requests==0.40b0
+opentelemetry-instrumentation-sqlalchemy==0.40b0
+opentelemetry-instrumentation-sqlite3==0.40b0
+opentelemetry-instrumentation-starlette==0.40b0
+opentelemetry-instrumentation-tornado==0.40b0
+opentelemetry-instrumentation-urllib==0.40b0
+opentelemetry-instrumentation-urllib3==0.40b0
+opentelemetry-instrumentation-system-metrics==0.40b0
+opentelemetry-instrumentation==0.40b0
+opentelemetry-sdk==1.19.0
 requests~=2.22
 protobuf!=3.20.0,!=3.20.1,<5.0,>=3.19
```

### Comparing `helios-opentelemetry-sdk-1.0.98/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.99/hstest/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.98/setup.py` & `helios-opentelemetry-sdk-1.0.99/setup.py`

 * *Files identical despite different names*

