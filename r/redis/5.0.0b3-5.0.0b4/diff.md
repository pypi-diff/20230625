# Comparing `tmp/redis-5.0.0b3.tar.gz` & `tmp/redis-5.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-5.0.0b3.tar", last modified: Thu May  4 09:43:28 2023, max compression
+gzip compressed data, was "redis-5.0.0b4.tar", last modified: Sun May 28 09:28:37 2023, max compression
```

## Comparing `redis-5.0.0b3.tar` & `redis-5.0.0b4.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.397854 redis-5.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 09:43:12.000000 redis-5.0.0b3/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 09:43:12.000000 redis-5.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 09:43:12.000000 redis-5.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-04 09:43:28.397854 redis-5.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-04 09:43:12.000000 redis-5.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55393 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    51222 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/backoff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80560 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    86601 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   216287 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    46593 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/ocsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/hiredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/resp2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/resp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:43:28.397854 redis-5.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-04 09:43:12.000000 redis-5.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.389854 redis-5.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/asynctests
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/synctests
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/test_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38371 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_sentinel_managed_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/test_asyncio/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/testdata/will_play_text.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/test_graph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/testdata/will_play_text.csv.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.120266 redis-5.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 09:28:22.000000 redis-5.0.0b4/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-28 09:28:22.000000 redis-5.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-28 09:28:22.000000 redis-5.0.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-28 09:28:37.120266 redis-5.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-28 09:28:22.000000 redis-5.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.104266 redis-5.0.0b4/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.104266 redis-5.0.0b4/redis/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55393 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51222 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/backoff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    83526 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90431 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   217363 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.108266 redis-5.0.0b4/redis/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.112266 redis-5.0.0b4/redis/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.112266 redis-5.0.0b4/redis/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46593 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/ocsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.112266 redis-5.0.0b4/redis/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/resp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/resp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/parsers/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-28 09:28:22.000000 redis-5.0.0b4/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.104266 redis-5.0.0b4/redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 09:28:37.000000 redis-5.0.0b4/redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 09:28:37.120266 redis-5.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-28 09:28:22.000000 redis-5.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.116266 redis-5.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/asynctests
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/synctests
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.116266 redis-5.0.0b4/tests/test_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38161 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_sentinel_managed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.116266 redis-5.0.0b4/tests/test_asyncio/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_asyncio/testdata/will_play_text.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.120266 redis-5.0.0b4/tests/test_graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_graph_utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42590 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:28:37.120266 redis-5.0.0b4/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-28 09:28:22.000000 redis-5.0.0b4/tests/testdata/will_play_text.csv.bz2
```

### Comparing `redis-5.0.0b3/LICENSE` & `redis-5.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/PKG-INFO` & `redis-5.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b3
+Version: 5.0.0b4
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b3/README.md` & `redis-5.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/__init__.py` & `redis-5.0.0b4/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/__init__.py` & `redis-5.0.0b4/redis/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/client.py` & `redis-5.0.0b4/redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/cluster.py` & `redis-5.0.0b4/redis/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/connection.py` & `redis-5.0.0b4/redis/asyncio/connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/lock.py` & `redis-5.0.0b4/redis/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/retry.py` & `redis-5.0.0b4/redis/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/sentinel.py` & `redis-5.0.0b4/redis/asyncio/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/asyncio/utils.py` & `redis-5.0.0b4/redis/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/backoff.py` & `redis-5.0.0b4/redis/backoff.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/client.py` & `redis-5.0.0b4/redis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -829,14 +829,15 @@
         "MODULE UNLOAD": parse_module_result,
         "MODULE LIST": lambda r: [pairs_to_dict(m) for m in r],
         "OBJECT": parse_object,
         "PING": lambda r: str_if_bytes(r) == "PONG",
         "QUIT": bool_ok,
         "STRALGO": parse_stralgo,
         "PUBSUB NUMSUB": parse_pubsub_numsub,
+        "PUBSUB SHARDNUMSUB": parse_pubsub_numsub,
         "RANDOMKEY": lambda r: r and r or None,
         "RESET": str_if_bytes,
         "SCAN": parse_scan,
         "SCRIPT EXISTS": lambda r: list(map(bool, r)),
         "SCRIPT FLUSH": bool_ok,
         "SCRIPT KILL": bool_ok,
         "SCRIPT LOAD": str_if_bytes,
