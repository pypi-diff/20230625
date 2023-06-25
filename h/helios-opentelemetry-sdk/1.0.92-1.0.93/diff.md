# Comparing `tmp/helios-opentelemetry-sdk-1.0.92.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.92.tar", last modified: Mon Jun 12 15:36:23 2023, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.93.tar", last modified: Sun Jun 25 09:18:47 2023, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.92.tar` & `helios-opentelemetry-sdk-1.0.93.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.067707 helios-opentelemetry-sdk-1.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-12 15:36:23.067707 helios-opentelemetry-sdk-1.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/base/
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/base_data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/redis_data_obfuscator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/base/span_attribute_dropper/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/span_attribute_dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.059707 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/confluent_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-12 15:36:22.000000 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-12 15:36:23.000000 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:36:22.000000 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 15:36:22.000000 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-12 15:36:22.000000 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 15:36:22.000000 helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:23.063707 helios-opentelemetry-sdk-1.0.92/hstest/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-12 15:36:23.067707 helios-opentelemetry-sdk-1.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-12 15:36:04.000000 helios-opentelemetry-sdk-1.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/base_data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/redis_data_obfuscator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.382330 helios-opentelemetry-sdk-1.0.93/helios/base/span_attribute_dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/span_attribute_dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.386330 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.386330 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.386330 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/confluent_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 09:18:47.000000 helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/hstest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-25 09:18:47.390331 helios-opentelemetry-sdk-1.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-25 09:18:28.000000 helios-opentelemetry-sdk-1.0.93/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.92/LICENSE` & `helios-opentelemetry-sdk-1.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/PKG-INFO` & `helios-opentelemetry-sdk-1.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.92
+Version: 1.0.93
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.92/README.md` & `helios-opentelemetry-sdk-1.0.93/README.md`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/base_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/base_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/data_obfuscator/redis_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/data_obfuscator/redis_data_obfuscator.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/span_attribute_dropper/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/span_attribute_dropper/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.93/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/helios.py` & `helios-opentelemetry-sdk-1.0.93/helios/helios.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.93/helios/helios_test_trace.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aio_pika.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aio_pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/aws_lambda.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/aws_lambda.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 def extract_lambda_module_and_function():
     lambda_handler = os.environ.get('ORIG_HANDLER', os.environ.get('_HANDLER'))
     if not lambda_handler:
         _LOG.info('Unable to extract lambda handler details, instrumentation is skipped')
         return None, None
 
     wrapped_module_name, wrapped_function_name = lambda_handler.rsplit('.', 1)
+    wrapped_module_name = wrapped_module_name.replace('/', '.')
     return wrapped_module_name, wrapped_function_name
 
 
 def _flush_timeout():
     flush_timeout_env = os.environ.get(
         'OTEL_INSTRUMENTATION_AWS_LAMBDA_FLUSH_TIMEOUT', None
     )
```

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/base_http_instrumentor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/s3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/confluent_kafka.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/confluent_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/django.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/fastapi.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/grpc.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/grpc.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/helios_asgi_middleware.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/httpx.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pika.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/redis.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/redis.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/requests.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/starlette.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/instrumentation/urllib3.py` & `helios-opentelemetry-sdk-1.0.93/helios/instrumentation/urllib3.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.93/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.93/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.93/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.93/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios/utils.py` & `helios-opentelemetry-sdk-1.0.93/helios/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.92
+Version: 1.0.93
 Summary: Helios OpenTelemetry SDK
 Home-page: https://docs.gethelios.dev/docs/python
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
 Classifier: Intended Audience :: Developers
```

### Comparing `helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.93/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.93/hstest/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.92/setup.py` & `helios-opentelemetry-sdk-1.0.93/setup.py`

 * *Files identical despite different names*