@@ -1436,16 +1437,16 @@
     PubSub provides publish, subscribe and listen support to Redis channels.
 
     After subscribing to one or more channels, the listen() method will block
     until a message arrives on one of the subscribed channels. That message
     will be returned and it's safe to start listening again.
     """
 
-    PUBLISH_MESSAGE_TYPES = ("message", "pmessage")
-    UNSUBSCRIBE_MESSAGE_TYPES = ("unsubscribe", "punsubscribe")
+    PUBLISH_MESSAGE_TYPES = ("message", "pmessage", "smessage")
+    UNSUBSCRIBE_MESSAGE_TYPES = ("unsubscribe", "punsubscribe", "sunsubscribe")
     HEALTH_CHECK_MESSAGE = "redis-py-health-check"
 
     def __init__(
         self,
         connection_pool,
         shard_hint=None,
         ignore_subscribe_messages=False,
@@ -1489,41 +1490,50 @@
 
     def reset(self):
         if self.connection:
             self.connection.disconnect()
             self.connection.clear_connect_callbacks()
             self.connection_pool.release(self.connection)
             self.connection = None
-        self.channels = {}
         self.health_check_response_counter = 0
+        self.channels = {}
         self.pending_unsubscribe_channels = set()
+        self.shard_channels = {}
+        self.pending_unsubscribe_shard_channels = set()
         self.patterns = {}
         self.pending_unsubscribe_patterns = set()
         self.subscribed_event.clear()
 
     def close(self):
         self.reset()
 
     def on_connect(self, connection):
         "Re-subscribe to any channels and patterns previously subscribed to"
         # NOTE: for python3, we can't pass bytestrings as keyword arguments
         # so we need to decode channel/pattern names back to unicode strings
         # before passing them to [p]subscribe.
         self.pending_unsubscribe_channels.clear()
         self.pending_unsubscribe_patterns.clear()
+        self.pending_unsubscribe_shard_channels.clear()
         if self.channels:
-            channels = {}
-            for k, v in self.channels.items():
-                channels[self.encoder.decode(k, force=True)] = v
+            channels = {
+                self.encoder.decode(k, force=True): v for k, v in self.channels.items()
+            }
             self.subscribe(**channels)
         if self.patterns:
-            patterns = {}
-            for k, v in self.patterns.items():
-                patterns[self.encoder.decode(k, force=True)] = v
+            patterns = {
+                self.encoder.decode(k, force=True): v for k, v in self.patterns.items()
+            }
             self.psubscribe(**patterns)
+        if self.shard_channels:
+            shard_channels = {
+                self.encoder.decode(k, force=True): v
+                for k, v in self.shard_channels.items()
+            }
+            self.ssubscribe(**shard_channels)
 
     @property
     def subscribed(self):
         """Indicates if there are subscriptions to any channels or patterns"""
         return self.subscribed_event.is_set()
 
     def execute_command(self, *args):
@@ -1724,14 +1734,53 @@
             args = list_or_args(args[0], args[1:])
             channels = self._normalize_keys(dict.fromkeys(args))
         else:
             channels = self.channels
         self.pending_unsubscribe_channels.update(channels)
         return self.execute_command("UNSUBSCRIBE", *args)
 
+    def ssubscribe(self, *args, target_node=None, **kwargs):
+        """
+        Subscribes the client to the specified shard channels.
+        Channels supplied as keyword arguments expect a channel name as the key
+        and a callable as the value. A channel's callable will be invoked automatically
+        when a message is received on that channel rather than producing a message via
+        ``listen()`` or ``get_sharded_message()``.
+        """
+        if args:
+            args = list_or_args(args[0], args[1:])
+        new_s_channels = dict.fromkeys(args)
+        new_s_channels.update(kwargs)
+        ret_val = self.execute_command("SSUBSCRIBE", *new_s_channels.keys())
+        # update the s_channels dict AFTER we send the command. we don't want to
+        # subscribe twice to these channels, once for the command and again
+        # for the reconnection.
+        new_s_channels = self._normalize_keys(new_s_channels)
+        self.shard_channels.update(new_s_channels)
+        if not self.subscribed:
+            # Set the subscribed_event flag to True
+            self.subscribed_event.set()
+            # Clear the health check counter
+            self.health_check_response_counter = 0
+        self.pending_unsubscribe_shard_channels.difference_update(new_s_channels)
+        return ret_val
+
+    def sunsubscribe(self, *args, target_node=None):
+        """
+        Unsubscribe from the supplied shard_channels. If empty, unsubscribe from
+        all shard_channels
+        """
+        if args:
+            args = list_or_args(args[0], args[1:])
+            s_channels = self._normalize_keys(dict.fromkeys(args))
+        else:
+            s_channels = self.shard_channels
+        self.pending_unsubscribe_shard_channels.update(s_channels)
+        return self.execute_command("SUNSUBSCRIBE", *args)
+
     def listen(self):
         "Listen for messages on channels this client has been subscribed to"
         while self.subscribed:
             response = self.handle_message(self.parse_response(block=True))
             if response is not None:
                 yield response
 
@@ -1758,14 +1807,16 @@
                 return None
 
         response = self.parse_response(block=(timeout is None), timeout=timeout)
         if response:
             return self.handle_message(response, ignore_subscribe_messages)
         return None
 
+    get_sharded_message = get_message
+
     def ping(self, message=None):
         """
         Ping the Redis server
         """
         args = ["PING", message] if message is not None else ["PING"]
         return self.execute_command(*args)
 
@@ -1805,28 +1856,35 @@
         # if this is an unsubscribe message, remove it from memory
         if message_type in self.UNSUBSCRIBE_MESSAGE_TYPES:
             if message_type == "punsubscribe":
                 pattern = response[1]
                 if pattern in self.pending_unsubscribe_patterns:
                     self.pending_unsubscribe_patterns.remove(pattern)
                     self.patterns.pop(pattern, None)
+            elif message_type == "sunsubscribe":
+                s_channel = response[1]
+                if s_channel in self.pending_unsubscribe_shard_channels:
+                    self.pending_unsubscribe_shard_channels.remove(s_channel)
+                    self.shard_channels.pop(s_channel, None)
             else:
                 channel = response[1]
                 if channel in self.pending_unsubscribe_channels:
                     self.pending_unsubscribe_channels.remove(channel)
                     self.channels.pop(channel, None)
-            if not self.channels and not self.patterns:
+            if not self.channels and not self.patterns and not self.shard_channels:
                 # There are no subscriptions anymore, set subscribed_event flag
                 # to false
                 self.subscribed_event.clear()
 
         if message_type in self.PUBLISH_MESSAGE_TYPES:
             # if there's a message handler, invoke it
             if message_type == "pmessage":
                 handler = self.patterns.get(message["pattern"], None)
+            elif message_type == "smessage":
+                handler = self.shard_channels.get(message["channel"], None)
             else:
                 handler = self.channels.get(message["channel"], None)
             if handler:
                 handler(message)
                 return None
         elif message_type != "pong":
             # this is a subscribe/unsubscribe message. ignore if we don't
@@ -1839,14 +1897,19 @@
     def run_in_thread(self, sleep_time=0, daemon=False, exception_handler=None):
         for channel, handler in self.channels.items():
             if handler is None:
                 raise PubSubError(f"Channel: '{channel}' has no handler registered")
         for pattern, handler in self.patterns.items():
             if handler is None:
                 raise PubSubError(f"Pattern: '{pattern}' has no handler registered")
+        for s_channel, handler in self.shard_channels.items():
+            if handler is None:
+                raise PubSubError(
+                    f"Shard Channel: '{s_channel}' has no handler registered"
+                )
 
         thread = PubSubWorkerThread(
             self, sleep_time, daemon=daemon, exception_handler=exception_handler
         )
         thread.start()
         return thread
```

### Comparing `redis-5.0.0b3/redis/cluster.py` & `redis-5.0.0b4/redis/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 from collections import OrderedDict
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from redis.backoff import default_backoff
 from redis.client import CaseInsensitiveDict, PubSub, Redis, parse_scan
 from redis.commands import READ_COMMANDS, RedisClusterCommands
+from redis.commands.helpers import list_or_args
 from redis.connection import ConnectionPool, DefaultParser, parse_url
 from redis.crc import REDIS_CLUSTER_HASH_SLOTS, key_slot
 from redis.exceptions import (
     AskError,
     AuthenticationError,
     ClusterCrossSlotError,
     ClusterDownError,
@@ -218,14 +219,16 @@
                 "CONFIG SET",
                 "CONFIG REWRITE",
                 "CONFIG RESETSTAT",
                 "TIME",
                 "PUBSUB CHANNELS",
                 "PUBSUB NUMPAT",
                 "PUBSUB NUMSUB",
+                "PUBSUB SHARDCHANNELS",
+                "PUBSUB SHARDNUMSUB",
                 "PING",
                 "INFO",
                 "SHUTDOWN",
                 "KEYS",
                 "DBSIZE",
                 "BGSAVE",
                 "SLOWLOG GET",
@@ -342,19 +345,21 @@
 
     CLUSTER_COMMANDS_RESPONSE_CALLBACKS = {
         "CLUSTER SLOTS": parse_cluster_slots,
         "CLUSTER SHARDS": parse_cluster_shards,
     }
 
     RESULT_CALLBACKS = dict_merge(
-        list_keys_to_dict(["PUBSUB NUMSUB"], parse_pubsub_numsub),
+        list_keys_to_dict(["PUBSUB NUMSUB", "PUBSUB SHARDNUMSUB"], parse_pubsub_numsub),
         list_keys_to_dict(
             ["PUBSUB NUMPAT"], lambda command, res: sum(list(res.values()))
         ),
-        list_keys_to_dict(["KEYS", "PUBSUB CHANNELS"], merge_result),
+        list_keys_to_dict(
+            ["KEYS", "PUBSUB CHANNELS", "PUBSUB SHARDCHANNELS"], merge_result
+        ),
         list_keys_to_dict(
             [
                 "PING",
                 "CONFIG SET",
                 "CONFIG REWRITE",
                 "CONFIG RESETSTAT",
                 "CLIENT SETNAME",
@@ -1621,14 +1626,16 @@
         self.set_pubsub_node(redis_cluster, node, host, port)
         connection_pool = (
             None
             if self.node is None
             else redis_cluster.get_redis_connection(self.node).connection_pool
         )
         self.cluster = redis_cluster
+        self.node_pubsub_mapping = {}
+        self._pubsubs_generator = self._pubsubs_generator()
         super().__init__(
             **kwargs, connection_pool=connection_pool, encoder=redis_cluster.encoder
         )
 
     def set_pubsub_node(self, cluster, node=None, host=None, port=None):
         """
         The pubsub node will be set according to the passed node, host and port
@@ -1674,17 +1681,17 @@
         the cluster.
         """
         if node is None or redis_cluster.get_node(node_name=node.name) is None:
             raise RedisClusterException(
                 f"Node {host}:{port} doesn't exist in the cluster"
             )
 
-    def execute_command(self, *args, **kwargs):
+    def execute_command(self, *args):
         """
-        Execute a publish/subscribe command.
+        Execute a subscribe/unsubscribe command.
 
         Taken code from redis-py and tweak to make it work within a cluster.
         """
         # NOTE: don't parse the response in this function -- it could pull a
         # legitimate message off the stack if the connection is already
         # subscribed to one or more channels
 
@@ -1709,21 +1716,111 @@
             )
             # register a callback that re-subscribes to any channels we
             # were listening to when we were disconnected
             self.connection.register_connect_callback(self.on_connect)
         connection = self.connection
         self._execute(connection, connection.send_command, *args)
 
+    def _get_node_pubsub(self, node):
+        try:
+            return self.node_pubsub_mapping[node.name]
+        except KeyError:
+            pubsub = node.redis_connection.pubsub()
+            self.node_pubsub_mapping[node.name] = pubsub
+            return pubsub
+
+    def _sharded_message_generator(self):
+        for _ in range(len(self.node_pubsub_mapping)):
+            pubsub = next(self._pubsubs_generator)
+            message = pubsub.get_message()
+            if message is not None:
+                return message
+        return None
+
+    def _pubsubs_generator(self):
+        while True:
+            for pubsub in self.node_pubsub_mapping.values():
+                yield pubsub
+
+    def get_sharded_message(
+        self, ignore_subscribe_messages=False, timeout=0.0, target_node=None
+    ):
+        if target_node:
+            message = self.node_pubsub_mapping[target_node.name].get_message(
+                ignore_subscribe_messages=ignore_subscribe_messages, timeout=timeout
+            )
+        else:
+            message = self._sharded_message_generator()
+        if message is None:
+            return None
+        elif str_if_bytes(message["type"]) == "sunsubscribe":
+            if message["channel"] in self.pending_unsubscribe_shard_channels:
+                self.pending_unsubscribe_shard_channels.remove(message["channel"])
+                self.shard_channels.pop(message["channel"], None)
+                node = self.cluster.get_node_from_key(message["channel"])
+                if self.node_pubsub_mapping[node.name].subscribed is False:
+                    self.node_pubsub_mapping.pop(node.name)
+        if not self.channels and not self.patterns and not self.shard_channels:
+            # There are no subscriptions anymore, set subscribed_event flag
+            # to false
+            self.subscribed_event.clear()
+        if self.ignore_subscribe_messages or ignore_subscribe_messages:
+            return None
+        return message
+
+    def ssubscribe(self, *args, **kwargs):
+        if args:
+            args = list_or_args(args[0], args[1:])
+        s_channels = dict.fromkeys(args)
+        s_channels.update(kwargs)
+        for s_channel, handler in s_channels.items():
+            node = self.cluster.get_node_from_key(s_channel)
+            pubsub = self._get_node_pubsub(node)
+            if handler:
+                pubsub.ssubscribe(**{s_channel: handler})
+            else:
+                pubsub.ssubscribe(s_channel)
+            self.shard_channels.update(pubsub.shard_channels)
+            self.pending_unsubscribe_shard_channels.difference_update(
+                self._normalize_keys({s_channel: None})
+            )
+            if pubsub.subscribed and not self.subscribed:
+                self.subscribed_event.set()
+                self.health_check_response_counter = 0
+
+    def sunsubscribe(self, *args):
+        if args:
+            args = list_or_args(args[0], args[1:])
+        else:
+            args = self.shard_channels
+
+        for s_channel in args:
+            node = self.cluster.get_node_from_key(s_channel)
+            p = self._get_node_pubsub(node)
+            p.sunsubscribe(s_channel)
+            self.pending_unsubscribe_shard_channels.update(
+                p.pending_unsubscribe_shard_channels
+            )
+
     def get_redis_connection(self):
         """
         Get the Redis connection of the pubsub connected node.
         """
         if self.node is not None:
             return self.node.redis_connection
 
+    def disconnect(self):
+        """
+        Disconnect the pubsub connection.
+        """
+        if self.connection:
+            self.connection.disconnect()
+        for pubsub in self.node_pubsub_mapping.values():
+            pubsub.connection.disconnect()
+
 
 class ClusterPipeline(RedisCluster):
     """
     Support for Redis pipeline
     in cluster mode
     """
```

### Comparing `redis-5.0.0b3/redis/commands/__init__.py` & `redis-5.0.0b4/redis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/bf/__init__.py` & `redis-5.0.0b4/redis/commands/bf/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/bf/commands.py` & `redis-5.0.0b4/redis/commands/bf/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/bf/info.py` & `redis-5.0.0b4/redis/commands/bf/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/cluster.py` & `redis-5.0.0b4/redis/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/core.py` & `redis-5.0.0b4/redis/commands/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -5099,22 +5099,39 @@
         Publish ``message`` on ``channel``.
         Returns the number of subscribers the message was delivered to.
 
         For more information see https://redis.io/commands/publish
         """
         return self.execute_command("PUBLISH", channel, message, **kwargs)
 
+    def spublish(self, shard_channel: ChannelT, message: EncodableT) -> ResponseT:
+        """
+        Posts a message to the given shard channel.
+        Returns the number of clients that received the message
+
+        For more information see https://redis.io/commands/spublish
+        """
+        return self.execute_command("SPUBLISH", shard_channel, message)
+
     def pubsub_channels(self, pattern: PatternT = "*", **kwargs) -> ResponseT:
         """
         Return a list of channels that have at least one subscriber
 
         For more information see https://redis.io/commands/pubsub-channels
         """
         return self.execute_command("PUBSUB CHANNELS", pattern, **kwargs)
 
+    def pubsub_shardchannels(self, pattern: PatternT = "*", **kwargs) -> ResponseT:
+        """
+        Return a list of shard_channels that have at least one subscriber
+
+        For more information see https://redis.io/commands/pubsub-shardchannels
+        """
+        return self.execute_command("PUBSUB SHARDCHANNELS", pattern, **kwargs)
+
     def pubsub_numpat(self, **kwargs) -> ResponseT:
         """
         Returns the number of subscriptions to patterns
 
         For more information see https://redis.io/commands/pubsub-numpat
         """
         return self.execute_command("PUBSUB NUMPAT", **kwargs)
@@ -5124,14 +5141,23 @@
         Return a list of (channel, number of subscribers) tuples
         for each channel given in ``*args``
 
         For more information see https://redis.io/commands/pubsub-numsub
         """
         return self.execute_command("PUBSUB NUMSUB", *args, **kwargs)
 
+    def pubsub_shardnumsub(self, *args: ChannelT, **kwargs) -> ResponseT:
+        """
+        Return a list of (shard_channel, number of subscribers) tuples
+        for each channel given in ``*args``
+
+        For more information see https://redis.io/commands/pubsub-shardnumsub
+        """
+        return self.execute_command("PUBSUB SHARDNUMSUB", *args, **kwargs)
+
 
 AsyncPubSubCommands = PubSubCommands
 
 
 class ScriptCommands(CommandsProtocol):
     """
     Redis Lua script commands. see:
```

### Comparing `redis-5.0.0b3/redis/commands/graph/__init__.py` & `redis-5.0.0b4/redis/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/graph/commands.py` & `redis-5.0.0b4/redis/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/graph/edge.py` & `redis-5.0.0b4/redis/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/graph/execution_plan.py` & `redis-5.0.0b4/redis/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/graph/node.py` & `redis-5.0.0b4/redis/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/graph/path.py` & `redis-5.0.0b4/redis/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/graph/query_result.py` & `redis-5.0.0b4/redis/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/helpers.py` & `redis-5.0.0b4/redis/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/json/__init__.py` & `redis-5.0.0b4/redis/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/json/commands.py` & `redis-5.0.0b4/redis/commands/json/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/json/decoders.py` & `redis-5.0.0b4/redis/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/redismodules.py` & `redis-5.0.0b4/redis/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/__init__.py` & `redis-5.0.0b4/redis/commands/search/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/aggregation.py` & `redis-5.0.0b4/redis/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/commands.py` & `redis-5.0.0b4/redis/commands/search/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/field.py` & `redis-5.0.0b4/redis/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/indexDefinition.py` & `redis-5.0.0b4/redis/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/query.py` & `redis-5.0.0b4/redis/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/querystring.py` & `redis-5.0.0b4/redis/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/reducers.py` & `redis-5.0.0b4/redis/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/result.py` & `redis-5.0.0b4/redis/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/search/suggestion.py` & `redis-5.0.0b4/redis/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/sentinel.py` & `redis-5.0.0b4/redis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/timeseries/__init__.py` & `redis-5.0.0b4/redis/commands/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/timeseries/commands.py` & `redis-5.0.0b4/redis/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/timeseries/info.py` & `redis-5.0.0b4/redis/commands/timeseries/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/commands/timeseries/utils.py` & `redis-5.0.0b4/redis/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/connection.py` & `redis-5.0.0b4/redis/connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/crc.py` & `redis-5.0.0b4/redis/crc.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/credentials.py` & `redis-5.0.0b4/redis/credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/exceptions.py` & `redis-5.0.0b4/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/lock.py` & `redis-5.0.0b4/redis/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/ocsp.py` & `redis-5.0.0b4/redis/ocsp.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/parsers/__init__.py` & `redis-5.0.0b4/redis/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/parsers/base.py` & `redis-5.0.0b4/redis/parsers/base.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/parsers/commands.py` & `redis-5.0.0b4/redis/parsers/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,21 +151,21 @@
         args = [str_if_bytes(arg) for arg in args]
         command = args[0].upper()
         keys = None
         if command == "PUBSUB":
             # the second argument is a part of the command name, e.g.
             # ['PUBSUB', 'NUMSUB', 'foo'].
             pubsub_type = args[1].upper()
-            if pubsub_type in ["CHANNELS", "NUMSUB"]:
+            if pubsub_type in ["CHANNELS", "NUMSUB", "SHARDCHANNELS", "SHARDNUMSUB"]:
                 keys = args[2:]
         elif command in ["SUBSCRIBE", "PSUBSCRIBE", "UNSUBSCRIBE", "PUNSUBSCRIBE"]:
             # format example:
             # SUBSCRIBE channel [channel ...]
             keys = list(args[1:])
-        elif command == "PUBLISH":
+        elif command in ["PUBLISH", "SPUBLISH"]:
             # format example:
             # PUBLISH channel message
             keys = [args[1]]
         return keys
 
 
 class AsyncCommandsParser:
```

### Comparing `redis-5.0.0b3/redis/parsers/encoders.py` & `redis-5.0.0b4/redis/parsers/encoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/parsers/hiredis.py` & `redis-5.0.0b4/redis/parsers/hiredis.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/parsers/resp2.py` & `redis-5.0.0b4/redis/parsers/resp2.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/parsers/resp3.py` & `redis-5.0.0b4/redis/parsers/resp3.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,22 +88,23 @@
             ]
             try:
                 response = set(response)
             except TypeError:
                 pass
         # map response
         elif byte == b"%":
-            response = {
-                self._read_response(
-                    disable_decoding=disable_decoding
-                ): self._read_response(
+            # we use this approach and not dict comprehension here
+            # because this dict comprehension fails in python 3.7
+            resp_dict = {}
+            for _ in range(int(response)):
+                key = self._read_response(disable_decoding=disable_decoding)
+                resp_dict[key] = self._read_response(
                     disable_decoding=disable_decoding, push_request=push_request
                 )
-                for _ in range(int(response))
-            }
+            response = resp_dict
         # push response
         elif byte == b">":
             response = [
                 self._read_response(
                     disable_decoding=disable_decoding, push_request=push_request
                 )
                 for _ in range(int(response))
```

### Comparing `redis-5.0.0b3/redis/parsers/socket.py` & `redis-5.0.0b4/redis/parsers/socket.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/retry.py` & `redis-5.0.0b4/redis/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/sentinel.py` & `redis-5.0.0b4/redis/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/typing.py` & `redis-5.0.0b4/redis/typing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis/utils.py` & `redis-5.0.0b4/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/redis.egg-info/PKG-INFO` & `redis-5.0.0b4/redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b3
+Version: 5.0.0b4
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b3/redis.egg-info/SOURCES.txt` & `redis-5.0.0b4/redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/setup.py` & `redis-5.0.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup(
     name="redis",
     description="Python client for Redis database and key-value store",
     long_description=open("README.md").read().strip(),
     long_description_content_type="text/markdown",
     keywords=["Redis", "key-value store", "database"],
     license="MIT",
-    version="5.0.0b3",
+    version="5.0.0b4",
     packages=find_packages(
         include=[
             "redis",
             "redis.asyncio",
             "redis.commands",
             "redis.commands.bf",
             "redis.commands.json",
```

### Comparing `redis-5.0.0b3/tests/asynctests` & `redis-5.0.0b4/tests/asynctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/conftest.py` & `redis-5.0.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/mocks.py` & `redis-5.0.0b4/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/synctests` & `redis-5.0.0b4/tests/synctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/conftest.py` & `redis-5.0.0b4/tests/test_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/mocks.py` & `redis-5.0.0b4/tests/test_asyncio/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_bloom.py` & `redis-5.0.0b4/tests/test_asyncio/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_cluster.py` & `redis-5.0.0b4/tests/test_asyncio/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_commands.py` & `redis-5.0.0b4/tests/test_asyncio/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_connection.py` & `redis-5.0.0b4/tests/test_asyncio/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_connection_pool.py` & `redis-5.0.0b4/tests/test_asyncio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_credentials.py` & `redis-5.0.0b4/tests/test_asyncio/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_encoding.py` & `redis-5.0.0b4/tests/test_asyncio/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_graph.py` & `redis-5.0.0b4/tests/test_asyncio/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_json.py` & `redis-5.0.0b4/tests/test_asyncio/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_lock.py` & `redis-5.0.0b4/tests/test_asyncio/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_monitor.py` & `redis-5.0.0b4/tests/test_asyncio/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_pipeline.py` & `redis-5.0.0b4/tests/test_asyncio/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_pubsub.py` & `redis-5.0.0b4/tests/test_asyncio/test_pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -671,26 +671,23 @@
 
         async def loop():
             # must make sure the task exits
             async with async_timeout(2):
                 nonlocal interrupt
                 await pubsub.subscribe("foo")
                 while True:
-                    # print("loop")
                     try:
                         try:
                             await pubsub.connect()
                             await loop_step()
-                            # print("succ")
                         except redis.ConnectionError:
                             await asyncio.sleep(0.1)
                     except asyncio.CancelledError:
                         # we use a cancel to interrupt the "listen"
                         # when we perform a disconnect
-                        # print("cancel", interrupt)
                         if interrupt:
                             interrupt = False
                         else:
                             raise
 
         async def loop_step():
             # get a single message via listen()
@@ -915,15 +912,14 @@
         while True:
             await asyncio.sleep(0.01)  # give main thread chance to get lock
             async with self.cond:
                 old_state = self.state
                 try:
                     if self.state == 4:
                         break
-                    # print("state a ", self.state)
                     got_msg = await self.get_message()
                     assert got_msg
                     if self.state in (1, 2):
                         self.state = 3  # successful reconnect
                 except redis.ConnectionError:
                     assert self.state in (1, 2)
                     self.state = 2  # signal that we noticed the disconnect
@@ -933,15 +929,14 @@
                 # or reconnected without any error
                 if old_state == 1:
                     assert self.state in (2, 3)
 
     async def loop_step_get_message(self):
         # get a single message via get_message
         message = await self.pubsub.get_message(timeout=0.1)
-        # print(message)
         if message is not None:
             await self.messages.put(message)
             return True
         return False
 
     async def loop_step_listen(self):
         # get a single message via listen()
```

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_retry.py` & `redis-5.0.0b4/tests/test_asyncio/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_scripting.py` & `redis-5.0.0b4/tests/test_asyncio/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_search.py` & `redis-5.0.0b4/tests/test_asyncio/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_sentinel.py` & `redis-5.0.0b4/tests/test_asyncio/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_sentinel_managed_connection.py` & `redis-5.0.0b4/tests/test_asyncio/test_sentinel_managed_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/test_timeseries.py` & `redis-5.0.0b4/tests/test_asyncio/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/testdata/jsontestdata.py` & `redis-5.0.0b4/tests/test_asyncio/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/testdata/titles.csv` & `redis-5.0.0b4/tests/test_asyncio/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_asyncio/testdata/will_play_text.csv.bz2` & `redis-5.0.0b4/tests/test_asyncio/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_bloom.py` & `redis-5.0.0b4/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_cluster.py` & `redis-5.0.0b4/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_command_parser.py` & `redis-5.0.0b4/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_commands.py` & `redis-5.0.0b4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_connection.py` & `redis-5.0.0b4/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_connection_pool.py` & `redis-5.0.0b4/tests/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_credentials.py` & `redis-5.0.0b4/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_encoding.py` & `redis-5.0.0b4/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_function.py` & `redis-5.0.0b4/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_graph.py` & `redis-5.0.0b4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_graph_utils/test_edge.py` & `redis-5.0.0b4/tests/test_graph_utils/test_edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_graph_utils/test_node.py` & `redis-5.0.0b4/tests/test_graph_utils/test_node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_graph_utils/test_path.py` & `redis-5.0.0b4/tests/test_graph_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_helpers.py` & `redis-5.0.0b4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_json.py` & `redis-5.0.0b4/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_lock.py` & `redis-5.0.0b4/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_monitor.py` & `redis-5.0.0b4/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_multiprocessing.py` & `redis-5.0.0b4/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_pipeline.py` & `redis-5.0.0b4/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_pubsub.py` & `redis-5.0.0b4/tests/test_pubsub.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import platform
 import queue
 import socket
 import threading
 import time
+from collections import defaultdict
 from unittest import mock
 from unittest.mock import patch
 
 import pytest
 
 import redis
 from redis.exceptions import ConnectionError
@@ -16,21 +17,30 @@
     _get_client,
     is_resp2_connection,
     skip_if_redis_enterprise,
     skip_if_server_version_lt,
 )
 
 
-def wait_for_message(pubsub, timeout=0.5, ignore_subscribe_messages=False):
+def wait_for_message(
+    pubsub, timeout=0.5, ignore_subscribe_messages=False, node=None, func=None
+):
     now = time.time()
     timeout = now + timeout
     while now < timeout:
-        message = pubsub.get_message(
-            ignore_subscribe_messages=ignore_subscribe_messages
-        )
+        if node:
+            message = pubsub.get_sharded_message(
+                ignore_subscribe_messages=ignore_subscribe_messages, target_node=node
+            )
+        elif func:
+            message = func(ignore_subscribe_messages=ignore_subscribe_messages)
+        else:
+            message = pubsub.get_message(
+                ignore_subscribe_messages=ignore_subscribe_messages
+            )
         if message is not None:
             return message
         time.sleep(0.01)
         now = time.time()
     return None
 
 
@@ -49,14 +59,23 @@
             "p": pubsub,
             "sub_type": "subscribe",
             "unsub_type": "unsubscribe",
             "sub_func": pubsub.subscribe,
             "unsub_func": pubsub.unsubscribe,
             "keys": ["foo", "bar", "uni" + chr(4456) + "code"],
         }
+    elif type == "shard_channel":
+        return {
+            "p": pubsub,
+            "sub_type": "ssubscribe",
+            "unsub_type": "sunsubscribe",
+            "sub_func": pubsub.ssubscribe,
+            "unsub_func": pubsub.sunsubscribe,
+            "keys": ["foo", "bar", "uni" + chr(4456) + "code"],
+        }
     elif type == "pattern":
         return {
             "p": pubsub,
             "sub_type": "psubscribe",
             "unsub_type": "punsubscribe",
             "sub_func": pubsub.psubscribe,
             "unsub_func": pubsub.punsubscribe,
@@ -89,14 +108,52 @@
         kwargs = make_subscribe_test_data(r.pubsub(), "channel")
         self._test_subscribe_unsubscribe(**kwargs)
 
     def test_pattern_subscribe_unsubscribe(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "pattern")
         self._test_subscribe_unsubscribe(**kwargs)
 
+    @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_shard_channel_subscribe_unsubscribe(self, r):
+        kwargs = make_subscribe_test_data(r.pubsub(), "shard_channel")
+        self._test_subscribe_unsubscribe(**kwargs)
+
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_shard_channel_subscribe_unsubscribe_cluster(self, r):
+        node_channels = defaultdict(int)
+        p = r.pubsub()
+        keys = {
+            "foo": r.get_node_from_key("foo"),
+            "bar": r.get_node_from_key("bar"),
+            "uni" + chr(4456) + "code": r.get_node_from_key("uni" + chr(4456) + "code"),
+        }
+
+        for key, node in keys.items():
+            assert p.ssubscribe(key) is None
+
+        # should be a message for each shard_channel we just subscribed to
+        for key, node in keys.items():
+            node_channels[node.name] += 1
+            assert wait_for_message(p, node=node) == make_message(
+                "ssubscribe", key, node_channels[node.name]
+            )
+
+        for key in keys.keys():
+            assert p.sunsubscribe(key) is None
+
+        # should be a message for each shard_channel we just unsubscribed
+        # from
+        for key, node in keys.items():
+            node_channels[node.name] -= 1
+            assert wait_for_message(p, node=node) == make_message(
+                "sunsubscribe", key, node_channels[node.name]
+            )
+
     def _test_resubscribe_on_reconnection(
         self, p, sub_type, unsub_type, sub_func, unsub_func, keys
     ):
 
         for key in keys:
             assert sub_func(key) is None
 
@@ -132,14 +189,20 @@
         self._test_resubscribe_on_reconnection(**kwargs)
 
     @pytest.mark.onlynoncluster
     def test_resubscribe_to_patterns_on_reconnection(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "pattern")
         self._test_resubscribe_on_reconnection(**kwargs)
 
+    @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_resubscribe_to_shard_channels_on_reconnection(self, r):
+        kwargs = make_subscribe_test_data(r.pubsub(), "shard_channel")
+        self._test_resubscribe_on_reconnection(**kwargs)
+
     def _test_subscribed_property(
         self, p, sub_type, unsub_type, sub_func, unsub_func, keys
     ):
 
         assert p.subscribed is False
         sub_func(keys[0])
         # we're now subscribed even though we haven't processed the
@@ -188,94 +251,219 @@
         self._test_subscribed_property(**kwargs)
 
     @pytest.mark.onlynoncluster
     def test_subscribe_property_with_patterns(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "pattern")
         self._test_subscribed_property(**kwargs)
 
+    @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_subscribe_property_with_shard_channels(self, r):
+        kwargs = make_subscribe_test_data(r.pubsub(), "shard_channel")
+        self._test_subscribed_property(**kwargs)
+
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_subscribe_property_with_shard_channels_cluster(self, r):
+        p = r.pubsub()
+        keys = ["foo", "bar", "uni" + chr(4456) + "code"]
+        nodes = [r.get_node_from_key(key) for key in keys]
+        assert p.subscribed is False
+        p.ssubscribe(keys[0])
+        # we're now subscribed even though we haven't processed the
+        # reply from the server just yet
+        assert p.subscribed is True
+        assert wait_for_message(p, node=nodes[0]) == make_message(
+            "ssubscribe", keys[0], 1
+        )
+        # we're still subscribed
+        assert p.subscribed is True
+
+        # unsubscribe from all shard_channels
+        p.sunsubscribe()
+        # we're still technically subscribed until we process the
+        # response messages from the server
+        assert p.subscribed is True
+        assert wait_for_message(p, node=nodes[0]) == make_message(
+            "sunsubscribe", keys[0], 0
+        )
+        # now we're no longer subscribed as no more messages can be delivered
+        # to any channels we were listening to
+        assert p.subscribed is False
+
+        # subscribing again flips the flag back
+        p.ssubscribe(keys[0])
+        assert p.subscribed is True
+        assert wait_for_message(p, node=nodes[0]) == make_message(
+            "ssubscribe", keys[0], 1
+        )
+
+        # unsubscribe again
+        p.sunsubscribe()
+        assert p.subscribed is True
+        # subscribe to another shard_channel before reading the unsubscribe response
+        p.ssubscribe(keys[1])
+        assert p.subscribed is True
+        # read the unsubscribe for key1
+        assert wait_for_message(p, node=nodes[0]) == make_message(
+            "sunsubscribe", keys[0], 0
+        )
+        # we're still subscribed to key2, so subscribed should still be True
+        assert p.subscribed is True
+        # read the key2 subscribe message
+        assert wait_for_message(p, node=nodes[1]) == make_message(
+            "ssubscribe", keys[1], 1
+        )
+        p.sunsubscribe()
+        # haven't read the message yet, so we're still subscribed
+        assert p.subscribed is True
+        assert wait_for_message(p, node=nodes[1]) == make_message(
+            "sunsubscribe", keys[1], 0
+        )
+        # now we're finally unsubscribed
+        assert p.subscribed is False
+
+    @skip_if_server_version_lt("7.0.0")
     def test_ignore_all_subscribe_messages(self, r):
         p = r.pubsub(ignore_subscribe_messages=True)
 
         checks = (
-            (p.subscribe, "foo"),
-            (p.unsubscribe, "foo"),
-            (p.psubscribe, "f*"),
-            (p.punsubscribe, "f*"),
+            (p.subscribe, "foo", p.get_message),
+            (p.unsubscribe, "foo", p.get_message),
+            (p.psubscribe, "f*", p.get_message),
+            (p.punsubscribe, "f*", p.get_message),
+            (p.ssubscribe, "foo", p.get_sharded_message),
+            (p.sunsubscribe, "foo", p.get_sharded_message),
         )
 
         assert p.subscribed is False
-        for func, channel in checks:
+        for func, channel, get_func in checks:
             assert func(channel) is None
             assert p.subscribed is True
-            assert wait_for_message(p) is None
+            assert wait_for_message(p, func=get_func) is None
         assert p.subscribed is False
 
+    @skip_if_server_version_lt("7.0.0")
     def test_ignore_individual_subscribe_messages(self, r):
         p = r.pubsub()
 
         checks = (
-            (p.subscribe, "foo"),
-            (p.unsubscribe, "foo"),
-            (p.psubscribe, "f*"),
-            (p.punsubscribe, "f*"),
+            (p.subscribe, "foo", p.get_message),
+            (p.unsubscribe, "foo", p.get_message),
+            (p.psubscribe, "f*", p.get_message),
+            (p.punsubscribe, "f*", p.get_message),
+            (p.ssubscribe, "foo", p.get_sharded_message),
+            (p.sunsubscribe, "foo", p.get_sharded_message),
         )
 
         assert p.subscribed is False
-        for func, channel in checks:
+        for func, channel, get_func in checks:
             assert func(channel) is None
             assert p.subscribed is True
-            message = wait_for_message(p, ignore_subscribe_messages=True)
+            message = wait_for_message(p, ignore_subscribe_messages=True, func=get_func)
             assert message is None
         assert p.subscribed is False
 
     def test_sub_unsub_resub_channels(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "channel")
         self._test_sub_unsub_resub(**kwargs)
 
     @pytest.mark.onlynoncluster
     def test_sub_unsub_resub_patterns(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "pattern")
         self._test_sub_unsub_resub(**kwargs)
 
+    @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_sub_unsub_resub_shard_channels(self, r):
+        kwargs = make_subscribe_test_data(r.pubsub(), "shard_channel")
+        self._test_sub_unsub_resub(**kwargs)
+
     def _test_sub_unsub_resub(
         self, p, sub_type, unsub_type, sub_func, unsub_func, keys
     ):
         # https://github.com/andymccurdy/redis-py/issues/764
         key = keys[0]
         sub_func(key)
         unsub_func(key)
         sub_func(key)
         assert p.subscribed is True
         assert wait_for_message(p) == make_message(sub_type, key, 1)
         assert wait_for_message(p) == make_message(unsub_type, key, 0)
         assert wait_for_message(p) == make_message(sub_type, key, 1)
         assert p.subscribed is True
 
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_sub_unsub_resub_shard_channels_cluster(self, r):
+        p = r.pubsub()
+        key = "foo"
+        p.ssubscribe(key)
+        p.sunsubscribe(key)
+        p.ssubscribe(key)
+        assert p.subscribed is True
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "ssubscribe", key, 1
+        )
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "sunsubscribe", key, 0
+        )
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "ssubscribe", key, 1
+        )
+        assert p.subscribed is True
+
     def test_sub_unsub_all_resub_channels(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "channel")
         self._test_sub_unsub_all_resub(**kwargs)
 
     def test_sub_unsub_all_resub_patterns(self, r):
         kwargs = make_subscribe_test_data(r.pubsub(), "pattern")
         self._test_sub_unsub_all_resub(**kwargs)
 
+    @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_sub_unsub_all_resub_shard_channels(self, r):
+        kwargs = make_subscribe_test_data(r.pubsub(), "shard_channel")
+        self._test_sub_unsub_all_resub(**kwargs)
+
     def _test_sub_unsub_all_resub(
         self, p, sub_type, unsub_type, sub_func, unsub_func, keys
     ):
         # https://github.com/andymccurdy/redis-py/issues/764
         key = keys[0]
         sub_func(key)
         unsub_func()
         sub_func(key)
         assert p.subscribed is True
         assert wait_for_message(p) == make_message(sub_type, key, 1)
         assert wait_for_message(p) == make_message(unsub_type, key, 0)
         assert wait_for_message(p) == make_message(sub_type, key, 1)
         assert p.subscribed is True
 
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_sub_unsub_all_resub_shard_channels_cluster(self, r):
+        p = r.pubsub()
+        key = "foo"
+        p.ssubscribe(key)
+        p.sunsubscribe()
+        p.ssubscribe(key)
+        assert p.subscribed is True
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "ssubscribe", key, 1
+        )
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "sunsubscribe", key, 0
+        )
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "ssubscribe", key, 1
+        )
+        assert p.subscribed is True
+
 
 class TestPubSubMessages:
     def setup_method(self, method):
         self.message = None
 
     def message_handler(self, message):
         self.message = message
@@ -286,14 +474,40 @@
         assert wait_for_message(p) == make_message("subscribe", "foo", 1)
         assert r.publish("foo", "test message") == 1
 
         message = wait_for_message(p)
         assert isinstance(message, dict)
         assert message == make_message("message", "foo", "test message")
 
+    @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_published_message_to_shard_channel(self, r):
+        p = r.pubsub()
+        p.ssubscribe("foo")
+        assert wait_for_message(p) == make_message("ssubscribe", "foo", 1)
+        assert r.spublish("foo", "test message") == 1
+
+        message = wait_for_message(p)
+        assert isinstance(message, dict)
+        assert message == make_message("smessage", "foo", "test message")
+
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_published_message_to_shard_channel_cluster(self, r):
+        p = r.pubsub()
+        p.ssubscribe("foo")
+        assert wait_for_message(p, func=p.get_sharded_message) == make_message(
+            "ssubscribe", "foo", 1
+        )
+        assert r.spublish("foo", "test message") == 1
+
+        message = wait_for_message(p, func=p.get_sharded_message)
+        assert isinstance(message, dict)
+        assert message == make_message("smessage", "foo", "test message")
+
     def test_published_message_to_pattern(self, r):
         p = r.pubsub()
         p.subscribe("foo")
         p.psubscribe("f*")
         assert wait_for_message(p) == make_message("subscribe", "foo", 1)
         assert wait_for_message(p) == make_message("psubscribe", "f*", 2)
         # 1 to pattern, 1 to channel
@@ -317,14 +531,23 @@
         p = r.pubsub(ignore_subscribe_messages=True)
         p.subscribe(foo=self.message_handler)
         assert wait_for_message(p) is None
         assert r.publish("foo", "test message") == 1
         assert wait_for_message(p) is None
         assert self.message == make_message("message", "foo", "test message")
 
+    @skip_if_server_version_lt("7.0.0")
+    def test_shard_channel_message_handler(self, r):
+        p = r.pubsub(ignore_subscribe_messages=True)
+        p.ssubscribe(foo=self.message_handler)
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert r.spublish("foo", "test message") == 1
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert self.message == make_message("smessage", "foo", "test message")
+
     @pytest.mark.onlynoncluster
     def test_pattern_message_handler(self, r):
         p = r.pubsub(ignore_subscribe_messages=True)
         p.psubscribe(**{"f*": self.message_handler})
         assert wait_for_message(p) is None
         assert r.publish("foo", "test message") == 1
         assert wait_for_message(p) is None
@@ -338,14 +561,25 @@
         channels = {channel: self.message_handler}
         p.subscribe(**channels)
         assert wait_for_message(p) is None
         assert r.publish(channel, "test message") == 1
         assert wait_for_message(p) is None
         assert self.message == make_message("message", channel, "test message")
 
+    @skip_if_server_version_lt("7.0.0")
+    def test_unicode_shard_channel_message_handler(self, r):
+        p = r.pubsub(ignore_subscribe_messages=True)
+        channel = "uni" + chr(4456) + "code"
+        channels = {channel: self.message_handler}
+        p.ssubscribe(**channels)
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert r.spublish(channel, "test message") == 1
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert self.message == make_message("smessage", channel, "test message")
+
     @pytest.mark.onlynoncluster
     # see: https://redis-py-cluster.readthedocs.io/en/stable/pubsub.html
     # #known-limitations-with-pubsub
     def test_unicode_pattern_message_handler(self, r):
         p = r.pubsub(ignore_subscribe_messages=True)
         pattern = "uni" + chr(4456) + "*"
         channel = "uni" + chr(4456) + "code"
@@ -407,14 +641,27 @@
         p = r.pubsub()
         p.psubscribe(self.pattern)
         assert wait_for_message(p) == self.make_message("psubscribe", self.pattern, 1)
 
         p.punsubscribe(self.pattern)
         assert wait_for_message(p) == self.make_message("punsubscribe", self.pattern, 0)
 
+    @skip_if_server_version_lt("7.0.0")
+    def test_shard_channel_subscribe_unsubscribe(self, r):
+        p = r.pubsub()
+        p.ssubscribe(self.channel)
+        assert wait_for_message(p, func=p.get_sharded_message) == self.make_message(
+            "ssubscribe", self.channel, 1
+        )
+
+        p.sunsubscribe(self.channel)
+        assert wait_for_message(p, func=p.get_sharded_message) == self.make_message(
+            "sunsubscribe", self.channel, 0
+        )
+
     def test_channel_publish(self, r):
         p = r.pubsub()
         p.subscribe(self.channel)
         assert wait_for_message(p) == self.make_message("subscribe", self.channel, 1)
         r.publish(self.channel, self.data)
         assert wait_for_message(p) == self.make_message(
             "message", self.channel, self.data
@@ -426,14 +673,26 @@
         p.psubscribe(self.pattern)
         assert wait_for_message(p) == self.make_message("psubscribe", self.pattern, 1)
         r.publish(self.channel, self.data)
         assert wait_for_message(p) == self.make_message(
             "pmessage", self.channel, self.data, pattern=self.pattern
         )
 
+    @skip_if_server_version_lt("7.0.0")
+    def test_shard_channel_publish(self, r):
+        p = r.pubsub()
+        p.ssubscribe(self.channel)
+        assert wait_for_message(p, func=p.get_sharded_message) == self.make_message(
+            "ssubscribe", self.channel, 1
+        )
+        r.spublish(self.channel, self.data)
+        assert wait_for_message(p, func=p.get_sharded_message) == self.make_message(
+            "smessage", self.channel, self.data
+        )
+
     def test_channel_message_handler(self, r):
         p = r.pubsub(ignore_subscribe_messages=True)
         p.subscribe(**{self.channel: self.message_handler})
         assert wait_for_message(p) is None
         r.publish(self.channel, self.data)
         assert wait_for_message(p) is None
         assert self.message == self.make_message("message", self.channel, self.data)
@@ -464,14 +723,38 @@
         new_data = self.data + "new data"
         r.publish(self.channel, new_data)
         assert wait_for_message(p) is None
         assert self.message == self.make_message(
             "pmessage", self.channel, new_data, pattern=self.pattern
         )
 
+    @skip_if_server_version_lt("7.0.0")
+    def test_shard_channel_message_handler(self, r):
+        p = r.pubsub(ignore_subscribe_messages=True)
+        p.ssubscribe(**{self.channel: self.message_handler})
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        r.spublish(self.channel, self.data)
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert self.message == self.make_message("smessage", self.channel, self.data)
+
+        # test that we reconnected to the correct channel
+        self.message = None
+        try:
+            # cluster mode
+            p.disconnect()
+        except AttributeError:
+            # standalone mode
+            p.connection.disconnect()
+        # should reconnect
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        new_data = self.data + "new data"
+        r.spublish(self.channel, new_data)
+        assert wait_for_message(p, func=p.get_sharded_message) is None
+        assert self.message == self.make_message("smessage", self.channel, new_data)
+
     def test_context_manager(self, r):
         with r.pubsub() as pubsub:
             pubsub.subscribe("foo")
             assert pubsub.connection is not None
 
         assert pubsub.connection is None
         assert pubsub.channels == {}
@@ -494,14 +777,46 @@
         p.subscribe("foo", "bar", "baz", "quux")
         for i in range(4):
             assert wait_for_message(p)["type"] == "subscribe"
         expected = [b"bar", b"baz", b"foo", b"quux"]
         assert all([channel in r.pubsub_channels() for channel in expected])
 
     @pytest.mark.onlynoncluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_pubsub_shardchannels(self, r):
+        p = r.pubsub()
+        p.ssubscribe("foo", "bar", "baz", "quux")
+        for i in range(4):
+            assert wait_for_message(p)["type"] == "ssubscribe"
+        expected = [b"bar", b"baz", b"foo", b"quux"]
+        assert all([channel in r.pubsub_shardchannels() for channel in expected])
+
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_pubsub_shardchannels_cluster(self, r):
+        channels = {
+            b"foo": r.get_node_from_key("foo"),
+            b"bar": r.get_node_from_key("bar"),
+            b"baz": r.get_node_from_key("baz"),
+            b"quux": r.get_node_from_key("quux"),
+        }
+        p = r.pubsub()
+        p.ssubscribe("foo", "bar", "baz", "quux")
+        for node in channels.values():
+            assert wait_for_message(p, node=node)["type"] == "ssubscribe"
+        for channel, node in channels.items():
+            assert channel in r.pubsub_shardchannels(target_nodes=node)
+        assert all(
+            [
+                channel in r.pubsub_shardchannels(target_nodes="all")
+                for channel in channels.keys()
+            ]
+        )
+
+    @pytest.mark.onlynoncluster
     @skip_if_server_version_lt("2.8.0")
     def test_pubsub_numsub(self, r):
         p1 = r.pubsub()
         p1.subscribe("foo", "bar", "baz")
         for i in range(3):
             assert wait_for_message(p1)["type"] == "subscribe"
         p2 = r.pubsub()
@@ -519,14 +834,40 @@
     def test_pubsub_numpat(self, r):
         p = r.pubsub()
         p.psubscribe("*oo", "*ar", "b*z")
         for i in range(3):
             assert wait_for_message(p)["type"] == "psubscribe"
         assert r.pubsub_numpat() == 3
 
+    @pytest.mark.onlycluster
+    @skip_if_server_version_lt("7.0.0")
+    def test_pubsub_shardnumsub(self, r):
+        channels = {
+            b"foo": r.get_node_from_key("foo"),
+            b"bar": r.get_node_from_key("bar"),
+            b"baz": r.get_node_from_key("baz"),
+        }
+        p1 = r.pubsub()
+        p1.ssubscribe(*channels.keys())
+        for node in channels.values():
+            assert wait_for_message(p1, node=node)["type"] == "ssubscribe"
+        p2 = r.pubsub()
+        p2.ssubscribe("bar", "baz")
+        for i in range(2):
+            assert (
+                wait_for_message(p2, func=p2.get_sharded_message)["type"]
+                == "ssubscribe"
+            )
+        p3 = r.pubsub()
+        p3.ssubscribe("baz")
+        assert wait_for_message(p3, node=channels[b"baz"])["type"] == "ssubscribe"
+
+        channels = [(b"foo", 1), (b"bar", 2), (b"baz", 3)]
+        assert r.pubsub_shardnumsub("foo", "bar", "baz", target_nodes="all") == channels
+
 
 class TestPubSubPings:
     @skip_if_server_version_lt("3.0.0")
     def test_send_pubsub_ping(self, r):
         p = r.pubsub(ignore_subscribe_messages=True)
         p.subscribe("foo")
         p.ping()
```

### Comparing `redis-5.0.0b3/tests/test_retry.py` & `redis-5.0.0b4/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_scripting.py` & `redis-5.0.0b4/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_search.py` & `redis-5.0.0b4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_sentinel.py` & `redis-5.0.0b4/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_ssl.py` & `redis-5.0.0b4/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/test_timeseries.py` & `redis-5.0.0b4/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/testdata/jsontestdata.py` & `redis-5.0.0b4/tests/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/testdata/titles.csv` & `redis-5.0.0b4/tests/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b3/tests/testdata/will_play_text.csv.bz2` & `redis-5.0.0b4/tests/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

