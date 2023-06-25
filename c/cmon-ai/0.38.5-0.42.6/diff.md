# Comparing `tmp/cmon-ai-0.38.5.tar.gz` & `tmp/cmon-ai-0.42.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmon-ai-0.38.5.tar", last modified: Fri Jun 23 16:21:16 2023, max compression
+gzip compressed data, was "cmon-ai-0.42.6.tar", last modified: Sun Jun 25 16:25:47 2023, max compression
```

## Comparing `cmon-ai-0.38.5.tar` & `cmon-ai-0.42.6.tar`

### file list

```diff
@@ -1,309 +1,831 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.032247 cmon-ai-0.38.5/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10826 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/LICENSE
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      218 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/MANIFEST.in
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15821 2023-06-23 16:21:16.032247 cmon-ai-0.38.5/PKG-INFO
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13830 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.992244 cmon-ai-0.38.5/cmon/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4701 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       69 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/__main__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      219 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/_docarray.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2794 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/checker.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/clients/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8347 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/clients/base/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7093 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11942 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    14582 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10197 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/http.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3760 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/retry.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2110 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/stream_rpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4227 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/unary_rpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9794 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/base/websocket.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2331 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2714 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2468 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/http.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    22535 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/mixin.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/clients/request/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3036 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/request/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2749 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/request/asyncio.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2748 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/request/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2443 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/clients/websocket.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2425 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/constants.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7782 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/enums.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5943 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/excepts.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2587 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/exporter.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    47518 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5996 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/importer.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/jaml/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    31248 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9313 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/jaml/parsers/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3249 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3169 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/base.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/jaml/parsers/deployment/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/deployment/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1922 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/deployment/legacy.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/jaml/parsers/executor/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/executor/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4515 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/executor/legacy.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.996244 cmon-ai-0.38.5/cmon/jaml/parsers/flow/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/flow/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6377 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/flow/v1.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.000244 cmon-ai-0.38.5/cmon/jaml/parsers/gateway/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/gateway/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2508 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/jaml/parsers/gateway/legacy.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.000244 cmon-ai-0.38.5/cmon/logging/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/logging/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2356 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/logging/formatter.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8318 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/logging/logger.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      113 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/logging/predefined.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8843 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/logging/profile.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.000244 cmon-ai-0.38.5/cmon/orchestrate/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.000244 cmon-ai-0.38.5/cmon/orchestrate/deployments/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    82370 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.000244 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    17751 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/docker_compose.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4560 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    15133 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8s.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.000244 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8slib/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8slib/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10662 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2914 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6916 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/deployments/install_requirements_helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.004245 cmon-ai-0.38.5/cmon/orchestrate/flow/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/flow/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2175 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/flow/asyncio.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)   145860 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/flow/base.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1704 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/flow/builder.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1144 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1800 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/orchestrator.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.004245 cmon-ai-0.38.5/cmon/orchestrate/pods/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12955 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/pods/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16580 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/pods/container.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2321 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/pods/container_helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1480 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/pods/factory.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2673 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/orchestrate/pods/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.004245 cmon-ai-0.38.5/cmon/parsers/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9433 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1322 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/base.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2520 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/client.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      574 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/create.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1108 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/deprecated.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3983 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/export.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1970 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/flow.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12817 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      505 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/logging.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.004245 cmon-ai-0.38.5/cmon/parsers/orchestrate/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5052 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/base.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2482 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/deployment.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9857 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/pod.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3439 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/container.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      710 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/grpc_channel.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1228 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/head.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9107 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/remote.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1209 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/runtime.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4276 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/worker.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1489 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/parsers/ping.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      227 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      457 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      477 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/docarray_v1/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9127 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb2/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb2/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16512 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb2/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/docarray_v2/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9118 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.008245 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb2/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb2/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    16503 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb2/cmon_pb2.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    23919 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6906 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/proto/serializer.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.012246 cmon-ai-0.38.5/cmon/resources/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2327 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/Python.gitignore
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4170 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/ci-vendors.json
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3922 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/cmon.logo
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.012246 cmon-ai-0.38.5/cmon/resources/completions/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      567 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/completions/cmon.bash
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      663 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/completions/cmon.fish
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      425 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/completions/cmon.zsh
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3645 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/extra-requirements.txt
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.012246 cmon-ai-0.38.5/cmon/resources/health_check/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/health_check/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1500 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/health_check/gateway.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      672 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/health_check/pod.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.988243 cmon-ai-0.38.5/cmon/resources/k8s/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/resources/k8s/template/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      141 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/configmap.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2053 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-executor.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2061 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-gateway.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3357 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-uses-after.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4801 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-uses-before-after.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3367 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-uses-before.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      103 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/namespace.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      245 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/service.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      281 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/service_monitor.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      354 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/service_monitoring.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2459 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/k8s/template/statefulset-executor.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      886 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/logging.default.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      654 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/logging.docker.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      174 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/logging.json.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      431 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/logging.profile.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      673 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/logging.quiet.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      517 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/logging.remote.yml
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:15.988243 cmon-ai-0.38.5/cmon/resources/project-template/
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/resources/project-template/deployment/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      176 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/deployment/client.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      120 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/deployment/deployment.yml
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/resources/project-template/deployment/executor1/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       45 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/deployment/executor1/config.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      225 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/deployment/executor1/executor.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/deployment/executor1/requirements.txt
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/resources/project-template/flow/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      176 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/flow/client.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/resources/project-template/flow/executor1/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       45 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/flow/executor1/config.yml
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      225 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/flow/executor1/executor.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/flow/executor1/requirements.txt
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      163 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/resources/project-template/flow/flow.yml
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/schemas/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1111 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1057 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/deployment.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      111 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/executor.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1583 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/flow.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      320 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/gateway.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1639 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2415 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/schemas/meta.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.016246 cmon-ai-0.38.5/cmon/serve/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/consensus/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2737 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/README.md
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2814 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/add_voter.go
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/consensus/cmon-go-proto/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    68606 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon-go-proto/cmon.pb.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    36116 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8324 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon.proto
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3053 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/cmonraft.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      784 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/executor_connection.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11122 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/fsm.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4737 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/rpc.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3521 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/snapshot.go
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/consensus/docarray-go-proto/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    42221 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/docarray-go-proto/docarray.pb.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2433 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/docarray.proto
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1004 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/go.mod
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    28154 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/go.sum
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2323 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/jraft.go
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2465 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/jraft.h
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    18360 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/run.go
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/consensus/scripts/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      641 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/scripts/fetch-protos.sh
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1313 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/consensus/scripts/protogen.sh
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/executors/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    51163 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/executors/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    20358 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/executors/decorators.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      928 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/executors/metas.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8398 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/executors/run.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6080 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.020246 cmon-ai-0.38.5/cmon/serve/instrumentation/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6869 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/instrumentation/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1739 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/monitoring.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/networking/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    24332 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7628 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/connection_pool_map.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9399 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/connection_stub.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3094 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/instrumentation.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10258 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/replica_list.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13447 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/sse.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10504 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/networking/utils.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/runtimes/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13845 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/asyncio.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10614 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/async_request_response_handling.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/composite/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      340 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/composite/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1650 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/gateway.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/graph/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/graph/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    32568 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/graph/topology_graph.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/grpc/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      306 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/grpc/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      732 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/health_model.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.024247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      416 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http/__init__.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http/fastapi/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      347 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http/fastapi/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    17411 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http_fastapi_app.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9476 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/load_balancer/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      290 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/load_balancer/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    10232 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/models.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    11182 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/request_handling.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    20367 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/streamer.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/websocket/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      339 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/websocket/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    12485 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/gateway/websocket_fastapi_app.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/runtimes/head/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/head/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    24494 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/head/request_handling.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     7742 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/helper.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9296 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/monitoring.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/runtimes/servers/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9783 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/servers/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3377 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/servers/composite.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8269 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/servers/grpc.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     9857 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/servers/http.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2255 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/servers/load_balancer.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4983 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/servers/websocket.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/runtimes/worker/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/worker/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6088 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/worker/batch_queue.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     6837 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/worker/http_fastapi_app.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    48714 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/runtimes/worker/request_handling.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/serve/stream/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13720 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/stream/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3505 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/serve/stream/helper.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/types/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/types/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3814 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/types/mixin.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.028247 cmon-ai-0.38.5/cmon/types/request/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     1631 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/types/request/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    14425 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/types/request/data.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     2189 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon/types/request/status.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.032247 cmon-ai-0.38.5/cmon_ai.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)    15821 2023-06-23 16:21:15.000000 cmon-ai-0.38.5/cmon_ai.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8522 2023-06-23 16:21:15.000000 cmon-ai-0.38.5/cmon_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 16:21:15.000000 cmon-ai-0.38.5/cmon_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       39 2023-06-23 16:21:15.000000 cmon-ai-0.38.5/cmon_ai.egg-info/entry_points.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-06-23 12:32:29.000000 cmon-ai-0.38.5/cmon_ai.egg-info/not-zip-safe
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       20 2023-06-23 16:21:15.000000 cmon-ai-0.38.5/cmon_ai.egg-info/top_level.txt
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-06-23 16:21:16.032247 cmon-ai-0.38.5/cmon_cli/
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4210 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon_cli/__init__.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     5173 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon_cli/api.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)    13006 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon_cli/autocomplete.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4165 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon_cli/export.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)      193 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon_cli/known_plugins.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4719 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/cmon_cli/lookup.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     3047 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/extra-requirements.txt
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     4095 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/fastentrypoints.py
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)       96 2023-06-23 09:57:47.000000 cmon-ai-0.38.5/pyproject.toml
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-06-23 16:21:16.032247 cmon-ai-0.38.5/setup.cfg
--rwxr-xr-x   0 lenovo    (1000) lenovo    (1000)     8295 2023-06-23 16:20:36.000000 cmon-ai-0.38.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.607296 cmon-ai-0.42.6/
+-rw-rw-rw-   0        0        0    10826 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/LICENSE
+-rw-rw-rw-   0        0        0      218 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    16300 2023-06-25 16:25:47.606306 cmon-ai-0.42.6/PKG-INFO
+-rw-rw-rw-   0        0        0    14262 2023-06-25 16:05:53.000000 cmon-ai-0.42.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.045274 cmon-ai-0.42.6/cmon/
+-rw-rw-rw-   0        0        0     4701 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/__main__.py
+-rw-rw-rw-   0        0        0      219 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/_docarray.py
+-rw-rw-rw-   0        0        0     2794 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.050280 cmon-ai-0.42.6/cmon/clients/
+-rw-rw-rw-   0        0        0     8347 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.058283 cmon-ai-0.42.6/cmon/clients/base/
+-rw-rw-rw-   0        0        0     7093 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/base/__init__.py
+-rw-rw-rw-   0        0        0    11942 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/base/grpc.py
+-rw-rw-rw-   0        0        0    14582 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/base/helper.py
+-rw-rw-rw-   0        0        0    10197 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/clients/base/http.py
+-rw-rw-rw-   0        0        0     3760 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/base/retry.py
+-rw-rw-rw-   0        0        0     2110 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/base/stream_rpc.py
+-rw-rw-rw-   0        0        0     4227 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/base/unary_rpc.py
+-rw-rw-rw-   0        0        0     9794 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/base/websocket.py
+-rw-rw-rw-   0        0        0     2331 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/grpc.py
+-rw-rw-rw-   0        0        0     2714 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/helper.py
+-rw-rw-rw-   0        0        0     2468 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/http.py
+-rw-rw-rw-   0        0        0    22535 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.061279 cmon-ai-0.42.6/cmon/clients/request/
+-rw-rw-rw-   0        0        0     3036 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/clients/request/__init__.py
+-rw-rw-rw-   0        0        0     2749 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/clients/request/asyncio.py
+-rw-rw-rw-   0        0        0     2748 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/request/helper.py
+-rw-rw-rw-   0        0        0     2443 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/clients/websocket.py
+-rw-rw-rw-   0        0        0     2425 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/constants.py
+-rw-rw-rw-   0        0        0     7782 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/enums.py
+-rw-rw-rw-   0        0        0     5943 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/excepts.py
+-rw-rw-rw-   0        0        0     2587 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/exporter.py
+-rw-rw-rw-   0        0        0    47518 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/helper.py
+-rw-rw-rw-   0        0        0     5996 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.062277 cmon-ai-0.42.6/cmon/jaml/
+-rw-rw-rw-   0        0        0    31248 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/__init__.py
+-rw-rw-rw-   0        0        0     9313 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.063780 cmon-ai-0.42.6/cmon/jaml/parsers/
+-rw-rw-rw-   0        0        0     3249 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/__init__.py
+-rw-rw-rw-   0        0        0     3169 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/base.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.065791 cmon-ai-0.42.6/cmon/jaml/parsers/deployment/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/deployment/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/deployment/legacy.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.067796 cmon-ai-0.42.6/cmon/jaml/parsers/executor/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/executor/__init__.py
+-rw-rw-rw-   0        0        0     4515 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/executor/legacy.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.068788 cmon-ai-0.42.6/cmon/jaml/parsers/flow/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/flow/__init__.py
+-rw-rw-rw-   0        0        0     6377 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/flow/v1.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.070786 cmon-ai-0.42.6/cmon/jaml/parsers/gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/gateway/__init__.py
+-rw-rw-rw-   0        0        0     2508 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/jaml/parsers/gateway/legacy.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.074786 cmon-ai-0.42.6/cmon/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/logging/__init__.py
+-rw-rw-rw-   0        0        0     2356 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/logging/formatter.py
+-rw-rw-rw-   0        0        0     8318 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/logging/logger.py
+-rw-rw-rw-   0        0        0      113 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/logging/predefined.py
+-rw-rw-rw-   0        0        0     8843 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/logging/profile.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.077784 cmon-ai-0.42.6/cmon/orchestrate/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.079795 cmon-ai-0.42.6/cmon/orchestrate/deployments/
+-rw-rw-rw-   0        0        0    82370 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.083786 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/__init__.py
+-rw-rw-rw-   0        0        0    17751 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/docker_compose.py
+-rw-rw-rw-   0        0        0     4560 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/helper.py
+-rw-rw-rw-   0        0        0    15133 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8s.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.085785 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8slib/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8slib/__init__.py
+-rw-rw-rw-   0        0        0    10662 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py
+-rw-rw-rw-   0        0        0     2914 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py
+-rw-rw-rw-   0        0        0     6916 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/deployments/install_requirements_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.089786 cmon-ai-0.42.6/cmon/orchestrate/flow/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/flow/__init__.py
+-rw-rw-rw-   0        0        0     2175 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/flow/asyncio.py
+-rw-rw-rw-   0        0        0   145860 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/orchestrate/flow/base.py
+-rw-rw-rw-   0        0        0     1704 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/flow/builder.py
+-rw-rw-rw-   0        0        0     1144 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/helper.py
+-rw-rw-rw-   0        0        0     1800 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/orchestrator.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.093787 cmon-ai-0.42.6/cmon/orchestrate/pods/
+-rw-rw-rw-   0        0        0    12955 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/pods/__init__.py
+-rw-rw-rw-   0        0        0    16580 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/pods/container.py
+-rw-rw-rw-   0        0        0     2321 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/pods/container_helper.py
+-rw-rw-rw-   0        0        0     1480 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/pods/factory.py
+-rw-rw-rw-   0        0        0     2673 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/orchestrate/pods/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.103786 cmon-ai-0.42.6/cmon/parsers/
+-rw-rw-rw-   0        0        0     9433 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/cmon/parsers/base.py
+-rw-rw-rw-   0        0        0     2520 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/client.py
+-rw-rw-rw-   0        0        0      574 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/create.py
+-rw-rw-rw-   0        0        0     1108 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/deprecated.py
+-rw-rw-rw-   0        0        0     3983 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/export.py
+-rw-rw-rw-   0        0        0     1970 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/flow.py
+-rw-rw-rw-   0        0        0    12817 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/helper.py
+-rw-rw-rw-   0        0        0      505 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/logging.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.107786 cmon-ai-0.42.6/cmon/parsers/orchestrate/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/__init__.py
+-rw-rw-rw-   0        0        0     5052 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/base.py
+-rw-rw-rw-   0        0        0     2482 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/deployment.py
+-rw-rw-rw-   0        0        0     9857 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/pod.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.113792 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/__init__.py
+-rw-rw-rw-   0        0        0     3439 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/container.py
+-rw-rw-rw-   0        0        0      710 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/grpc_channel.py
+-rw-rw-rw-   0        0        0     1228 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/head.py
+-rw-rw-rw-   0        0        0     9107 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/remote.py
+-rw-rw-rw-   0        0        0     1209 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/runtime.py
+-rw-rw-rw-   0        0        0     4276 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/worker.py
+-rw-rw-rw-   0        0        0     1489 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/parsers/ping.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.117785 cmon-ai-0.42.6/cmon/proto/
+-rw-rw-rw-   0        0        0      227 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/__init__.py
+-rw-rw-rw-   0        0        0      457 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/proto/cmon_pb2.py
+-rw-rw-rw-   0        0        0      477 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/proto/cmon_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.118788 cmon-ai-0.42.6/cmon/proto/docarray_v1/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.121785 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb/__init__.py
+-rw-rw-rw-   0        0        0     9127 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb/cmon_pb2.py
+-rw-rw-rw-   0        0        0    23919 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.124786 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb2/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb2/__init__.py
+-rw-rw-rw-   0        0        0    16512 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb2/cmon_pb2.py
+-rw-rw-rw-   0        0        0    23919 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.125790 cmon-ai-0.42.6/cmon/proto/docarray_v2/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.127787 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb/__init__.py
+-rw-rw-rw-   0        0        0     9118 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb/cmon_pb2.py
+-rw-rw-rw-   0        0        0    23919 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.130787 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb2/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb2/__init__.py
+-rw-rw-rw-   0        0        0    16503 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb2/cmon_pb2.py
+-rw-rw-rw-   0        0        0    23919 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6906 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/proto/serializer.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.139791 cmon-ai-0.42.6/cmon/resources/
+-rw-rw-rw-   0        0        0     2327 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/Python.gitignore
+-rw-rw-rw-   0        0        0     4170 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/ci-vendors.json
+-rw-rw-rw-   0        0        0      774 2023-06-25 16:01:56.000000 cmon-ai-0.42.6/cmon/resources/cmon.logo
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.142786 cmon-ai-0.42.6/cmon/resources/completions/
+-rw-rw-rw-   0        0        0      567 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/completions/cmon.bash
+-rw-rw-rw-   0        0        0      663 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/completions/cmon.fish
+-rw-rw-rw-   0        0        0      425 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/completions/cmon.zsh
+-rw-rw-rw-   0        0        0     3645 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/resources/extra-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.145787 cmon-ai-0.42.6/cmon/resources/health_check/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/health_check/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/health_check/gateway.py
+-rw-rw-rw-   0        0        0      672 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/health_check/pod.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:46.974272 cmon-ai-0.42.6/cmon/resources/k8s/
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.155810 cmon-ai-0.42.6/cmon/resources/k8s/template/
+-rw-rw-rw-   0        0        0      141 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/configmap.yml
+-rw-rw-rw-   0        0        0     2053 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-executor.yml
+-rw-rw-rw-   0        0        0     2061 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-gateway.yml
+-rw-rw-rw-   0        0        0     3357 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-uses-after.yml
+-rw-rw-rw-   0        0        0     4801 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-uses-before-after.yml
+-rw-rw-rw-   0        0        0     3367 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-uses-before.yml
+-rw-rw-rw-   0        0        0      103 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/namespace.yml
+-rw-rw-rw-   0        0        0      245 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/service.yml
+-rw-rw-rw-   0        0        0      281 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/service_monitor.yml
+-rw-rw-rw-   0        0        0      354 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/service_monitoring.yml
+-rw-rw-rw-   0        0        0     2459 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/k8s/template/statefulset-executor.yml
+-rw-rw-rw-   0        0        0      886 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/logging.default.yml
+-rw-rw-rw-   0        0        0      654 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/logging.docker.yml
+-rw-rw-rw-   0        0        0      174 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/logging.json.yml
+-rw-rw-rw-   0        0        0      431 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/logging.profile.yml
+-rw-rw-rw-   0        0        0      673 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/logging.quiet.yml
+-rw-rw-rw-   0        0        0      517 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/logging.remote.yml
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:46.975272 cmon-ai-0.42.6/cmon/resources/project-template/
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.156802 cmon-ai-0.42.6/cmon/resources/project-template/deployment/
+-rw-rw-rw-   0        0        0      176 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/deployment/client.py
+-rw-rw-rw-   0        0        0      120 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/deployment/deployment.yml
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.159803 cmon-ai-0.42.6/cmon/resources/project-template/deployment/executor1/
+-rw-rw-rw-   0        0        0       45 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/deployment/executor1/config.yml
+-rw-rw-rw-   0        0        0      225 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/deployment/executor1/executor.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/deployment/executor1/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.161813 cmon-ai-0.42.6/cmon/resources/project-template/flow/
+-rw-rw-rw-   0        0        0      176 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/flow/client.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.164309 cmon-ai-0.42.6/cmon/resources/project-template/flow/executor1/
+-rw-rw-rw-   0        0        0       45 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/flow/executor1/config.yml
+-rw-rw-rw-   0        0        0      225 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/flow/executor1/executor.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/flow/executor1/requirements.txt
+-rw-rw-rw-   0        0        0      163 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/resources/project-template/flow/flow.yml
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.170314 cmon-ai-0.42.6/cmon/schemas/
+-rw-rw-rw-   0        0        0     1111 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/cmon/schemas/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/schemas/deployment.py
+-rw-rw-rw-   0        0        0      111 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/schemas/executor.py
+-rw-rw-rw-   0        0        0     1583 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/schemas/flow.py
+-rw-rw-rw-   0        0        0      320 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/schemas/gateway.py
+-rw-rw-rw-   0        0        0     1639 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/schemas/helper.py
+-rw-rw-rw-   0        0        0     2415 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/schemas/meta.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.172323 cmon-ai-0.42.6/cmon/serve/
+-rw-rw-rw-   0        0        0        1 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.180318 cmon-ai-0.42.6/cmon/serve/consensus/
+-rw-rw-rw-   0        0        0     2737 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/README.md
+-rw-rw-rw-   0        0        0     2814 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/add_voter.go
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.182319 cmon-ai-0.42.6/cmon/serve/consensus/cmon-go-proto/
+-rw-rw-rw-   0        0        0    68606 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon-go-proto/cmon.pb.go
+-rw-rw-rw-   0        0        0    36116 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go
+-rw-rw-rw-   0        0        0     8324 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon.proto
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.187315 cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/
+-rw-rw-rw-   0        0        0     3053 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/cmonraft.go
+-rw-rw-rw-   0        0        0      784 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/executor_connection.go
+-rw-rw-rw-   0        0        0    11122 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/fsm.go
+-rw-rw-rw-   0        0        0     4737 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/rpc.go
+-rw-rw-rw-   0        0        0     3521 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/snapshot.go
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.188315 cmon-ai-0.42.6/cmon/serve/consensus/docarray-go-proto/
+-rw-rw-rw-   0        0        0    42221 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/docarray-go-proto/docarray.pb.go
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.189314 cmon-ai-0.42.6/cmon/serve/consensus/docarray-go-proto (2)/
+-rw-rw-rw-   0        0        0    42221 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/docarray-go-proto (2)/docarray.pb.go
+-rw-rw-rw-   0        0        0     2433 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/docarray.proto
+-rw-rw-rw-   0        0        0     1004 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/go.mod
+-rw-rw-rw-   0        0        0    28154 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/go.sum
+-rw-rw-rw-   0        0        0     2323 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/jraft.go
+-rw-rw-rw-   0        0        0     2465 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/jraft.h
+-rw-rw-rw-   0        0        0    18360 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/consensus/run.go
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.190322 cmon-ai-0.42.6/cmon/serve/consensus/scripts/
+-rw-rw-rw-   0        0        0      641 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/scripts/fetch-protos.sh
+-rw-rw-rw-   0        0        0     1313 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/consensus/scripts/protogen.sh
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.195325 cmon-ai-0.42.6/cmon/serve/executors/
+-rw-rw-rw-   0        0        0    51163 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/executors/__init__.py
+-rw-rw-rw-   0        0        0    20358 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/executors/decorators.py
+-rw-rw-rw-   0        0        0      928 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/executors/metas.py
+-rw-rw-rw-   0        0        0     8398 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/executors/run.py
+-rw-rw-rw-   0        0        0     6080 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.196325 cmon-ai-0.42.6/cmon/serve/instrumentation/
+-rw-rw-rw-   0        0        0     6869 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/instrumentation/__init__.py
+-rw-rw-rw-   0        0        0     1739 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/monitoring.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.203323 cmon-ai-0.42.6/cmon/serve/networking/
+-rw-rw-rw-   0        0        0    24332 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/__init__.py
+-rw-rw-rw-   0        0        0     7628 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/connection_pool_map.py
+-rw-rw-rw-   0        0        0     9399 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/connection_stub.py
+-rw-rw-rw-   0        0        0     3094 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/instrumentation.py
+-rw-rw-rw-   0        0        0    10258 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/replica_list.py
+-rw-rw-rw-   0        0        0    13447 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/sse.py
+-rw-rw-rw-   0        0        0    10504 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/networking/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.206315 cmon-ai-0.42.6/cmon/serve/runtimes/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/__init__.py
+-rw-rw-rw-   0        0        0    13845 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/asyncio.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.215323 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/__init__.py
+-rw-rw-rw-   0        0        0    10614 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/async_request_response_handling.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.216322 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/composite/
+-rw-rw-rw-   0        0        0      340 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/composite/__init__.py
+-rw-rw-rw-   0        0        0     1650 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.217315 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/graph/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/graph/__init__.py
+-rw-rw-rw-   0        0        0    32568 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/graph/topology_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.218313 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/grpc/
+-rw-rw-rw-   0        0        0      306 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/grpc/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/health_model.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.219314 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http/
+-rw-rw-rw-   0        0        0      416 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.220317 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http/fastapi/
+-rw-rw-rw-   0        0        0      347 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http/fastapi/__init__.py
+-rw-rw-rw-   0        0        0    17411 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http_fastapi_app.py
+-rw-rw-rw-   0        0        0     9476 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.221314 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/load_balancer/
+-rw-rw-rw-   0        0        0      290 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/load_balancer/__init__.py
+-rw-rw-rw-   0        0        0    10232 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/models.py
+-rw-rw-rw-   0        0        0    11182 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/request_handling.py
+-rw-rw-rw-   0        0        0    20367 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/streamer.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.222314 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/websocket/
+-rw-rw-rw-   0        0        0      339 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/websocket/__init__.py
+-rw-rw-rw-   0        0        0    12485 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/gateway/websocket_fastapi_app.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.224326 cmon-ai-0.42.6/cmon/serve/runtimes/head/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/head/__init__.py
+-rw-rw-rw-   0        0        0    24494 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/head/request_handling.py
+-rw-rw-rw-   0        0        0     7742 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/helper.py
+-rw-rw-rw-   0        0        0     9296 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/monitoring.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.229320 cmon-ai-0.42.6/cmon/serve/runtimes/servers/
+-rw-rw-rw-   0        0        0     9783 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/servers/__init__.py
+-rw-rw-rw-   0        0        0     3377 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/servers/composite.py
+-rw-rw-rw-   0        0        0     8269 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/serve/runtimes/servers/grpc.py
+-rw-rw-rw-   0        0        0     9857 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/serve/runtimes/servers/http.py
+-rw-rw-rw-   0        0        0     2255 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/servers/load_balancer.py
+-rw-rw-rw-   0        0        0     4983 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/serve/runtimes/servers/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.232316 cmon-ai-0.42.6/cmon/serve/runtimes/worker/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/runtimes/worker/__init__.py
+-rw-rw-rw-   0        0        0     6088 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/cmon/serve/runtimes/worker/batch_queue.py
+-rw-rw-rw-   0        0        0     6837 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/worker/http_fastapi_app.py
+-rw-rw-rw-   0        0        0    48714 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/serve/runtimes/worker/request_handling.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.234323 cmon-ai-0.42.6/cmon/serve/stream/
+-rw-rw-rw-   0        0        0    13720 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/stream/__init__.py
+-rw-rw-rw-   0        0        0     3505 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/serve/stream/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.236322 cmon-ai-0.42.6/cmon/types/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/types/__init__.py
+-rw-rw-rw-   0        0        0     3814 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/types/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.238316 cmon-ai-0.42.6/cmon/types/request/
+-rw-rw-rw-   0        0        0     1631 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/types/request/__init__.py
+-rw-rw-rw-   0        0        0    14425 2023-06-25 14:00:01.000000 cmon-ai-0.42.6/cmon/types/request/data.py
+-rw-rw-rw-   0        0        0     2189 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon/types/request/status.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.267723 cmon-ai-0.42.6/cmon_ai.egg-info/
+-rw-rw-rw-   0        0        0    16300 2023-06-25 16:25:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    27701 2023-06-25 16:25:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:25:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-25 16:25:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-25 16:23:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       72 2023-06-25 16:25:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-25 16:25:46.000000 cmon-ai-0.42.6/cmon_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.274733 cmon-ai-0.42.6/cmon_cli/
+-rw-rw-rw-   0        0        0     4210 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon_cli/__init__.py
+-rw-rw-rw-   0        0        0     5173 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon_cli/api.py
+-rw-rw-rw-   0        0        0    13006 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon_cli/autocomplete.py
+-rw-rw-rw-   0        0        0     4165 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/cmon_cli/export.py
+-rw-rw-rw-   0        0        0      193 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon_cli/known_plugins.py
+-rw-rw-rw-   0        0        0     4719 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/cmon_cli/lookup.py
+-rw-rw-rw-   0        0        0     3103 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/extra-requirements.txt
+-rw-rw-rw-   0        0        0     4095 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/fastentrypoints.py
+-rw-rw-rw-   0        0        0       96 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 16:25:47.608293 cmon-ai-0.42.6/setup.cfg
+-rw-rw-rw-   0        0        0     8303 2023-06-25 16:25:30.000000 cmon-ai-0.42.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.276727 cmon-ai-0.42.6/tests/
+-rw-rw-rw-   0        0        0     1733 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.278723 cmon-ai-0.42.6/tests/cmonhub/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/cmonhub/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/cmonhub/app.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.279722 cmon-ai-0.42.6/tests/cmonhub/hub_mwu/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/cmonhub/hub_mwu/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/cmonhub/hub_mwu/mwu_encoder.py
+-rw-rw-rw-   0        0        0     2212 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.282719 cmon-ai-0.42.6/tests/docker_compose/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/__init__.py
+-rw-rw-rw-   0        0        0     3516 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.284722 cmon-ai-0.42.6/tests/docker_compose/custom-gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/custom-gateway/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/docker_compose/custom-gateway/dummy_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.286721 cmon-ai-0.42.6/tests/docker_compose/multiprotocol-gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/multiprotocol-gateway/__init__.py
+-rw-rw-rw-   0        0        0     2620 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/multiprotocol-gateway/multiprotocol_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.287716 cmon-ai-0.42.6/tests/docker_compose/reload-executor/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/reload-executor/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/reload-executor/reload_executor.py
+-rw-rw-rw-   0        0        0    10722 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/test_deployment_docker_compose.py
+-rw-rw-rw-   0        0        0    10445 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/docker_compose/test_flow_docker_compose.py
+-rw-rw-rw-   0        0        0     1162 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.289713 cmon-ai-0.42.6/tests/integration/
+-rw-rw-rw-   0        0        0      122 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.291724 cmon-ai-0.42.6/tests/integration/clients_extra_kwargs/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/clients_extra_kwargs/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/clients_extra_kwargs/test_clients_post_extra_kwargs.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.294722 cmon-ai-0.42.6/tests/integration/concurrent_clients/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/concurrent_clients/__init__.py
+-rw-rw-rw-   0        0        0     2072 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/concurrent_clients/test_concurrent_clients.py
+-rw-rw-rw-   0        0        0     1562 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/concurrent_clients/test_multithread_client.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.295722 cmon-ai-0.42.6/tests/integration/conditions_feature/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/conditions_feature/__init__.py
+-rw-rw-rw-   0        0        0     6340 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/conditions_feature/test_condition_behavior.py
+-rw-rw-rw-   0        0        0      496 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.297714 cmon-ai-0.42.6/tests/integration/container_runtime_args/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/container_runtime_args/__init__.py
+-rw-rw-rw-   0        0        0     1194 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/container_runtime_args/test_container_get_args.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.298722 cmon-ai-0.42.6/tests/integration/crud/
+-rw-rw-rw-   0        0        0     3549 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/crud/__init__.py
+-rw-rw-rw-   0        0        0     4254 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/crud/test_crud.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.300722 cmon-ai-0.42.6/tests/integration/dataclass_executor/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/dataclass_executor/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/dataclass_executor/test_dataclass_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.303714 cmon-ai-0.42.6/tests/integration/deployment_http_composite/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/deployment_http_composite/__init__.py
+-rw-rw-rw-   0        0        0     7681 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/deployment_http_composite/test_deployment_http_composite.py
+-rw-rw-rw-   0        0        0     9396 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/deployment_http_composite/test_deployment_http_composite_docarray_v2.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.305713 cmon-ai-0.42.6/tests/integration/deployments/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/deployments/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/deployments/executor.py
+-rw-rw-rw-   0        0        0    15192 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/deployments/test_deployment.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.308718 cmon-ai-0.42.6/tests/integration/distributed-replicas/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/distributed-replicas/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/distributed-replicas/exec.py
+-rw-rw-rw-   0        0        0     5464 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/distributed-replicas/test_distributed_replicas.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.310723 cmon-ai-0.42.6/tests/integration/docarray_v2/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/docarray_v2/__init__.py
+-rw-rw-rw-   0        0        0     2816 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/tests/integration/docarray_v2/test_streaming.py
+-rw-rw-rw-   0        0        0    39066 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/docarray_v2/test_v2.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.312714 cmon-ai-0.42.6/tests/integration/docker_volumes/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/docker_volumes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.314728 cmon-ai-0.42.6/tests/integration/docker_volumes/filewriter-exec/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/docker_volumes/filewriter-exec/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/docker_volumes/filewriter-exec/executor.py
+-rw-rw-rw-   0        0        0     1562 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/docker_volumes/test_volumes_in_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.316715 cmon-ai-0.42.6/tests/integration/dynamic_batching/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/dynamic_batching/__init__.py
+-rw-rw-rw-   0        0        0    20802 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/dynamic_batching/test_dynamic_batching.py
+-rw-rw-rw-   0        0        0     1315 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/dynamic_batching/test_dynamic_batching_config.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.318715 cmon-ai-0.42.6/tests/integration/external_deployment/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/external_deployment/__init__.py
+-rw-rw-rw-   0        0        0    15022 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/external_deployment/test_external_deployment.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.320720 cmon-ai-0.42.6/tests/integration/floating_deployments/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/floating_deployments/__init__.py
+-rw-rw-rw-   0        0        0    10608 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/floating_deployments/test_floating_deployments.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.322721 cmon-ai-0.42.6/tests/integration/flow_dry_run/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/flow_dry_run/__init__.py
+-rw-rw-rw-   0        0        0     1016 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/flow_dry_run/test_flow_dry_run.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.329727 cmon-ai-0.42.6/tests/integration/gateway_clients/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/gateway_clients/__init__.py
+-rw-rw-rw-   0        0        0    17530 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/gateway_clients/test_clients_gateways.py
+-rw-rw-rw-   0        0        0     1712 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/gateway_clients/test_executor_timeout_failures.py
+-rw-rw-rw-   0        0        0      450 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/gateway_clients/test_host_scheme.py
+-rw-rw-rw-   0        0        0      720 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/gateway_clients/test_long_flow_keepalive.py
+-rw-rw-rw-   0        0        0    16282 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/gateway_clients/test_streaming.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.330715 cmon-ai-0.42.6/tests/integration/gateway_non_blocking/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/gateway_non_blocking/__init__.py
+-rw-rw-rw-   0        0        0     1147 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/gateway_non_blocking/test_gateway_non_blocking.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.332717 cmon-ai-0.42.6/tests/integration/gateway_streamer/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/gateway_streamer/__init__.py
+-rw-rw-rw-   0        0        0     6038 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/gateway_streamer/test_gateway_streamer.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.333714 cmon-ai-0.42.6/tests/integration/graphql/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/graphql/__init__.py
+-rw-rw-rw-   0        0        0     9543 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/graphql/test_graphql.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.335726 cmon-ai-0.42.6/tests/integration/grpc_bytes_census/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/grpc_bytes_census/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/grpc_bytes_census/test_bytes_census.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.337720 cmon-ai-0.42.6/tests/integration/high_order_matches/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/high_order_matches/__init__.py
+-rw-rw-rw-   0        0        0     1585 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/high_order_matches/test_document.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.342723 cmon-ai-0.42.6/tests/integration/hot_reload/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.344718 cmon-ai-0.42.6/tests/integration/hot_reload/exec1/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec1/__init__.py
+-rw-rw-rw-   0        0        0      406 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec1/my_executor1.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.346718 cmon-ai-0.42.6/tests/integration/hot_reload/exec2/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec2/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec2/helper.py
+-rw-rw-rw-   0        0        0      295 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec2/my_executor2.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.348722 cmon-ai-0.42.6/tests/integration/hot_reload/exec3/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec3/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec3/my_executor3.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.349740 cmon-ai-0.42.6/tests/integration/hot_reload/exec4/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec4/__init__.py
+-rw-rw-rw-   0        0        0      406 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/exec4/my_executor4.py
+-rw-rw-rw-   0        0        0       56 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/helper2.py
+-rw-rw-rw-   0        0        0      404 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/my_executor_1_new.py
+-rw-rw-rw-   0        0        0      313 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/my_executor_3_new.py
+-rw-rw-rw-   0        0        0      404 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/my_executor_4_new.py
+-rw-rw-rw-   0        0        0     5102 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hot_reload/test_hot_reload.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.351739 cmon-ai-0.42.6/tests/integration/hub_usage/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.354731 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub/
+-rw-rw-rw-   0        0        0      185 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.355747 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_abs/
+-rw-rw-rw-   0        0        0      186 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_abs/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_abs/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.357741 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_pretrained/
+-rw-rw-rw-   0        0        0      430 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_pretrained/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.358733 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_slow/
+-rw-rw-rw-   0        0        0      223 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_slow/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/dummyhub_slow/helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.360733 cmon-ai-0.42.6/tests/integration/hub_usage/hub-mwu/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/hub-mwu/__init__.py
+-rw-rw-rw-   0        0        0      292 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/hub_usage/hub-mwu/mwu_encoder.py
+-rw-rw-rw-   0        0        0     3273 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/integration/hub_usage/test_hub_usage.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.361744 cmon-ai-0.42.6/tests/integration/inspect_deployments_flow/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/inspect_deployments_flow/__init__.py
+-rw-rw-rw-   0        0        0     5172 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/inspect_deployments_flow/test_inspect_deployments_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.363737 cmon-ai-0.42.6/tests/integration/install_requirements/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/install_requirements/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.365218 cmon-ai-0.42.6/tests/integration/install_requirements/exec/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/install_requirements/exec/__init__.py
+-rw-rw-rw-   0        0        0      101 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/install_requirements/exec/my_executor.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/install_requirements/test_install_requirements.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.370217 cmon-ai-0.42.6/tests/integration/instrumentation/
+-rw-rw-rw-   0        0        0     5481 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/instrumentation/__init__.py
+-rw-rw-rw-   0        0        0     3157 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/instrumentation/conftest.py
+-rw-rw-rw-   0        0        0     1349 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/instrumentation/test_container_instrumentation.py
+-rw-rw-rw-   0        0        0    13851 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/instrumentation/test_flow_instrumentation.py
+-rw-rw-rw-   0        0        0     1443 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/instrumentation/test_worker_instrumentation.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.372218 cmon-ai-0.42.6/tests/integration/issues/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.373222 cmon-ai-0.42.6/tests/integration/issues/github_1546/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_1546/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.375225 cmon-ai-0.42.6/tests/integration/issues/github_1546/good_old/
+-rw-rw-rw-   0        0        0      210 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_1546/good_old/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_1546/good_old/helper.py
+-rw-rw-rw-   0        0        0     2480 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/integration/issues/github_1546/test_pymodules_import.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.376227 cmon-ai-0.42.6/tests/integration/issues/github_2103/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_2103/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/issues/github_2103/test_search_attributes.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.378226 cmon-ai-0.42.6/tests/integration/issues/github_2371/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_2371/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_2371/test_pod.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.379229 cmon-ai-0.42.6/tests/integration/issues/github_2910/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_2910/__init__.py
+-rw-rw-rw-   0        0        0      814 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_2910/test_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.380221 cmon-ai-0.42.6/tests/integration/issues/github_3124/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_3124/__init__.py
+-rw-rw-rw-   0        0        0      617 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_3124/test_cli_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.382223 cmon-ai-0.42.6/tests/integration/issues/github_3271/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_3271/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.383227 cmon-ai-0.42.6/tests/integration/issues/github_3271/executors/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_3271/executors/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_3271/executors/executor_fails_import_twice.py
+-rw-rw-rw-   0        0        0      872 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_3271/test_python_single_import.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.385225 cmon-ai-0.42.6/tests/integration/issues/github_4488/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_4488/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/issues/github_4488/test_deployment_protocol.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.387217 cmon-ai-0.42.6/tests/integration/issues/github_4521/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_4521/__init__.py
+-rw-rw-rw-   0        0        0      867 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/issues/github_4521/test_blob_transmission.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.388217 cmon-ai-0.42.6/tests/integration/issues/github_5141/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_5141/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_5141/test_invalid_input_raises_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.390226 cmon-ai-0.42.6/tests/integration/issues/github_5543/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_5543/__init__.py
+-rw-rw-rw-   0        0        0      342 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_5543/test_reentrant_flows.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.391221 cmon-ai-0.42.6/tests/integration/issues/github_5735/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_5735/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/issues/github_5735/test_inherited_executor.py
+-rw-rw-rw-   0        0        0      363 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/issues/test_5661.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.396221 cmon-ai-0.42.6/tests/integration/monitoring/
+-rw-rw-rw-   0        0        0      660 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/monitoring/__init__.py
+-rw-rw-rw-   0        0        0     2506 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/monitoring/test_deprecated_metric.py
+-rw-rw-rw-   0        0        0     3090 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/monitoring/test_executor.py
+-rw-rw-rw-   0        0        0     7527 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/monitoring/test_manual_flow.py
+-rw-rw-rw-   0        0        0    12095 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/monitoring/test_monitoring.py
+-rw-rw-rw-   0        0        0     5829 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/monitoring/test_request_size.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.398231 cmon-ai-0.42.6/tests/integration/multiple_protocol_gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/multiple_protocol_gateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.400219 cmon-ai-0.42.6/tests/integration/multiple_protocol_gateway/gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/multiple_protocol_gateway/gateway/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/multiple_protocol_gateway/gateway/multiprotocol_gateway.py
+-rw-rw-rw-   0        0        0     1525 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/multiple_protocol_gateway/test_multiple_protocols_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.401229 cmon-ai-0.42.6/tests/integration/multiprocessing_spawn/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/multiprocessing_spawn/__init__.py
+-rw-rw-rw-   0        0        0     1136 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/multiprocessing_spawn/test_spawn.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.403218 cmon-ai-0.42.6/tests/integration/needs-merge/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/needs-merge/__init__.py
+-rw-rw-rw-   0        0        0      627 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/needs-merge/test_needs_merge.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.405217 cmon-ai-0.42.6/tests/integration/network_failures/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/network_failures/__init__.py
+-rw-rw-rw-   0        0        0    28715 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/network_failures/test_network_failures.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.408223 cmon-ai-0.42.6/tests/integration/networking/
+-rw-rw-rw-   0        0        0      195 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/networking/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/networking/conftest.py
+-rw-rw-rw-   0        0        0     3237 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/networking/test_connection_stub.py
+-rw-rw-rw-   0        0        0     4532 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/networking/test_grpc_connection_pool.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.409222 cmon-ai-0.42.6/tests/integration/override_config_params/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.412224 cmon-ai-0.42.6/tests/integration/override_config_params/container/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/container/__init__.py
+-rw-rw-rw-   0        0        0      613 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/container/executor.py
+-rw-rw-rw-   0        0        0     2142 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/container/test_override_config_params.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.414224 cmon-ai-0.42.6/tests/integration/override_config_params/worker/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/worker/__init__.py
+-rw-rw-rw-   0        0        0      613 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/worker/executor.py
+-rw-rw-rw-   0        0        0     3989 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_config_params/worker/test_override_config_params.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.415223 cmon-ai-0.42.6/tests/integration/override_executor_specific_params/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_executor_specific_params/__init__.py
+-rw-rw-rw-   0        0        0     1959 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/override_executor_specific_params/test_specific_params.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.417224 cmon-ai-0.42.6/tests/integration/pods/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/pods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.419219 cmon-ai-0.42.6/tests/integration/pods/container/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/pods/container/__init__.py
+-rw-rw-rw-   0        0        0     4329 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/pods/container/test_pod.py
+-rw-rw-rw-   0        0        0    17366 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/pods/test_pod.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.421222 cmon-ai-0.42.6/tests/integration/reduce/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reduce/__init__.py
+-rw-rw-rw-   0        0        0     7651 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reduce/test_reduce.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.423224 cmon-ai-0.42.6/tests/integration/reload/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reload/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.426225 cmon-ai-0.42.6/tests/integration/reload/exec/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reload/exec/__init__.py
+-rw-rw-rw-   0        0        0      272 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reload/exec/exec1.py
+-rw-rw-rw-   0        0        0      270 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reload/exec/exec2.py
+-rw-rw-rw-   0        0        0     3134 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reload/test_deployments_reload.py
+-rw-rw-rw-   0        0        0     2709 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/reload/test_flow_reload.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.427224 cmon-ai-0.42.6/tests/integration/replica-exec/
+-rw-rw-rw-   0        0        0      543 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/replica-exec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.428223 cmon-ai-0.42.6/tests/integration/rr_cuda/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/rr_cuda/__init__.py
+-rw-rw-rw-   0        0        0     1800 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/rr_cuda/test_rr_cuda.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.430217 cmon-ai-0.42.6/tests/integration/runtime_signal_handling/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtime_signal_handling/__init__.py
+-rw-rw-rw-   0        0        0     2515 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtime_signal_handling/test_runtime_captures_signals.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.434220 cmon-ai-0.42.6/tests/integration/runtimes/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtimes/__init__.py
+-rw-rw-rw-   0        0        0     3641 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtimes/test_cmon_info.py
+-rw-rw-rw-   0        0        0     3805 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtimes/test_gateway_dry_run.py
+-rw-rw-rw-   0        0        0    30390 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtimes/test_runtimes.py
+-rw-rw-rw-   0        0        0     2990 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/runtimes/test_warmup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.436229 cmon-ai-0.42.6/tests/integration/sandbox/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/sandbox/__init__.py
+-rw-rw-rw-   0        0        0      701 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/integration/sandbox/test_sandbox.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.438220 cmon-ai-0.42.6/tests/integration/sparse_pipeline/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/sparse_pipeline/__init__.py
+-rw-rw-rw-   0        0        0     2072 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/sparse_pipeline/test_sparse_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.439228 cmon-ai-0.42.6/tests/integration/specific_executor_params/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/specific_executor_params/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/specific_executor_params/test_specific_params.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.441226 cmon-ai-0.42.6/tests/integration/stateful/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/stateful/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.442227 cmon-ai-0.42.6/tests/integration/stateful/stateful_no_snapshot_exec/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/stateful/stateful_no_snapshot_exec/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/stateful/stateful_no_snapshot_exec/executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.444226 cmon-ai-0.42.6/tests/integration/stateful/stateful_snapshot_exec/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/stateful/stateful_snapshot_exec/__init__.py
+-rw-rw-rw-   0        0        0     2353 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/stateful/stateful_snapshot_exec/executor.py
+-rw-rw-rw-   0        0        0    10459 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/stateful/test_stateful.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.446217 cmon-ai-0.42.6/tests/integration/streaming/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/streaming/__init__.py
+-rw-rw-rw-   0        0        0    10666 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/streaming/test_clients_streaming.py
+-rw-rw-rw-   0        0        0     2581 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/tests/integration/streaming/test_streaming.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.448227 cmon-ai-0.42.6/tests/integration/test_grpc_compression/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/test_grpc_compression/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/test_grpc_compression/test_grpc_compression.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.449236 cmon-ai-0.42.6/tests/integration/test_prefetch/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/test_prefetch/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/test_prefetch/test_prefetch.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.451243 cmon-ai-0.42.6/tests/integration/test_return_order/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/test_return_order/__init__.py
+-rw-rw-rw-   0        0        0     1293 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/test_return_order/test_return_order.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.456245 cmon-ai-0.42.6/tests/integration/v2_api/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/v2_api/__init__.py
+-rw-rw-rw-   0        0        0     3120 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/integration/v2_api/test_docs_matrix_tail_pea.py
+-rw-rw-rw-   0        0        0     7148 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/v2_api/test_func_routing.py
+-rw-rw-rw-   0        0        0     2258 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/v2_api/test_override_requests.py
+-rw-rw-rw-   0        0        0     1506 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/v2_api/test_returns.py
+-rw-rw-rw-   0        0        0     1646 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/v2_api/test_yaml_dump_load.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.458238 cmon-ai-0.42.6/tests/integration/websocket_gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/websocket_gateway/__init__.py
+-rw-rw-rw-   0        0        0     3595 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/integration/websocket_gateway/test_subprotocols.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.462233 cmon-ai-0.42.6/tests/k8s/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/__init__.py
+-rw-rw-rw-   0        0        0     8409 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.464768 cmon-ai-0.42.6/tests/k8s/custom-gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/custom-gateway/__init__.py
+-rw-rw-rw-   0        0        0     1659 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/k8s/custom-gateway/dummy_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.466776 cmon-ai-0.42.6/tests/k8s/multiprotocol-gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/multiprotocol-gateway/__init__.py
+-rw-rw-rw-   0        0        0     2397 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/multiprotocol-gateway/multiprotocol_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.467778 cmon-ai-0.42.6/tests/k8s/reload-executor/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/reload-executor/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/reload-executor/reload_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.469782 cmon-ai-0.42.6/tests/k8s/test-stateful-executor/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/test-stateful-executor/__init__.py
+-rw-rw-rw-   0        0        0      723 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/k8s/test-stateful-executor/stateful_executor.py
+-rw-rw-rw-   0        0        0     6946 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/k8s/test_k8s_deployment.py
+-rw-rw-rw-   0        0        0    12095 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/test_k8s_failures.py
+-rw-rw-rw-   0        0        0    57105 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/k8s/test_k8s_flow.py
+-rw-rw-rw-   0        0        0    14581 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s/test_k8s_graceful_request_handling.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.474776 cmon-ai-0.42.6/tests/k8s_otel/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s_otel/__init__.py
+-rw-rw-rw-   0        0        0     2065 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s_otel/conftest.py
+-rw-rw-rw-   0        0        0     8940 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s_otel/kind_wrapper.py
+-rw-rw-rw-   0        0        0     4703 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s_otel/test_k8s_instrumentation.py
+-rw-rw-rw-   0        0        0      794 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/k8s_otel/util.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.480778 cmon-ai-0.42.6/tests/unit/
+-rw-rw-rw-   0        0        0      102 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.485776 cmon-ai-0.42.6/tests/unit/clients/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.489776 cmon-ai-0.42.6/tests/unit/clients/python/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/clients/python/__init__.py
+-rw-rw-rw-   0        0        0     5773 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/clients/python/test_client.py
+-rw-rw-rw-   0        0        0     7582 2023-06-25 13:50:20.000000 cmon-ai-0.42.6/tests/unit/clients/python/test_client_errors.py
+-rw-rw-rw-   0        0        0     2396 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/clients/python/test_on_err.py
+-rw-rw-rw-   0        0        0     6572 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/clients/python/test_request.py
+-rw-rw-rw-   0        0        0     1689 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/clients/test_asyncio.py
+-rw-rw-rw-   0        0        0      886 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/clients/test_client_grpc_channel_options.py
+-rw-rw-rw-   0        0        0     4511 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/clients/test_helper.py
+-rw-rw-rw-   0        0        0     2274 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/clients/test_interface.py
+-rw-rw-rw-   0        0        0      847 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/clients/test_log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.491768 cmon-ai-0.42.6/tests/unit/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     2502 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/exceptions/test_exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.493767 cmon-ai-0.42.6/tests/unit/jaml/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/jaml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.494769 cmon-ai-0.42.6/tests/unit/jaml/parsers/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/jaml/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.496775 cmon-ai-0.42.6/tests/unit/jaml/parsers/executors/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/jaml/parsers/executors/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/jaml/parsers/executors/test_legacy.py
+-rw-rw-rw-   0        0        0     1646 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/jaml/test_gateway_parse.py
+-rw-rw-rw-   0        0        0     6957 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/jaml/test_type_parse.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.499776 cmon-ai-0.42.6/tests/unit/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/logging/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/logging/test_formatter.py
+-rw-rw-rw-   0        0        0     3093 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/logging/test_logging.py
+-rw-rw-rw-   0        0        0      548 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/logging/test_logging_profile.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.500769 cmon-ai-0.42.6/tests/unit/orchestrate/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.503768 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.507776 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.508767 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/k8slib/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/k8slib/__init__.py
+-rw-rw-rw-   0        0        0     1686 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/k8slib/test_kubernetes_tools.py
+-rw-rw-rw-   0        0        0    23684 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/test_docker_compose_pod_config.py
+-rw-rw-rw-   0        0        0     2312 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/test_helper.py
+-rw-rw-rw-   0        0        0    29781 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/config/test_k8s_deployment_config.py
+-rw-rw-rw-   0        0        0     2116 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/test_cuda_assignment.py
+-rw-rw-rw-   0        0        0    20749 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/test_deployments.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/deployments/test_load_config.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.509766 cmon-ai-0.42.6/tests/unit/orchestrate/flow/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.511772 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-async/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-async/__init__.py
+-rw-rw-rw-   0        0        0     6188 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-async/test_asyncflow.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.524767 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.526772 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/executor/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/executor/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/executor/executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.527776 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/executor-invalid-import/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/executor-invalid-import/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/executor-invalid-import/executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.529772 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/mwu-encoder/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/mwu-encoder/__init__.py
+-rw-rw-rw-   0        0        0      635 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/mwu-encoder/mwu_encoder.py
+-rw-rw-rw-   0        0        0    20123 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow.py
+-rw-rw-rw-   0        0        0     4255 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_custom_gateway.py
+-rw-rw-rw-   0        0        0     2049 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_deployment.py
+-rw-rw-rw-   0        0        0     7882 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_except.py
+-rw-rw-rw-   0        0        0     1161 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_monitoring.py
+-rw-rw-rw-   0        0        0     4802 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_multiprotocol.py
+-rw-rw-rw-   0        0        0     1997 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_skip.py
+-rw-rw-rw-   0        0        0      946 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_start_noblock.py
+-rw-rw-rw-   0        0        0    17660 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_to_docker_compose_yaml.py
+-rw-rw-rw-   0        0        0    28301 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_to_k8s_yaml.py
+-rw-rw-rw-   0        0        0     3995 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_visualization.py
+-rw-rw-rw-   0        0        0     7089 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_flow_yaml_parser.py
+-rw-rw-rw-   0        0        0      523 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-construct/test_slow_executor_shutdown.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.532771 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-example/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-example/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-example/test_flow_empty_request.py
+-rw-rw-rw-   0        0        0     2022 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-example/test_flow_examples.py
+-rw-rw-rw-   0        0        0     1215 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-example/test_flow_segmenter.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.542770 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/__init__.py
+-rw-rw-rw-   0        0        0     2629 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_before_after.py
+-rw-rw-rw-   0        0        0     1351 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_change_gateway.py
+-rw-rw-rw-   0        0        0     2880 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_complex_topology.py
+-rw-rw-rw-   0        0        0     2181 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_docarray_return.py
+-rw-rw-rw-   0        0        0     1029 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_http_extend.py
+-rw-rw-rw-   0        0        0     2173 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_merge.py
+-rw-rw-rw-   0        0        0     4273 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_flow_routing.py
+-rw-rw-rw-   0        0        0     2356 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/flow/flow-orchestrate/test_ndarray_type.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.544776 cmon-ai-0.42.6/tests/unit/orchestrate/pods/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.546776 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.547776 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/custom-gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/custom-gateway/__init__.py
+-rw-rw-rw-   0        0        0     1836 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/custom-gateway/dummy_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.549783 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/dummy-exec/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/dummy-exec/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/dummy-exec/executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.550775 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/env-checker/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/env-checker/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/env-checker/executor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.552793 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/fail-start/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/fail-start/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/fail-start/executor.py
+-rw-rw-rw-   0        0        0     8068 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/container/test_container_pod.py
+-rw-rw-rw-   0        0        0     4502 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/test_pod.py
+-rw-rw-rw-   0        0        0      631 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/orchestrate/pods/test_pod_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.553779 cmon-ai-0.42.6/tests/unit/parsers/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.554783 cmon-ai-0.42.6/tests/unit/parsers/peapods/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/peapods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.558775 cmon-ai-0.42.6/tests/unit/parsers/peapods/runtimes/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/peapods/runtimes/__init__.py
+-rw-rw-rw-   0        0        0     3388 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/peapods/runtimes/test_port_protocol_parser.py
+-rw-rw-rw-   0        0        0      793 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/peapods/runtimes/test_remote_parser.py
+-rw-rw-rw-   0        0        0      829 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/peapods/runtimes/test_runtime_parser.py
+-rw-rw-rw-   0        0        0     2825 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/parsers/test_warnings.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.559775 cmon-ai-0.42.6/tests/unit/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/schemas/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/schemas/test_schema.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.560776 cmon-ai-0.42.6/tests/unit/serve/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.561779 cmon-ai-0.42.6/tests/unit/serve/dynamic_batching/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/dynamic_batching/__init__.py
+-rw-rw-rw-   0        0        0     3003 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/dynamic_batching/test_batch_queue.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.568296 cmon-ai-0.42.6/tests/unit/serve/executors/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/dummy_executor.py
+-rw-rw-rw-   0        0        0      171 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/metas_executors.py
+-rw-rw-rw-   0        0        0     1201 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/test_bad_executor_constructor.py
+-rw-rw-rw-   0        0        0     1938 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/test_decorators.py
+-rw-rw-rw-   0        0        0    19905 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/executors/test_executor.py
+-rw-rw-rw-   0        0        0      585 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/test_runtime_args.py
+-rw-rw-rw-   0        0        0     2253 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/executors/test_set_metas.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.572290 cmon-ai-0.42.6/tests/unit/serve/gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/gateway/__init__.py
+-rw-rw-rw-   0        0        0     9083 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/gateway/test_gateway.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.577290 cmon-ai-0.42.6/tests/unit/serve/networking/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/networking/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/networking/conftest.py
+-rw-rw-rw-   0        0        0     5982 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/networking/test_connection_pool_map.py
+-rw-rw-rw-   0        0        0     3284 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/networking/test_replica_list.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.579290 cmon-ai-0.42.6/tests/unit/serve/runtimes/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.580291 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.582290 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/graph/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/graph/__init__.py
+-rw-rw-rw-   0        0        0    42500 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/graph/test_topology_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.586305 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/grpc/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/grpc/__init__.py
+-rw-rw-rw-   0        0        0    16245 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/grpc/test_grpc_gateway_runtime.py
+-rw-rw-rw-   0        0        0     1625 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/grpc/test_grpc_tls.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.591298 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/http/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/http/__init__.py
+-rw-rw-rw-   0        0        0    12374 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/http/test_app.py
+-rw-rw-rw-   0        0        0     1690 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/gateway/http/test_models.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.593292 cmon-ai-0.42.6/tests/unit/serve/runtimes/head/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/head/__init__.py
+-rw-rw-rw-   0        0        0    10960 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/head/test_head_runtime.py
+-rw-rw-rw-   0        0        0    12038 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/test_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.596293 cmon-ai-0.42.6/tests/unit/serve/runtimes/worker/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/worker/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/worker/test_worker_request_handler.py
+-rw-rw-rw-   0        0        0    11899 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/runtimes/worker/test_worker_runtime.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.600293 cmon-ai-0.42.6/tests/unit/serve/stream/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/serve/stream/__init__.py
+-rw-rw-rw-   0        0        0     1807 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/stream/test_helper.py
+-rw-rw-rw-   0        0        0     4711 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/serve/stream/test_stream.py
+-rw-rw-rw-   0        0        0     3870 2023-06-25 03:53:50.000000 cmon-ai-0.42.6/tests/unit/test_cli.py
+-rw-rw-rw-   0        0        0      536 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/test_extend_fastapi.py
+-rw-rw-rw-   0        0        0     2143 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/test_gateway.py
+-rw-rw-rw-   0        0        0    10242 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/test_helper.py
+-rw-rw-rw-   0        0        0     1867 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/test_importer.py
+-rw-rw-rw-   0        0        0      690 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/test_progress_bar.py
+-rw-rw-rw-   0        0        0     7886 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/test_yamlparser.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.601290 cmon-ai-0.42.6/tests/unit/types/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:25:47.605293 cmon-ai-0.42.6/tests/unit/types/request/
+-rw-rw-rw-   0        0        0        0 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/types/request/__init__.py
+-rw-rw-rw-   0        0        0     9742 2023-06-25 14:00:00.000000 cmon-ai-0.42.6/tests/unit/types/request/test_request.py
+-rw-rw-rw-   0        0        0     1195 2023-06-23 15:59:49.000000 cmon-ai-0.42.6/tests/unit/types/request/test_status_message.py
```

### Comparing `cmon-ai-0.38.5/LICENSE` & `cmon-ai-0.42.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/PKG-INFO` & `cmon-ai-0.42.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,989 +1,1019 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 636d 6f6e  : 2.1.Name: cmon
-00000020: 2d61 690a 5665 7273 696f 6e3a 2030 2e33  -ai.Version: 0.3
-00000030: 382e 350a 5375 6d6d 6172 793a 2042 7569  8.5.Summary: Bui
-00000040: 6c64 206d 756c 7469 6d6f 6461 6c20 4149  ld multimodal AI
-00000050: 2073 6572 7669 6365 7320 7669 6120 636c   services via cl
-00000060: 6f75 6420 6e61 7469 7665 2074 6563 686e  oud native techn
-00000070: 6f6c 6f67 6965 7320 c2b7 204e 6575 7261  ologies .. Neura
-00000080: 6c20 5365 6172 6368 20c2 b720 4765 6e65  l Search .. Gene
-00000090: 7261 7469 7665 2041 4920 c2b7 204d 4c4f  rative AI .. MLO
-000000a0: 7073 0a48 6f6d 652d 7061 6765 3a20 6874  ps.Home-page: ht
-000000b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000c0: 2f61 6c69 6e6f 6f72 6979 616e 2f43 6d6f  /alinooriyan/Cmo
-000000d0: 6e2d 4149 0a44 6f77 6e6c 6f61 642d 5552  n-AI.Download-UR
-000000e0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
-000000f0: 622e 636f 6d2f 616c 696e 6f6f 7269 7961  b.com/alinooriya
-00000100: 6e2f 436d 6f6e 2d41 492f 6172 6368 6976  n/Cmon-AI/archiv
-00000110: 652f 7265 6673 2f74 6167 732f 4149 2e7a  e/refs/tags/AI.z
-00000120: 6970 0a41 7574 686f 723a 2043 6d6f 6e20  ip.Author: Cmon 
-00000130: 4149 0a41 7574 686f 722d 656d 6169 6c3a  AI.Author-email:
-00000140: 2068 656c 6c6f 4063 6d6f 6e2e 6169 0a4c   hello@cmon.ai.L
-00000150: 6963 656e 7365 3a20 4170 6163 6865 2032  icense: Apache 2
-00000160: 2e30 0a50 726f 6a65 6374 2d55 524c 3a20  .0.Project-URL: 
-00000170: 446f 6375 6d65 6e74 6174 696f 6e2c 2068  Documentation, h
-00000180: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00000190: 2e70 770a 5072 6f6a 6563 742d 5552 4c3a  .pw.Project-URL:
-000001a0: 2053 6f75 7263 652c 2068 7474 7073 3a2f   Source, https:/
-000001b0: 2f67 6974 6875 622e 636f 6d2f 616c 696e  /github.com/alin
-000001c0: 6f6f 7269 7961 6e2f 636d 6f6e 2d61 692f  ooriyan/cmon-ai/
-000001d0: 0a50 726f 6a65 6374 2d55 524c 3a20 5472  .Project-URL: Tr
-000001e0: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
-000001f0: 6974 6875 622e 636f 6d2f 616c 696e 6f6f  ithub.com/alinoo
-00000200: 7269 7961 6e2f 636d 6f6e 2d61 692f 6973  riyan/cmon-ai/is
-00000210: 7375 6573 0a4b 6579 776f 7264 733a 2063  sues.Keywords: c
-00000220: 6d6f 6e20 636c 6f75 642d 6e61 7469 7665  mon cloud-native
-00000230: 2063 726f 7373 2d6d 6f64 616c 206d 756c   cross-modal mul
-00000240: 7469 6d6f 6461 6c20 6e65 7572 616c 2d73  timodal neural-s
-00000250: 6561 7263 6820 7175 6572 7920 7365 6172  earch query sear
-00000260: 6368 2069 6e64 6578 2065 6c61 7374 6963  ch index elastic
-00000270: 206e 6575 7261 6c2d 6e65 7477 6f72 6b20   neural-network 
-00000280: 656e 636f 6469 6e67 2065 6d62 6564 6469  encoding embeddi
-00000290: 6e67 2073 6572 7669 6e67 2064 6f63 6b65  ng serving docke
-000002a0: 7220 636f 6e74 6169 6e65 7220 696d 6167  r container imag
-000002b0: 6520 7669 6465 6f20 6175 6469 6f20 6465  e video audio de
-000002c0: 6570 2d6c 6561 726e 696e 6720 6d6c 6f70  ep-learning mlop
-000002d0: 730a 436c 6173 7369 6669 6572 3a20 4465  s.Classifier: De
-000002e0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-000002f0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-00000300: 6f6e 2f53 7461 626c 650a 436c 6173 7369  on/Stable.Classi
-00000310: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000320: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000330: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
-00000340: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000350: 6e63 6520 3a3a 2045 6475 6361 7469 6f6e  nce :: Education
-00000360: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-00000370: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000380: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000390: 6368 0a43 6c61 7373 6966 6965 723a 2050  ch.Classifier: P
-000003a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003c0: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
-000003d0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000003e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003f0: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
-00000400: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000410: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000420: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
-00000430: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000440: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000450: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-00000460: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000470: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000480: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
-00000490: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000004a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000004b0: 3a3a 2055 6e69 7820 5368 656c 6c0a 436c  :: Unix Shell.Cl
-000004c0: 6173 7369 6669 6572 3a20 456e 7669 726f  assifier: Enviro
-000004d0: 6e6d 656e 7420 3a3a 2043 6f6e 736f 6c65  nment :: Console
-000004e0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-000004f0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000500: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
-00000510: 6f66 7477 6172 6520 4c69 6365 6e73 650a  oftware License.
-00000520: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000530: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000540: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
-00000550: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000560: 203a 3a20 4461 7461 6261 7365 203a 3a20   :: Database :: 
-00000570: 4461 7461 6261 7365 2045 6e67 696e 6573  Database Engines
-00000580: 2f53 6572 7665 7273 0a43 6c61 7373 6966  /Servers.Classif
-00000590: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-000005a0: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-000005b0: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
-000005c0: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
-000005d0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-000005e0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-000005f0: 2057 5757 2f48 5454 5020 3a3a 2049 6e64   WWW/HTTP :: Ind
-00000600: 6578 696e 672f 5365 6172 6368 0a43 6c61  exing/Search.Cla
-00000610: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000620: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
-00000630: 696e 6565 7269 6e67 203a 3a20 496d 6167  ineering :: Imag
-00000640: 6520 5265 636f 676e 6974 696f 6e0a 436c  e Recognition.Cl
-00000650: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000660: 3a3a 204d 756c 7469 6d65 6469 6120 3a3a  :: Multimedia ::
-00000670: 2056 6964 656f 0a43 6c61 7373 6966 6965   Video.Classifie
-00000680: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-00000690: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-000006a0: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
-000006b0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-000006c0: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-000006d0: 3a20 4d61 7468 656d 6174 6963 730a 436c  : Mathematics.Cl
-000006e0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000006f0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000700: 6c6f 706d 656e 740a 436c 6173 7369 6669  lopment.Classifi
-00000710: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-00000720: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000730: 7420 3a3a 204c 6962 7261 7269 6573 0a43  t :: Libraries.C
-00000740: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000750: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000760: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000770: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
-00000780: 4d6f 6475 6c65 730a 4465 7363 7269 7074  Modules.Descript
-00000790: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000007a0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000007b0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000007c0: 4345 4e53 450a 0a3c 7020 616c 6967 6e3d  CENSE..<p align=
-000007d0: 2263 656e 7465 7222 3e0a 3c21 2d2d 2073  "center">.<!-- s
-000007e0: 7572 7665 7920 6261 6e6e 6572 2073 7461  urvey banner sta
-000007f0: 7274 202d 2d3e 0a3c 6120 6872 6566 3d22  rt -->.<a href="
-00000800: 6874 7470 733a 2f2f 3130 7377 3174 6370  https://10sw1tcp
-00000810: 6c64 342e 7479 7065 666f 726d 2e63 6f6d  ld4.typeform.com
-00000820: 2f74 6f2f 4547 4145 5265 4d37 3f75 746d  /to/EGAEReM7?utm
-00000830: 5f73 6f75 7263 653d 7265 6164 6d65 2675  _source=readme&u
-00000840: 746d 5f6d 6564 6975 6d3d 6769 7468 7562  tm_medium=github
-00000850: 2675 746d 5f63 616d 7061 6967 6e3d 7573  &utm_campaign=us
-00000860: 6572 2532 3065 7870 6572 6965 6e63 6526  er%20experience&
-00000870: 7574 6d5f 7465 726d 3d66 6562 3230 3233  utm_term=feb2023
-00000880: 2675 746d 5f63 6f6e 7465 6e74 3d73 7572  &utm_content=sur
-00000890: 7665 7922 3e0a 2020 3c69 6d67 2073 7263  vey">.  <img src
-000008a0: 3d22 2e2f 2e67 6974 6875 622f 6261 6e6e  ="./.github/bann
-000008b0: 6572 2e73 7667 3f72 6177 3d74 7275 6522  er.svg?raw=true"
-000008c0: 3e0a 3c2f 613e 0a3c 212d 2d20 7375 7276  >.</a>.<!-- surv
-000008d0: 6579 2062 616e 6e65 7220 7374 6172 7420  ey banner start 
-000008e0: 2d2d 3e0a 0a3c 7020 616c 6967 6e3d 2263  -->..<p align="c
-000008f0: 656e 7465 7222 3e0a 3c61 2068 7265 663d  enter">.<a href=
-00000900: 2268 7474 7073 3a2f 2f64 6f63 732e 636d  "https://docs.cm
-00000910: 6f6e 2e61 6922 3e3c 696d 6720 7372 633d  on.ai"><img src=
-00000920: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000930: 636f 6d2f 636d 6f6e 2d61 692f 636d 6f6e  com/cmon-ai/cmon
-00000940: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-00000950: 732f 5f73 7461 7469 632f 6c6f 676f 2d6c  s/_static/logo-l
-00000960: 6967 6874 2e73 7667 3f72 6177 3d74 7275  ight.svg?raw=tru
-00000970: 6522 2061 6c74 3d22 436d 6f6e 206c 6f67  e" alt="Cmon log
-00000980: 6f3a 2042 7569 6c64 206d 756c 7469 6d6f  o: Build multimo
-00000990: 6461 6c20 4149 2073 6572 7669 6365 7320  dal AI services 
-000009a0: 7669 6120 636c 6f75 6420 6e61 7469 7665  via cloud native
-000009b0: 2074 6563 686e 6f6c 6f67 6965 7320 c2b7   technologies ..
-000009c0: 204e 6575 7261 6c20 5365 6172 6368 20c2   Neural Search .
-000009d0: b720 4765 6e65 7261 7469 7665 2041 4920  . Generative AI 
-000009e0: c2b7 2043 6c6f 7564 204e 6174 6976 6522  .. Cloud Native"
-000009f0: 2077 6964 7468 3d22 3135 3070 7822 3e3c   width="150px"><
-00000a00: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
-00000a10: 676e 3d22 6365 6e74 6572 223e 0a3c 623e  gn="center">.<b>
-00000a20: 4275 696c 6420 6d75 6c74 696d 6f64 616c  Build multimodal
-00000a30: 2041 4920 7365 7276 6963 6573 2077 6974   AI services wit
-00000a40: 6820 636c 6f75 6420 6e61 7469 7665 2074  h cloud native t
-00000a50: 6563 686e 6f6c 6f67 6965 733c 2f62 3e0a  echnologies</b>.
-00000a60: 3c2f 703e 0a0a 3c70 2061 6c69 676e 3d63  </p>..<p align=c
-00000a70: 656e 7465 723e 0a3c 6120 6872 6566 3d22  enter>.<a href="
-00000a80: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000a90: 2f70 726f 6a65 6374 2f63 6d6f 6e2f 223e  /project/cmon/">
-00000aa0: 3c69 6d67 2061 6c74 3d22 5079 5049 2220  <img alt="PyPI" 
-00000ab0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000ac0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000ad0: 2f76 2f63 6d6f 6e3f 6c61 6265 6c3d 5265  /v/cmon?label=Re
-00000ae0: 6c65 6173 6526 7374 796c 653d 666c 6174  lease&style=flat
-00000af0: 2d73 7175 6172 6522 3e3c 2f61 3e0a 3c21  -square"></a>.<!
-00000b00: 2d2d 3c61 2068 7265 663d 2268 7474 7073  --<a href="https
-00000b10: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000b20: 2f63 6d6f 6e2d 6169 2f63 6d6f 6e22 3e3c  /cmon-ai/cmon"><
-00000b30: 696d 6720 616c 743d 2243 6f64 6563 6f76  img alt="Codecov
-00000b40: 2062 7261 6e63 6822 2073 7263 3d22 6874   branch" src="ht
-00000b50: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000b60: 732e 696f 2f63 6f64 6563 6f76 2f63 2f67  s.io/codecov/c/g
-00000b70: 6974 6875 622f 636d 6f6e 2d61 692f 636d  ithub/cmon-ai/cm
-00000b80: 6f6e 2f6d 6173 7465 723f 266c 6f67 6f3d  on/master?&logo=
-00000b90: 436f 6465 636f 7626 6c6f 676f 436f 6c6f  Codecov&logoColo
-00000ba0: 723d 7768 6974 6526 7374 796c 653d 666c  r=white&style=fl
-00000bb0: 6174 2d73 7175 6172 6522 3e3c 2f61 3e2d  at-square"></a>-
-00000bc0: 2d3e 0a3c 6120 6872 6566 3d22 6874 7470  ->.<a href="http
-00000bd0: 733a 2f2f 6469 7363 6f72 642e 636d 6f6e  s://discord.cmon
-00000be0: 2e61 6922 3e3c 696d 6720 7372 633d 2268  .ai"><img src="h
-00000bf0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000c00: 6473 2e69 6f2f 6469 7363 6f72 642f 3131  ds.io/discord/11
-00000c10: 3036 3534 3232 3230 3131 3233 3032 3133  0654222011230213
-00000c20: 303f 6c6f 676f 3d64 6973 636f 7264 266c  0?logo=discord&l
-00000c30: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2673  ogoColor=white&s
-00000c40: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000c50: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00000c60: 6874 7470 733a 2f2f 7079 7069 7374 6174  https://pypistat
-00000c70: 732e 6f72 672f 7061 636b 6167 6573 2f63  s.org/packages/c
-00000c80: 6d6f 6e22 3e3c 696d 6720 616c 743d 2250  mon"><img alt="P
-00000c90: 7950 4920 2d20 446f 776e 6c6f 6164 7320  yPI - Downloads 
-00000ca0: 6672 6f6d 206f 6666 6963 6961 6c20 7079  from official py
-00000cb0: 7069 7374 6174 7322 2073 7263 3d22 6874  pistats" src="ht
-00000cc0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000cd0: 732e 696f 2f70 7970 692f 646d 2f63 6d6f  s.io/pypi/dm/cmo
-00000ce0: 6e3f 7374 796c 653d 666c 6174 2d73 7175  n?style=flat-squ
-00000cf0: 6172 6522 3e3c 2f61 3e0a 3c61 2068 7265  are"></a>.<a hre
-00000d00: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000d10: 622e 636f 6d2f 636d 6f6e 2d61 692f 636d  b.com/cmon-ai/cm
-00000d20: 6f6e 2f61 6374 696f 6e73 2f77 6f72 6b66  on/actions/workf
-00000d30: 6c6f 7773 2f63 642e 796d 6c22 3e3c 696d  lows/cd.yml"><im
-00000d40: 6720 616c 743d 2247 6974 6875 6220 4344  g alt="Github CD
-00000d50: 2073 7461 7475 7322 2073 7263 3d22 6874   status" src="ht
-00000d60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000d70: 2f63 6d6f 6e2d 6169 2f63 6d6f 6e2f 6163  /cmon-ai/cmon/ac
-00000d80: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000d90: 6364 2e79 6d6c 2f62 6164 6765 2e73 7667  cd.yml/badge.svg
-00000da0: 223e 3c2f 613e 0a3c 2f70 3e0a 0a3c 212d  "></a>.</p>..<!-
-00000db0: 2d20 7374 6172 7420 636d 6f6e 2d64 6573  - start cmon-des
-00000dc0: 6372 6970 7469 6f6e 202d 2d3e 0a0a 436d  cription -->..Cm
-00000dd0: 6f6e 206c 6574 7320 796f 7520 6275 696c  on lets you buil
-00000de0: 6420 6d75 6c74 696d 6f64 616c 205b 2a2a  d multimodal [**
-00000df0: 4149 2073 6572 7669 6365 732a 2a5d 2823  AI services**](#
-00000e00: 6275 696c 642d 6169 2d73 6572 7669 6365  build-ai-service
-00000e10: 7329 2061 6e64 205b 2a2a 7069 7065 6c69  s) and [**pipeli
-00000e20: 6e65 732a 2a5d 2823 6275 696c 642d 612d  nes**](#build-a-
-00000e30: 7069 7065 6c69 6e65 2920 7468 6174 2063  pipeline) that c
-00000e40: 6f6d 6d75 6e69 6361 7465 2076 6961 2067  ommunicate via g
-00000e50: 5250 432c 2048 5454 5020 616e 6420 5765  RPC, HTTP and We
-00000e60: 6253 6f63 6b65 7473 2c20 7468 656e 2073  bSockets, then s
-00000e70: 6361 6c65 2074 6865 6d20 7570 2061 6e64  cale them up and
-00000e80: 2064 6570 6c6f 7920 746f 2070 726f 6475   deploy to produ
-00000e90: 6374 696f 6e2e 2059 6f75 2063 616e 2066  ction. You can f
-00000ea0: 6f63 7573 206f 6e20 796f 7572 206c 6f67  ocus on your log
-00000eb0: 6963 2061 6e64 2061 6c67 6f72 6974 686d  ic and algorithm
-00000ec0: 732c 2077 6974 686f 7574 2077 6f72 7279  s, without worry
-00000ed0: 696e 6720 6162 6f75 7420 7468 6520 696e  ing about the in
-00000ee0: 6672 6173 7472 7563 7475 7265 2063 6f6d  frastructure com
-00000ef0: 706c 6578 6974 792e 0a0a 215b 5d28 2e2f  plexity...![](./
-00000f00: 2e67 6974 6875 622f 696d 6167 6573 2f62  .github/images/b
-00000f10: 7569 6c64 2d64 6570 6c6f 792e 706e 6729  uild-deploy.png)
-00000f20: 0a0a 436d 6f6e 2070 726f 7669 6465 7320  ..Cmon provides 
-00000f30: 6120 736d 6f6f 7468 2050 7974 686f 6e69  a smooth Pythoni
-00000f40: 6320 6578 7065 7269 656e 6365 2074 7261  c experience tra
-00000f50: 6e73 6974 696f 6e69 6e67 2066 726f 6d20  nsitioning from 
-00000f60: 6c6f 6361 6c20 6465 706c 6f79 6d65 6e74  local deployment
-00000f70: 2074 6f20 6164 7661 6e63 6564 206f 7263   to advanced orc
-00000f80: 6865 7374 7261 7469 6f6e 2066 7261 6d65  hestration frame
-00000f90: 776f 726b 7320 6c69 6b65 2044 6f63 6b65  works like Docke
-00000fa0: 722d 436f 6d70 6f73 652c 204b 7562 6572  r-Compose, Kuber
-00000fb0: 6e65 7465 732c 206f 7220 436d 6f6e 2041  netes, or Cmon A
-00000fc0: 4920 436c 6f75 642e 2043 6d6f 6e20 6d61  I Cloud. Cmon ma
-00000fd0: 6b65 7320 6164 7661 6e63 6564 2073 6f6c  kes advanced sol
-00000fe0: 7574 696f 6e20 656e 6769 6e65 6572 696e  ution engineerin
-00000ff0: 6720 616e 6420 636c 6f75 642d 6e61 7469  g and cloud-nati
-00001000: 7665 2074 6563 686e 6f6c 6f67 6965 7320  ve technologies 
-00001010: 6163 6365 7373 6962 6c65 2074 6f20 6576  accessible to ev
-00001020: 6572 7920 6465 7665 6c6f 7065 722e 0a0a  ery developer...
-00001030: 2d20 4275 696c 6420 6170 706c 6963 6174  - Build applicat
-00001040: 696f 6e73 2066 6f72 2061 6e79 205b 6461  ions for any [da
-00001050: 7461 2074 7970 655d 2868 7474 7073 3a2f  ta type](https:/
-00001060: 2f64 6f63 732e 646f 6361 7272 6179 2e6f  /docs.docarray.o
-00001070: 7267 2f64 6174 615f 7479 7065 732f 6669  rg/data_types/fi
-00001080: 7273 745f 7374 6570 732f 292c 2061 6e79  rst_steps/), any
-00001090: 206d 6169 6e73 7472 6561 6d20 5b64 6565   mainstream [dee
-000010a0: 7020 6c65 6172 6e69 6e67 2066 7261 6d65  p learning frame
-000010b0: 776f 726b 5d28 292c 2061 6e64 2061 6e79  work](), and any
-000010c0: 205b 7072 6f74 6f63 6f6c 5d28 6874 7470   [protocol](http
-000010d0: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-000010e0: 2f63 6f6e 6365 7074 732f 7365 7276 696e  /concepts/servin
-000010f0: 672f 6761 7465 7761 792f 2373 6574 2d70  g/gateway/#set-p
-00001100: 726f 746f 636f 6c2d 696e 2d70 7974 686f  rotocol-in-pytho
-00001110: 6e29 2e0a 2d20 4465 7369 676e 2068 6967  n)..- Design hig
-00001120: 682d 7065 7266 6f72 6d61 6e63 6520 6d69  h-performance mi
-00001130: 6372 6f73 6572 7669 6365 732c 2077 6974  croservices, wit
-00001140: 6820 5b65 6173 7920 7363 616c 696e 675d  h [easy scaling]
-00001150: 2868 7474 7073 3a2f 2f64 6f63 732e 636d  (https://docs.cm
-00001160: 6f6e 2e61 692f 636f 6e63 6570 7473 2f6f  on.ai/concepts/o
-00001170: 7263 6865 7374 7261 7469 6f6e 2f73 6361  rchestration/sca
-00001180: 6c65 2d6f 7574 2f29 2c20 6475 706c 6578  le-out/), duplex
-00001190: 2063 6c69 656e 742d 7365 7276 6572 2073   client-server s
-000011a0: 7472 6561 6d69 6e67 2c20 616e 6420 6173  treaming, and as
-000011b0: 796e 632f 6e6f 6e2d 626c 6f63 6b69 6e67  ync/non-blocking
-000011c0: 2064 6174 6120 7072 6f63 6573 7369 6e67   data processing
-000011d0: 206f 7665 7220 6479 6e61 6d69 6320 666c   over dynamic fl
-000011e0: 6f77 732e 0a2d 2044 6f63 6b65 7220 636f  ows..- Docker co
-000011f0: 6e74 6169 6e65 7220 696e 7465 6772 6174  ntainer integrat
-00001200: 696f 6e20 7669 6120 5b45 7865 6375 746f  ion via [Executo
-00001210: 7220 4875 625d 2868 7474 7073 3a2f 2f63  r Hub](https://c
-00001220: 6c6f 7564 2e63 6d6f 6e2e 6169 292c 204f  loud.cmon.ai), O
-00001230: 7065 6e54 656c 656d 6574 7279 2f50 726f  penTelemetry/Pro
-00001240: 6d65 7468 6575 7320 6f62 7365 7276 6162  metheus observab
-00001250: 696c 6974 792c 2061 6e64 2066 6173 7420  ility, and fast 
-00001260: 4b75 6265 726e 6574 6573 2f44 6f63 6b65  Kubernetes/Docke
-00001270: 722d 436f 6d70 6f73 6520 6465 706c 6f79  r-Compose deploy
-00001280: 6d65 6e74 2e0a 2d20 4350 552f 4750 5520  ment..- CPU/GPU 
-00001290: 686f 7374 696e 6720 7669 6120 5b43 6d6f  hosting via [Cmo
-000012a0: 6e20 4149 2043 6c6f 7564 5d28 6874 7470  n AI Cloud](http
-000012b0: 733a 2f2f 636c 6f75 642e 636d 6f6e 2e61  s://cloud.cmon.a
-000012c0: 6929 2e0a 0a3c 6465 7461 696c 733e 0a20  i)...<details>. 
-000012d0: 2020 203c 7375 6d6d 6172 793e 3c73 7472     <summary><str
-000012e0: 6f6e 673e 5761 6974 2c20 686f 7720 6973  ong>Wait, how is
-000012f0: 2043 6d6f 6e20 6469 6666 6572 656e 7420   Cmon different 
-00001300: 6672 6f6d 2046 6173 7441 5049 3f3c 2f73  from FastAPI?</s
-00001310: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
-00001320: 0a43 6d6f 6e27 7320 7661 6c75 6520 7072  .Cmon's value pr
-00001330: 6f70 6f73 6974 696f 6e20 6d61 7920 7365  oposition may se
-00001340: 656d 2071 7569 7465 2073 696d 696c 6172  em quite similar
-00001350: 2074 6f20 7468 6174 206f 6620 4661 7374   to that of Fast
-00001360: 4150 492e 2048 6f77 6576 6572 2c20 7468  API. However, th
-00001370: 6572 6520 6172 6520 7365 7665 7261 6c20  ere are several 
-00001380: 6675 6e64 616d 656e 7461 6c20 6469 6666  fundamental diff
-00001390: 6572 656e 6365 733a 0a0a 202a 2a44 6174  erences:.. **Dat
-000013a0: 6120 7374 7275 6374 7572 6520 616e 6420  a structure and 
-000013b0: 636f 6d6d 756e 6963 6174 696f 6e20 7072  communication pr
-000013c0: 6f74 6f63 6f6c 732a 2a0a 2020 2d20 4661  otocols**.  - Fa
-000013d0: 7374 4150 4920 636f 6d6d 756e 6963 6174  stAPI communicat
-000013e0: 696f 6e20 7265 6c69 6573 206f 6e20 5079  ion relies on Py
-000013f0: 6461 6e74 6963 2061 6e64 2043 6d6f 6e20  dantic and Cmon 
-00001400: 7265 6c69 6573 206f 6e20 5b44 6f63 4172  relies on [DocAr
-00001410: 7261 795d 2868 7474 7073 3a2f 2f67 6974  ray](https://git
-00001420: 6875 622e 636f 6d2f 646f 6361 7272 6179  hub.com/docarray
-00001430: 2f64 6f63 6172 7261 7929 2061 6c6c 6f77  /docarray) allow
-00001440: 696e 6720 436d 6f6e 2074 6f20 7375 7070  ing Cmon to supp
-00001450: 6f72 7420 6d75 6c74 6970 6c65 2070 726f  ort multiple pro
-00001460: 746f 636f 6c73 0a20 2074 6f20 6578 706f  tocols.  to expo
-00001470: 7365 2069 7473 2073 6572 7669 6365 732e  se its services.
-00001480: 0a0a 202a 2a41 6476 616e 6365 6420 6f72  .. **Advanced or
-00001490: 6368 6573 7472 6174 696f 6e20 616e 6420  chestration and 
-000014a0: 7363 616c 696e 6720 6361 7061 6269 6c69  scaling capabili
-000014b0: 7469 6573 2a2a 0a20 202d 2043 6d6f 6e20  ties**.  - Cmon 
-000014c0: 6c65 7473 2079 6f75 2064 6570 6c6f 7920  lets you deploy 
-000014d0: 6170 706c 6963 6174 696f 6e73 2066 6f72  applications for
-000014e0: 6d65 6420 6672 6f6d 206d 756c 7469 706c  med from multipl
-000014f0: 6520 6d69 6372 6f73 6572 7669 6365 7320  e microservices 
-00001500: 7468 6174 2063 616e 2062 6520 636f 6e74  that can be cont
-00001510: 6169 6e65 7269 7a65 6420 616e 6420 7363  ainerized and sc
-00001520: 616c 6564 2069 6e64 6570 656e 6465 6e74  aled independent
-00001530: 6c79 2e0a 2020 2d20 436d 6f6e 2061 6c6c  ly..  - Cmon all
-00001540: 6f77 7320 796f 7520 746f 2065 6173 696c  ows you to easil
-00001550: 7920 636f 6e74 6169 6e65 7269 7a65 2061  y containerize a
-00001560: 6e64 206f 7263 6865 7374 7261 7465 2079  nd orchestrate y
-00001570: 6f75 7220 7365 7276 6963 6573 2c20 7072  our services, pr
-00001580: 6f76 6964 696e 6720 636f 6e63 7572 7265  oviding concurre
-00001590: 6e63 7920 616e 6420 7363 616c 6162 696c  ncy and scalabil
-000015a0: 6974 792e 0a0a 202a 2a4a 6f75 726e 6579  ity... **Journey
-000015b0: 2074 6f20 7468 6520 636c 6f75 642a 2a0a   to the cloud**.
-000015c0: 2020 2d20 436d 6f6e 2070 726f 7669 6465    - Cmon provide
-000015d0: 7320 6120 736d 6f6f 7468 2074 7261 6e73  s a smooth trans
-000015e0: 6974 696f 6e20 6672 6f6d 206c 6f63 616c  ition from local
-000015f0: 2064 6576 656c 6f70 6d65 6e74 2028 7573   development (us
-00001600: 696e 6720 5b44 6f63 4172 7261 795d 2868  ing [DocArray](h
-00001610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001620: 6d2f 646f 6361 7272 6179 2f64 6f63 6172  m/docarray/docar
-00001630: 7261 7929 2920 746f 206c 6f63 616c 2073  ray)) to local s
-00001640: 6572 7669 6e67 2075 7369 6e67 2028 436d  erving using (Cm
-00001650: 6f6e 2773 206f 7263 6865 7374 7261 7469  on's orchestrati
-00001660: 6f6e 206c 6179 6572 290a 2020 746f 2068  on layer).  to h
-00001670: 6176 696e 6720 7072 6f64 7563 7469 6f6e  aving production
-00001680: 2d72 6561 6479 2073 6572 7669 6365 7320  -ready services 
-00001690: 6279 2075 7369 6e67 204b 7562 6572 6e65  by using Kuberne
-000016a0: 7465 7320 6361 7061 6369 7479 2074 6f20  tes capacity to 
-000016b0: 6f72 6368 6573 7472 6174 6520 7468 6520  orchestrate the 
-000016c0: 6c69 6665 7469 6d65 206f 6620 636f 6e74  lifetime of cont
-000016d0: 6169 6e65 7273 2e0a 2020 2d20 4279 2075  ainers..  - By u
-000016e0: 7369 6e67 205b 436d 6f6e 2041 4920 436c  sing [Cmon AI Cl
-000016f0: 6f75 645d 2868 7474 7073 3a2f 2f63 6c6f  oud](https://clo
-00001700: 7564 2e63 6d6f 6e2e 6169 2920 796f 7520  ud.cmon.ai) you 
-00001710: 6861 7665 2061 6363 6573 7320 746f 2073  have access to s
-00001720: 6361 6c61 626c 6520 616e 6420 7365 7276  calable and serv
-00001730: 6572 6c65 7373 2064 6570 6c6f 796d 656e  erless deploymen
-00001740: 7473 206f 6620 796f 7572 2061 7070 6c69  ts of your appli
-00001750: 6361 7469 6f6e 7320 696e 206f 6e65 2063  cations in one c
-00001760: 6f6d 6d61 6e64 2e0a 3c2f 6465 7461 696c  ommand..</detail
-00001770: 733e 0a0a 3c21 2d2d 2065 6e64 2063 6d6f  s>..<!-- end cmo
-00001780: 6e2d 6465 7363 7269 7074 696f 6e20 2d2d  n-description --
-00001790: 3e0a 0a23 2320 5b44 6f63 756d 656e 7461  >..## [Documenta
-000017a0: 7469 6f6e 5d28 6874 7470 733a 2f2f 646f  tion](https://do
-000017b0: 6373 2e63 6d6f 6e2e 6169 290a 0a23 2320  cs.cmon.ai)..## 
-000017c0: 496e 7374 616c 6c20 0a0a 4e6f 7465 3a20  Install ..Note: 
-000017d0: 2857 696e 646f 7773 2920 6e6f 7420 7375  (Windows) not su
-000017e0: 7070 6f72 7465 6420 6174 2074 6869 7320  pported at this 
-000017f0: 6d6f 6d65 6e74 2120 596f 7520 6d61 7920  moment! You may 
-00001800: 7265 7175 6972 6520 746f 2069 6e73 7461  require to insta
-00001810: 6c6c 2069 7420 6f6e 2028 5753 4c29 2e0a  ll it on (WSL)..
-00001820: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-00001830: 7461 6c6c 2063 6d6f 6e0a 6060 600a 0a46  tall cmon.```..F
-00001840: 696e 6420 6d6f 7265 2069 6e73 7461 6c6c  ind more install
-00001850: 206f 7074 696f 6e73 206f 6e20 5b41 7070   options on [App
-00001860: 6c65 2053 696c 6963 6f6e 5d28 6874 7470  le Silicon](http
-00001870: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-00001880: 2f67 6574 2d73 7461 7274 6564 2f69 6e73  /get-started/ins
-00001890: 7461 6c6c 2f61 7070 6c65 2d73 696c 6963  tall/apple-silic
-000018a0: 6f6e 2d6d 312d 6d32 2f29 0a0a 0a23 2320  on-m1-m2/)...## 
-000018b0: 4765 7420 5374 6172 7465 640a 0a23 2323  Get Started..###
-000018c0: 2042 6173 6963 2043 6f6e 6365 7074 730a   Basic Concepts.
-000018d0: 0a43 6d6f 6e20 6861 7320 666f 7572 2066  .Cmon has four f
-000018e0: 756e 6461 6d65 6e74 616c 2063 6f6e 6365  undamental conce
-000018f0: 7074 733a 0a0a 2d20 4120 5b2a 2a44 6f63  pts:..- A [**Doc
-00001900: 756d 656e 742a 2a5d 2868 7474 7073 3a2f  ument**](https:/
-00001910: 2f64 6f63 6172 7261 792e 636d 6f6e 2e61  /docarray.cmon.a
-00001920: 692f 2920 2866 726f 6d20 5b44 6f63 4172  i/) (from [DocAr
-00001930: 7261 795d 2868 7474 7073 3a2f 2f67 6974  ray](https://git
-00001940: 6875 622e 636f 6d2f 646f 6361 7272 6179  hub.com/docarray
-00001950: 2f64 6f63 6172 7261 7929 2920 6973 2074  /docarray)) is t
-00001960: 6865 2069 6e70 7574 2f6f 7574 7075 7420  he input/output 
-00001970: 666f 726d 6174 2069 6e20 436d 6f6e 2e0a  format in Cmon..
-00001980: 2d20 416e 205b 2a2a 4578 6563 7574 6f72  - An [**Executor
-00001990: 2a2a 5d28 6874 7470 733a 2f2f 646f 6373  **](https://docs
-000019a0: 2e63 6d6f 6e2e 6169 2f63 6f6e 6365 7074  .cmon.ai/concept
-000019b0: 732f 7365 7276 696e 672f 6578 6563 7574  s/serving/execut
-000019c0: 6f72 2f29 2069 7320 6120 5079 7468 6f6e  or/) is a Python
-000019d0: 2063 6c61 7373 2074 6861 7420 7472 616e   class that tran
-000019e0: 7366 6f72 6d73 2061 6e64 2070 726f 6365  sforms and proce
-000019f0: 7373 6573 2044 6f63 756d 656e 7473 2e0a  sses Documents..
-00001a00: 2d20 4120 5b2a 2a44 6570 6c6f 796d 656e  - A [**Deploymen
-00001a10: 742a 2a5d 2868 7474 7073 3a2f 2f64 6f63  t**](https://doc
-00001a20: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00001a30: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
-00001a40: 2f64 6570 6c6f 796d 656e 7429 2073 6572  /deployment) ser
-00001a50: 7665 7320 6120 7369 6e67 6c65 2045 7865  ves a single Exe
-00001a60: 6375 746f 722c 2077 6869 6c65 2061 205b  cutor, while a [
-00001a70: 2a2a 466c 6f77 2a2a 5d28 6874 7470 733a  **Flow**](https:
-00001a80: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-00001a90: 6f6e 6365 7074 732f 6f72 6368 6573 7472  oncepts/orchestr
-00001aa0: 6174 696f 6e2f 666c 6f77 2f29 2073 6572  ation/flow/) ser
-00001ab0: 7665 7320 4578 6563 7574 6f72 7320 6368  ves Executors ch
-00001ac0: 6169 6e65 6420 696e 746f 2061 2070 6970  ained into a pip
-00001ad0: 656c 696e 652e 0a0a 0a5b 5468 6520 6675  eline....[The fu
-00001ae0: 6c6c 2067 6c6f 7373 6172 7920 6973 2065  ll glossary is e
-00001af0: 7870 6c61 696e 6564 2068 6572 655d 2868  xplained here](h
-00001b00: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00001b10: 2e61 692f 636f 6e63 6570 7473 2f70 7265  .ai/concepts/pre
-00001b20: 6c69 6d69 6e61 7269 6573 2f23 292e 0a0a  liminaries/#)...
-00001b30: 2323 2320 4275 696c 6420 4149 2053 6572  ### Build AI Ser
-00001b40: 7669 6365 730a 3c21 2d2d 2073 7461 7274  vices.<!-- start
-00001b50: 2062 7569 6c64 2d61 692d 7365 7276 6963   build-ai-servic
-00001b60: 6573 202d 2d3e 0a0a 4c65 7427 7320 6275  es -->..Let's bu
-00001b70: 696c 6420 6120 6661 7374 2c20 7265 6c69  ild a fast, reli
-00001b80: 6162 6c65 2061 6e64 2073 6361 6c61 626c  able and scalabl
-00001b90: 6520 6752 5043 2d62 6173 6564 2041 4920  e gRPC-based AI 
-00001ba0: 7365 7276 6963 652e 2049 6e20 436d 6f6e  service. In Cmon
-00001bb0: 2077 6520 6361 6c6c 2074 6869 7320 616e   we call this an
-00001bc0: 202a 2a5b 4578 6563 7574 6f72 5d28 6874   **[Executor](ht
-00001bd0: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
-00001be0: 6169 2f63 6f6e 6365 7074 732f 6578 6563  ai/concepts/exec
-00001bf0: 7574 6f72 2f29 2a2a 2e20 4f75 7220 7369  utor/)**. Our si
-00001c00: 6d70 6c65 2045 7865 6375 746f 7220 7769  mple Executor wi
-00001c10: 6c6c 2077 7261 7020 7468 6520 5b53 7461  ll wrap the [Sta
-00001c20: 626c 654c 4d5d 2868 7474 7073 3a2f 2f68  bleLM](https://h
-00001c30: 7567 6769 6e67 6661 6365 2e63 6f2f 7374  uggingface.co/st
-00001c40: 6162 696c 6974 7961 692f 7374 6162 6c65  abilityai/stable
-00001c50: 6c6d 2d62 6173 652d 616c 7068 612d 3362  lm-base-alpha-3b
-00001c60: 2920 4c4c 4d20 6672 6f6d 2053 7461 6269  ) LLM from Stabi
-00001c70: 6c69 7479 2041 492e 2057 6527 6c6c 2074  lity AI. We'll t
-00001c80: 6865 6e20 7573 6520 6120 2a2a 4465 706c  hen use a **Depl
-00001c90: 6f79 6d65 6e74 2a2a 2074 6f20 7365 7276  oyment** to serv
-00001ca0: 6520 6974 2e0a 0a21 5b5d 282e 2f2e 6769  e it...![](./.gi
-00001cb0: 7468 7562 2f69 6d61 6765 732f 6465 706c  thub/images/depl
-00001cc0: 6f79 6d65 6e74 2d64 6961 6772 616d 2e70  oyment-diagram.p
-00001cd0: 6e67 290a 0a3e 202a 2a4e 6f74 652a 2a0a  ng)..> **Note**.
-00001ce0: 3e20 4120 4465 706c 6f79 6d65 6e74 2073  > A Deployment s
-00001cf0: 6572 7665 7320 6a75 7374 206f 6e65 2045  erves just one E
-00001d00: 7865 6375 746f 722e 2054 6f20 636f 6d62  xecutor. To comb
-00001d10: 696e 6520 6d75 6c74 6970 6c65 2045 7865  ine multiple Exe
-00001d20: 6375 746f 7273 2069 6e74 6f20 6120 7069  cutors into a pi
-00001d30: 7065 6c69 6e65 2061 6e64 2073 6572 7665  peline and serve
-00001d40: 2074 6861 742c 2075 7365 2061 205b 466c   that, use a [Fl
-00001d50: 6f77 5d28 2362 7569 6c64 2d61 2d70 6970  ow](#build-a-pip
-00001d60: 656c 696e 6529 2e0a 0a4c 6574 2773 2069  eline)...Let's i
-00001d70: 6d70 6c65 6d65 6e74 2074 6865 2073 6572  mplement the ser
-00001d80: 7669 6365 2773 206c 6f67 6963 3a0a 0a3c  vice's logic:..<
-00001d90: 7461 626c 653e 0a3c 7472 3e0a 3c74 683e  table>.<tr>.<th>
-00001da0: 3c63 6f64 653e 6578 6563 7574 6f72 2e70  <code>executor.p
-00001db0: 793c 2f63 6f64 653e 3c2f 7468 3e20 0a3c  y</code></th> .<
-00001dc0: 7472 3e0a 3c74 643e 0a0a 6060 6070 7974  tr>.<td>..```pyt
-00001dd0: 686f 6e0a 6672 6f6d 2063 6d6f 6e20 696d  hon.from cmon im
-00001de0: 706f 7274 2045 7865 6375 746f 722c 2072  port Executor, r
-00001df0: 6571 7565 7374 730a 6672 6f6d 2064 6f63  equests.from doc
-00001e00: 6172 7261 7920 696d 706f 7274 2044 6f63  array import Doc
-00001e10: 756d 656e 7441 7272 6179 0a0a 6672 6f6d  umentArray..from
-00001e20: 2074 7261 6e73 666f 726d 6572 7320 696d   transformers im
-00001e30: 706f 7274 2070 6970 656c 696e 650a 0a0a  port pipeline...
-00001e40: 636c 6173 7320 5374 6162 6c65 4c4d 2845  class StableLM(E
-00001e50: 7865 6375 746f 7229 3a0a 0a20 2020 2064  xecutor):..    d
-00001e60: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00001e70: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00001e80: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001e90: 6e69 745f 5f28 2a2a 6b77 6172 6773 290a  nit__(**kwargs).
-00001ea0: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
-00001eb0: 6572 6174 6f72 203d 2070 6970 656c 696e  erator = pipelin
-00001ec0: 6528 2774 6578 742d 6765 6e65 7261 7469  e('text-generati
-00001ed0: 6f6e 272c 206d 6f64 656c 3d27 7374 6162  on', model='stab
-00001ee0: 6c65 6c6d 2d33 6227 290a 0a20 2020 2040  lelm-3b')..    @
-00001ef0: 7265 7175 6573 7473 0a20 2020 2064 6566  requests.    def
-00001f00: 2067 656e 6572 6174 6528 7365 6c66 2c20   generate(self, 
-00001f10: 646f 6373 3a20 446f 6375 6d65 6e74 4172  docs: DocumentAr
-00001f20: 7261 792c 202a 2a6b 7761 7267 7329 3a0a  ray, **kwargs):.
-00001f30: 2020 2020 2020 2020 6765 6e65 7261 7465          generate
-00001f40: 645f 7465 7874 203d 2073 656c 662e 6765  d_text = self.ge
-00001f50: 6e65 7261 746f 7228 646f 6373 2e74 6578  nerator(docs.tex
-00001f60: 7473 290a 2020 2020 2020 2020 646f 6373  ts).        docs
-00001f70: 2e74 6578 7473 203d 205b 6765 6e5b 305d  .texts = [gen[0]
-00001f80: 5b27 6765 6e65 7261 7465 645f 7465 7874  ['generated_text
-00001f90: 275d 2066 6f72 2067 656e 2069 6e20 6765  '] for gen in ge
-00001fa0: 6e65 7261 7465 645f 7465 7874 5d0a 6060  nerated_text].``
-00001fb0: 600a 0a3c 2f74 643e 0a3c 2f74 723e 0a3c  `..</td>.</tr>.<
-00001fc0: 2f74 6162 6c65 3e0a 0a54 6865 6e20 7765  /table>..Then we
-00001fd0: 2064 6570 6c6f 7920 6974 2077 6974 6820   deploy it with 
-00001fe0: 6569 7468 6572 2074 6865 2050 7974 686f  either the Pytho
-00001ff0: 6e20 4150 4920 6f72 2059 414d 4c3a 0a3c  n API or YAML:.<
-00002000: 6469 7620 636c 6173 733d 2274 6162 6c65  div class="table
-00002010: 2d77 7261 7070 6572 223e 0a3c 7461 626c  -wrapper">.<tabl
-00002020: 653e 0a3c 7472 3e0a 3c74 683e 2050 7974  e>.<tr>.<th> Pyt
-00002030: 686f 6e20 4150 493a 203c 636f 6465 3e64  hon API: <code>d
-00002040: 6570 6c6f 796d 656e 742e 7079 3c2f 636f  eployment.py</co
-00002050: 6465 3e20 3c2f 7468 3e20 0a3c 7468 3e20  de> </th> .<th> 
-00002060: 5941 4d4c 3a20 3c63 6f64 653e 6465 706c  YAML: <code>depl
-00002070: 6f79 6d65 6e74 2e79 6d6c 3c2f 636f 6465  oyment.yml</code
-00002080: 3e20 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  > </th>.</tr>.<t
-00002090: 723e 0a3c 7464 3e0a 0a60 6060 7079 7468  r>.<td>..```pyth
-000020a0: 6f6e 0a66 726f 6d20 636d 6f6e 2069 6d70  on.from cmon imp
-000020b0: 6f72 7420 4465 706c 6f79 6d65 6e74 0a66  ort Deployment.f
-000020c0: 726f 6d20 6578 6563 7574 6f72 2069 6d70  rom executor imp
-000020d0: 6f72 7420 5374 6162 6c65 4c4d 0a0a 6465  ort StableLM..de
-000020e0: 7020 3d20 4465 706c 6f79 6d65 6e74 2875  p = Deployment(u
-000020f0: 7365 733d 5374 6162 6c65 4c4d 2c20 7469  ses=StableLM, ti
-00002100: 6d65 6f75 745f 7265 6164 793d 2d31 2c20  meout_ready=-1, 
-00002110: 706f 7274 3d31 3233 3435 290a 0a77 6974  port=12345)..wit
-00002120: 6820 6465 703a 0a20 2020 2064 6570 2e62  h dep:.    dep.b
-00002130: 6c6f 636b 2829 0a60 6060 0a0a 3c2f 7464  lock().```..</td
-00002140: 3e0a 3c74 643e 0a0a 6060 6079 616d 6c0a  >.<td>..```yaml.
-00002150: 6a74 7970 653a 2044 6570 6c6f 796d 656e  jtype: Deploymen
-00002160: 740a 7769 7468 3a0a 2020 7573 6573 3a20  t.with:.  uses: 
-00002170: 5374 6162 6c65 4c4d 0a20 2070 795f 6d6f  StableLM.  py_mo
-00002180: 6475 6c65 733a 0a20 2020 202d 2065 7865  dules:.    - exe
-00002190: 6375 746f 722e 7079 0a20 2074 696d 656f  cutor.py.  timeo
-000021a0: 7574 5f72 6561 6479 3a20 2d31 0a20 2070  ut_ready: -1.  p
-000021b0: 6f72 743a 2031 3233 3435 0a60 6060 0a0a  ort: 12345.```..
-000021c0: 416e 6420 7275 6e20 7468 6520 5941 4d4c  And run the YAML
-000021d0: 2044 6570 6c6f 796d 656e 7420 7769 7468   Deployment with
-000021e0: 2074 6865 2043 4c49 3a20 6063 6d6f 6e20   the CLI: `cmon 
-000021f0: 6465 706c 6f79 6d65 6e74 202d 2d75 7365  deployment --use
-00002200: 7320 6465 706c 6f79 6d65 6e74 2e79 6d6c  s deployment.yml
-00002210: 600a 0a3c 2f74 643e 0a3c 2f74 723e 0a3c  `..</td>.</tr>.<
-00002220: 2f74 6162 6c65 3e0a 3c2f 6469 763e 0a0a  /table>.</div>..
-00002230: 5573 6520 5b43 6d6f 6e20 436c 6965 6e74  Use [Cmon Client
-00002240: 5d28 6874 7470 733a 2f2f 646f 6373 2e63  ](https://docs.c
-00002250: 6d6f 6e2e 6169 2f63 6f6e 6365 7074 732f  mon.ai/concepts/
-00002260: 636c 6965 6e74 2f29 2074 6f20 6d61 6b65  client/) to make
-00002270: 2072 6571 7565 7374 7320 746f 2074 6865   requests to the
-00002280: 2073 6572 7669 6365 3a0a 0a60 6060 7079   service:..```py
-00002290: 7468 6f6e 0a66 726f 6d20 646f 6361 7272  thon.from docarr
-000022a0: 6179 2069 6d70 6f72 7420 446f 6375 6d65  ay import Docume
-000022b0: 6e74 0a66 726f 6d20 636d 6f6e 2069 6d70  nt.from cmon imp
-000022c0: 6f72 7420 436c 6965 6e74 0a0a 7072 6f6d  ort Client..prom
-000022d0: 7074 203d 2044 6f63 756d 656e 7428 0a20  pt = Document(. 
-000022e0: 2020 2074 6167 7320 3d20 7b27 7072 6f6d     tags = {'prom
-000022f0: 7074 273a 2027 7375 6767 6573 7420 616e  pt': 'suggest an
-00002300: 2069 6e74 6572 6573 7469 6e67 2069 6d61   interesting ima
-00002310: 6765 2067 656e 6572 6174 696f 6e20 7072  ge generation pr
-00002320: 6f6d 7074 2066 6f72 2061 206d 6f6e 6120  ompt for a mona 
-00002330: 6c69 7361 2076 6172 6961 6e74 277d 0a29  lisa variant'}.)
-00002340: 0a0a 636c 6965 6e74 203d 2043 6c69 656e  ..client = Clien
-00002350: 7428 706f 7274 3d31 3233 3435 2920 2023  t(port=12345)  #
-00002360: 2075 7365 2070 6f72 7420 6672 6f6d 206f   use port from o
-00002370: 7574 7075 7420 6162 6f76 650a 7265 7370  utput above.resp
-00002380: 6f6e 7365 203d 2063 6c69 656e 742e 706f  onse = client.po
-00002390: 7374 286f 6e3d 272f 272c 2069 6e70 7574  st(on='/', input
-000023a0: 733d 5b70 726f 6d70 745d 290a 0a70 7269  s=[prompt])..pri
-000023b0: 6e74 2872 6573 706f 6e73 655b 305d 2e74  nt(response[0].t
-000023c0: 6578 7429 0a60 6060 0a0a 6060 6074 6578  ext).```..```tex
-000023d0: 740a 6120 7374 6561 6d70 756e 6b20 7665  t.a steampunk ve
-000023e0: 7273 696f 6e20 6f66 2074 6865 204d 6f6e  rsion of the Mon
-000023f0: 6120 4c69 7361 2c20 696e 636f 7270 6f72  a Lisa, incorpor
-00002400: 6174 696e 6720 6d65 6368 616e 6963 616c  ating mechanical
-00002410: 2067 6561 7273 2c20 6272 6173 7320 656c   gears, brass el
-00002420: 656d 656e 7473 2c20 616e 6420 5669 6374  ements, and Vict
-00002430: 6f72 6961 6e20 6572 6120 636c 6f74 6869  orian era clothi
-00002440: 6e67 2064 6574 6169 6c73 0a60 6060 0a0a  ng details.```..
-00002450: 3c21 2d2d 2065 6e64 2062 7569 6c64 2d61  <!-- end build-a
-00002460: 692d 7365 7276 6963 6573 202d 2d3e 0a0a  i-services -->..
-00002470: 3e20 2a2a 4e6f 7465 2a2a 0a3e 2049 6e20  > **Note**.> In 
-00002480: 6120 6e6f 7465 626f 6f6b 2c20 796f 7520  a notebook, you 
-00002490: 6361 6e27 7420 7573 6520 6064 6570 6c6f  can't use `deplo
-000024a0: 796d 656e 742e 626c 6f63 6b28 2960 2061  yment.block()` a
-000024b0: 6e64 2074 6865 6e20 6d61 6b65 2072 6571  nd then make req
-000024c0: 7565 7374 7320 746f 2074 6865 2063 6c69  uests to the cli
-000024d0: 656e 742e 2050 6c65 6173 6520 7265 6665  ent. Please refe
-000024e0: 7220 746f 2074 6865 2043 6f6c 6162 206c  r to the Colab l
-000024f0: 696e 6b20 6162 6f76 6520 666f 7220 7265  ink above for re
-00002500: 7072 6f64 7563 6962 6c65 204a 7570 7974  producible Jupyt
-00002510: 6572 204e 6f74 6562 6f6f 6b20 636f 6465  er Notebook code
-00002520: 2073 6e69 7070 6574 732e 0a0a 2323 2320   snippets...### 
-00002530: 4275 696c 6420 6120 7069 7065 6c69 6e65  Build a pipeline
-00002540: 0a0a 3c21 2d2d 2073 7461 7274 2062 7569  ..<!-- start bui
-00002550: 6c64 2d70 6970 656c 696e 6573 202d 2d3e  ld-pipelines -->
-00002560: 0a0a 536f 6d65 7469 6d65 7320 796f 7520  ..Sometimes you 
-00002570: 7761 6e74 2074 6f20 6368 6169 6e20 6d69  want to chain mi
-00002580: 6372 6f73 6572 7669 6365 7320 746f 6765  croservices toge
-00002590: 7468 6572 2069 6e74 6f20 6120 7069 7065  ther into a pipe
-000025a0: 6c69 6e65 2e20 5468 6174 2773 2077 6865  line. That's whe
-000025b0: 7265 2061 205b 466c 6f77 5d28 6874 7470  re a [Flow](http
-000025c0: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-000025d0: 2f63 6f6e 6365 7074 732f 666c 6f77 2f29  /concepts/flow/)
-000025e0: 2063 6f6d 6573 2069 6e2e 0a0a 4120 466c   comes in...A Fl
-000025f0: 6f77 2069 7320 6120 5b44 4147 5d28 6874  ow is a [DAG](ht
-00002600: 7470 733a 2f2f 6465 2e77 696b 6970 6564  tps://de.wikiped
-00002610: 6961 2e6f 7267 2f77 696b 692f 4441 4729  ia.org/wiki/DAG)
-00002620: 2070 6970 656c 696e 652c 2063 6f6d 706f   pipeline, compo
-00002630: 7365 6420 6f66 2061 2073 6574 206f 6620  sed of a set of 
-00002640: 7374 6570 732c 2049 7420 6f72 6368 6573  steps, It orches
-00002650: 7472 6174 6573 2061 2073 6574 206f 6620  trates a set of 
-00002660: 5b45 7865 6375 746f 7273 5d28 6874 7470  [Executors](http
-00002670: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-00002680: 2f63 6f6e 6365 7074 732f 6578 6563 7574  /concepts/execut
-00002690: 6f72 2f29 2061 6e64 2061 205b 4761 7465  or/) and a [Gate
-000026a0: 7761 795d 2868 7474 7073 3a2f 2f64 6f63  way](https://doc
-000026b0: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-000026c0: 7473 2f67 6174 6577 6179 2f29 2074 6f20  ts/gateway/) to 
-000026d0: 6f66 6665 7220 616e 2065 6e64 2d74 6f2d  offer an end-to-
-000026e0: 656e 6420 7365 7276 6963 652e 0a0a 3e20  end service...> 
-000026f0: 2a2a 4e6f 7465 2a2a 0a3e 2049 6620 796f  **Note**.> If yo
-00002700: 7520 6a75 7374 2077 616e 7420 746f 2073  u just want to s
-00002710: 6572 7665 2061 2073 696e 676c 6520 4578  erve a single Ex
-00002720: 6563 7574 6f72 2c20 796f 7520 6361 6e20  ecutor, you can 
-00002730: 7573 6520 6120 5b44 6570 6c6f 796d 656e  use a [Deploymen
-00002740: 745d 2823 6275 696c 642d 6169 2d2d 6d6c  t](#build-ai--ml
-00002750: 2d73 6572 7669 6365 7329 2e0a 0a46 6f72  -services)...For
-00002760: 2069 6e73 7461 6e63 652c 206c 6574 2773   instance, let's
-00002770: 2063 6f6d 6269 6e65 205b 6f75 7220 5374   combine [our St
-00002780: 6162 6c65 4c4d 206c 616e 6775 6167 6520  ableLM language 
-00002790: 6d6f 6465 6c5d 2823 6275 696c 642d 6169  model](#build-ai
-000027a0: 2d2d 6d6c 2d73 6572 7669 6365 7329 2077  --ml-services) w
-000027b0: 6974 6820 6120 5374 6162 6c65 2044 6966  ith a Stable Dif
-000027c0: 6675 7369 6f6e 2069 6d61 6765 2067 656e  fusion image gen
-000027d0: 6572 6174 696f 6e20 7365 7276 6963 6520  eration service 
-000027e0: 6672 6f6d 2043 6d6f 6e20 4149 2773 205b  from Cmon AI's [
-000027f0: 4578 6563 7574 6f72 2048 7562 5d28 6874  Executor Hub](ht
-00002800: 7470 733a 2f2f 636c 6f75 642e 636d 6f6e  tps://cloud.cmon
-00002810: 2e61 692f 6578 6563 7574 6f72 7329 2e20  .ai/executors). 
-00002820: 4368 6169 6e69 6e67 2074 6865 7365 2073  Chaining these s
-00002830: 6572 7669 6365 7320 746f 6765 7468 6572  ervices together
-00002840: 2069 6e74 6f20 6120 5b46 6c6f 775d 2868   into a [Flow](h
-00002850: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00002860: 2e61 692f 636f 6e63 6570 7473 2f66 6c6f  .ai/concepts/flo
-00002870: 772f 2920 7769 6c6c 2067 6976 6520 7573  w/) will give us
-00002880: 2061 2073 6572 7669 6365 2074 6861 7420   a service that 
-00002890: 7769 6c6c 2067 656e 6572 6174 6520 696d  will generate im
-000028a0: 6167 6573 2062 6173 6564 206f 6e20 6120  ages based on a 
-000028b0: 7072 6f6d 7074 2067 656e 6572 6174 6564  prompt generated
-000028c0: 2062 7920 7468 6520 4c4c 4d2e 0a0a 215b   by the LLM...![
-000028d0: 5d28 2e2f 2e67 6974 6875 622f 696d 6167  ](./.github/imag
-000028e0: 6573 2f66 6c6f 772d 6469 6167 7261 6d2e  es/flow-diagram.
-000028f0: 706e 6729 0a0a 4275 696c 6420 7468 6520  png)..Build the 
-00002900: 466c 6f77 2077 6974 6820 6569 7468 6572  Flow with either
-00002910: 2050 7974 686f 6e20 6f72 2059 414d 4c3a   Python or YAML:
-00002920: 0a0a 3c64 6976 2063 6c61 7373 3d22 7461  ..<div class="ta
-00002930: 626c 652d 7772 6170 7065 7222 3e0a 3c74  ble-wrapper">.<t
-00002940: 6162 6c65 3e0a 3c74 723e 0a3c 7468 3e20  able>.<tr>.<th> 
-00002950: 5079 7468 6f6e 2041 5049 3a20 3c63 6f64  Python API: <cod
-00002960: 653e 666c 6f77 2e70 793c 2f63 6f64 653e  e>flow.py</code>
-00002970: 203c 2f74 683e 200a 3c74 683e 2059 414d   </th> .<th> YAM
-00002980: 4c3a 203c 636f 6465 3e66 6c6f 772e 796d  L: <code>flow.ym
-00002990: 6c3c 2f63 6f64 653e 203c 2f74 683e 0a3c  l</code> </th>.<
-000029a0: 2f74 723e 0a3c 7472 3e0a 3c74 643e 0a0a  /tr>.<tr>.<td>..
-000029b0: 6060 6070 7974 686f 6e0a 6672 6f6d 2063  ```python.from c
-000029c0: 6d6f 6e20 696d 706f 7274 2046 6c6f 770a  mon import Flow.
-000029d0: 6672 6f6d 2065 7865 6375 746f 7220 696d  from executor im
-000029e0: 706f 7274 2053 7461 626c 654c 4d0a 0a66  port StableLM..f
-000029f0: 6c6f 7720 3d20 280a 2020 2020 466c 6f77  low = (.    Flow
-00002a00: 2829 0a20 2020 202e 6164 6428 7573 6573  ().    .add(uses
-00002a10: 3d53 7461 626c 654c 4d2c 2074 696d 656f  =StableLM, timeo
-00002a20: 7574 5f72 6561 6479 3d2d 312c 2070 6f72  ut_ready=-1, por
-00002a30: 743d 3132 3334 3529 0a20 2020 202e 6164  t=12345).    .ad
-00002a40: 6428 0a20 2020 2020 2020 2075 7365 733d  d(.        uses=
-00002a50: 2763 6d6f 6e61 693a 2f2f 636d 6f6e 2d61  'cmonai://cmon-a
-00002a60: 692f 5465 7874 546f 496d 6167 6527 2c0a  i/TextToImage',.
-00002a70: 2020 2020 2020 2020 7469 6d65 6f75 745f          timeout_
-00002a80: 7265 6164 793d 2d31 2c0a 2020 2020 2020  ready=-1,.      
-00002a90: 2020 696e 7374 616c 6c5f 7265 7175 6972    install_requir
-00002aa0: 656d 656e 7473 3d54 7275 652c 0a20 2020  ements=True,.   
-00002ab0: 2029 0a29 2020 2320 7573 6520 7468 6520   ).)  # use the 
-00002ac0: 4578 6563 7574 6f72 2066 726f 6d20 436d  Executor from Cm
-00002ad0: 6f6e 2773 2045 7865 6375 746f 7220 6875  on's Executor hu
-00002ae0: 620a 0a77 6974 6820 666c 6f77 3a0a 2020  b..with flow:.  
-00002af0: 2020 666c 6f77 2e62 6c6f 636b 2829 0a60    flow.block().`
-00002b00: 6060 0a0a 3c2f 7464 3e0a 3c74 643e 0a0a  ``..</td>.<td>..
-00002b10: 6060 6079 616d 6c0a 6a74 7970 653a 2046  ```yaml.jtype: F
-00002b20: 6c6f 770a 7769 7468 3a0a 2020 2020 706f  low.with:.    po
-00002b30: 7274 3a20 3132 3334 350a 6578 6563 7574  rt: 12345.execut
-00002b40: 6f72 733a 0a20 202d 2075 7365 733a 2053  ors:.  - uses: S
-00002b50: 7461 626c 654c 4d0a 2020 2020 7469 6d65  tableLM.    time
-00002b60: 6f75 745f 7265 6164 793a 202d 310a 2020  out_ready: -1.  
-00002b70: 2020 7079 5f6d 6f64 756c 6573 3a0a 2020    py_modules:.  
-00002b80: 2020 2020 2d20 6578 6563 7574 6f72 2e70      - executor.p
-00002b90: 790a 2020 2d20 7573 6573 3a20 636d 6f6e  y.  - uses: cmon
-00002ba0: 6169 3a2f 2f63 6d6f 6e2d 6169 2f54 6578  ai://cmon-ai/Tex
-00002bb0: 7454 6f49 6d61 6765 0a20 2020 2074 696d  tToImage.    tim
-00002bc0: 656f 7574 5f72 6561 6479 3a20 2d31 0a20  eout_ready: -1. 
-00002bd0: 2020 2069 6e73 7461 6c6c 5f72 6571 7569     install_requi
-00002be0: 7265 6d65 6e74 733a 2074 7275 650a 6060  rements: true.``
-00002bf0: 600a 0a54 6865 6e20 7275 6e20 7468 6520  `..Then run the 
-00002c00: 5941 4d4c 2046 6c6f 7720 7769 7468 2074  YAML Flow with t
-00002c10: 6865 2043 4c49 3a20 6063 6d6f 6e20 666c  he CLI: `cmon fl
-00002c20: 6f77 202d 2d75 7365 7320 666c 6f77 2e79  ow --uses flow.y
-00002c30: 6d6c 600a 0a3c 2f74 643e 0a3c 2f74 723e  ml`..</td>.</tr>
-00002c40: 0a3c 2f74 6162 6c65 3e0a 3c2f 6469 763e  .</table>.</div>
-00002c50: 0a0a 5468 656e 2c20 7573 6520 5b43 6d6f  ..Then, use [Cmo
-00002c60: 6e20 436c 6965 6e74 5d28 6874 7470 733a  n Client](https:
-00002c70: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-00002c80: 6f6e 6365 7074 732f 636c 6965 6e74 2f29  oncepts/client/)
-00002c90: 2074 6f20 6d61 6b65 2072 6571 7565 7374   to make request
-00002ca0: 7320 746f 2074 6865 2046 6c6f 773a 0a0a  s to the Flow:..
-00002cb0: 6060 6070 7974 686f 6e0a 6672 6f6d 2063  ```python.from c
-00002cc0: 6d6f 6e20 696d 706f 7274 2043 6c69 656e  mon import Clien
-00002cd0: 742c 2044 6f63 756d 656e 740a 0a63 6c69  t, Document..cli
-00002ce0: 656e 7420 3d20 436c 6965 6e74 2870 6f72  ent = Client(por
-00002cf0: 743d 3132 3334 3529 0a0a 7072 6f6d 7074  t=12345)..prompt
-00002d00: 203d 2044 6f63 756d 656e 7428 0a20 2020   = Document(.   
-00002d10: 2074 6167 7320 3d20 7b27 7072 6f6d 7074   tags = {'prompt
-00002d20: 273a 2027 7375 6767 6573 7420 616e 2069  ': 'suggest an i
-00002d30: 6e74 6572 6573 7469 6e67 2069 6d61 6765  nteresting image
-00002d40: 2067 656e 6572 6174 696f 6e20 7072 6f6d   generation prom
-00002d50: 7074 2066 6f72 2061 206d 6f6e 6120 6c69  pt for a mona li
-00002d60: 7361 2076 6172 6961 6e74 277d 0a29 0a0a  sa variant'}.)..
-00002d70: 7265 7370 6f6e 7365 203d 2063 6c69 656e  response = clien
-00002d80: 742e 706f 7374 286f 6e3d 272f 272c 2069  t.post(on='/', i
-00002d90: 6e70 7574 733d 5b70 726f 6d70 745d 290a  nputs=[prompt]).
-00002da0: 0a72 6573 706f 6e73 655b 305d 2e64 6973  .response[0].dis
-00002db0: 706c 6179 2829 0a60 6060 0a0a 215b 5d28  play().```..![](
-00002dc0: 2e2f 2e67 6974 6875 622f 696d 6167 6573  ./.github/images
-00002dd0: 2f6d 6f6e 612d 6c69 7361 2e70 6e67 290a  /mona-lisa.png).
-00002de0: 0a23 2320 4465 706c 6f79 2074 6f20 7468  .## Deploy to th
-00002df0: 6520 636c 6f75 640a 0a59 6f75 2063 616e  e cloud..You can
-00002e00: 2061 6c73 6f20 6465 706c 6f79 2061 2046   also deploy a F
-00002e10: 6c6f 7720 746f 204a 436c 6f75 642e 0a0a  low to JCloud...
-00002e20: 4669 7273 742c 2074 7572 6e20 7468 6520  First, turn the 
-00002e30: 6066 6c6f 772e 796d 6c60 2066 696c 6520  `flow.yml` file 
-00002e40: 696e 746f 2061 205b 4a43 6c6f 7564 2d63  into a [JCloud-c
-00002e50: 6f6d 7061 7469 626c 6520 5941 4d4c 5d28  ompatible YAML](
-00002e60: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
-00002e70: 6e2e 6169 2f63 6f6e 6365 7074 732f 6a63  n.ai/concepts/jc
-00002e80: 6c6f 7564 2f79 616d 6c2d 7370 6563 2f29  loud/yaml-spec/)
-00002e90: 2062 7920 7370 6563 6966 7969 6e67 2072   by specifying r
-00002ea0: 6573 6f75 7263 6520 7265 7175 6972 656d  esource requirem
-00002eb0: 656e 7473 2061 6e64 2075 7369 6e67 2063  ents and using c
-00002ec0: 6f6e 7461 696e 6572 697a 6564 2048 7562  ontainerized Hub
-00002ed0: 2045 7865 6375 746f 7273 2e0a 0a54 6865   Executors...The
-00002ee0: 6e2c 2075 7365 2060 636d 6f6e 2063 6c6f  n, use `cmon clo
-00002ef0: 7564 2064 6570 6c6f 7960 2063 6f6d 6d61  ud deploy` comma
-00002f00: 6e64 2074 6f20 6465 706c 6f79 2074 6f20  nd to deploy to 
-00002f10: 7468 6520 636c 6f75 643a 0a0a 6060 6073  the cloud:..```s
-00002f20: 6865 6c6c 0a77 6765 7420 6874 7470 733a  hell.wget https:
-00002f30: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00002f40: 636f 6e74 656e 742e 636f 6d2f 636d 6f6e  content.com/cmon
-00002f50: 2d61 692f 636d 6f6e 2f6d 6173 7465 722f  -ai/cmon/master/
-00002f60: 2e67 6974 6875 622f 6765 7474 696e 672d  .github/getting-
-00002f70: 7374 6172 7465 642f 6a63 6c6f 7564 2d66  started/jcloud-f
-00002f80: 6c6f 772e 796d 6c0a 636d 6f6e 2063 6c6f  low.yml.cmon clo
-00002f90: 7564 2064 6570 6c6f 7920 6a63 6c6f 7564  ud deploy jcloud
-00002fa0: 2d66 6c6f 772e 796d 6c0a 6060 600a 0a3e  -flow.yml.```..>
-00002fb0: 202a 2a57 6172 6e69 6e67 2a2a 0a3e 0a3e   **Warning**.>.>
-00002fc0: 204d 616b 6520 7375 7265 2074 6f20 6465   Make sure to de
-00002fd0: 6c65 7465 2f63 6c65 616e 2075 7020 7468  lete/clean up th
-00002fe0: 6520 466c 6f77 206f 6e63 6520 796f 7520  e Flow once you 
-00002ff0: 6172 6520 646f 6e65 2077 6974 6820 7468  are done with th
-00003000: 6973 2074 7574 6f72 6961 6c20 746f 2073  is tutorial to s
-00003010: 6176 6520 7265 736f 7572 6365 7320 616e  ave resources an
-00003020: 6420 6372 6564 6974 732e 0a0a 5265 6164  d credits...Read
-00003030: 206d 6f72 6520 6162 6f75 7420 5b64 6570   more about [dep
-00003040: 6c6f 7969 6e67 2046 6c6f 7773 2074 6f20  loying Flows to 
-00003050: 4a43 6c6f 7564 5d28 6874 7470 733a 2f2f  JCloud](https://
-00003060: 646f 6373 2e63 6d6f 6e2e 6169 2f63 6f6e  docs.cmon.ai/con
-00003070: 6365 7074 732f 6a63 6c6f 7564 2f23 6465  cepts/jcloud/#de
-00003080: 706c 6f79 292e 0a0a 3c21 2d2d 2065 6e64  ploy)...<!-- end
-00003090: 2062 7569 6c64 2d70 6970 656c 696e 6573   build-pipelines
-000030a0: 202d 2d3e 0a0a 4368 6563 6b20 5b74 6865   -->..Check [the
-000030b0: 2067 6574 7469 6e67 2d73 7461 7274 6564   getting-started
-000030c0: 2070 726f 6a65 6374 2073 6f75 7263 6520   project source 
-000030d0: 636f 6465 5d28 6874 7470 733a 2f2f 6769  code](https://gi
-000030e0: 7468 7562 2e63 6f6d 2f63 6d6f 6e2d 6169  thub.com/cmon-ai
-000030f0: 2f63 6d6f 6e2f 7472 6565 2f6d 6173 7465  /cmon/tree/maste
-00003100: 722f 2e67 6974 6875 622f 6765 7474 696e  r/.github/gettin
-00003110: 672d 7374 6172 7465 6429 2e0a 0a23 2323  g-started)...###
-00003120: 2045 6173 7920 7363 616c 6162 696c 6974   Easy scalabilit
-00003130: 7920 616e 6420 636f 6e63 7572 7265 6e63  y and concurrenc
-00003140: 790a 0a57 6879 206e 6f74 206a 7573 7420  y..Why not just 
-00003150: 7573 6520 7374 616e 6461 7264 2050 7974  use standard Pyt
-00003160: 686f 6e20 746f 2062 7569 6c64 2074 6861  hon to build tha
-00003170: 7420 6d69 6372 6f73 6572 7669 6365 2061  t microservice a
-00003180: 6e64 2070 6970 656c 696e 653f 2043 6d6f  nd pipeline? Cmo
-00003190: 6e20 6163 6365 6c65 7261 7465 7320 7469  n accelerates ti
-000031a0: 6d65 2074 6f20 6d61 726b 6574 206f 6620  me to market of 
-000031b0: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
-000031c0: 2062 7920 6d61 6b69 6e67 2069 7420 6d6f   by making it mo
-000031d0: 7265 2073 6361 6c61 626c 6520 616e 6420  re scalable and 
-000031e0: 636c 6f75 642d 6e61 7469 7665 2e20 436d  cloud-native. Cm
-000031f0: 6f6e 2061 6c73 6f20 6861 6e64 6c65 7320  on also handles 
-00003200: 7468 6520 696e 6672 6173 7472 7563 7475  the infrastructu
-00003210: 7265 2063 6f6d 706c 6578 6974 7920 696e  re complexity in
-00003220: 2070 726f 6475 6374 696f 6e20 616e 6420   production and 
-00003230: 6f74 6865 7220 4461 792d 3220 6f70 6572  other Day-2 oper
-00003240: 6174 696f 6e73 2073 6f20 7468 6174 2079  ations so that y
-00003250: 6f75 2063 616e 2066 6f63 7573 206f 6e20  ou can focus on 
-00003260: 7468 6520 6461 7461 2061 7070 6c69 6361  the data applica
-00003270: 7469 6f6e 2069 7473 656c 662e 0a0a 496e  tion itself...In
-00003280: 6372 6561 7365 2079 6f75 7220 6170 706c  crease your appl
-00003290: 6963 6174 696f 6e27 7320 7468 726f 7567  ication's throug
-000032a0: 6870 7574 2077 6974 6820 7363 616c 6162  hput with scalab
-000032b0: 696c 6974 7920 6665 6174 7572 6573 206f  ility features o
-000032c0: 7574 206f 6620 7468 6520 626f 782c 206c  ut of the box, l
-000032d0: 696b 6520 5b72 6570 6c69 6361 735d 2868  ike [replicas](h
-000032e0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-000032f0: 2e61 692f 636f 6e63 6570 7473 2f6f 7263  .ai/concepts/orc
-00003300: 6865 7374 7261 7469 6f6e 2f73 6361 6c65  hestration/scale
-00003310: 2d6f 7574 2f23 7265 706c 6963 6174 652d  -out/#replicate-
-00003320: 6578 6563 7574 6f72 7329 2c20 5b73 6861  executors), [sha
-00003330: 7264 735d 2868 7474 7073 3a2f 2f64 6f63  rds](https://doc
-00003340: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00003350: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
-00003360: 2f73 6361 6c65 2d6f 7574 2f23 6375 7374  /scale-out/#cust
-00003370: 6f6d 697a 652d 706f 6c6c 696e 672d 6265  omize-polling-be
-00003380: 6861 7669 6f72 7329 2061 6e64 205b 6479  haviors) and [dy
-00003390: 6e61 6d69 6320 6261 7463 6869 6e67 5d28  namic batching](
-000033a0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
-000033b0: 6e2e 6169 2f63 6f6e 6365 7074 732f 7365  n.ai/concepts/se
-000033c0: 7276 696e 672f 6578 6563 7574 6f72 2f64  rving/executor/d
-000033d0: 796e 616d 6963 2d62 6174 6368 696e 672f  ynamic-batching/
-000033e0: 292e 0a0a 4c65 7427 7320 7363 616c 6520  )...Let's scale 
-000033f0: 6120 5374 6162 6c65 2044 6966 6675 7369  a Stable Diffusi
-00003400: 6f6e 2045 7865 6375 746f 7220 6465 706c  on Executor depl
-00003410: 6f79 6d65 6e74 2077 6974 6820 7265 706c  oyment with repl
-00003420: 6963 6173 2061 6e64 2064 796e 616d 6963  icas and dynamic
-00003430: 2062 6174 6368 696e 673a 0a0a 215b 5d28   batching:..![](
-00003440: 2e2f 2e67 6974 6875 622f 696d 6167 6573  ./.github/images
-00003450: 2f73 6361 6c65 642d 6465 706c 6f79 6d65  /scaled-deployme
-00003460: 6e74 2e70 6e67 290a 0a2a 2043 7265 6174  nt.png)..* Creat
-00003470: 6520 7477 6f20 7265 706c 6963 6173 2c20  e two replicas, 
-00003480: 7769 7468 205b 6120 4750 5520 6173 7369  with [a GPU assi
-00003490: 676e 6564 2066 6f72 2065 6163 685d 2868  gned for each](h
-000034a0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-000034b0: 2e61 692f 636f 6e63 6570 7473 2f66 6c6f  .ai/concepts/flo
-000034c0: 772f 7363 616c 652d 6f75 742f 2372 6570  w/scale-out/#rep
-000034d0: 6c69 6361 7465 2d6f 6e2d 6d75 6c74 6970  licate-on-multip
-000034e0: 6c65 2d67 7075 7329 2e0a 2a20 456e 6162  le-gpus)..* Enab
-000034f0: 6c65 2064 796e 616d 6963 2062 6174 6368  le dynamic batch
-00003500: 696e 6720 746f 2070 726f 6365 7373 2069  ing to process i
-00003510: 6e63 6f6d 696e 6720 7061 7261 6c6c 656c  ncoming parallel
-00003520: 2072 6571 7565 7374 7320 746f 6765 7468   requests togeth
-00003530: 6572 2077 6974 6820 7468 6520 7361 6d65  er with the same
-00003540: 206d 6f64 656c 2069 6e66 6572 656e 6365   model inference
-00003550: 2e0a 0a0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
-00003560: 7461 626c 652d 7772 6170 7065 7222 3e0a  table-wrapper">.
-00003570: 3c74 6162 6c65 3e0a 3c74 723e 0a3c 7468  <table>.<tr>.<th
-00003580: 3e20 4e6f 726d 616c 2044 6570 6c6f 796d  > Normal Deploym
-00003590: 656e 7420 3c2f 7468 3e20 0a3c 7468 3e20  ent </th> .<th> 
-000035a0: 5363 616c 6564 2044 6570 6c6f 796d 656e  Scaled Deploymen
-000035b0: 7420 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  t </th>.</tr>.<t
-000035c0: 723e 0a3c 7464 3e0a 0a60 6060 7961 6d6c  r>.<td>..```yaml
-000035d0: 0a6a 7479 7065 3a20 4465 706c 6f79 6d65  .jtype: Deployme
-000035e0: 6e74 0a77 6974 683a 0a20 2074 696d 656f  nt.with:.  timeo
-000035f0: 7574 5f72 6561 6479 3a20 2d31 0a20 2075  ut_ready: -1.  u
-00003600: 7365 733a 2063 6d6f 6e61 693a 2f2f 636d  ses: cmonai://cm
-00003610: 6f6e 2d61 692f 5465 7874 546f 496d 6167  on-ai/TextToImag
-00003620: 650a 2020 696e 7374 616c 6c5f 7265 7175  e.  install_requ
-00003630: 6972 656d 656e 7473 3a20 7472 7565 0a60  irements: true.`
-00003640: 6060 0a0a 3c2f 7464 3e0a 3c74 643e 0a0a  ``..</td>.<td>..
-00003650: 6060 6079 616d 6c0a 6a74 7970 653a 2044  ```yaml.jtype: D
-00003660: 6570 6c6f 796d 656e 740a 7769 7468 3a0a  eployment.with:.
-00003670: 2020 7469 6d65 6f75 745f 7265 6164 793a    timeout_ready:
-00003680: 202d 310a 2020 7573 6573 3a20 636d 6f6e   -1.  uses: cmon
-00003690: 6169 3a2f 2f63 6d6f 6e2d 6169 2f54 6578  ai://cmon-ai/Tex
-000036a0: 7454 6f49 6d61 6765 0a20 2069 6e73 7461  tToImage.  insta
-000036b0: 6c6c 5f72 6571 7569 7265 6d65 6e74 733a  ll_requirements:
-000036c0: 2074 7275 650a 2020 656e 763a 0a20 2020   true.  env:.   
-000036d0: 4355 4441 5f56 4953 4942 4c45 5f44 4556  CUDA_VISIBLE_DEV
-000036e0: 4943 4553 3a20 5252 0a20 2072 6570 6c69  ICES: RR.  repli
-000036f0: 6361 733a 2032 0a20 2075 7365 735f 6479  cas: 2.  uses_dy
-00003700: 6e61 6d69 635f 6261 7463 6869 6e67 3a20  namic_batching: 
-00003710: 2320 636f 6e66 6967 7572 6520 6479 6e61  # configure dyna
-00003720: 6d69 6320 6261 7463 6869 6e67 0a20 2020  mic batching.   
-00003730: 202f 6465 6661 756c 743a 0a20 2020 2020   /default:.     
-00003740: 2070 7265 6665 7272 6564 5f62 6174 6368   preferred_batch
-00003750: 5f73 697a 653a 2031 300a 2020 2020 2020  _size: 10.      
-00003760: 7469 6d65 6f75 743a 2032 3030 0a60 6060  timeout: 200.```
-00003770: 0a0a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c2f  ..</td>.</tr>.</
-00003780: 7461 626c 653e 0a3c 2f64 6976 3e0a 0a41  table>.</div>..A
-00003790: 7373 756d 696e 6720 796f 7572 206d 6163  ssuming your mac
-000037a0: 6869 6e65 2068 6173 2074 776f 2047 5055  hine has two GPU
-000037b0: 732c 2075 7369 6e67 2074 6865 2073 6361  s, using the sca
-000037c0: 6c65 6420 6465 706c 6f79 6d65 6e74 2059  led deployment Y
-000037d0: 414d 4c20 7769 6c6c 2067 6976 6520 6265  AML will give be
-000037e0: 7474 6572 2074 6872 6f75 6768 7075 7420  tter throughput 
-000037f0: 636f 6d70 6172 6564 2074 6f20 7468 6520  compared to the 
-00003800: 6e6f 726d 616c 2064 6570 6c6f 796d 656e  normal deploymen
-00003810: 742e 0a0a 5468 6573 6520 6665 6174 7572  t...These featur
-00003820: 6573 2061 7070 6c79 2074 6f20 626f 7468  es apply to both
-00003830: 205b 4465 706c 6f79 6d65 6e74 2059 414d   [Deployment YAM
-00003840: 4c5d 2868 7474 7073 3a2f 2f64 6f63 732e  L](https://docs.
-00003850: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-00003860: 2f65 7865 6375 746f 722f 6465 706c 6f79  /executor/deploy
-00003870: 6d65 6e74 2d79 616d 6c2d 7370 6563 2f23  ment-yaml-spec/#
-00003880: 6465 706c 6f79 6d65 6e74 2d79 616d 6c2d  deployment-yaml-
-00003890: 7370 6563 2920 616e 6420 5b46 6c6f 7720  spec) and [Flow 
-000038a0: 5941 4d4c 5d28 6874 7470 733a 2f2f 646f  YAML](https://do
-000038b0: 6373 2e63 6d6f 6e2e 6169 2f63 6f6e 6365  cs.cmon.ai/conce
-000038c0: 7074 732f 666c 6f77 2f79 616d 6c2d 7370  pts/flow/yaml-sp
-000038d0: 6563 2f29 2e20 5468 616e 6b73 2074 6f20  ec/). Thanks to 
-000038e0: 7468 6520 5941 4d4c 2073 796e 7461 782c  the YAML syntax,
-000038f0: 2079 6f75 2063 616e 2069 6e6a 6563 7420   you can inject 
-00003900: 6465 706c 6f79 6d65 6e74 2063 6f6e 6669  deployment confi
-00003910: 6775 7261 7469 6f6e 7320 7265 6761 7264  gurations regard
-00003920: 6c65 7373 206f 6620 4578 6563 7574 6f72  less of Executor
-00003930: 2063 6f64 652e 0a0a 2323 2320 4765 7420   code...### Get 
-00003940: 6f6e 2074 6865 2066 6173 7420 6c61 6e65  on the fast lane
-00003950: 2074 6f20 636c 6f75 642d 6e61 7469 7665   to cloud-native
-00003960: 0a0a 5573 696e 6720 4b75 6265 726e 6574  ..Using Kubernet
-00003970: 6573 2077 6974 6820 436d 6f6e 2069 7320  es with Cmon is 
-00003980: 6561 7379 3a0a 0a60 6060 6261 7368 0a63  easy:..```bash.c
-00003990: 6d6f 6e20 6578 706f 7274 206b 7562 6572  mon export kuber
-000039a0: 6e65 7465 7320 666c 6f77 2e79 6d6c 202e  netes flow.yml .
-000039b0: 2f6d 792d 6b38 730a 6b75 6265 6374 6c20  /my-k8s.kubectl 
-000039c0: 6170 706c 7920 2d52 202d 6620 6d79 2d6b  apply -R -f my-k
-000039d0: 3873 0a60 6060 0a0a 416e 6420 736f 2069  8s.```..And so i
-000039e0: 7320 446f 636b 6572 2043 6f6d 706f 7365  s Docker Compose
-000039f0: 3a0a 0a60 6060 6261 7368 0a63 6d6f 6e20  :..```bash.cmon 
-00003a00: 6578 706f 7274 2064 6f63 6b65 722d 636f  export docker-co
-00003a10: 6d70 6f73 6520 666c 6f77 2e79 6d6c 2064  mpose flow.yml d
-00003a20: 6f63 6b65 722d 636f 6d70 6f73 652e 796d  ocker-compose.ym
-00003a30: 6c0a 646f 636b 6572 2d63 6f6d 706f 7365  l.docker-compose
-00003a40: 2075 700a 6060 600a 0a3e 202a 2a4e 6f74   up.```..> **Not
-00003a50: 652a 2a0a 3e20 596f 7520 6361 6e20 616c  e**.> You can al
-00003a60: 736f 2065 7870 6f72 7420 4465 706c 6f79  so export Deploy
-00003a70: 6d65 6e74 2059 414d 4c20 746f 205b 4b75  ment YAML to [Ku
-00003a80: 6265 726e 6574 6573 5d28 6874 7470 733a  bernetes](https:
-00003a90: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-00003aa0: 6f6e 6365 7074 732f 6578 6563 7574 6f72  oncepts/executor
-00003ab0: 2f73 6572 7665 2f23 7365 7276 652d 7669  /serve/#serve-vi
-00003ac0: 612d 6b75 6265 726e 6574 6573 2920 616e  a-kubernetes) an
-00003ad0: 6420 5b44 6f63 6b65 7220 436f 6d70 6f73  d [Docker Compos
-00003ae0: 655d 2868 7474 7073 3a2f 2f64 6f63 732e  e](https://docs.
-00003af0: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-00003b00: 2f65 7865 6375 746f 722f 7365 7276 652f  /executor/serve/
-00003b10: 2373 6572 7665 2d76 6961 2d64 6f63 6b65  #serve-via-docke
-00003b20: 722d 636f 6d70 6f73 6529 2e0a 0a54 6861  r-compose)...Tha
-00003b30: 7427 7320 6e6f 7420 616c 6c2e 2057 6520  t's not all. We 
-00003b40: 616c 736f 2073 7570 706f 7274 205b 4f70  also support [Op
-00003b50: 656e 5465 6c65 6d65 7472 792c 2050 726f  enTelemetry, Pro
-00003b60: 6d65 7468 6575 732c 2061 6e64 204a 6165  metheus, and Jae
-00003b70: 6765 725d 2868 7474 7073 3a2f 2f64 6f63  ger](https://doc
-00003b80: 732e 636d 6f6e 2e61 692f 636c 6f75 642d  s.cmon.ai/cloud-
-00003b90: 6e61 7469 7665 6e65 7373 2f6f 7065 6e74  nativeness/opent
-00003ba0: 656c 656d 6574 7279 2f29 2e0a 0a57 6861  elemetry/)...Wha
-00003bb0: 7420 636c 6f75 642d 6e61 7469 7665 2074  t cloud-native t
-00003bc0: 6563 686e 6f6c 6f67 7920 6973 2073 7469  echnology is sti
-00003bd0: 6c6c 2063 6861 6c6c 656e 6769 6e67 2074  ll challenging t
-00003be0: 6f20 796f 753f 205b 5465 6c6c 2075 735d  o you? [Tell us]
-00003bf0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003c00: 636f 6d2f 636d 6f6e 2d61 692f 636d 6f6e  com/cmon-ai/cmon
-00003c10: 2f69 7373 7565 7329 2061 6e64 2077 6527  /issues) and we'
-00003c20: 6c6c 2068 616e 646c 6520 7468 6520 636f  ll handle the co
-00003c30: 6d70 6c65 7869 7479 2061 6e64 206d 616b  mplexity and mak
-00003c40: 6520 6974 2065 6173 7920 666f 7220 796f  e it easy for yo
-00003c50: 752e 0a0a 3c21 2d2d 2073 7461 7274 2073  u...<!-- start s
-00003c60: 7570 706f 7274 2d70 6974 6368 202d 2d3e  upport-pitch -->
-00003c70: 0a0a 2323 2053 7570 706f 7274 0a0a 2d20  ..## Support..- 
-00003c80: 4a6f 696e 206f 7572 205b 4469 7363 6f72  Join our [Discor
-00003c90: 6420 636f 6d6d 756e 6974 795d 2868 7474  d community](htt
-00003ca0: 7073 3a2f 2f64 6973 636f 7264 2e63 6d6f  ps://discord.cmo
-00003cb0: 6e2e 6169 2920 616e 6420 6368 6174 2077  n.ai) and chat w
-00003cc0: 6974 6820 6f74 6865 7220 636f 6d6d 756e  ith other commun
-00003cd0: 6974 7920 6d65 6d62 6572 7320 6162 6f75  ity members abou
-00003ce0: 7420 6964 6561 732e 0a2d 2053 7562 7363  t ideas..- Subsc
-00003cf0: 7269 6265 2074 6f20 7468 6520 6c61 7465  ribe to the late
-00003d00: 7374 2076 6964 656f 2074 7574 6f72 6961  st video tutoria
-00003d10: 6c73 206f 6e20 6f75 7220 5b59 6f75 5475  ls on our [YouTu
-00003d20: 6265 2063 6861 6e6e 656c 5d28 6874 7470  be channel](http
-00003d30: 733a 2f2f 796f 7574 7562 652e 636f 6d2f  s://youtube.com/
-00003d40: 632f 636d 6f6e 2d61 6929 0a0a 2323 204a  c/cmon-ai)..## J
-00003d50: 6f69 6e20 5573 0a0a 436d 6f6e 2069 7320  oin Us..Cmon is 
-00003d60: 6261 636b 6564 2062 7920 5b43 6d6f 6e20  backed by [Cmon 
-00003d70: 4149 5d28 6874 7470 733a 2f2f 636d 6f6e  AI](https://cmon
-00003d80: 2e61 6929 2061 6e64 206c 6963 656e 7365  .ai) and license
-00003d90: 6420 756e 6465 7220 5b41 7061 6368 652d  d under [Apache-
-00003da0: 322e 305d 282e 2f4c 4943 454e 5345 292e  2.0](./LICENSE).
-00003db0: 0a0a 3c21 2d2d 2065 6e64 2073 7570 706f  ..<!-- end suppo
-00003dc0: 7274 2d70 6974 6368 202d 2d3e 0a         rt-pitch -->.
+00000010: 3a20 322e 310d 0a4e 616d 653a 2063 6d6f  : 2.1..Name: cmo
+00000020: 6e2d 6169 0d0a 5665 7273 696f 6e3a 2030  n-ai..Version: 0
+00000030: 2e34 322e 360d 0a53 756d 6d61 7279 3a20  .42.6..Summary: 
+00000040: 4275 696c 6420 6d75 6c74 696d 6f64 616c  Build multimodal
+00000050: 2041 4920 7365 7276 6963 6573 2076 6961   AI services via
+00000060: 2063 6c6f 7564 206e 6174 6976 6520 7465   cloud native te
+00000070: 6368 6e6f 6c6f 6769 6573 20c2 b720 4e65  chnologies .. Ne
+00000080: 7572 616c 2053 6561 7263 6820 c2b7 2047  ural Search .. G
+00000090: 656e 6572 6174 6976 6520 4149 20c2 b720  enerative AI .. 
+000000a0: 4d4c 4f70 730d 0a48 6f6d 652d 7061 6765  MLOps..Home-page
+000000b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000c0: 2e63 6f6d 2f6f 7065 6e61 692d 6165 2f43  .com/openai-ae/C
+000000d0: 6d6f 6e2d 4149 2d4c 6962 7261 7279 0d0a  mon-AI-Library..
+000000e0: 446f 776e 6c6f 6164 2d55 524c 3a20 6874  Download-URL: ht
+000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000100: 2f6f 7065 6e61 692d 6165 2f43 6d6f 6e2d  /openai-ae/Cmon-
+00000110: 4149 2d4c 6962 7261 7279 2f61 7263 6869  AI-Library/archi
+00000120: 7665 2f72 6566 732f 7461 6773 2f41 492e  ve/refs/tags/AI.
+00000130: 7a69 700d 0a41 7574 686f 723a 2043 6d6f  zip..Author: Cmo
+00000140: 6e20 4149 0d0a 4175 7468 6f72 2d65 6d61  n AI..Author-ema
+00000150: 696c 3a20 6865 6c6c 6f40 636d 6f6e 2e70  il: hello@cmon.p
+00000160: 770d 0a4c 6963 656e 7365 3a20 4170 6163  w..License: Apac
+00000170: 6865 2032 2e30 0d0a 5072 6f6a 6563 742d  he 2.0..Project-
+00000180: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
+00000190: 6f6e 2c20 6874 7470 733a 2f2f 646f 6373  on, https://docs
+000001a0: 2e63 6d6f 6e2e 7077 0d0a 5072 6f6a 6563  .cmon.pw..Projec
+000001b0: 742d 5552 4c3a 2053 6f75 7263 652c 2068  t-URL: Source, h
+000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001d0: 6d2f 6f70 656e 6169 2d61 652f 636d 6f6e  m/openai-ae/cmon
+000001e0: 2d61 692f 0d0a 5072 6f6a 6563 742d 5552  -ai/..Project-UR
+000001f0: 4c3a 2054 7261 636b 6572 2c20 6874 7470  L: Tracker, http
+00000200: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000210: 7065 6e61 692d 6165 2f63 6d6f 6e2d 6169  penai-ae/cmon-ai
+00000220: 2f69 7373 7565 730d 0a4b 6579 776f 7264  /issues..Keyword
+00000230: 733a 2063 6d6f 6e20 636c 6f75 642d 6e61  s: cmon cloud-na
+00000240: 7469 7665 2063 726f 7373 2d6d 6f64 616c  tive cross-modal
+00000250: 206d 756c 7469 6d6f 6461 6c20 6e65 7572   multimodal neur
+00000260: 616c 2d73 6561 7263 6820 7175 6572 7920  al-search query 
+00000270: 7365 6172 6368 2069 6e64 6578 2065 6c61  search index ela
+00000280: 7374 6963 206e 6575 7261 6c2d 6e65 7477  stic neural-netw
+00000290: 6f72 6b20 656e 636f 6469 6e67 2065 6d62  ork encoding emb
+000002a0: 6564 6469 6e67 2073 6572 7669 6e67 2064  edding serving d
+000002b0: 6f63 6b65 7220 636f 6e74 6169 6e65 7220  ocker container 
+000002c0: 696d 6167 6520 7669 6465 6f20 6175 6469  image video audi
+000002d0: 6f20 6465 6570 2d6c 6561 726e 696e 6720  o deep-learning 
+000002e0: 6d6c 6f70 730d 0a43 6c61 7373 6966 6965  mlops..Classifie
+000002f0: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000300: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00000310: 6475 6374 696f 6e2f 5374 6162 6c65 0d0a  duction/Stable..
+00000320: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000330: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000340: 2044 6576 656c 6f70 6572 730d 0a43 6c61   Developers..Cla
+00000350: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000360: 6420 4175 6469 656e 6365 203a 3a20 4564  d Audience :: Ed
+00000370: 7563 6174 696f 6e0d 0a43 6c61 7373 6966  ucation..Classif
+00000380: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+00000390: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
+000003a0: 652f 5265 7365 6172 6368 0d0a 436c 6173  e/Research..Clas
+000003b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003d0: 5079 7468 6f6e 203a 3a20 332e 370d 0a43  Python :: 3.7..C
+000003e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000003f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000400: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000410: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000420: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000430: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000440: 332e 390d 0a43 6c61 7373 6966 6965 723a  3.9..Classifier:
+00000450: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000460: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000470: 3a3a 2033 2e31 300d 0a43 6c61 7373 6966  :: 3.10..Classif
+00000480: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000490: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000004a0: 686f 6e20 3a3a 2033 2e31 310d 0a43 6c61  hon :: 3.11..Cla
+000004b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000004c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000004d0: 2055 6e69 7820 5368 656c 6c0d 0a43 6c61   Unix Shell..Cla
+000004e0: 7373 6966 6965 723a 2045 6e76 6972 6f6e  ssifier: Environ
+000004f0: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650d  ment :: Console.
+00000500: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000510: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000520: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
+00000530: 6f66 7477 6172 6520 4c69 6365 6e73 650d  oftware License.
+00000540: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000550: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000560: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000570: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000580: 6963 203a 3a20 4461 7461 6261 7365 203a  ic :: Database :
+00000590: 3a20 4461 7461 6261 7365 2045 6e67 696e  : Database Engin
+000005a0: 6573 2f53 6572 7665 7273 0d0a 436c 6173  es/Servers..Clas
+000005b0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000005c0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+000005d0: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+000005e0: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+000005f0: 6365 0d0a 436c 6173 7369 6669 6572 3a20  ce..Classifier: 
+00000600: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+00000610: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
+00000620: 2049 6e64 6578 696e 672f 5365 6172 6368   Indexing/Search
+00000630: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
+00000640: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
+00000650: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
+00000660: 2049 6d61 6765 2052 6563 6f67 6e69 7469   Image Recogniti
+00000670: 6f6e 0d0a 436c 6173 7369 6669 6572 3a20  on..Classifier: 
+00000680: 546f 7069 6320 3a3a 204d 756c 7469 6d65  Topic :: Multime
+00000690: 6469 6120 3a3a 2056 6964 656f 0d0a 436c  dia :: Video..Cl
+000006a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+000006b0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000006c0: 6769 6e65 6572 696e 670d 0a43 6c61 7373  gineering..Class
+000006d0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000006e0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+000006f0: 6565 7269 6e67 203a 3a20 4d61 7468 656d  eering :: Mathem
+00000700: 6174 6963 730d 0a43 6c61 7373 6966 6965  atics..Classifie
+00000710: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+00000720: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000730: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
+00000740: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000750: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000760: 6962 7261 7269 6573 0d0a 436c 6173 7369  ibraries..Classi
+00000770: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000780: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000790: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+000007a0: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
+000007b0: 6573 0d0a 4465 7363 7269 7074 696f 6e2d  es..Description-
+000007c0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+000007d0: 7874 2f6d 6172 6b64 6f77 6e0d 0a4c 6963  xt/markdown..Lic
+000007e0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000007f0: 5345 0d0a 0d0a 3c70 2061 6c69 676e 3d22  SE....<p align="
+00000800: 6365 6e74 6572 223e 0d0a 3c21 2d2d 2073  center">..<!-- s
+00000810: 7572 7665 7920 6261 6e6e 6572 2073 7461  urvey banner sta
+00000820: 7274 202d 2d3e 0d0a 3c61 2068 7265 663d  rt -->..<a href=
+00000830: 2268 7474 7073 3a2f 2f31 3073 7731 7463  "https://10sw1tc
+00000840: 706c 6434 2e74 7970 6566 6f72 6d2e 636f  pld4.typeform.co
+00000850: 6d2f 746f 2f45 4741 4552 654d 373f 7574  m/to/EGAEReM7?ut
+00000860: 6d5f 736f 7572 6365 3d72 6561 646d 6526  m_source=readme&
+00000870: 7574 6d5f 6d65 6469 756d 3d67 6974 6875  utm_medium=githu
+00000880: 6226 7574 6d5f 6361 6d70 6169 676e 3d75  b&utm_campaign=u
+00000890: 7365 7225 3230 6578 7065 7269 656e 6365  ser%20experience
+000008a0: 2675 746d 5f74 6572 6d3d 6665 6232 3032  &utm_term=feb202
+000008b0: 3326 7574 6d5f 636f 6e74 656e 743d 7375  3&utm_content=su
+000008c0: 7276 6579 223e 0d0a 2020 3c69 6d67 2073  rvey">..  <img s
+000008d0: 7263 3d22 2e2f 2e67 6974 6875 622f 6261  rc="./.github/ba
+000008e0: 6e6e 6572 2e73 7667 3f72 6177 3d74 7275  nner.svg?raw=tru
+000008f0: 6522 3e0d 0a3c 2f61 3e0d 0a3c 212d 2d20  e">..</a>..<!-- 
+00000900: 7375 7276 6579 2062 616e 6e65 7220 7374  survey banner st
+00000910: 6172 7420 2d2d 3e0d 0a0d 0a3c 7020 616c  art -->....<p al
+00000920: 6967 6e3d 2263 656e 7465 7222 3e0d 0a3c  ign="center">..<
+00000930: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000940: 646f 6373 2e63 6d6f 6e2e 7077 223e 3c69  docs.cmon.pw"><i
+00000950: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000960: 6769 7468 7562 2e63 6f6d 2f63 6d6f 6e2e  github.com/cmon.
+00000970: 7077 2f63 6d6f 6e2f 626c 6f62 2f6d 6173  pw/cmon/blob/mas
+00000980: 7465 722f 646f 6373 2f5f 7374 6174 6963  ter/docs/_static
+00000990: 2f6c 6f67 6f2d 6c69 6768 742e 7376 673f  /logo-light.svg?
+000009a0: 7261 773d 7472 7565 2220 616c 743d 2243  raw=true" alt="C
+000009b0: 6d6f 6e20 6c6f 676f 3a20 4275 696c 6420  mon logo: Build 
+000009c0: 6d75 6c74 696d 6f64 616c 2041 4920 7365  multimodal AI se
+000009d0: 7276 6963 6573 2076 6961 2063 6c6f 7564  rvices via cloud
+000009e0: 206e 6174 6976 6520 7465 6368 6e6f 6c6f   native technolo
+000009f0: 6769 6573 20c2 b720 4e65 7572 616c 2053  gies .. Neural S
+00000a00: 6561 7263 6820 c2b7 2047 656e 6572 6174  earch .. Generat
+00000a10: 6976 6520 4149 20c2 b720 436c 6f75 6420  ive AI .. Cloud 
+00000a20: 4e61 7469 7665 2220 7769 6474 683d 2231  Native" width="1
+00000a30: 3530 7078 223e 3c2f 613e 0d0a 3c2f 703e  50px"></a>..</p>
+00000a40: 0d0a 0d0a 3c70 2061 6c69 676e 3d22 6365  ....<p align="ce
+00000a50: 6e74 6572 223e 0d0a 3c62 3e42 7569 6c64  nter">..<b>Build
+00000a60: 206d 756c 7469 6d6f 6461 6c20 4149 2073   multimodal AI s
+00000a70: 6572 7669 6365 7320 7769 7468 2063 6c6f  ervices with clo
+00000a80: 7564 206e 6174 6976 6520 7465 6368 6e6f  ud native techno
+00000a90: 6c6f 6769 6573 3c2f 623e 0d0a 3c2f 703e  logies</b>..</p>
+00000aa0: 0d0a 0d0a 3c70 2061 6c69 676e 3d63 656e  ....<p align=cen
+00000ab0: 7465 723e 0d0a 3c61 2068 7265 663d 2268  ter>..<a href="h
+00000ac0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000ad0: 7072 6f6a 6563 742f 636d 6f6e 2f22 3e3c  project/cmon/"><
+00000ae0: 696d 6720 616c 743d 2250 7950 4922 2073  img alt="PyPI" s
+00000af0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000b00: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000b10: 762f 636d 6f6e 3f6c 6162 656c 3d52 656c  v/cmon?label=Rel
+00000b20: 6561 7365 2673 7479 6c65 3d66 6c61 742d  ease&style=flat-
+00000b30: 7371 7561 7265 223e 3c2f 613e 0d0a 3c21  square"></a>..<!
+00000b40: 2d2d 3c61 2068 7265 663d 2268 7474 7073  --<a href="https
+00000b50: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000b60: 2f63 6d6f 6e2e 7077 2f63 6d6f 6e22 3e3c  /cmon.pw/cmon"><
+00000b70: 696d 6720 616c 743d 2243 6f64 6563 6f76  img alt="Codecov
+00000b80: 2062 7261 6e63 6822 2073 7263 3d22 6874   branch" src="ht
+00000b90: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000ba0: 732e 696f 2f63 6f64 6563 6f76 2f63 2f67  s.io/codecov/c/g
+00000bb0: 6974 6875 622f 636d 6f6e 2e70 772f 636d  ithub/cmon.pw/cm
+00000bc0: 6f6e 2f6d 6173 7465 723f 266c 6f67 6f3d  on/master?&logo=
+00000bd0: 436f 6465 636f 7626 6c6f 676f 436f 6c6f  Codecov&logoColo
+00000be0: 723d 7768 6974 6526 7374 796c 653d 666c  r=white&style=fl
+00000bf0: 6174 2d73 7175 6172 6522 3e3c 2f61 3e2d  at-square"></a>-
+00000c00: 2d3e 0d0a 3c61 2068 7265 663d 2268 7474  ->..<a href="htt
+00000c10: 7073 3a2f 2f64 6973 636f 7264 2e63 6d6f  ps://discord.cmo
+00000c20: 6e2e 7077 223e 3c69 6d67 2073 7263 3d22  n.pw"><img src="
+00000c30: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000c40: 6c64 732e 696f 2f64 6973 636f 7264 2f31  lds.io/discord/1
+00000c50: 3130 3635 3432 3232 3031 3132 3330 3231  1065422201123021
+00000c60: 3330 3f6c 6f67 6f3d 6469 7363 6f72 6426  30?logo=discord&
+00000c70: 6c6f 676f 436f 6c6f 723d 7768 6974 6526  logoColor=white&
+00000c80: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
+00000c90: 6522 3e3c 2f61 3e0d 0a3c 6120 6872 6566  e"></a>..<a href
+00000ca0: 3d22 6874 7470 733a 2f2f 7079 7069 7374  ="https://pypist
+00000cb0: 6174 732e 6f72 672f 7061 636b 6167 6573  ats.org/packages
+00000cc0: 2f63 6d6f 6e22 3e3c 696d 6720 616c 743d  /cmon"><img alt=
+00000cd0: 2250 7950 4920 2d20 446f 776e 6c6f 6164  "PyPI - Download
+00000ce0: 7320 6672 6f6d 206f 6666 6963 6961 6c20  s from official 
+00000cf0: 7079 7069 7374 6174 7322 2073 7263 3d22  pypistats" src="
+00000d00: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000d10: 6c64 732e 696f 2f70 7970 692f 646d 2f63  lds.io/pypi/dm/c
+00000d20: 6d6f 6e3f 7374 796c 653d 666c 6174 2d73  mon?style=flat-s
+00000d30: 7175 6172 6522 3e3c 2f61 3e0d 0a3c 6120  quare"></a>..<a 
+00000d40: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000d50: 7468 7562 2e63 6f6d 2f63 6d6f 6e2e 7077  thub.com/cmon.pw
+00000d60: 2f63 6d6f 6e2f 6163 7469 6f6e 732f 776f  /cmon/actions/wo
+00000d70: 726b 666c 6f77 732f 6364 2e79 6d6c 223e  rkflows/cd.yml">
+00000d80: 3c69 6d67 2061 6c74 3d22 4769 7468 7562  <img alt="Github
+00000d90: 2043 4420 7374 6174 7573 2220 7372 633d   CD status" src=
+00000da0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000db0: 636f 6d2f 636d 6f6e 2e70 772f 636d 6f6e  com/cmon.pw/cmon
+00000dc0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000dd0: 7773 2f63 642e 796d 6c2f 6261 6467 652e  ws/cd.yml/badge.
+00000de0: 7376 6722 3e3c 2f61 3e0d 0a3c 2f70 3e0d  svg"></a>..</p>.
+00000df0: 0a0d 0a3c 212d 2d20 7374 6172 7420 636d  ...<!-- start cm
+00000e00: 6f6e 2d64 6573 6372 6970 7469 6f6e 202d  on-description -
+00000e10: 2d3e 0d0a 0d0a 436d 6f6e 206c 6574 7320  ->....Cmon lets 
+00000e20: 796f 7520 6275 696c 6420 6d75 6c74 696d  you build multim
+00000e30: 6f64 616c 205b 2a2a 4149 2073 6572 7669  odal [**AI servi
+00000e40: 6365 732a 2a5d 2823 6275 696c 642d 6169  ces**](#build-ai
+00000e50: 2d73 6572 7669 6365 7329 2061 6e64 205b  -services) and [
+00000e60: 2a2a 7069 7065 6c69 6e65 732a 2a5d 2823  **pipelines**](#
+00000e70: 6275 696c 642d 612d 7069 7065 6c69 6e65  build-a-pipeline
+00000e80: 2920 7468 6174 2063 6f6d 6d75 6e69 6361  ) that communica
+00000e90: 7465 2076 6961 2067 5250 432c 2048 5454  te via gRPC, HTT
+00000ea0: 5020 616e 6420 5765 6253 6f63 6b65 7473  P and WebSockets
+00000eb0: 2c20 7468 656e 2073 6361 6c65 2074 6865  , then scale the
+00000ec0: 6d20 7570 2061 6e64 2064 6570 6c6f 7920  m up and deploy 
+00000ed0: 746f 2070 726f 6475 6374 696f 6e2e 2059  to production. Y
+00000ee0: 6f75 2063 616e 2066 6f63 7573 206f 6e20  ou can focus on 
+00000ef0: 796f 7572 206c 6f67 6963 2061 6e64 2061  your logic and a
+00000f00: 6c67 6f72 6974 686d 732c 2077 6974 686f  lgorithms, witho
+00000f10: 7574 2077 6f72 7279 696e 6720 6162 6f75  ut worrying abou
+00000f20: 7420 7468 6520 696e 6672 6173 7472 7563  t the infrastruc
+00000f30: 7475 7265 2063 6f6d 706c 6578 6974 792e  ture complexity.
+00000f40: 0d0a 0d0a 215b 5d28 2e2f 2e67 6974 6875  ....![](./.githu
+00000f50: 622f 696d 6167 6573 2f62 7569 6c64 2d64  b/images/build-d
+00000f60: 6570 6c6f 792e 706e 6729 0d0a 0d0a 436d  eploy.png)....Cm
+00000f70: 6f6e 2070 726f 7669 6465 7320 6120 736d  on provides a sm
+00000f80: 6f6f 7468 2050 7974 686f 6e69 6320 6578  ooth Pythonic ex
+00000f90: 7065 7269 656e 6365 2074 7261 6e73 6974  perience transit
+00000fa0: 696f 6e69 6e67 2066 726f 6d20 6c6f 6361  ioning from loca
+00000fb0: 6c20 6465 706c 6f79 6d65 6e74 2074 6f20  l deployment to 
+00000fc0: 6164 7661 6e63 6564 206f 7263 6865 7374  advanced orchest
+00000fd0: 7261 7469 6f6e 2066 7261 6d65 776f 726b  ration framework
+00000fe0: 7320 6c69 6b65 2044 6f63 6b65 722d 436f  s like Docker-Co
+00000ff0: 6d70 6f73 652c 204b 7562 6572 6e65 7465  mpose, Kubernete
+00001000: 732c 206f 7220 436d 6f6e 2041 4920 436c  s, or Cmon AI Cl
+00001010: 6f75 642e 2043 6d6f 6e20 6d61 6b65 7320  oud. Cmon makes 
+00001020: 6164 7661 6e63 6564 2073 6f6c 7574 696f  advanced solutio
+00001030: 6e20 656e 6769 6e65 6572 696e 6720 616e  n engineering an
+00001040: 6420 636c 6f75 642d 6e61 7469 7665 2074  d cloud-native t
+00001050: 6563 686e 6f6c 6f67 6965 7320 6163 6365  echnologies acce
+00001060: 7373 6962 6c65 2074 6f20 6576 6572 7920  ssible to every 
+00001070: 6465 7665 6c6f 7065 722e 0d0a 0d0a 2d20  developer.....- 
+00001080: 4275 696c 6420 6170 706c 6963 6174 696f  Build applicatio
+00001090: 6e73 2066 6f72 2061 6e79 205b 6461 7461  ns for any [data
+000010a0: 2074 7970 655d 2868 7474 7073 3a2f 2f64   type](https://d
+000010b0: 6f63 732e 646f 6361 7272 6179 2e6f 7267  ocs.docarray.org
+000010c0: 2f64 6174 615f 7479 7065 732f 6669 7273  /data_types/firs
+000010d0: 745f 7374 6570 732f 292c 2061 6e79 206d  t_steps/), any m
+000010e0: 6169 6e73 7472 6561 6d20 5b64 6565 7020  ainstream [deep 
+000010f0: 6c65 6172 6e69 6e67 2066 7261 6d65 776f  learning framewo
+00001100: 726b 5d28 292c 2061 6e64 2061 6e79 205b  rk](), and any [
+00001110: 7072 6f74 6f63 6f6c 5d28 6874 7470 733a  protocol](https:
+00001120: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+00001130: 6f6e 6365 7074 732f 7365 7276 696e 672f  oncepts/serving/
+00001140: 6761 7465 7761 792f 2373 6574 2d70 726f  gateway/#set-pro
+00001150: 746f 636f 6c2d 696e 2d70 7974 686f 6e29  tocol-in-python)
+00001160: 2e0d 0a2d 2044 6573 6967 6e20 6869 6768  ...- Design high
+00001170: 2d70 6572 666f 726d 616e 6365 206d 6963  -performance mic
+00001180: 726f 7365 7276 6963 6573 2c20 7769 7468  roservices, with
+00001190: 205b 6561 7379 2073 6361 6c69 6e67 5d28   [easy scaling](
+000011a0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+000011b0: 6e2e 7077 2f63 6f6e 6365 7074 732f 6f72  n.pw/concepts/or
+000011c0: 6368 6573 7472 6174 696f 6e2f 7363 616c  chestration/scal
+000011d0: 652d 6f75 742f 292c 2064 7570 6c65 7820  e-out/), duplex 
+000011e0: 636c 6965 6e74 2d73 6572 7665 7220 7374  client-server st
+000011f0: 7265 616d 696e 672c 2061 6e64 2061 7379  reaming, and asy
+00001200: 6e63 2f6e 6f6e 2d62 6c6f 636b 696e 6720  nc/non-blocking 
+00001210: 6461 7461 2070 726f 6365 7373 696e 6720  data processing 
+00001220: 6f76 6572 2064 796e 616d 6963 2066 6c6f  over dynamic flo
+00001230: 7773 2e0d 0a2d 2044 6f63 6b65 7220 636f  ws...- Docker co
+00001240: 6e74 6169 6e65 7220 696e 7465 6772 6174  ntainer integrat
+00001250: 696f 6e20 7669 6120 5b45 7865 6375 746f  ion via [Executo
+00001260: 7220 4875 625d 2868 7474 7073 3a2f 2f63  r Hub](https://c
+00001270: 6c6f 7564 2e63 6d6f 6e2e 7077 292c 204f  loud.cmon.pw), O
+00001280: 7065 6e54 656c 656d 6574 7279 2f50 726f  penTelemetry/Pro
+00001290: 6d65 7468 6575 7320 6f62 7365 7276 6162  metheus observab
+000012a0: 696c 6974 792c 2061 6e64 2066 6173 7420  ility, and fast 
+000012b0: 4b75 6265 726e 6574 6573 2f44 6f63 6b65  Kubernetes/Docke
+000012c0: 722d 436f 6d70 6f73 6520 6465 706c 6f79  r-Compose deploy
+000012d0: 6d65 6e74 2e0d 0a2d 2043 5055 2f47 5055  ment...- CPU/GPU
+000012e0: 2068 6f73 7469 6e67 2076 6961 205b 436d   hosting via [Cm
+000012f0: 6f6e 2041 4920 436c 6f75 645d 2868 7474  on AI Cloud](htt
+00001300: 7073 3a2f 2f63 6c6f 7564 2e63 6d6f 6e2e  ps://cloud.cmon.
+00001310: 7077 292e 0d0a 0d0a 3c64 6574 6169 6c73  pw).....<details
+00001320: 3e0d 0a20 2020 203c 7375 6d6d 6172 793e  >..    <summary>
+00001330: 3c73 7472 6f6e 673e 5761 6974 2c20 686f  <strong>Wait, ho
+00001340: 7720 6973 2043 6d6f 6e20 6469 6666 6572  w is Cmon differ
+00001350: 656e 7420 6672 6f6d 2046 6173 7441 5049  ent from FastAPI
+00001360: 3f3c 2f73 7472 6f6e 673e 3c2f 7375 6d6d  ?</strong></summ
+00001370: 6172 793e 0d0a 436d 6f6e 2773 2076 616c  ary>..Cmon's val
+00001380: 7565 2070 726f 706f 7369 7469 6f6e 206d  ue proposition m
+00001390: 6179 2073 6565 6d20 7175 6974 6520 7369  ay seem quite si
+000013a0: 6d69 6c61 7220 746f 2074 6861 7420 6f66  milar to that of
+000013b0: 2046 6173 7441 5049 2e20 486f 7765 7665   FastAPI. Howeve
+000013c0: 722c 2074 6865 7265 2061 7265 2073 6576  r, there are sev
+000013d0: 6572 616c 2066 756e 6461 6d65 6e74 616c  eral fundamental
+000013e0: 2064 6966 6665 7265 6e63 6573 3a0d 0a0d   differences:...
+000013f0: 0a20 2a2a 4461 7461 2073 7472 7563 7475  . **Data structu
+00001400: 7265 2061 6e64 2063 6f6d 6d75 6e69 6361  re and communica
+00001410: 7469 6f6e 2070 726f 746f 636f 6c73 2a2a  tion protocols**
+00001420: 0d0a 2020 2d20 4661 7374 4150 4920 636f  ..  - FastAPI co
+00001430: 6d6d 756e 6963 6174 696f 6e20 7265 6c69  mmunication reli
+00001440: 6573 206f 6e20 5079 6461 6e74 6963 2061  es on Pydantic a
+00001450: 6e64 2043 6d6f 6e20 7265 6c69 6573 206f  nd Cmon relies o
+00001460: 6e20 5b64 6f63 6172 7261 795d 2868 7474  n [docarray](htt
+00001470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001480: 646f 6361 7272 6179 2f64 6f63 6172 7261  docarray/docarra
+00001490: 7929 2061 6c6c 6f77 696e 6720 436d 6f6e  y) allowing Cmon
+000014a0: 2074 6f20 7375 7070 6f72 7420 6d75 6c74   to support mult
+000014b0: 6970 6c65 2070 726f 746f 636f 6c73 0d0a  iple protocols..
+000014c0: 2020 746f 2065 7870 6f73 6520 6974 7320    to expose its 
+000014d0: 7365 7276 6963 6573 2e0d 0a0d 0a20 2a2a  services..... **
+000014e0: 4164 7661 6e63 6564 206f 7263 6865 7374  Advanced orchest
+000014f0: 7261 7469 6f6e 2061 6e64 2073 6361 6c69  ration and scali
+00001500: 6e67 2063 6170 6162 696c 6974 6965 732a  ng capabilities*
+00001510: 2a0d 0a20 202d 2043 6d6f 6e20 6c65 7473  *..  - Cmon lets
+00001520: 2079 6f75 2064 6570 6c6f 7920 6170 706c   you deploy appl
+00001530: 6963 6174 696f 6e73 2066 6f72 6d65 6420  ications formed 
+00001540: 6672 6f6d 206d 756c 7469 706c 6520 6d69  from multiple mi
+00001550: 6372 6f73 6572 7669 6365 7320 7468 6174  croservices that
+00001560: 2063 616e 2062 6520 636f 6e74 6169 6e65   can be containe
+00001570: 7269 7a65 6420 616e 6420 7363 616c 6564  rized and scaled
+00001580: 2069 6e64 6570 656e 6465 6e74 6c79 2e0d   independently..
+00001590: 0a20 202d 2043 6d6f 6e20 616c 6c6f 7773  .  - Cmon allows
+000015a0: 2079 6f75 2074 6f20 6561 7369 6c79 2063   you to easily c
+000015b0: 6f6e 7461 696e 6572 697a 6520 616e 6420  ontainerize and 
+000015c0: 6f72 6368 6573 7472 6174 6520 796f 7572  orchestrate your
+000015d0: 2073 6572 7669 6365 732c 2070 726f 7669   services, provi
+000015e0: 6469 6e67 2063 6f6e 6375 7272 656e 6379  ding concurrency
+000015f0: 2061 6e64 2073 6361 6c61 6269 6c69 7479   and scalability
+00001600: 2e0d 0a0d 0a20 2a2a 4a6f 7572 6e65 7920  ..... **Journey 
+00001610: 746f 2074 6865 2063 6c6f 7564 2a2a 0d0a  to the cloud**..
+00001620: 2020 2d20 436d 6f6e 2070 726f 7669 6465    - Cmon provide
+00001630: 7320 6120 736d 6f6f 7468 2074 7261 6e73  s a smooth trans
+00001640: 6974 696f 6e20 6672 6f6d 206c 6f63 616c  ition from local
+00001650: 2064 6576 656c 6f70 6d65 6e74 2028 7573   development (us
+00001660: 696e 6720 5b64 6f63 6172 7261 795d 2868  ing [docarray](h
+00001670: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001680: 6d2f 646f 6361 7272 6179 2f64 6f63 6172  m/docarray/docar
+00001690: 7261 7929 2920 746f 206c 6f63 616c 2073  ray)) to local s
+000016a0: 6572 7669 6e67 2075 7369 6e67 2028 436d  erving using (Cm
+000016b0: 6f6e 2773 206f 7263 6865 7374 7261 7469  on's orchestrati
+000016c0: 6f6e 206c 6179 6572 290d 0a20 2074 6f20  on layer)..  to 
+000016d0: 6861 7669 6e67 2070 726f 6475 6374 696f  having productio
+000016e0: 6e2d 7265 6164 7920 7365 7276 6963 6573  n-ready services
+000016f0: 2062 7920 7573 696e 6720 4b75 6265 726e   by using Kubern
+00001700: 6574 6573 2063 6170 6163 6974 7920 746f  etes capacity to
+00001710: 206f 7263 6865 7374 7261 7465 2074 6865   orchestrate the
+00001720: 206c 6966 6574 696d 6520 6f66 2063 6f6e   lifetime of con
+00001730: 7461 696e 6572 732e 0d0a 2020 2d20 4279  tainers...  - By
+00001740: 2075 7369 6e67 205b 436d 6f6e 2041 4920   using [Cmon AI 
+00001750: 436c 6f75 645d 2868 7474 7073 3a2f 2f63  Cloud](https://c
+00001760: 6c6f 7564 2e63 6d6f 6e2e 7077 2920 796f  loud.cmon.pw) yo
+00001770: 7520 6861 7665 2061 6363 6573 7320 746f  u have access to
+00001780: 2073 6361 6c61 626c 6520 616e 6420 7365   scalable and se
+00001790: 7276 6572 6c65 7373 2064 6570 6c6f 796d  rverless deploym
+000017a0: 656e 7473 206f 6620 796f 7572 2061 7070  ents of your app
+000017b0: 6c69 6361 7469 6f6e 7320 696e 206f 6e65  lications in one
+000017c0: 2063 6f6d 6d61 6e64 2e0d 0a3c 2f64 6574   command...</det
+000017d0: 6169 6c73 3e0d 0a0d 0a3c 212d 2d20 656e  ails>....<!-- en
+000017e0: 6420 636d 6f6e 2d64 6573 6372 6970 7469  d cmon-descripti
+000017f0: 6f6e 202d 2d3e 0d0a 0d0a 2323 205b 446f  on -->....## [Do
+00001800: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00001810: 7073 3a2f 2f64 6f63 732e 636d 6f6e 2e70  ps://docs.cmon.p
+00001820: 7729 0d0a 0d0a 2323 2049 6e73 7461 6c6c  w)....## Install
+00001830: 200d 0a0d 0a4e 6f74 653a 2028 5769 6e64   ....Note: (Wind
+00001840: 6f77 7329 206e 6f74 2073 7570 706f 7274  ows) not support
+00001850: 6564 2061 7420 7468 6973 206d 6f6d 656e  ed at this momen
+00001860: 7421 2059 6f75 206d 6179 2072 6571 7569  t! You may requi
+00001870: 7265 2074 6f20 696e 7374 616c 6c20 6974  re to install it
+00001880: 206f 6e20 2857 534c 292e 0d0a 5b20 2055   on (WSL)...[  U
+00001890: 5044 4154 4520 205d 203a 2057 696e 646f  PDATE  ] : Windo
+000018a0: 7773 2053 7570 706f 7274 2061 6464 6564  ws Support added
+000018b0: 210d 0a0d 0a60 6060 6261 7368 0d0a 7069  !....```bash..pi
+000018c0: 7020 696e 7374 616c 6c20 636d 6f6e 2d61  p install cmon-a
+000018d0: 690d 0a60 6060 0d0a 0d0a 4669 6e64 206d  i..```....Find m
+000018e0: 6f72 6520 696e 7374 616c 6c20 6f70 7469  ore install opti
+000018f0: 6f6e 7320 6f6e 205b 4170 706c 6520 5369  ons on [Apple Si
+00001900: 6c69 636f 6e5d 2868 7474 7073 3a2f 2f64  licon](https://d
+00001910: 6f63 732e 636d 6f6e 2e70 772f 6765 742d  ocs.cmon.pw/get-
+00001920: 7374 6172 7465 642f 696e 7374 616c 6c2f  started/install/
+00001930: 6170 706c 652d 7369 6c69 636f 6e2d 6d31  apple-silicon-m1
+00001940: 2d6d 322f 290d 0a0d 0a0d 0a23 2320 4765  -m2/)......## Ge
+00001950: 7420 5374 6172 7465 640d 0a0d 0a23 2323  t Started....###
+00001960: 2042 6173 6963 2043 6f6e 6365 7074 730d   Basic Concepts.
+00001970: 0a0d 0a43 6d6f 6e20 6861 7320 666f 7572  ...Cmon has four
+00001980: 2066 756e 6461 6d65 6e74 616c 2063 6f6e   fundamental con
+00001990: 6365 7074 733a 0d0a 0d0a 2d20 4120 5b2a  cepts:....- A [*
+000019a0: 2a44 6f63 756d 656e 742a 2a5d 2868 7474  *Document**](htt
+000019b0: 7073 3a2f 2f64 6f63 6172 7261 792e 636d  ps://docarray.cm
+000019c0: 6f6e 2e70 772f 2920 2866 726f 6d20 5b64  on.pw/) (from [d
+000019d0: 6f63 6172 7261 795d 2868 7474 7073 3a2f  ocarray](https:/
+000019e0: 2f67 6974 6875 622e 636f 6d2f 646f 6361  /github.com/doca
+000019f0: 7272 6179 2f64 6f63 6172 7261 7929 2920  rray/docarray)) 
+00001a00: 6973 2074 6865 2069 6e70 7574 2f6f 7574  is the input/out
+00001a10: 7075 7420 666f 726d 6174 2069 6e20 436d  put format in Cm
+00001a20: 6f6e 2e0d 0a2d 2041 6e20 5b2a 2a45 7865  on...- An [**Exe
+00001a30: 6375 746f 722a 2a5d 2868 7474 7073 3a2f  cutor**](https:/
+00001a40: 2f64 6f63 732e 636d 6f6e 2e70 772f 636f  /docs.cmon.pw/co
+00001a50: 6e63 6570 7473 2f73 6572 7669 6e67 2f65  ncepts/serving/e
+00001a60: 7865 6375 746f 722f 2920 6973 2061 2050  xecutor/) is a P
+00001a70: 7974 686f 6e20 636c 6173 7320 7468 6174  ython class that
+00001a80: 2074 7261 6e73 666f 726d 7320 616e 6420   transforms and 
+00001a90: 7072 6f63 6573 7365 7320 446f 6375 6d65  processes Docume
+00001aa0: 6e74 732e 0d0a 2d20 4120 5b2a 2a44 6570  nts...- A [**Dep
+00001ab0: 6c6f 796d 656e 742a 2a5d 2868 7474 7073  loyment**](https
+00001ac0: 3a2f 2f64 6f63 732e 636d 6f6e 2e70 772f  ://docs.cmon.pw/
+00001ad0: 636f 6e63 6570 7473 2f6f 7263 6865 7374  concepts/orchest
+00001ae0: 7261 7469 6f6e 2f64 6570 6c6f 796d 656e  ration/deploymen
+00001af0: 7429 2073 6572 7665 7320 6120 7369 6e67  t) serves a sing
+00001b00: 6c65 2045 7865 6375 746f 722c 2077 6869  le Executor, whi
+00001b10: 6c65 2061 205b 2a2a 466c 6f77 2a2a 5d28  le a [**Flow**](
+00001b20: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00001b30: 6e2e 7077 2f63 6f6e 6365 7074 732f 6f72  n.pw/concepts/or
+00001b40: 6368 6573 7472 6174 696f 6e2f 666c 6f77  chestration/flow
+00001b50: 2f29 2073 6572 7665 7320 4578 6563 7574  /) serves Execut
+00001b60: 6f72 7320 6368 6169 6e65 6420 696e 746f  ors chained into
+00001b70: 2061 2070 6970 656c 696e 652e 0d0a 0d0a   a pipeline.....
+00001b80: 0d0a 5b54 6865 2066 756c 6c20 676c 6f73  ..[The full glos
+00001b90: 7361 7279 2069 7320 6578 706c 6169 6e65  sary is explaine
+00001ba0: 6420 6865 7265 5d28 6874 7470 733a 2f2f  d here](https://
+00001bb0: 646f 6373 2e63 6d6f 6e2e 7077 2f63 6f6e  docs.cmon.pw/con
+00001bc0: 6365 7074 732f 7072 656c 696d 696e 6172  cepts/preliminar
+00001bd0: 6965 732f 2329 2e0d 0a0d 0a23 2323 2042  ies/#).....### B
+00001be0: 7569 6c64 2041 4920 5365 7276 6963 6573  uild AI Services
+00001bf0: 0d0a 3c21 2d2d 2073 7461 7274 2062 7569  ..<!-- start bui
+00001c00: 6c64 2d61 692d 7365 7276 6963 6573 202d  ld-ai-services -
+00001c10: 2d3e 0d0a 0d0a 4c65 7427 7320 6275 696c  ->....Let's buil
+00001c20: 6420 6120 6661 7374 2c20 7265 6c69 6162  d a fast, reliab
+00001c30: 6c65 2061 6e64 2073 6361 6c61 626c 6520  le and scalable 
+00001c40: 6752 5043 2d62 6173 6564 2041 4920 7365  gRPC-based AI se
+00001c50: 7276 6963 652e 2049 6e20 436d 6f6e 2077  rvice. In Cmon w
+00001c60: 6520 6361 6c6c 2074 6869 7320 616e 202a  e call this an *
+00001c70: 2a5b 4578 6563 7574 6f72 5d28 6874 7470  *[Executor](http
+00001c80: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 7077  s://docs.cmon.pw
+00001c90: 2f63 6f6e 6365 7074 732f 6578 6563 7574  /concepts/execut
+00001ca0: 6f72 2f29 2a2a 2e20 4f75 7220 7369 6d70  or/)**. Our simp
+00001cb0: 6c65 2045 7865 6375 746f 7220 7769 6c6c  le Executor will
+00001cc0: 2077 7261 7020 7468 6520 5b53 7461 626c   wrap the [Stabl
+00001cd0: 654c 4d5d 2868 7474 7073 3a2f 2f68 7567  eLM](https://hug
+00001ce0: 6769 6e67 6661 6365 2e63 6f2f 7374 6162  gingface.co/stab
+00001cf0: 696c 6974 7961 692f 7374 6162 6c65 6c6d  ilityai/stablelm
+00001d00: 2d62 6173 652d 616c 7068 612d 3362 2920  -base-alpha-3b) 
+00001d10: 4c4c 4d20 6672 6f6d 2053 7461 6269 6c69  LLM from Stabili
+00001d20: 7479 2041 492e 2057 6527 6c6c 2074 6865  ty AI. We'll the
+00001d30: 6e20 7573 6520 6120 2a2a 4465 706c 6f79  n use a **Deploy
+00001d40: 6d65 6e74 2a2a 2074 6f20 7365 7276 6520  ment** to serve 
+00001d50: 6974 2e0d 0a0d 0a21 5b5d 282e 2f2e 6769  it.....![](./.gi
+00001d60: 7468 7562 2f69 6d61 6765 732f 6465 706c  thub/images/depl
+00001d70: 6f79 6d65 6e74 2d64 6961 6772 616d 2e70  oyment-diagram.p
+00001d80: 6e67 290d 0a0d 0a3e 202a 2a4e 6f74 652a  ng)....> **Note*
+00001d90: 2a0d 0a3e 2041 2044 6570 6c6f 796d 656e  *..> A Deploymen
+00001da0: 7420 7365 7276 6573 206a 7573 7420 6f6e  t serves just on
+00001db0: 6520 4578 6563 7574 6f72 2e20 546f 2063  e Executor. To c
+00001dc0: 6f6d 6269 6e65 206d 756c 7469 706c 6520  ombine multiple 
+00001dd0: 4578 6563 7574 6f72 7320 696e 746f 2061  Executors into a
+00001de0: 2070 6970 656c 696e 6520 616e 6420 7365   pipeline and se
+00001df0: 7276 6520 7468 6174 2c20 7573 6520 6120  rve that, use a 
+00001e00: 5b46 6c6f 775d 2823 6275 696c 642d 612d  [Flow](#build-a-
+00001e10: 7069 7065 6c69 6e65 292e 0d0a 0d0a 4c65  pipeline).....Le
+00001e20: 7427 7320 696d 706c 656d 656e 7420 7468  t's implement th
+00001e30: 6520 7365 7276 6963 6527 7320 6c6f 6769  e service's logi
+00001e40: 633a 0d0a 0d0a 3c74 6162 6c65 3e0d 0a3c  c:....<table>..<
+00001e50: 7472 3e0d 0a3c 7468 3e3c 636f 6465 3e65  tr>..<th><code>e
+00001e60: 7865 6375 746f 722e 7079 3c2f 636f 6465  xecutor.py</code
+00001e70: 3e3c 2f74 683e 200d 0a3c 7472 3e0d 0a3c  ></th> ..<tr>..<
+00001e80: 7464 3e0d 0a0d 0a60 6060 7079 7468 6f6e  td>....```python
+00001e90: 0d0a 6672 6f6d 2063 6d6f 6e20 696d 706f  ..from cmon impo
+00001ea0: 7274 2045 7865 6375 746f 722c 2072 6571  rt Executor, req
+00001eb0: 7565 7374 730d 0a66 726f 6d20 646f 6361  uests..from doca
+00001ec0: 7272 6179 2069 6d70 6f72 7420 446f 6375  rray import Docu
+00001ed0: 6d65 6e74 4172 7261 790d 0a0d 0a66 726f  mentArray....fro
+00001ee0: 6d20 7472 616e 7366 6f72 6d65 7273 2069  m transformers i
+00001ef0: 6d70 6f72 7420 7069 7065 6c69 6e65 0d0a  mport pipeline..
+00001f00: 0d0a 0d0a 636c 6173 7320 5374 6162 6c65  ....class Stable
+00001f10: 4c4d 2845 7865 6375 746f 7229 3a0d 0a0d  LM(Executor):...
+00001f20: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001f30: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
+00001f40: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
+00001f50: 7228 292e 5f5f 696e 6974 5f5f 282a 2a6b  r().__init__(**k
+00001f60: 7761 7267 7329 0d0a 2020 2020 2020 2020  wargs)..        
+00001f70: 7365 6c66 2e67 656e 6572 6174 6f72 203d  self.generator =
+00001f80: 2070 6970 656c 696e 6528 2774 6578 742d   pipeline('text-
+00001f90: 6765 6e65 7261 7469 6f6e 272c 206d 6f64  generation', mod
+00001fa0: 656c 3d27 7374 6162 6c65 6c6d 2d33 6227  el='stablelm-3b'
+00001fb0: 290d 0a0d 0a20 2020 2040 7265 7175 6573  )....    @reques
+00001fc0: 7473 0d0a 2020 2020 6465 6620 6765 6e65  ts..    def gene
+00001fd0: 7261 7465 2873 656c 662c 2064 6f63 733a  rate(self, docs:
+00001fe0: 2044 6f63 756d 656e 7441 7272 6179 2c20   DocumentArray, 
+00001ff0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+00002000: 2020 2020 6765 6e65 7261 7465 645f 7465      generated_te
+00002010: 7874 203d 2073 656c 662e 6765 6e65 7261  xt = self.genera
+00002020: 746f 7228 646f 6373 2e74 6578 7473 290d  tor(docs.texts).
+00002030: 0a20 2020 2020 2020 2064 6f63 732e 7465  .        docs.te
+00002040: 7874 7320 3d20 5b67 656e 5b30 5d5b 2767  xts = [gen[0]['g
+00002050: 656e 6572 6174 6564 5f74 6578 7427 5d20  enerated_text'] 
+00002060: 666f 7220 6765 6e20 696e 2067 656e 6572  for gen in gener
+00002070: 6174 6564 5f74 6578 745d 0d0a 6060 600d  ated_text]..```.
+00002080: 0a0d 0a3c 2f74 643e 0d0a 3c2f 7472 3e0d  ...</td>..</tr>.
+00002090: 0a3c 2f74 6162 6c65 3e0d 0a0d 0a54 6865  .</table>....The
+000020a0: 6e20 7765 2064 6570 6c6f 7920 6974 2077  n we deploy it w
+000020b0: 6974 6820 6569 7468 6572 2074 6865 2050  ith either the P
+000020c0: 7974 686f 6e20 4150 4920 6f72 2059 414d  ython API or YAM
+000020d0: 4c3a 0d0a 3c64 6976 2063 6c61 7373 3d22  L:..<div class="
+000020e0: 7461 626c 652d 7772 6170 7065 7222 3e0d  table-wrapper">.
+000020f0: 0a3c 7461 626c 653e 0d0a 3c74 723e 0d0a  .<table>..<tr>..
+00002100: 3c74 683e 2050 7974 686f 6e20 4150 493a  <th> Python API:
+00002110: 203c 636f 6465 3e64 6570 6c6f 796d 656e   <code>deploymen
+00002120: 742e 7079 3c2f 636f 6465 3e20 3c2f 7468  t.py</code> </th
+00002130: 3e20 0d0a 3c74 683e 2059 414d 4c3a 203c  > ..<th> YAML: <
+00002140: 636f 6465 3e64 6570 6c6f 796d 656e 742e  code>deployment.
+00002150: 796d 6c3c 2f63 6f64 653e 203c 2f74 683e  yml</code> </th>
+00002160: 0d0a 3c2f 7472 3e0d 0a3c 7472 3e0d 0a3c  ..</tr>..<tr>..<
+00002170: 7464 3e0d 0a0d 0a60 6060 7079 7468 6f6e  td>....```python
+00002180: 0d0a 6672 6f6d 2063 6d6f 6e20 696d 706f  ..from cmon impo
+00002190: 7274 2044 6570 6c6f 796d 656e 740d 0a66  rt Deployment..f
+000021a0: 726f 6d20 6578 6563 7574 6f72 2069 6d70  rom executor imp
+000021b0: 6f72 7420 5374 6162 6c65 4c4d 0d0a 0d0a  ort StableLM....
+000021c0: 6465 7020 3d20 4465 706c 6f79 6d65 6e74  dep = Deployment
+000021d0: 2875 7365 733d 5374 6162 6c65 4c4d 2c20  (uses=StableLM, 
+000021e0: 7469 6d65 6f75 745f 7265 6164 793d 2d31  timeout_ready=-1
+000021f0: 2c20 706f 7274 3d31 3233 3435 290d 0a0d  , port=12345)...
+00002200: 0a77 6974 6820 6465 703a 0d0a 2020 2020  .with dep:..    
+00002210: 6465 702e 626c 6f63 6b28 290d 0a60 6060  dep.block()..```
+00002220: 0d0a 0d0a 3c2f 7464 3e0d 0a3c 7464 3e0d  ....</td>..<td>.
+00002230: 0a0d 0a60 6060 7961 6d6c 0d0a 6a74 7970  ...```yaml..jtyp
+00002240: 653a 2044 6570 6c6f 796d 656e 740d 0a77  e: Deployment..w
+00002250: 6974 683a 0d0a 2020 7573 6573 3a20 5374  ith:..  uses: St
+00002260: 6162 6c65 4c4d 0d0a 2020 7079 5f6d 6f64  ableLM..  py_mod
+00002270: 756c 6573 3a0d 0a20 2020 202d 2065 7865  ules:..    - exe
+00002280: 6375 746f 722e 7079 0d0a 2020 7469 6d65  cutor.py..  time
+00002290: 6f75 745f 7265 6164 793a 202d 310d 0a20  out_ready: -1.. 
+000022a0: 2070 6f72 743a 2031 3233 3435 0d0a 6060   port: 12345..``
+000022b0: 600d 0a0d 0a41 6e64 2072 756e 2074 6865  `....And run the
+000022c0: 2059 414d 4c20 4465 706c 6f79 6d65 6e74   YAML Deployment
+000022d0: 2077 6974 6820 7468 6520 434c 493a 2060   with the CLI: `
+000022e0: 636d 6f6e 2064 6570 6c6f 796d 656e 7420  cmon deployment 
+000022f0: 2d2d 7573 6573 2064 6570 6c6f 796d 656e  --uses deploymen
+00002300: 742e 796d 6c60 0d0a 0d0a 3c2f 7464 3e0d  t.yml`....</td>.
+00002310: 0a3c 2f74 723e 0d0a 3c2f 7461 626c 653e  .</tr>..</table>
+00002320: 0d0a 3c2f 6469 763e 0d0a 0d0a 5573 6520  ..</div>....Use 
+00002330: 5b43 6d6f 6e20 436c 6965 6e74 5d28 6874  [Cmon Client](ht
+00002340: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
+00002350: 7077 2f63 6f6e 6365 7074 732f 636c 6965  pw/concepts/clie
+00002360: 6e74 2f29 2074 6f20 6d61 6b65 2072 6571  nt/) to make req
+00002370: 7565 7374 7320 746f 2074 6865 2073 6572  uests to the ser
+00002380: 7669 6365 3a0d 0a0d 0a60 6060 7079 7468  vice:....```pyth
+00002390: 6f6e 0d0a 6672 6f6d 2064 6f63 6172 7261  on..from docarra
+000023a0: 7920 696d 706f 7274 2044 6f63 756d 656e  y import Documen
+000023b0: 740d 0a66 726f 6d20 636d 6f6e 2069 6d70  t..from cmon imp
+000023c0: 6f72 7420 436c 6965 6e74 0d0a 0d0a 7072  ort Client....pr
+000023d0: 6f6d 7074 203d 2044 6f63 756d 656e 7428  ompt = Document(
+000023e0: 0d0a 2020 2020 7461 6773 203d 207b 2770  ..    tags = {'p
+000023f0: 726f 6d70 7427 3a20 2773 7567 6765 7374  rompt': 'suggest
+00002400: 2061 6e20 696e 7465 7265 7374 696e 6720   an interesting 
+00002410: 696d 6167 6520 6765 6e65 7261 7469 6f6e  image generation
+00002420: 2070 726f 6d70 7420 666f 7220 6120 6d6f   prompt for a mo
+00002430: 6e61 206c 6973 6120 7661 7269 616e 7427  na lisa variant'
+00002440: 7d0d 0a29 0d0a 0d0a 636c 6965 6e74 203d  }..)....client =
+00002450: 2043 6c69 656e 7428 706f 7274 3d31 3233   Client(port=123
+00002460: 3435 2920 2023 2075 7365 2070 6f72 7420  45)  # use port 
+00002470: 6672 6f6d 206f 7574 7075 7420 6162 6f76  from output abov
+00002480: 650d 0a72 6573 706f 6e73 6520 3d20 636c  e..response = cl
+00002490: 6965 6e74 2e70 6f73 7428 6f6e 3d27 2f27  ient.post(on='/'
+000024a0: 2c20 696e 7075 7473 3d5b 7072 6f6d 7074  , inputs=[prompt
+000024b0: 5d29 0d0a 0d0a 7072 696e 7428 7265 7370  ])....print(resp
+000024c0: 6f6e 7365 5b30 5d2e 7465 7874 290d 0a60  onse[0].text)..`
+000024d0: 6060 0d0a 0d0a 6060 6074 6578 740d 0a61  ``....```text..a
+000024e0: 2073 7465 616d 7075 6e6b 2076 6572 7369   steampunk versi
+000024f0: 6f6e 206f 6620 7468 6520 4d6f 6e61 204c  on of the Mona L
+00002500: 6973 612c 2069 6e63 6f72 706f 7261 7469  isa, incorporati
+00002510: 6e67 206d 6563 6861 6e69 6361 6c20 6765  ng mechanical ge
+00002520: 6172 732c 2062 7261 7373 2065 6c65 6d65  ars, brass eleme
+00002530: 6e74 732c 2061 6e64 2056 6963 746f 7269  nts, and Victori
+00002540: 616e 2065 7261 2063 6c6f 7468 696e 6720  an era clothing 
+00002550: 6465 7461 696c 730d 0a60 6060 0d0a 0d0a  details..```....
+00002560: 3c21 2d2d 2065 6e64 2062 7569 6c64 2d61  <!-- end build-a
+00002570: 692d 7365 7276 6963 6573 202d 2d3e 0d0a  i-services -->..
+00002580: 0d0a 3e20 2a2a 4e6f 7465 2a2a 0d0a 3e20  ..> **Note**..> 
+00002590: 496e 2061 206e 6f74 6562 6f6f 6b2c 2079  In a notebook, y
+000025a0: 6f75 2063 616e 2774 2075 7365 2060 6465  ou can't use `de
+000025b0: 706c 6f79 6d65 6e74 2e62 6c6f 636b 2829  ployment.block()
+000025c0: 6020 616e 6420 7468 656e 206d 616b 6520  ` and then make 
+000025d0: 7265 7175 6573 7473 2074 6f20 7468 6520  requests to the 
+000025e0: 636c 6965 6e74 2e20 506c 6561 7365 2072  client. Please r
+000025f0: 6566 6572 2074 6f20 7468 6520 436f 6c61  efer to the Cola
+00002600: 6220 6c69 6e6b 2061 626f 7665 2066 6f72  b link above for
+00002610: 2072 6570 726f 6475 6369 626c 6520 4a75   reproducible Ju
+00002620: 7079 7465 7220 4e6f 7465 626f 6f6b 2063  pyter Notebook c
+00002630: 6f64 6520 736e 6970 7065 7473 2e0d 0a0d  ode snippets....
+00002640: 0a23 2323 2042 7569 6c64 2061 2070 6970  .### Build a pip
+00002650: 656c 696e 650d 0a0d 0a3c 212d 2d20 7374  eline....<!-- st
+00002660: 6172 7420 6275 696c 642d 7069 7065 6c69  art build-pipeli
+00002670: 6e65 7320 2d2d 3e0d 0a0d 0a53 6f6d 6574  nes -->....Somet
+00002680: 696d 6573 2079 6f75 2077 616e 7420 746f  imes you want to
+00002690: 2063 6861 696e 206d 6963 726f 7365 7276   chain microserv
+000026a0: 6963 6573 2074 6f67 6574 6865 7220 696e  ices together in
+000026b0: 746f 2061 2070 6970 656c 696e 652e 2054  to a pipeline. T
+000026c0: 6861 7427 7320 7768 6572 6520 6120 5b46  hat's where a [F
+000026d0: 6c6f 775d 2868 7474 7073 3a2f 2f64 6f63  low](https://doc
+000026e0: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+000026f0: 7473 2f66 6c6f 772f 2920 636f 6d65 7320  ts/flow/) comes 
+00002700: 696e 2e0d 0a0d 0a41 2046 6c6f 7720 6973  in.....A Flow is
+00002710: 2061 205b 4441 475d 2868 7474 7073 3a2f   a [DAG](https:/
+00002720: 2f64 652e 7769 6b69 7065 6469 612e 6f72  /de.wikipedia.or
+00002730: 672f 7769 6b69 2f44 4147 2920 7069 7065  g/wiki/DAG) pipe
+00002740: 6c69 6e65 2c20 636f 6d70 6f73 6564 206f  line, composed o
+00002750: 6620 6120 7365 7420 6f66 2073 7465 7073  f a set of steps
+00002760: 2c20 4974 206f 7263 6865 7374 7261 7465  , It orchestrate
+00002770: 7320 6120 7365 7420 6f66 205b 4578 6563  s a set of [Exec
+00002780: 7574 6f72 735d 2868 7474 7073 3a2f 2f64  utors](https://d
+00002790: 6f63 732e 636d 6f6e 2e70 772f 636f 6e63  ocs.cmon.pw/conc
+000027a0: 6570 7473 2f65 7865 6375 746f 722f 2920  epts/executor/) 
+000027b0: 616e 6420 6120 5b47 6174 6577 6179 5d28  and a [Gateway](
+000027c0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+000027d0: 6e2e 7077 2f63 6f6e 6365 7074 732f 6761  n.pw/concepts/ga
+000027e0: 7465 7761 792f 2920 746f 206f 6666 6572  teway/) to offer
+000027f0: 2061 6e20 656e 642d 746f 2d65 6e64 2073   an end-to-end s
+00002800: 6572 7669 6365 2e0d 0a0d 0a3e 202a 2a4e  ervice.....> **N
+00002810: 6f74 652a 2a0d 0a3e 2049 6620 796f 7520  ote**..> If you 
+00002820: 6a75 7374 2077 616e 7420 746f 2073 6572  just want to ser
+00002830: 7665 2061 2073 696e 676c 6520 4578 6563  ve a single Exec
+00002840: 7574 6f72 2c20 796f 7520 6361 6e20 7573  utor, you can us
+00002850: 6520 6120 5b44 6570 6c6f 796d 656e 745d  e a [Deployment]
+00002860: 2823 6275 696c 642d 6169 2d2d 6d6c 2d73  (#build-ai--ml-s
+00002870: 6572 7669 6365 7329 2e0d 0a0d 0a46 6f72  ervices).....For
+00002880: 2069 6e73 7461 6e63 652c 206c 6574 2773   instance, let's
+00002890: 2063 6f6d 6269 6e65 205b 6f75 7220 5374   combine [our St
+000028a0: 6162 6c65 4c4d 206c 616e 6775 6167 6520  ableLM language 
+000028b0: 6d6f 6465 6c5d 2823 6275 696c 642d 6169  model](#build-ai
+000028c0: 2d2d 6d6c 2d73 6572 7669 6365 7329 2077  --ml-services) w
+000028d0: 6974 6820 6120 5374 6162 6c65 2044 6966  ith a Stable Dif
+000028e0: 6675 7369 6f6e 2069 6d61 6765 2067 656e  fusion image gen
+000028f0: 6572 6174 696f 6e20 7365 7276 6963 6520  eration service 
+00002900: 6672 6f6d 2043 6d6f 6e20 4149 2773 205b  from Cmon AI's [
+00002910: 4578 6563 7574 6f72 2048 7562 5d28 6874  Executor Hub](ht
+00002920: 7470 733a 2f2f 636c 6f75 642e 636d 6f6e  tps://cloud.cmon
+00002930: 2e70 772f 6578 6563 7574 6f72 7329 2e20  .pw/executors). 
+00002940: 4368 6169 6e69 6e67 2074 6865 7365 2073  Chaining these s
+00002950: 6572 7669 6365 7320 746f 6765 7468 6572  ervices together
+00002960: 2069 6e74 6f20 6120 5b46 6c6f 775d 2868   into a [Flow](h
+00002970: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
+00002980: 2e70 772f 636f 6e63 6570 7473 2f66 6c6f  .pw/concepts/flo
+00002990: 772f 2920 7769 6c6c 2067 6976 6520 7573  w/) will give us
+000029a0: 2061 2073 6572 7669 6365 2074 6861 7420   a service that 
+000029b0: 7769 6c6c 2067 656e 6572 6174 6520 696d  will generate im
+000029c0: 6167 6573 2062 6173 6564 206f 6e20 6120  ages based on a 
+000029d0: 7072 6f6d 7074 2067 656e 6572 6174 6564  prompt generated
+000029e0: 2062 7920 7468 6520 4c4c 4d2e 0d0a 0d0a   by the LLM.....
+000029f0: 215b 5d28 2e2f 2e67 6974 6875 622f 696d  ![](./.github/im
+00002a00: 6167 6573 2f66 6c6f 772d 6469 6167 7261  ages/flow-diagra
+00002a10: 6d2e 706e 6729 0d0a 0d0a 4275 696c 6420  m.png)....Build 
+00002a20: 7468 6520 466c 6f77 2077 6974 6820 6569  the Flow with ei
+00002a30: 7468 6572 2050 7974 686f 6e20 6f72 2059  ther Python or Y
+00002a40: 414d 4c3a 0d0a 0d0a 3c64 6976 2063 6c61  AML:....<div cla
+00002a50: 7373 3d22 7461 626c 652d 7772 6170 7065  ss="table-wrappe
+00002a60: 7222 3e0d 0a3c 7461 626c 653e 0d0a 3c74  r">..<table>..<t
+00002a70: 723e 0d0a 3c74 683e 2050 7974 686f 6e20  r>..<th> Python 
+00002a80: 4150 493a 203c 636f 6465 3e66 6c6f 772e  API: <code>flow.
+00002a90: 7079 3c2f 636f 6465 3e20 3c2f 7468 3e20  py</code> </th> 
+00002aa0: 0d0a 3c74 683e 2059 414d 4c3a 203c 636f  ..<th> YAML: <co
+00002ab0: 6465 3e66 6c6f 772e 796d 6c3c 2f63 6f64  de>flow.yml</cod
+00002ac0: 653e 203c 2f74 683e 0d0a 3c2f 7472 3e0d  e> </th>..</tr>.
+00002ad0: 0a3c 7472 3e0d 0a3c 7464 3e0d 0a0d 0a60  .<tr>..<td>....`
+00002ae0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2063  ``python..from c
+00002af0: 6d6f 6e20 696d 706f 7274 2046 6c6f 770d  mon import Flow.
+00002b00: 0a66 726f 6d20 6578 6563 7574 6f72 2069  .from executor i
+00002b10: 6d70 6f72 7420 5374 6162 6c65 4c4d 0d0a  mport StableLM..
+00002b20: 0d0a 666c 6f77 203d 2028 0d0a 2020 2020  ..flow = (..    
+00002b30: 466c 6f77 2829 0d0a 2020 2020 2e61 6464  Flow()..    .add
+00002b40: 2875 7365 733d 5374 6162 6c65 4c4d 2c20  (uses=StableLM, 
+00002b50: 7469 6d65 6f75 745f 7265 6164 793d 2d31  timeout_ready=-1
+00002b60: 2c20 706f 7274 3d31 3233 3435 290d 0a20  , port=12345).. 
+00002b70: 2020 202e 6164 6428 0d0a 2020 2020 2020     .add(..      
+00002b80: 2020 7573 6573 3d27 636d 6f6e 6169 3a2f    uses='cmonai:/
+00002b90: 2f63 6d6f 6e2e 7077 2f54 6578 7454 6f49  /cmon.pw/TextToI
+00002ba0: 6d61 6765 272c 0d0a 2020 2020 2020 2020  mage',..        
+00002bb0: 7469 6d65 6f75 745f 7265 6164 793d 2d31  timeout_ready=-1
+00002bc0: 2c0d 0a20 2020 2020 2020 2069 6e73 7461  ,..        insta
+00002bd0: 6c6c 5f72 6571 7569 7265 6d65 6e74 733d  ll_requirements=
+00002be0: 5472 7565 2c0d 0a20 2020 2029 0d0a 2920  True,..    )..) 
+00002bf0: 2023 2075 7365 2074 6865 2045 7865 6375   # use the Execu
+00002c00: 746f 7220 6672 6f6d 2043 6d6f 6e27 7320  tor from Cmon's 
+00002c10: 4578 6563 7574 6f72 2068 7562 0d0a 0d0a  Executor hub....
+00002c20: 7769 7468 2066 6c6f 773a 0d0a 2020 2020  with flow:..    
+00002c30: 666c 6f77 2e62 6c6f 636b 2829 0d0a 6060  flow.block()..``
+00002c40: 600d 0a0d 0a3c 2f74 643e 0d0a 3c74 643e  `....</td>..<td>
+00002c50: 0d0a 0d0a 6060 6079 616d 6c0d 0a6a 7479  ....```yaml..jty
+00002c60: 7065 3a20 466c 6f77 0d0a 7769 7468 3a0d  pe: Flow..with:.
+00002c70: 0a20 2020 2070 6f72 743a 2031 3233 3435  .    port: 12345
+00002c80: 0d0a 6578 6563 7574 6f72 733a 0d0a 2020  ..executors:..  
+00002c90: 2d20 7573 6573 3a20 5374 6162 6c65 4c4d  - uses: StableLM
+00002ca0: 0d0a 2020 2020 7469 6d65 6f75 745f 7265  ..    timeout_re
+00002cb0: 6164 793a 202d 310d 0a20 2020 2070 795f  ady: -1..    py_
+00002cc0: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
+00002cd0: 2d20 6578 6563 7574 6f72 2e70 790d 0a20  - executor.py.. 
+00002ce0: 202d 2075 7365 733a 2063 6d6f 6e61 693a   - uses: cmonai:
+00002cf0: 2f2f 636d 6f6e 2e70 772f 5465 7874 546f  //cmon.pw/TextTo
+00002d00: 496d 6167 650d 0a20 2020 2074 696d 656f  Image..    timeo
+00002d10: 7574 5f72 6561 6479 3a20 2d31 0d0a 2020  ut_ready: -1..  
+00002d20: 2020 696e 7374 616c 6c5f 7265 7175 6972    install_requir
+00002d30: 656d 656e 7473 3a20 7472 7565 0d0a 6060  ements: true..``
+00002d40: 600d 0a0d 0a54 6865 6e20 7275 6e20 7468  `....Then run th
+00002d50: 6520 5941 4d4c 2046 6c6f 7720 7769 7468  e YAML Flow with
+00002d60: 2074 6865 2043 4c49 3a20 6063 6d6f 6e20   the CLI: `cmon 
+00002d70: 666c 6f77 202d 2d75 7365 7320 666c 6f77  flow --uses flow
+00002d80: 2e79 6d6c 600d 0a0d 0a3c 2f74 643e 0d0a  .yml`....</td>..
+00002d90: 3c2f 7472 3e0d 0a3c 2f74 6162 6c65 3e0d  </tr>..</table>.
+00002da0: 0a3c 2f64 6976 3e0d 0a0d 0a54 6865 6e2c  .</div>....Then,
+00002db0: 2075 7365 205b 436d 6f6e 2043 6c69 656e   use [Cmon Clien
+00002dc0: 745d 2868 7474 7073 3a2f 2f64 6f63 732e  t](https://docs.
+00002dd0: 636d 6f6e 2e70 772f 636f 6e63 6570 7473  cmon.pw/concepts
+00002de0: 2f63 6c69 656e 742f 2920 746f 206d 616b  /client/) to mak
+00002df0: 6520 7265 7175 6573 7473 2074 6f20 7468  e requests to th
+00002e00: 6520 466c 6f77 3a0d 0a0d 0a60 6060 7079  e Flow:....```py
+00002e10: 7468 6f6e 0d0a 6672 6f6d 2063 6d6f 6e20  thon..from cmon 
+00002e20: 696d 706f 7274 2043 6c69 656e 742c 2044  import Client, D
+00002e30: 6f63 756d 656e 740d 0a0d 0a63 6c69 656e  ocument....clien
+00002e40: 7420 3d20 436c 6965 6e74 2870 6f72 743d  t = Client(port=
+00002e50: 3132 3334 3529 0d0a 0d0a 7072 6f6d 7074  12345)....prompt
+00002e60: 203d 2044 6f63 756d 656e 7428 0d0a 2020   = Document(..  
+00002e70: 2020 7461 6773 203d 207b 2770 726f 6d70    tags = {'promp
+00002e80: 7427 3a20 2773 7567 6765 7374 2061 6e20  t': 'suggest an 
+00002e90: 696e 7465 7265 7374 696e 6720 696d 6167  interesting imag
+00002ea0: 6520 6765 6e65 7261 7469 6f6e 2070 726f  e generation pro
+00002eb0: 6d70 7420 666f 7220 6120 6d6f 6e61 206c  mpt for a mona l
+00002ec0: 6973 6120 7661 7269 616e 7427 7d0d 0a29  isa variant'}..)
+00002ed0: 0d0a 0d0a 7265 7370 6f6e 7365 203d 2063  ....response = c
+00002ee0: 6c69 656e 742e 706f 7374 286f 6e3d 272f  lient.post(on='/
+00002ef0: 272c 2069 6e70 7574 733d 5b70 726f 6d70  ', inputs=[promp
+00002f00: 745d 290d 0a0d 0a72 6573 706f 6e73 655b  t])....response[
+00002f10: 305d 2e64 6973 706c 6179 2829 0d0a 6060  0].display()..``
+00002f20: 600d 0a0d 0a21 5b5d 282e 2f2e 6769 7468  `....![](./.gith
+00002f30: 7562 2f69 6d61 6765 732f 6d6f 6e61 2d6c  ub/images/mona-l
+00002f40: 6973 612e 706e 6729 0d0a 0d0a 2323 2044  isa.png)....## D
+00002f50: 6570 6c6f 7920 746f 2074 6865 2063 6c6f  eploy to the clo
+00002f60: 7564 0d0a 0d0a 596f 7520 6361 6e20 616c  ud....You can al
+00002f70: 736f 2064 6570 6c6f 7920 6120 466c 6f77  so deploy a Flow
+00002f80: 2074 6f20 4a43 6c6f 7564 2e0d 0a0d 0a46   to JCloud.....F
+00002f90: 6972 7374 2c20 7475 726e 2074 6865 2060  irst, turn the `
+00002fa0: 666c 6f77 2e79 6d6c 6020 6669 6c65 2069  flow.yml` file i
+00002fb0: 6e74 6f20 6120 5b4a 436c 6f75 642d 636f  nto a [JCloud-co
+00002fc0: 6d70 6174 6962 6c65 2059 414d 4c5d 2868  mpatible YAML](h
+00002fd0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
+00002fe0: 2e70 772f 636f 6e63 6570 7473 2f6a 636c  .pw/concepts/jcl
+00002ff0: 6f75 642f 7961 6d6c 2d73 7065 632f 2920  oud/yaml-spec/) 
+00003000: 6279 2073 7065 6369 6679 696e 6720 7265  by specifying re
+00003010: 736f 7572 6365 2072 6571 7569 7265 6d65  source requireme
+00003020: 6e74 7320 616e 6420 7573 696e 6720 636f  nts and using co
+00003030: 6e74 6169 6e65 7269 7a65 6420 4875 6220  ntainerized Hub 
+00003040: 4578 6563 7574 6f72 732e 0d0a 0d0a 5468  Executors.....Th
+00003050: 656e 2c20 7573 6520 6063 6d6f 6e20 636c  en, use `cmon cl
+00003060: 6f75 6420 6465 706c 6f79 6020 636f 6d6d  oud deploy` comm
+00003070: 616e 6420 746f 2064 6570 6c6f 7920 746f  and to deploy to
+00003080: 2074 6865 2063 6c6f 7564 3a0d 0a0d 0a60   the cloud:....`
+00003090: 6060 7368 656c 6c0d 0a77 6765 7420 6874  ``shell..wget ht
+000030a0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+000030b0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000030c0: 636d 6f6e 2e70 772f 636d 6f6e 2f6d 6173  cmon.pw/cmon/mas
+000030d0: 7465 722f 2e67 6974 6875 622f 6765 7474  ter/.github/gett
+000030e0: 696e 672d 7374 6172 7465 642f 6a63 6c6f  ing-started/jclo
+000030f0: 7564 2d66 6c6f 772e 796d 6c0d 0a63 6d6f  ud-flow.yml..cmo
+00003100: 6e20 636c 6f75 6420 6465 706c 6f79 206a  n cloud deploy j
+00003110: 636c 6f75 642d 666c 6f77 2e79 6d6c 0d0a  cloud-flow.yml..
+00003120: 6060 600d 0a0d 0a3e 202a 2a57 6172 6e69  ```....> **Warni
+00003130: 6e67 2a2a 0d0a 3e0d 0a3e 204d 616b 6520  ng**..>..> Make 
+00003140: 7375 7265 2074 6f20 6465 6c65 7465 2f63  sure to delete/c
+00003150: 6c65 616e 2075 7020 7468 6520 466c 6f77  lean up the Flow
+00003160: 206f 6e63 6520 796f 7520 6172 6520 646f   once you are do
+00003170: 6e65 2077 6974 6820 7468 6973 2074 7574  ne with this tut
+00003180: 6f72 6961 6c20 746f 2073 6176 6520 7265  orial to save re
+00003190: 736f 7572 6365 7320 616e 6420 6372 6564  sources and cred
+000031a0: 6974 732e 0d0a 0d0a 5265 6164 206d 6f72  its.....Read mor
+000031b0: 6520 6162 6f75 7420 5b64 6570 6c6f 7969  e about [deployi
+000031c0: 6e67 2046 6c6f 7773 2074 6f20 4a43 6c6f  ng Flows to JClo
+000031d0: 7564 5d28 6874 7470 733a 2f2f 646f 6373  ud](https://docs
+000031e0: 2e63 6d6f 6e2e 7077 2f63 6f6e 6365 7074  .cmon.pw/concept
+000031f0: 732f 6a63 6c6f 7564 2f23 6465 706c 6f79  s/jcloud/#deploy
+00003200: 292e 0d0a 0d0a 3c21 2d2d 2065 6e64 2062  ).....<!-- end b
+00003210: 7569 6c64 2d70 6970 656c 696e 6573 202d  uild-pipelines -
+00003220: 2d3e 0d0a 0d0a 4368 6563 6b20 5b74 6865  ->....Check [the
+00003230: 2067 6574 7469 6e67 2d73 7461 7274 6564   getting-started
+00003240: 2070 726f 6a65 6374 2073 6f75 7263 6520   project source 
+00003250: 636f 6465 5d28 6874 7470 733a 2f2f 6769  code](https://gi
+00003260: 7468 7562 2e63 6f6d 2f63 6d6f 6e2e 7077  thub.com/cmon.pw
+00003270: 2f63 6d6f 6e2f 7472 6565 2f6d 6173 7465  /cmon/tree/maste
+00003280: 722f 2e67 6974 6875 622f 6765 7474 696e  r/.github/gettin
+00003290: 672d 7374 6172 7465 6429 2e0d 0a0d 0a23  g-started).....#
+000032a0: 2323 2045 6173 7920 7363 616c 6162 696c  ## Easy scalabil
+000032b0: 6974 7920 616e 6420 636f 6e63 7572 7265  ity and concurre
+000032c0: 6e63 790d 0a0d 0a57 6879 206e 6f74 206a  ncy....Why not j
+000032d0: 7573 7420 7573 6520 7374 616e 6461 7264  ust use standard
+000032e0: 2050 7974 686f 6e20 746f 2062 7569 6c64   Python to build
+000032f0: 2074 6861 7420 6d69 6372 6f73 6572 7669   that microservi
+00003300: 6365 2061 6e64 2070 6970 656c 696e 653f  ce and pipeline?
+00003310: 2043 6d6f 6e20 6163 6365 6c65 7261 7465   Cmon accelerate
+00003320: 7320 7469 6d65 2074 6f20 6d61 726b 6574  s time to market
+00003330: 206f 6620 796f 7572 2061 7070 6c69 6361   of your applica
+00003340: 7469 6f6e 2062 7920 6d61 6b69 6e67 2069  tion by making i
+00003350: 7420 6d6f 7265 2073 6361 6c61 626c 6520  t more scalable 
+00003360: 616e 6420 636c 6f75 642d 6e61 7469 7665  and cloud-native
+00003370: 2e20 436d 6f6e 2061 6c73 6f20 6861 6e64  . Cmon also hand
+00003380: 6c65 7320 7468 6520 696e 6672 6173 7472  les the infrastr
+00003390: 7563 7475 7265 2063 6f6d 706c 6578 6974  ucture complexit
+000033a0: 7920 696e 2070 726f 6475 6374 696f 6e20  y in production 
+000033b0: 616e 6420 6f74 6865 7220 4461 792d 3220  and other Day-2 
+000033c0: 6f70 6572 6174 696f 6e73 2073 6f20 7468  operations so th
+000033d0: 6174 2079 6f75 2063 616e 2066 6f63 7573  at you can focus
+000033e0: 206f 6e20 7468 6520 6461 7461 2061 7070   on the data app
+000033f0: 6c69 6361 7469 6f6e 2069 7473 656c 662e  lication itself.
+00003400: 0d0a 0d0a 496e 6372 6561 7365 2079 6f75  ....Increase you
+00003410: 7220 6170 706c 6963 6174 696f 6e27 7320  r application's 
+00003420: 7468 726f 7567 6870 7574 2077 6974 6820  throughput with 
+00003430: 7363 616c 6162 696c 6974 7920 6665 6174  scalability feat
+00003440: 7572 6573 206f 7574 206f 6620 7468 6520  ures out of the 
+00003450: 626f 782c 206c 696b 6520 5b72 6570 6c69  box, like [repli
+00003460: 6361 735d 2868 7474 7073 3a2f 2f64 6f63  cas](https://doc
+00003470: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+00003480: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
+00003490: 2f73 6361 6c65 2d6f 7574 2f23 7265 706c  /scale-out/#repl
+000034a0: 6963 6174 652d 6578 6563 7574 6f72 7329  icate-executors)
+000034b0: 2c20 5b73 6861 7264 735d 2868 7474 7073  , [shards](https
+000034c0: 3a2f 2f64 6f63 732e 636d 6f6e 2e70 772f  ://docs.cmon.pw/
+000034d0: 636f 6e63 6570 7473 2f6f 7263 6865 7374  concepts/orchest
+000034e0: 7261 7469 6f6e 2f73 6361 6c65 2d6f 7574  ration/scale-out
+000034f0: 2f23 6375 7374 6f6d 697a 652d 706f 6c6c  /#customize-poll
+00003500: 696e 672d 6265 6861 7669 6f72 7329 2061  ing-behaviors) a
+00003510: 6e64 205b 6479 6e61 6d69 6320 6261 7463  nd [dynamic batc
+00003520: 6869 6e67 5d28 6874 7470 733a 2f2f 646f  hing](https://do
+00003530: 6373 2e63 6d6f 6e2e 7077 2f63 6f6e 6365  cs.cmon.pw/conce
+00003540: 7074 732f 7365 7276 696e 672f 6578 6563  pts/serving/exec
+00003550: 7574 6f72 2f64 796e 616d 6963 2d62 6174  utor/dynamic-bat
+00003560: 6368 696e 672f 292e 0d0a 0d0a 4c65 7427  ching/).....Let'
+00003570: 7320 7363 616c 6520 6120 5374 6162 6c65  s scale a Stable
+00003580: 2044 6966 6675 7369 6f6e 2045 7865 6375   Diffusion Execu
+00003590: 746f 7220 6465 706c 6f79 6d65 6e74 2077  tor deployment w
+000035a0: 6974 6820 7265 706c 6963 6173 2061 6e64  ith replicas and
+000035b0: 2064 796e 616d 6963 2062 6174 6368 696e   dynamic batchin
+000035c0: 673a 0d0a 0d0a 215b 5d28 2e2f 2e67 6974  g:....![](./.git
+000035d0: 6875 622f 696d 6167 6573 2f73 6361 6c65  hub/images/scale
+000035e0: 642d 6465 706c 6f79 6d65 6e74 2e70 6e67  d-deployment.png
+000035f0: 290d 0a0d 0a2a 2043 7265 6174 6520 7477  )....* Create tw
+00003600: 6f20 7265 706c 6963 6173 2c20 7769 7468  o replicas, with
+00003610: 205b 6120 4750 5520 6173 7369 676e 6564   [a GPU assigned
+00003620: 2066 6f72 2065 6163 685d 2868 7474 7073   for each](https
+00003630: 3a2f 2f64 6f63 732e 636d 6f6e 2e70 772f  ://docs.cmon.pw/
+00003640: 636f 6e63 6570 7473 2f66 6c6f 772f 7363  concepts/flow/sc
+00003650: 616c 652d 6f75 742f 2372 6570 6c69 6361  ale-out/#replica
+00003660: 7465 2d6f 6e2d 6d75 6c74 6970 6c65 2d67  te-on-multiple-g
+00003670: 7075 7329 2e0d 0a2a 2045 6e61 626c 6520  pus)...* Enable 
+00003680: 6479 6e61 6d69 6320 6261 7463 6869 6e67  dynamic batching
+00003690: 2074 6f20 7072 6f63 6573 7320 696e 636f   to process inco
+000036a0: 6d69 6e67 2070 6172 616c 6c65 6c20 7265  ming parallel re
+000036b0: 7175 6573 7473 2074 6f67 6574 6865 7220  quests together 
+000036c0: 7769 7468 2074 6865 2073 616d 6520 6d6f  with the same mo
+000036d0: 6465 6c20 696e 6665 7265 6e63 652e 0d0a  del inference...
+000036e0: 0d0a 0d0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
+000036f0: 7461 626c 652d 7772 6170 7065 7222 3e0d  table-wrapper">.
+00003700: 0a3c 7461 626c 653e 0d0a 3c74 723e 0d0a  .<table>..<tr>..
+00003710: 3c74 683e 204e 6f72 6d61 6c20 4465 706c  <th> Normal Depl
+00003720: 6f79 6d65 6e74 203c 2f74 683e 200d 0a3c  oyment </th> ..<
+00003730: 7468 3e20 5363 616c 6564 2044 6570 6c6f  th> Scaled Deplo
+00003740: 796d 656e 7420 3c2f 7468 3e0d 0a3c 2f74  yment </th>..</t
+00003750: 723e 0d0a 3c74 723e 0d0a 3c74 643e 0d0a  r>..<tr>..<td>..
+00003760: 0d0a 6060 6079 616d 6c0d 0a6a 7479 7065  ..```yaml..jtype
+00003770: 3a20 4465 706c 6f79 6d65 6e74 0d0a 7769  : Deployment..wi
+00003780: 7468 3a0d 0a20 2074 696d 656f 7574 5f72  th:..  timeout_r
+00003790: 6561 6479 3a20 2d31 0d0a 2020 7573 6573  eady: -1..  uses
+000037a0: 3a20 636d 6f6e 6169 3a2f 2f63 6d6f 6e2e  : cmonai://cmon.
+000037b0: 7077 2f54 6578 7454 6f49 6d61 6765 0d0a  pw/TextToImage..
+000037c0: 2020 696e 7374 616c 6c5f 7265 7175 6972    install_requir
+000037d0: 656d 656e 7473 3a20 7472 7565 0d0a 6060  ements: true..``
+000037e0: 600d 0a0d 0a3c 2f74 643e 0d0a 3c74 643e  `....</td>..<td>
+000037f0: 0d0a 0d0a 6060 6079 616d 6c0d 0a6a 7479  ....```yaml..jty
+00003800: 7065 3a20 4465 706c 6f79 6d65 6e74 0d0a  pe: Deployment..
+00003810: 7769 7468 3a0d 0a20 2074 696d 656f 7574  with:..  timeout
+00003820: 5f72 6561 6479 3a20 2d31 0d0a 2020 7573  _ready: -1..  us
+00003830: 6573 3a20 636d 6f6e 6169 3a2f 2f63 6d6f  es: cmonai://cmo
+00003840: 6e2e 7077 2f54 6578 7454 6f49 6d61 6765  n.pw/TextToImage
+00003850: 0d0a 2020 696e 7374 616c 6c5f 7265 7175  ..  install_requ
+00003860: 6972 656d 656e 7473 3a20 7472 7565 0d0a  irements: true..
+00003870: 2020 656e 763a 0d0a 2020 2043 5544 415f    env:..   CUDA_
+00003880: 5649 5349 424c 455f 4445 5649 4345 533a  VISIBLE_DEVICES:
+00003890: 2052 520d 0a20 2072 6570 6c69 6361 733a   RR..  replicas:
+000038a0: 2032 0d0a 2020 7573 6573 5f64 796e 616d   2..  uses_dynam
+000038b0: 6963 5f62 6174 6368 696e 673a 2023 2063  ic_batching: # c
+000038c0: 6f6e 6669 6775 7265 2064 796e 616d 6963  onfigure dynamic
+000038d0: 2062 6174 6368 696e 670d 0a20 2020 202f   batching..    /
+000038e0: 6465 6661 756c 743a 0d0a 2020 2020 2020  default:..      
+000038f0: 7072 6566 6572 7265 645f 6261 7463 685f  preferred_batch_
+00003900: 7369 7a65 3a20 3130 0d0a 2020 2020 2020  size: 10..      
+00003910: 7469 6d65 6f75 743a 2032 3030 0d0a 6060  timeout: 200..``
+00003920: 600d 0a0d 0a3c 2f74 643e 0d0a 3c2f 7472  `....</td>..</tr
+00003930: 3e0d 0a3c 2f74 6162 6c65 3e0d 0a3c 2f64  >..</table>..</d
+00003940: 6976 3e0d 0a0d 0a41 7373 756d 696e 6720  iv>....Assuming 
+00003950: 796f 7572 206d 6163 6869 6e65 2068 6173  your machine has
+00003960: 2074 776f 2047 5055 732c 2075 7369 6e67   two GPUs, using
+00003970: 2074 6865 2073 6361 6c65 6420 6465 706c   the scaled depl
+00003980: 6f79 6d65 6e74 2059 414d 4c20 7769 6c6c  oyment YAML will
+00003990: 2067 6976 6520 6265 7474 6572 2074 6872   give better thr
+000039a0: 6f75 6768 7075 7420 636f 6d70 6172 6564  oughput compared
+000039b0: 2074 6f20 7468 6520 6e6f 726d 616c 2064   to the normal d
+000039c0: 6570 6c6f 796d 656e 742e 0d0a 0d0a 5468  eployment.....Th
+000039d0: 6573 6520 6665 6174 7572 6573 2061 7070  ese features app
+000039e0: 6c79 2074 6f20 626f 7468 205b 4465 706c  ly to both [Depl
+000039f0: 6f79 6d65 6e74 2059 414d 4c5d 2868 7474  oyment YAML](htt
+00003a00: 7073 3a2f 2f64 6f63 732e 636d 6f6e 2e70  ps://docs.cmon.p
+00003a10: 772f 636f 6e63 6570 7473 2f65 7865 6375  w/concepts/execu
+00003a20: 746f 722f 6465 706c 6f79 6d65 6e74 2d79  tor/deployment-y
+00003a30: 616d 6c2d 7370 6563 2f23 6465 706c 6f79  aml-spec/#deploy
+00003a40: 6d65 6e74 2d79 616d 6c2d 7370 6563 2920  ment-yaml-spec) 
+00003a50: 616e 6420 5b46 6c6f 7720 5941 4d4c 5d28  and [Flow YAML](
+00003a60: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00003a70: 6e2e 7077 2f63 6f6e 6365 7074 732f 666c  n.pw/concepts/fl
+00003a80: 6f77 2f79 616d 6c2d 7370 6563 2f29 2e20  ow/yaml-spec/). 
+00003a90: 5468 616e 6b73 2074 6f20 7468 6520 5941  Thanks to the YA
+00003aa0: 4d4c 2073 796e 7461 782c 2079 6f75 2063  ML syntax, you c
+00003ab0: 616e 2069 6e6a 6563 7420 6465 706c 6f79  an inject deploy
+00003ac0: 6d65 6e74 2063 6f6e 6669 6775 7261 7469  ment configurati
+00003ad0: 6f6e 7320 7265 6761 7264 6c65 7373 206f  ons regardless o
+00003ae0: 6620 4578 6563 7574 6f72 2063 6f64 652e  f Executor code.
+00003af0: 0d0a 0d0a 2323 2320 4765 7420 6f6e 2074  ....### Get on t
+00003b00: 6865 2066 6173 7420 6c61 6e65 2074 6f20  he fast lane to 
+00003b10: 636c 6f75 642d 6e61 7469 7665 0d0a 0d0a  cloud-native....
+00003b20: 5573 696e 6720 4b75 6265 726e 6574 6573  Using Kubernetes
+00003b30: 2077 6974 6820 436d 6f6e 2069 7320 6561   with Cmon is ea
+00003b40: 7379 3a0d 0a0d 0a60 6060 6261 7368 0d0a  sy:....```bash..
+00003b50: 636d 6f6e 2065 7870 6f72 7420 6b75 6265  cmon export kube
+00003b60: 726e 6574 6573 2066 6c6f 772e 796d 6c20  rnetes flow.yml 
+00003b70: 2e2f 6d79 2d6b 3873 0d0a 6b75 6265 6374  ./my-k8s..kubect
+00003b80: 6c20 6170 706c 7920 2d52 202d 6620 6d79  l apply -R -f my
+00003b90: 2d6b 3873 0d0a 6060 600d 0a0d 0a41 6e64  -k8s..```....And
+00003ba0: 2073 6f20 6973 2044 6f63 6b65 7220 436f   so is Docker Co
+00003bb0: 6d70 6f73 653a 0d0a 0d0a 6060 6062 6173  mpose:....```bas
+00003bc0: 680d 0a63 6d6f 6e20 6578 706f 7274 2064  h..cmon export d
+00003bd0: 6f63 6b65 722d 636f 6d70 6f73 6520 666c  ocker-compose fl
+00003be0: 6f77 2e79 6d6c 2064 6f63 6b65 722d 636f  ow.yml docker-co
+00003bf0: 6d70 6f73 652e 796d 6c0d 0a64 6f63 6b65  mpose.yml..docke
+00003c00: 722d 636f 6d70 6f73 6520 7570 0d0a 6060  r-compose up..``
+00003c10: 600d 0a0d 0a3e 202a 2a4e 6f74 652a 2a0d  `....> **Note**.
+00003c20: 0a3e 2059 6f75 2063 616e 2061 6c73 6f20  .> You can also 
+00003c30: 6578 706f 7274 2044 6570 6c6f 796d 656e  export Deploymen
+00003c40: 7420 5941 4d4c 2074 6f20 5b4b 7562 6572  t YAML to [Kuber
+00003c50: 6e65 7465 735d 2868 7474 7073 3a2f 2f64  netes](https://d
+00003c60: 6f63 732e 636d 6f6e 2e70 772f 636f 6e63  ocs.cmon.pw/conc
+00003c70: 6570 7473 2f65 7865 6375 746f 722f 7365  epts/executor/se
+00003c80: 7276 652f 2373 6572 7665 2d76 6961 2d6b  rve/#serve-via-k
+00003c90: 7562 6572 6e65 7465 7329 2061 6e64 205b  ubernetes) and [
+00003ca0: 446f 636b 6572 2043 6f6d 706f 7365 5d28  Docker Compose](
+00003cb0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00003cc0: 6e2e 7077 2f63 6f6e 6365 7074 732f 6578  n.pw/concepts/ex
+00003cd0: 6563 7574 6f72 2f73 6572 7665 2f23 7365  ecutor/serve/#se
+00003ce0: 7276 652d 7669 612d 646f 636b 6572 2d63  rve-via-docker-c
+00003cf0: 6f6d 706f 7365 292e 0d0a 0d0a 5468 6174  ompose).....That
+00003d00: 2773 206e 6f74 2061 6c6c 2e20 5765 2061  's not all. We a
+00003d10: 6c73 6f20 7375 7070 6f72 7420 5b4f 7065  lso support [Ope
+00003d20: 6e54 656c 656d 6574 7279 2c20 5072 6f6d  nTelemetry, Prom
+00003d30: 6574 6865 7573 2c20 616e 6420 4a61 6567  etheus, and Jaeg
+00003d40: 6572 5d28 6874 7470 733a 2f2f 646f 6373  er](https://docs
+00003d50: 2e63 6d6f 6e2e 7077 2f63 6c6f 7564 2d6e  .cmon.pw/cloud-n
+00003d60: 6174 6976 656e 6573 732f 6f70 656e 7465  ativeness/opente
+00003d70: 6c65 6d65 7472 792f 292e 0d0a 0d0a 5768  lemetry/).....Wh
+00003d80: 6174 2063 6c6f 7564 2d6e 6174 6976 6520  at cloud-native 
+00003d90: 7465 6368 6e6f 6c6f 6779 2069 7320 7374  technology is st
+00003da0: 696c 6c20 6368 616c 6c65 6e67 696e 6720  ill challenging 
+00003db0: 746f 2079 6f75 3f20 5b54 656c 6c20 7573  to you? [Tell us
+00003dc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003dd0: 2e63 6f6d 2f63 6d6f 6e2e 7077 2f63 6d6f  .com/cmon.pw/cmo
+00003de0: 6e2f 6973 7375 6573 2920 616e 6420 7765  n/issues) and we
+00003df0: 276c 6c20 6861 6e64 6c65 2074 6865 2063  'll handle the c
+00003e00: 6f6d 706c 6578 6974 7920 616e 6420 6d61  omplexity and ma
+00003e10: 6b65 2069 7420 6561 7379 2066 6f72 2079  ke it easy for y
+00003e20: 6f75 2e0d 0a0d 0a3c 212d 2d20 7374 6172  ou.....<!-- star
+00003e30: 7420 7375 7070 6f72 742d 7069 7463 6820  t support-pitch 
+00003e40: 2d2d 3e0d 0a0d 0a23 2320 5375 7070 6f72  -->....## Suppor
+00003e50: 740d 0a0d 0a2d 204a 6f69 6e20 6f75 7220  t....- Join our 
+00003e60: 5b44 6973 636f 7264 2063 6f6d 6d75 6e69  [Discord communi
+00003e70: 7479 5d28 6874 7470 733a 2f2f 6469 7363  ty](https://disc
+00003e80: 6f72 642e 636d 6f6e 2e70 7729 2061 6e64  ord.cmon.pw) and
+00003e90: 2063 6861 7420 7769 7468 206f 7468 6572   chat with other
+00003ea0: 2063 6f6d 6d75 6e69 7479 206d 656d 6265   community membe
+00003eb0: 7273 2061 626f 7574 2069 6465 6173 2e0d  rs about ideas..
+00003ec0: 0a2d 2053 7562 7363 7269 6265 2074 6f20  .- Subscribe to 
+00003ed0: 7468 6520 6c61 7465 7374 2076 6964 656f  the latest video
+00003ee0: 2074 7574 6f72 6961 6c73 206f 6e20 6f75   tutorials on ou
+00003ef0: 7220 5b59 6f75 5475 6265 2063 6861 6e6e  r [YouTube chann
+00003f00: 656c 5d28 6874 7470 733a 2f2f 796f 7574  el](https://yout
+00003f10: 7562 652e 636f 6d2f 632f 636d 6f6e 2e70  ube.com/c/cmon.p
+00003f20: 7729 0d0a 0d0a 2323 204a 6f69 6e20 5573  w)....## Join Us
+00003f30: 0d0a 0d0a 436d 6f6e 2069 7320 6261 636b  ....Cmon is back
+00003f40: 6564 2062 7920 5b43 6d6f 6e20 4149 5d28  ed by [Cmon AI](
+00003f50: 6874 7470 733a 2f2f 636d 6f6e 2e70 7729  https://cmon.pw)
+00003f60: 2061 6e64 206c 6963 656e 7365 6420 756e   and licensed un
+00003f70: 6465 7220 5b41 7061 6368 652d 322e 305d  der [Apache-2.0]
+00003f80: 282e 2f4c 4943 454e 5345 292e 0d0a 0d0a  (./LICENSE).....
+00003f90: 3c21 2d2d 2065 6e64 2073 7570 706f 7274  <!-- end support
+00003fa0: 2d70 6974 6368 202d 2d3e 0d0a            -pitch -->..
```

### Comparing `cmon-ai-0.38.5/README.md` & `cmon-ai-0.42.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,865 +1,892 @@
 00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a3c 212d 2d20 7375 7276 6579 2062  ">.<!-- survey b
-00000020: 616e 6e65 7220 7374 6172 7420 2d2d 3e0a  anner start -->.
-00000030: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000040: 2f31 3073 7731 7463 706c 6434 2e74 7970  /10sw1tcpld4.typ
-00000050: 6566 6f72 6d2e 636f 6d2f 746f 2f45 4741  eform.com/to/EGA
-00000060: 4552 654d 373f 7574 6d5f 736f 7572 6365  EReM7?utm_source
-00000070: 3d72 6561 646d 6526 7574 6d5f 6d65 6469  =readme&utm_medi
-00000080: 756d 3d67 6974 6875 6226 7574 6d5f 6361  um=github&utm_ca
-00000090: 6d70 6169 676e 3d75 7365 7225 3230 6578  mpaign=user%20ex
-000000a0: 7065 7269 656e 6365 2675 746d 5f74 6572  perience&utm_ter
-000000b0: 6d3d 6665 6232 3032 3326 7574 6d5f 636f  m=feb2023&utm_co
-000000c0: 6e74 656e 743d 7375 7276 6579 223e 0a20  ntent=survey">. 
-000000d0: 203c 696d 6720 7372 633d 222e 2f2e 6769   <img src="./.gi
-000000e0: 7468 7562 2f62 616e 6e65 722e 7376 673f  thub/banner.svg?
-000000f0: 7261 773d 7472 7565 223e 0a3c 2f61 3e0a  raw=true">.</a>.
-00000100: 3c21 2d2d 2073 7572 7665 7920 6261 6e6e  <!-- survey bann
-00000110: 6572 2073 7461 7274 202d 2d3e 0a0a 3c70  er start -->..<p
-00000120: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00000130: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000140: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 223e  //docs.cmon.ai">
-00000150: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000160: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6d6f  //github.com/cmo
-00000170: 6e2d 6169 2f63 6d6f 6e2f 626c 6f62 2f6d  n-ai/cmon/blob/m
-00000180: 6173 7465 722f 646f 6373 2f5f 7374 6174  aster/docs/_stat
-00000190: 6963 2f6c 6f67 6f2d 6c69 6768 742e 7376  ic/logo-light.sv
-000001a0: 673f 7261 773d 7472 7565 2220 616c 743d  g?raw=true" alt=
-000001b0: 2243 6d6f 6e20 6c6f 676f 3a20 4275 696c  "Cmon logo: Buil
-000001c0: 6420 6d75 6c74 696d 6f64 616c 2041 4920  d multimodal AI 
-000001d0: 7365 7276 6963 6573 2076 6961 2063 6c6f  services via clo
-000001e0: 7564 206e 6174 6976 6520 7465 6368 6e6f  ud native techno
-000001f0: 6c6f 6769 6573 20c2 b720 4e65 7572 616c  logies .. Neural
-00000200: 2053 6561 7263 6820 c2b7 2047 656e 6572   Search .. Gener
-00000210: 6174 6976 6520 4149 20c2 b720 436c 6f75  ative AI .. Clou
-00000220: 6420 4e61 7469 7665 2220 7769 6474 683d  d Native" width=
-00000230: 2231 3530 7078 223e 3c2f 613e 0a3c 2f70  "150px"></a>.</p
-00000240: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
-00000250: 7465 7222 3e0a 3c62 3e42 7569 6c64 206d  ter">.<b>Build m
-00000260: 756c 7469 6d6f 6461 6c20 4149 2073 6572  ultimodal AI ser
-00000270: 7669 6365 7320 7769 7468 2063 6c6f 7564  vices with cloud
-00000280: 206e 6174 6976 6520 7465 6368 6e6f 6c6f   native technolo
-00000290: 6769 6573 3c2f 623e 0a3c 2f70 3e0a 0a3c  gies</b>.</p>..<
-000002a0: 7020 616c 6967 6e3d 6365 6e74 6572 3e0a  p align=center>.
-000002b0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000002c0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-000002d0: 742f 636d 6f6e 2f22 3e3c 696d 6720 616c  t/cmon/"><img al
-000002e0: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
-000002f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000300: 732e 696f 2f70 7970 692f 762f 636d 6f6e  s.io/pypi/v/cmon
-00000310: 3f6c 6162 656c 3d52 656c 6561 7365 2673  ?label=Release&s
-00000320: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000330: 223e 3c2f 613e 0a3c 212d 2d3c 6120 6872  "></a>.<!--<a hr
-00000340: 6566 3d22 6874 7470 733a 2f2f 636f 6465  ef="https://code
-00000350: 636f 762e 696f 2f67 682f 636d 6f6e 2d61  cov.io/gh/cmon-a
-00000360: 692f 636d 6f6e 223e 3c69 6d67 2061 6c74  i/cmon"><img alt
-00000370: 3d22 436f 6465 636f 7620 6272 616e 6368  ="Codecov branch
-00000380: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000390: 6d67 2e73 6869 656c 6473 2e69 6f2f 636f  mg.shields.io/co
-000003a0: 6465 636f 762f 632f 6769 7468 7562 2f63  decov/c/github/c
-000003b0: 6d6f 6e2d 6169 2f63 6d6f 6e2f 6d61 7374  mon-ai/cmon/mast
-000003c0: 6572 3f26 6c6f 676f 3d43 6f64 6563 6f76  er?&logo=Codecov
-000003d0: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-000003e0: 2673 7479 6c65 3d66 6c61 742d 7371 7561  &style=flat-squa
-000003f0: 7265 223e 3c2f 613e 2d2d 3e0a 3c61 2068  re"></a>-->.<a h
-00000400: 7265 663d 2268 7474 7073 3a2f 2f64 6973  ref="https://dis
-00000410: 636f 7264 2e63 6d6f 6e2e 6169 223e 3c69  cord.cmon.ai"><i
-00000420: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000430: 696d 672e 7368 6965 6c64 732e 696f 2f64  img.shields.io/d
-00000440: 6973 636f 7264 2f31 3130 3635 3432 3232  iscord/110654222
-00000450: 3031 3132 3330 3231 3330 3f6c 6f67 6f3d  0112302130?logo=
-00000460: 6469 7363 6f72 6426 6c6f 676f 436f 6c6f  discord&logoColo
-00000470: 723d 7768 6974 6526 7374 796c 653d 666c  r=white&style=fl
-00000480: 6174 2d73 7175 6172 6522 3e3c 2f61 3e0a  at-square"></a>.
-00000490: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000004a0: 2f70 7970 6973 7461 7473 2e6f 7267 2f70  /pypistats.org/p
-000004b0: 6163 6b61 6765 732f 636d 6f6e 223e 3c69  ackages/cmon"><i
-000004c0: 6d67 2061 6c74 3d22 5079 5049 202d 2044  mg alt="PyPI - D
-000004d0: 6f77 6e6c 6f61 6473 2066 726f 6d20 6f66  ownloads from of
-000004e0: 6669 6369 616c 2070 7970 6973 7461 7473  ficial pypistats
-000004f0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000500: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000510: 7069 2f64 6d2f 636d 6f6e 3f73 7479 6c65  pi/dm/cmon?style
-00000520: 3d66 6c61 742d 7371 7561 7265 223e 3c2f  =flat-square"></
-00000530: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
-00000540: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00000550: 6d6f 6e2d 6169 2f63 6d6f 6e2f 6163 7469  mon-ai/cmon/acti
-00000560: 6f6e 732f 776f 726b 666c 6f77 732f 6364  ons/workflows/cd
-00000570: 2e79 6d6c 223e 3c69 6d67 2061 6c74 3d22  .yml"><img alt="
-00000580: 4769 7468 7562 2043 4420 7374 6174 7573  Github CD status
-00000590: 2220 7372 633d 2268 7474 7073 3a2f 2f67  " src="https://g
-000005a0: 6974 6875 622e 636f 6d2f 636d 6f6e 2d61  ithub.com/cmon-a
-000005b0: 692f 636d 6f6e 2f61 6374 696f 6e73 2f77  i/cmon/actions/w
-000005c0: 6f72 6b66 6c6f 7773 2f63 642e 796d 6c2f  orkflows/cd.yml/
-000005d0: 6261 6467 652e 7376 6722 3e3c 2f61 3e0a  badge.svg"></a>.
-000005e0: 3c2f 703e 0a0a 3c21 2d2d 2073 7461 7274  </p>..<!-- start
-000005f0: 2063 6d6f 6e2d 6465 7363 7269 7074 696f   cmon-descriptio
-00000600: 6e20 2d2d 3e0a 0a43 6d6f 6e20 6c65 7473  n -->..Cmon lets
-00000610: 2079 6f75 2062 7569 6c64 206d 756c 7469   you build multi
-00000620: 6d6f 6461 6c20 5b2a 2a41 4920 7365 7276  modal [**AI serv
-00000630: 6963 6573 2a2a 5d28 2362 7569 6c64 2d61  ices**](#build-a
-00000640: 692d 7365 7276 6963 6573 2920 616e 6420  i-services) and 
-00000650: 5b2a 2a70 6970 656c 696e 6573 2a2a 5d28  [**pipelines**](
-00000660: 2362 7569 6c64 2d61 2d70 6970 656c 696e  #build-a-pipelin
-00000670: 6529 2074 6861 7420 636f 6d6d 756e 6963  e) that communic
-00000680: 6174 6520 7669 6120 6752 5043 2c20 4854  ate via gRPC, HT
-00000690: 5450 2061 6e64 2057 6562 536f 636b 6574  TP and WebSocket
-000006a0: 732c 2074 6865 6e20 7363 616c 6520 7468  s, then scale th
-000006b0: 656d 2075 7020 616e 6420 6465 706c 6f79  em up and deploy
-000006c0: 2074 6f20 7072 6f64 7563 7469 6f6e 2e20   to production. 
-000006d0: 596f 7520 6361 6e20 666f 6375 7320 6f6e  You can focus on
-000006e0: 2079 6f75 7220 6c6f 6769 6320 616e 6420   your logic and 
-000006f0: 616c 676f 7269 7468 6d73 2c20 7769 7468  algorithms, with
-00000700: 6f75 7420 776f 7272 7969 6e67 2061 626f  out worrying abo
-00000710: 7574 2074 6865 2069 6e66 7261 7374 7275  ut the infrastru
-00000720: 6374 7572 6520 636f 6d70 6c65 7869 7479  cture complexity
-00000730: 2e0a 0a21 5b5d 282e 2f2e 6769 7468 7562  ...![](./.github
-00000740: 2f69 6d61 6765 732f 6275 696c 642d 6465  /images/build-de
-00000750: 706c 6f79 2e70 6e67 290a 0a43 6d6f 6e20  ploy.png)..Cmon 
-00000760: 7072 6f76 6964 6573 2061 2073 6d6f 6f74  provides a smoot
-00000770: 6820 5079 7468 6f6e 6963 2065 7870 6572  h Pythonic exper
-00000780: 6965 6e63 6520 7472 616e 7369 7469 6f6e  ience transition
-00000790: 696e 6720 6672 6f6d 206c 6f63 616c 2064  ing from local d
-000007a0: 6570 6c6f 796d 656e 7420 746f 2061 6476  eployment to adv
-000007b0: 616e 6365 6420 6f72 6368 6573 7472 6174  anced orchestrat
-000007c0: 696f 6e20 6672 616d 6577 6f72 6b73 206c  ion frameworks l
-000007d0: 696b 6520 446f 636b 6572 2d43 6f6d 706f  ike Docker-Compo
-000007e0: 7365 2c20 4b75 6265 726e 6574 6573 2c20  se, Kubernetes, 
-000007f0: 6f72 2043 6d6f 6e20 4149 2043 6c6f 7564  or Cmon AI Cloud
-00000800: 2e20 436d 6f6e 206d 616b 6573 2061 6476  . Cmon makes adv
-00000810: 616e 6365 6420 736f 6c75 7469 6f6e 2065  anced solution e
-00000820: 6e67 696e 6565 7269 6e67 2061 6e64 2063  ngineering and c
-00000830: 6c6f 7564 2d6e 6174 6976 6520 7465 6368  loud-native tech
-00000840: 6e6f 6c6f 6769 6573 2061 6363 6573 7369  nologies accessi
-00000850: 626c 6520 746f 2065 7665 7279 2064 6576  ble to every dev
-00000860: 656c 6f70 6572 2e0a 0a2d 2042 7569 6c64  eloper...- Build
-00000870: 2061 7070 6c69 6361 7469 6f6e 7320 666f   applications fo
-00000880: 7220 616e 7920 5b64 6174 6120 7479 7065  r any [data type
-00000890: 5d28 6874 7470 733a 2f2f 646f 6373 2e64  ](https://docs.d
-000008a0: 6f63 6172 7261 792e 6f72 672f 6461 7461  ocarray.org/data
-000008b0: 5f74 7970 6573 2f66 6972 7374 5f73 7465  _types/first_ste
-000008c0: 7073 2f29 2c20 616e 7920 6d61 696e 7374  ps/), any mainst
-000008d0: 7265 616d 205b 6465 6570 206c 6561 726e  ream [deep learn
-000008e0: 696e 6720 6672 616d 6577 6f72 6b5d 2829  ing framework]()
-000008f0: 2c20 616e 6420 616e 7920 5b70 726f 746f  , and any [proto
-00000900: 636f 6c5d 2868 7474 7073 3a2f 2f64 6f63  col](https://doc
-00000910: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00000920: 7473 2f73 6572 7669 6e67 2f67 6174 6577  ts/serving/gatew
-00000930: 6179 2f23 7365 742d 7072 6f74 6f63 6f6c  ay/#set-protocol
-00000940: 2d69 6e2d 7079 7468 6f6e 292e 0a2d 2044  -in-python)..- D
-00000950: 6573 6967 6e20 6869 6768 2d70 6572 666f  esign high-perfo
-00000960: 726d 616e 6365 206d 6963 726f 7365 7276  rmance microserv
-00000970: 6963 6573 2c20 7769 7468 205b 6561 7379  ices, with [easy
-00000980: 2073 6361 6c69 6e67 5d28 6874 7470 733a   scaling](https:
-00000990: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-000009a0: 6f6e 6365 7074 732f 6f72 6368 6573 7472  oncepts/orchestr
-000009b0: 6174 696f 6e2f 7363 616c 652d 6f75 742f  ation/scale-out/
-000009c0: 292c 2064 7570 6c65 7820 636c 6965 6e74  ), duplex client
-000009d0: 2d73 6572 7665 7220 7374 7265 616d 696e  -server streamin
-000009e0: 672c 2061 6e64 2061 7379 6e63 2f6e 6f6e  g, and async/non
-000009f0: 2d62 6c6f 636b 696e 6720 6461 7461 2070  -blocking data p
-00000a00: 726f 6365 7373 696e 6720 6f76 6572 2064  rocessing over d
-00000a10: 796e 616d 6963 2066 6c6f 7773 2e0a 2d20  ynamic flows..- 
-00000a20: 446f 636b 6572 2063 6f6e 7461 696e 6572  Docker container
-00000a30: 2069 6e74 6567 7261 7469 6f6e 2076 6961   integration via
-00000a40: 205b 4578 6563 7574 6f72 2048 7562 5d28   [Executor Hub](
-00000a50: 6874 7470 733a 2f2f 636c 6f75 642e 636d  https://cloud.cm
-00000a60: 6f6e 2e61 6929 2c20 4f70 656e 5465 6c65  on.ai), OpenTele
-00000a70: 6d65 7472 792f 5072 6f6d 6574 6865 7573  metry/Prometheus
-00000a80: 206f 6273 6572 7661 6269 6c69 7479 2c20   observability, 
-00000a90: 616e 6420 6661 7374 204b 7562 6572 6e65  and fast Kuberne
-00000aa0: 7465 732f 446f 636b 6572 2d43 6f6d 706f  tes/Docker-Compo
-00000ab0: 7365 2064 6570 6c6f 796d 656e 742e 0a2d  se deployment..-
-00000ac0: 2043 5055 2f47 5055 2068 6f73 7469 6e67   CPU/GPU hosting
-00000ad0: 2076 6961 205b 436d 6f6e 2041 4920 436c   via [Cmon AI Cl
-00000ae0: 6f75 645d 2868 7474 7073 3a2f 2f63 6c6f  oud](https://clo
-00000af0: 7564 2e63 6d6f 6e2e 6169 292e 0a0a 3c64  ud.cmon.ai)...<d
-00000b00: 6574 6169 6c73 3e0a 2020 2020 3c73 756d  etails>.    <sum
-00000b10: 6d61 7279 3e3c 7374 726f 6e67 3e57 6169  mary><strong>Wai
-00000b20: 742c 2068 6f77 2069 7320 436d 6f6e 2064  t, how is Cmon d
-00000b30: 6966 6665 7265 6e74 2066 726f 6d20 4661  ifferent from Fa
-00000b40: 7374 4150 493f 3c2f 7374 726f 6e67 3e3c  stAPI?</strong><
-00000b50: 2f73 756d 6d61 7279 3e0a 436d 6f6e 2773  /summary>.Cmon's
-00000b60: 2076 616c 7565 2070 726f 706f 7369 7469   value propositi
-00000b70: 6f6e 206d 6179 2073 6565 6d20 7175 6974  on may seem quit
-00000b80: 6520 7369 6d69 6c61 7220 746f 2074 6861  e similar to tha
-00000b90: 7420 6f66 2046 6173 7441 5049 2e20 486f  t of FastAPI. Ho
-00000ba0: 7765 7665 722c 2074 6865 7265 2061 7265  wever, there are
-00000bb0: 2073 6576 6572 616c 2066 756e 6461 6d65   several fundame
-00000bc0: 6e74 616c 2064 6966 6665 7265 6e63 6573  ntal differences
-00000bd0: 3a0a 0a20 2a2a 4461 7461 2073 7472 7563  :.. **Data struc
-00000be0: 7475 7265 2061 6e64 2063 6f6d 6d75 6e69  ture and communi
-00000bf0: 6361 7469 6f6e 2070 726f 746f 636f 6c73  cation protocols
-00000c00: 2a2a 0a20 202d 2046 6173 7441 5049 2063  **.  - FastAPI c
-00000c10: 6f6d 6d75 6e69 6361 7469 6f6e 2072 656c  ommunication rel
-00000c20: 6965 7320 6f6e 2050 7964 616e 7469 6320  ies on Pydantic 
-00000c30: 616e 6420 436d 6f6e 2072 656c 6965 7320  and Cmon relies 
-00000c40: 6f6e 205b 446f 6341 7272 6179 5d28 6874  on [DocArray](ht
-00000c50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c60: 2f64 6f63 6172 7261 792f 646f 6361 7272  /docarray/docarr
-00000c70: 6179 2920 616c 6c6f 7769 6e67 2043 6d6f  ay) allowing Cmo
-00000c80: 6e20 746f 2073 7570 706f 7274 206d 756c  n to support mul
-00000c90: 7469 706c 6520 7072 6f74 6f63 6f6c 730a  tiple protocols.
-00000ca0: 2020 746f 2065 7870 6f73 6520 6974 7320    to expose its 
-00000cb0: 7365 7276 6963 6573 2e0a 0a20 2a2a 4164  services... **Ad
-00000cc0: 7661 6e63 6564 206f 7263 6865 7374 7261  vanced orchestra
-00000cd0: 7469 6f6e 2061 6e64 2073 6361 6c69 6e67  tion and scaling
-00000ce0: 2063 6170 6162 696c 6974 6965 732a 2a0a   capabilities**.
-00000cf0: 2020 2d20 436d 6f6e 206c 6574 7320 796f    - Cmon lets yo
-00000d00: 7520 6465 706c 6f79 2061 7070 6c69 6361  u deploy applica
-00000d10: 7469 6f6e 7320 666f 726d 6564 2066 726f  tions formed fro
-00000d20: 6d20 6d75 6c74 6970 6c65 206d 6963 726f  m multiple micro
-00000d30: 7365 7276 6963 6573 2074 6861 7420 6361  services that ca
-00000d40: 6e20 6265 2063 6f6e 7461 696e 6572 697a  n be containeriz
-00000d50: 6564 2061 6e64 2073 6361 6c65 6420 696e  ed and scaled in
-00000d60: 6465 7065 6e64 656e 746c 792e 0a20 202d  dependently..  -
-00000d70: 2043 6d6f 6e20 616c 6c6f 7773 2079 6f75   Cmon allows you
-00000d80: 2074 6f20 6561 7369 6c79 2063 6f6e 7461   to easily conta
-00000d90: 696e 6572 697a 6520 616e 6420 6f72 6368  inerize and orch
-00000da0: 6573 7472 6174 6520 796f 7572 2073 6572  estrate your ser
-00000db0: 7669 6365 732c 2070 726f 7669 6469 6e67  vices, providing
-00000dc0: 2063 6f6e 6375 7272 656e 6379 2061 6e64   concurrency and
-00000dd0: 2073 6361 6c61 6269 6c69 7479 2e0a 0a20   scalability... 
-00000de0: 2a2a 4a6f 7572 6e65 7920 746f 2074 6865  **Journey to the
-00000df0: 2063 6c6f 7564 2a2a 0a20 202d 2043 6d6f   cloud**.  - Cmo
-00000e00: 6e20 7072 6f76 6964 6573 2061 2073 6d6f  n provides a smo
-00000e10: 6f74 6820 7472 616e 7369 7469 6f6e 2066  oth transition f
-00000e20: 726f 6d20 6c6f 6361 6c20 6465 7665 6c6f  rom local develo
-00000e30: 706d 656e 7420 2875 7369 6e67 205b 446f  pment (using [Do
-00000e40: 6341 7272 6179 5d28 6874 7470 733a 2f2f  cArray](https://
-00000e50: 6769 7468 7562 2e63 6f6d 2f64 6f63 6172  github.com/docar
-00000e60: 7261 792f 646f 6361 7272 6179 2929 2074  ray/docarray)) t
-00000e70: 6f20 6c6f 6361 6c20 7365 7276 696e 6720  o local serving 
-00000e80: 7573 696e 6720 2843 6d6f 6e27 7320 6f72  using (Cmon's or
-00000e90: 6368 6573 7472 6174 696f 6e20 6c61 7965  chestration laye
-00000ea0: 7229 0a20 2074 6f20 6861 7669 6e67 2070  r).  to having p
-00000eb0: 726f 6475 6374 696f 6e2d 7265 6164 7920  roduction-ready 
-00000ec0: 7365 7276 6963 6573 2062 7920 7573 696e  services by usin
-00000ed0: 6720 4b75 6265 726e 6574 6573 2063 6170  g Kubernetes cap
-00000ee0: 6163 6974 7920 746f 206f 7263 6865 7374  acity to orchest
-00000ef0: 7261 7465 2074 6865 206c 6966 6574 696d  rate the lifetim
-00000f00: 6520 6f66 2063 6f6e 7461 696e 6572 732e  e of containers.
-00000f10: 0a20 202d 2042 7920 7573 696e 6720 5b43  .  - By using [C
-00000f20: 6d6f 6e20 4149 2043 6c6f 7564 5d28 6874  mon AI Cloud](ht
-00000f30: 7470 733a 2f2f 636c 6f75 642e 636d 6f6e  tps://cloud.cmon
-00000f40: 2e61 6929 2079 6f75 2068 6176 6520 6163  .ai) you have ac
-00000f50: 6365 7373 2074 6f20 7363 616c 6162 6c65  cess to scalable
-00000f60: 2061 6e64 2073 6572 7665 726c 6573 7320   and serverless 
-00000f70: 6465 706c 6f79 6d65 6e74 7320 6f66 2079  deployments of y
-00000f80: 6f75 7220 6170 706c 6963 6174 696f 6e73  our applications
-00000f90: 2069 6e20 6f6e 6520 636f 6d6d 616e 642e   in one command.
-00000fa0: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 212d  .</details>..<!-
-00000fb0: 2d20 656e 6420 636d 6f6e 2d64 6573 6372  - end cmon-descr
-00000fc0: 6970 7469 6f6e 202d 2d3e 0a0a 2323 205b  iption -->..## [
-00000fd0: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-00000fe0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00000ff0: 2e61 6929 0a0a 2323 2049 6e73 7461 6c6c  .ai)..## Install
-00001000: 200a 0a4e 6f74 653a 2028 5769 6e64 6f77   ..Note: (Window
-00001010: 7329 206e 6f74 2073 7570 706f 7274 6564  s) not supported
-00001020: 2061 7420 7468 6973 206d 6f6d 656e 7421   at this moment!
-00001030: 2059 6f75 206d 6179 2072 6571 7569 7265   You may require
-00001040: 2074 6f20 696e 7374 616c 6c20 6974 206f   to install it o
-00001050: 6e20 2857 534c 292e 0a0a 6060 6062 6173  n (WSL)...```bas
-00001060: 680a 7069 7020 696e 7374 616c 6c20 636d  h.pip install cm
-00001070: 6f6e 0a60 6060 0a0a 4669 6e64 206d 6f72  on.```..Find mor
-00001080: 6520 696e 7374 616c 6c20 6f70 7469 6f6e  e install option
-00001090: 7320 6f6e 205b 4170 706c 6520 5369 6c69  s on [Apple Sili
-000010a0: 636f 6e5d 2868 7474 7073 3a2f 2f64 6f63  con](https://doc
-000010b0: 732e 636d 6f6e 2e61 692f 6765 742d 7374  s.cmon.ai/get-st
-000010c0: 6172 7465 642f 696e 7374 616c 6c2f 6170  arted/install/ap
-000010d0: 706c 652d 7369 6c69 636f 6e2d 6d31 2d6d  ple-silicon-m1-m
-000010e0: 322f 290a 0a0a 2323 2047 6574 2053 7461  2/)...## Get Sta
-000010f0: 7274 6564 0a0a 2323 2320 4261 7369 6320  rted..### Basic 
-00001100: 436f 6e63 6570 7473 0a0a 436d 6f6e 2068  Concepts..Cmon h
-00001110: 6173 2066 6f75 7220 6675 6e64 616d 656e  as four fundamen
-00001120: 7461 6c20 636f 6e63 6570 7473 3a0a 0a2d  tal concepts:..-
-00001130: 2041 205b 2a2a 446f 6375 6d65 6e74 2a2a   A [**Document**
-00001140: 5d28 6874 7470 733a 2f2f 646f 6361 7272  ](https://docarr
-00001150: 6179 2e63 6d6f 6e2e 6169 2f29 2028 6672  ay.cmon.ai/) (fr
-00001160: 6f6d 205b 446f 6341 7272 6179 5d28 6874  om [DocArray](ht
-00001170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001180: 2f64 6f63 6172 7261 792f 646f 6361 7272  /docarray/docarr
-00001190: 6179 2929 2069 7320 7468 6520 696e 7075  ay)) is the inpu
-000011a0: 742f 6f75 7470 7574 2066 6f72 6d61 7420  t/output format 
-000011b0: 696e 2043 6d6f 6e2e 0a2d 2041 6e20 5b2a  in Cmon..- An [*
-000011c0: 2a45 7865 6375 746f 722a 2a5d 2868 7474  *Executor**](htt
-000011d0: 7073 3a2f 2f64 6f63 732e 636d 6f6e 2e61  ps://docs.cmon.a
-000011e0: 692f 636f 6e63 6570 7473 2f73 6572 7669  i/concepts/servi
-000011f0: 6e67 2f65 7865 6375 746f 722f 2920 6973  ng/executor/) is
-00001200: 2061 2050 7974 686f 6e20 636c 6173 7320   a Python class 
-00001210: 7468 6174 2074 7261 6e73 666f 726d 7320  that transforms 
-00001220: 616e 6420 7072 6f63 6573 7365 7320 446f  and processes Do
-00001230: 6375 6d65 6e74 732e 0a2d 2041 205b 2a2a  cuments..- A [**
-00001240: 4465 706c 6f79 6d65 6e74 2a2a 5d28 6874  Deployment**](ht
-00001250: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
-00001260: 6169 2f63 6f6e 6365 7074 732f 6f72 6368  ai/concepts/orch
-00001270: 6573 7472 6174 696f 6e2f 6465 706c 6f79  estration/deploy
-00001280: 6d65 6e74 2920 7365 7276 6573 2061 2073  ment) serves a s
-00001290: 696e 676c 6520 4578 6563 7574 6f72 2c20  ingle Executor, 
-000012a0: 7768 696c 6520 6120 5b2a 2a46 6c6f 772a  while a [**Flow*
-000012b0: 2a5d 2868 7474 7073 3a2f 2f64 6f63 732e  *](https://docs.
-000012c0: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-000012d0: 2f6f 7263 6865 7374 7261 7469 6f6e 2f66  /orchestration/f
-000012e0: 6c6f 772f 2920 7365 7276 6573 2045 7865  low/) serves Exe
-000012f0: 6375 746f 7273 2063 6861 696e 6564 2069  cutors chained i
-00001300: 6e74 6f20 6120 7069 7065 6c69 6e65 2e0a  nto a pipeline..
-00001310: 0a0a 5b54 6865 2066 756c 6c20 676c 6f73  ..[The full glos
-00001320: 7361 7279 2069 7320 6578 706c 6169 6e65  sary is explaine
-00001330: 6420 6865 7265 5d28 6874 7470 733a 2f2f  d here](https://
-00001340: 646f 6373 2e63 6d6f 6e2e 6169 2f63 6f6e  docs.cmon.ai/con
-00001350: 6365 7074 732f 7072 656c 696d 696e 6172  cepts/preliminar
-00001360: 6965 732f 2329 2e0a 0a23 2323 2042 7569  ies/#)...### Bui
-00001370: 6c64 2041 4920 5365 7276 6963 6573 0a3c  ld AI Services.<
-00001380: 212d 2d20 7374 6172 7420 6275 696c 642d  !-- start build-
-00001390: 6169 2d73 6572 7669 6365 7320 2d2d 3e0a  ai-services -->.
-000013a0: 0a4c 6574 2773 2062 7569 6c64 2061 2066  .Let's build a f
-000013b0: 6173 742c 2072 656c 6961 626c 6520 616e  ast, reliable an
-000013c0: 6420 7363 616c 6162 6c65 2067 5250 432d  d scalable gRPC-
-000013d0: 6261 7365 6420 4149 2073 6572 7669 6365  based AI service
-000013e0: 2e20 496e 2043 6d6f 6e20 7765 2063 616c  . In Cmon we cal
-000013f0: 6c20 7468 6973 2061 6e20 2a2a 5b45 7865  l this an **[Exe
-00001400: 6375 746f 725d 2868 7474 7073 3a2f 2f64  cutor](https://d
-00001410: 6f63 732e 636d 6f6e 2e61 692f 636f 6e63  ocs.cmon.ai/conc
-00001420: 6570 7473 2f65 7865 6375 746f 722f 292a  epts/executor/)*
-00001430: 2a2e 204f 7572 2073 696d 706c 6520 4578  *. Our simple Ex
-00001440: 6563 7574 6f72 2077 696c 6c20 7772 6170  ecutor will wrap
-00001450: 2074 6865 205b 5374 6162 6c65 4c4d 5d28   the [StableLM](
-00001460: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00001470: 6163 652e 636f 2f73 7461 6269 6c69 7479  ace.co/stability
-00001480: 6169 2f73 7461 626c 656c 6d2d 6261 7365  ai/stablelm-base
-00001490: 2d61 6c70 6861 2d33 6229 204c 4c4d 2066  -alpha-3b) LLM f
-000014a0: 726f 6d20 5374 6162 696c 6974 7920 4149  rom Stability AI
-000014b0: 2e20 5765 276c 6c20 7468 656e 2075 7365  . We'll then use
-000014c0: 2061 202a 2a44 6570 6c6f 796d 656e 742a   a **Deployment*
-000014d0: 2a20 746f 2073 6572 7665 2069 742e 0a0a  * to serve it...
-000014e0: 215b 5d28 2e2f 2e67 6974 6875 622f 696d  ![](./.github/im
-000014f0: 6167 6573 2f64 6570 6c6f 796d 656e 742d  ages/deployment-
-00001500: 6469 6167 7261 6d2e 706e 6729 0a0a 3e20  diagram.png)..> 
-00001510: 2a2a 4e6f 7465 2a2a 0a3e 2041 2044 6570  **Note**.> A Dep
-00001520: 6c6f 796d 656e 7420 7365 7276 6573 206a  loyment serves j
-00001530: 7573 7420 6f6e 6520 4578 6563 7574 6f72  ust one Executor
-00001540: 2e20 546f 2063 6f6d 6269 6e65 206d 756c  . To combine mul
-00001550: 7469 706c 6520 4578 6563 7574 6f72 7320  tiple Executors 
-00001560: 696e 746f 2061 2070 6970 656c 696e 6520  into a pipeline 
-00001570: 616e 6420 7365 7276 6520 7468 6174 2c20  and serve that, 
-00001580: 7573 6520 6120 5b46 6c6f 775d 2823 6275  use a [Flow](#bu
-00001590: 696c 642d 612d 7069 7065 6c69 6e65 292e  ild-a-pipeline).
-000015a0: 0a0a 4c65 7427 7320 696d 706c 656d 656e  ..Let's implemen
-000015b0: 7420 7468 6520 7365 7276 6963 6527 7320  t the service's 
-000015c0: 6c6f 6769 633a 0a0a 3c74 6162 6c65 3e0a  logic:..<table>.
-000015d0: 3c74 723e 0a3c 7468 3e3c 636f 6465 3e65  <tr>.<th><code>e
-000015e0: 7865 6375 746f 722e 7079 3c2f 636f 6465  xecutor.py</code
-000015f0: 3e3c 2f74 683e 200a 3c74 723e 0a3c 7464  ></th> .<tr>.<td
-00001600: 3e0a 0a60 6060 7079 7468 6f6e 0a66 726f  >..```python.fro
-00001610: 6d20 636d 6f6e 2069 6d70 6f72 7420 4578  m cmon import Ex
-00001620: 6563 7574 6f72 2c20 7265 7175 6573 7473  ecutor, requests
-00001630: 0a66 726f 6d20 646f 6361 7272 6179 2069  .from docarray i
-00001640: 6d70 6f72 7420 446f 6375 6d65 6e74 4172  mport DocumentAr
-00001650: 7261 790a 0a66 726f 6d20 7472 616e 7366  ray..from transf
-00001660: 6f72 6d65 7273 2069 6d70 6f72 7420 7069  ormers import pi
-00001670: 7065 6c69 6e65 0a0a 0a63 6c61 7373 2053  peline...class S
-00001680: 7461 626c 654c 4d28 4578 6563 7574 6f72  tableLM(Executor
-00001690: 293a 0a0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-000016a0: 6974 5f5f 2873 656c 662c 202a 2a6b 7761  it__(self, **kwa
-000016b0: 7267 7329 3a0a 2020 2020 2020 2020 7375  rgs):.        su
-000016c0: 7065 7228 292e 5f5f 696e 6974 5f5f 282a  per().__init__(*
-000016d0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-000016e0: 2073 656c 662e 6765 6e65 7261 746f 7220   self.generator 
-000016f0: 3d20 7069 7065 6c69 6e65 2827 7465 7874  = pipeline('text
-00001700: 2d67 656e 6572 6174 696f 6e27 2c20 6d6f  -generation', mo
-00001710: 6465 6c3d 2773 7461 626c 656c 6d2d 3362  del='stablelm-3b
-00001720: 2729 0a0a 2020 2020 4072 6571 7565 7374  ')..    @request
-00001730: 730a 2020 2020 6465 6620 6765 6e65 7261  s.    def genera
-00001740: 7465 2873 656c 662c 2064 6f63 733a 2044  te(self, docs: D
-00001750: 6f63 756d 656e 7441 7272 6179 2c20 2a2a  ocumentArray, **
-00001760: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
-00001770: 2067 656e 6572 6174 6564 5f74 6578 7420   generated_text 
-00001780: 3d20 7365 6c66 2e67 656e 6572 6174 6f72  = self.generator
-00001790: 2864 6f63 732e 7465 7874 7329 0a20 2020  (docs.texts).   
-000017a0: 2020 2020 2064 6f63 732e 7465 7874 7320       docs.texts 
-000017b0: 3d20 5b67 656e 5b30 5d5b 2767 656e 6572  = [gen[0]['gener
-000017c0: 6174 6564 5f74 6578 7427 5d20 666f 7220  ated_text'] for 
-000017d0: 6765 6e20 696e 2067 656e 6572 6174 6564  gen in generated
-000017e0: 5f74 6578 745d 0a60 6060 0a0a 3c2f 7464  _text].```..</td
-000017f0: 3e0a 3c2f 7472 3e0a 3c2f 7461 626c 653e  >.</tr>.</table>
-00001800: 0a0a 5468 656e 2077 6520 6465 706c 6f79  ..Then we deploy
-00001810: 2069 7420 7769 7468 2065 6974 6865 7220   it with either 
-00001820: 7468 6520 5079 7468 6f6e 2041 5049 206f  the Python API o
-00001830: 7220 5941 4d4c 3a0a 3c64 6976 2063 6c61  r YAML:.<div cla
-00001840: 7373 3d22 7461 626c 652d 7772 6170 7065  ss="table-wrappe
-00001850: 7222 3e0a 3c74 6162 6c65 3e0a 3c74 723e  r">.<table>.<tr>
-00001860: 0a3c 7468 3e20 5079 7468 6f6e 2041 5049  .<th> Python API
-00001870: 3a20 3c63 6f64 653e 6465 706c 6f79 6d65  : <code>deployme
-00001880: 6e74 2e70 793c 2f63 6f64 653e 203c 2f74  nt.py</code> </t
-00001890: 683e 200a 3c74 683e 2059 414d 4c3a 203c  h> .<th> YAML: <
-000018a0: 636f 6465 3e64 6570 6c6f 796d 656e 742e  code>deployment.
-000018b0: 796d 6c3c 2f63 6f64 653e 203c 2f74 683e  yml</code> </th>
-000018c0: 0a3c 2f74 723e 0a3c 7472 3e0a 3c74 643e  .</tr>.<tr>.<td>
-000018d0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-000018e0: 2063 6d6f 6e20 696d 706f 7274 2044 6570   cmon import Dep
-000018f0: 6c6f 796d 656e 740a 6672 6f6d 2065 7865  loyment.from exe
-00001900: 6375 746f 7220 696d 706f 7274 2053 7461  cutor import Sta
-00001910: 626c 654c 4d0a 0a64 6570 203d 2044 6570  bleLM..dep = Dep
-00001920: 6c6f 796d 656e 7428 7573 6573 3d53 7461  loyment(uses=Sta
-00001930: 626c 654c 4d2c 2074 696d 656f 7574 5f72  bleLM, timeout_r
-00001940: 6561 6479 3d2d 312c 2070 6f72 743d 3132  eady=-1, port=12
-00001950: 3334 3529 0a0a 7769 7468 2064 6570 3a0a  345)..with dep:.
-00001960: 2020 2020 6465 702e 626c 6f63 6b28 290a      dep.block().
-00001970: 6060 600a 0a3c 2f74 643e 0a3c 7464 3e0a  ```..</td>.<td>.
-00001980: 0a60 6060 7961 6d6c 0a6a 7479 7065 3a20  .```yaml.jtype: 
-00001990: 4465 706c 6f79 6d65 6e74 0a77 6974 683a  Deployment.with:
-000019a0: 0a20 2075 7365 733a 2053 7461 626c 654c  .  uses: StableL
-000019b0: 4d0a 2020 7079 5f6d 6f64 756c 6573 3a0a  M.  py_modules:.
-000019c0: 2020 2020 2d20 6578 6563 7574 6f72 2e70      - executor.p
-000019d0: 790a 2020 7469 6d65 6f75 745f 7265 6164  y.  timeout_read
-000019e0: 793a 202d 310a 2020 706f 7274 3a20 3132  y: -1.  port: 12
-000019f0: 3334 350a 6060 600a 0a41 6e64 2072 756e  345.```..And run
-00001a00: 2074 6865 2059 414d 4c20 4465 706c 6f79   the YAML Deploy
-00001a10: 6d65 6e74 2077 6974 6820 7468 6520 434c  ment with the CL
-00001a20: 493a 2060 636d 6f6e 2064 6570 6c6f 796d  I: `cmon deploym
-00001a30: 656e 7420 2d2d 7573 6573 2064 6570 6c6f  ent --uses deplo
-00001a40: 796d 656e 742e 796d 6c60 0a0a 3c2f 7464  yment.yml`..</td
-00001a50: 3e0a 3c2f 7472 3e0a 3c2f 7461 626c 653e  >.</tr>.</table>
-00001a60: 0a3c 2f64 6976 3e0a 0a55 7365 205b 436d  .</div>..Use [Cm
-00001a70: 6f6e 2043 6c69 656e 745d 2868 7474 7073  on Client](https
-00001a80: 3a2f 2f64 6f63 732e 636d 6f6e 2e61 692f  ://docs.cmon.ai/
-00001a90: 636f 6e63 6570 7473 2f63 6c69 656e 742f  concepts/client/
-00001aa0: 2920 746f 206d 616b 6520 7265 7175 6573  ) to make reques
-00001ab0: 7473 2074 6f20 7468 6520 7365 7276 6963  ts to the servic
-00001ac0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
-00001ad0: 6f6d 2064 6f63 6172 7261 7920 696d 706f  om docarray impo
-00001ae0: 7274 2044 6f63 756d 656e 740a 6672 6f6d  rt Document.from
-00001af0: 2063 6d6f 6e20 696d 706f 7274 2043 6c69   cmon import Cli
-00001b00: 656e 740a 0a70 726f 6d70 7420 3d20 446f  ent..prompt = Do
-00001b10: 6375 6d65 6e74 280a 2020 2020 7461 6773  cument(.    tags
-00001b20: 203d 207b 2770 726f 6d70 7427 3a20 2773   = {'prompt': 's
-00001b30: 7567 6765 7374 2061 6e20 696e 7465 7265  uggest an intere
-00001b40: 7374 696e 6720 696d 6167 6520 6765 6e65  sting image gene
-00001b50: 7261 7469 6f6e 2070 726f 6d70 7420 666f  ration prompt fo
-00001b60: 7220 6120 6d6f 6e61 206c 6973 6120 7661  r a mona lisa va
-00001b70: 7269 616e 7427 7d0a 290a 0a63 6c69 656e  riant'}.)..clien
-00001b80: 7420 3d20 436c 6965 6e74 2870 6f72 743d  t = Client(port=
-00001b90: 3132 3334 3529 2020 2320 7573 6520 706f  12345)  # use po
-00001ba0: 7274 2066 726f 6d20 6f75 7470 7574 2061  rt from output a
-00001bb0: 626f 7665 0a72 6573 706f 6e73 6520 3d20  bove.response = 
-00001bc0: 636c 6965 6e74 2e70 6f73 7428 6f6e 3d27  client.post(on='
-00001bd0: 2f27 2c20 696e 7075 7473 3d5b 7072 6f6d  /', inputs=[prom
-00001be0: 7074 5d29 0a0a 7072 696e 7428 7265 7370  pt])..print(resp
-00001bf0: 6f6e 7365 5b30 5d2e 7465 7874 290a 6060  onse[0].text).``
-00001c00: 600a 0a60 6060 7465 7874 0a61 2073 7465  `..```text.a ste
-00001c10: 616d 7075 6e6b 2076 6572 7369 6f6e 206f  ampunk version o
-00001c20: 6620 7468 6520 4d6f 6e61 204c 6973 612c  f the Mona Lisa,
-00001c30: 2069 6e63 6f72 706f 7261 7469 6e67 206d   incorporating m
-00001c40: 6563 6861 6e69 6361 6c20 6765 6172 732c  echanical gears,
-00001c50: 2062 7261 7373 2065 6c65 6d65 6e74 732c   brass elements,
-00001c60: 2061 6e64 2056 6963 746f 7269 616e 2065   and Victorian e
-00001c70: 7261 2063 6c6f 7468 696e 6720 6465 7461  ra clothing deta
-00001c80: 696c 730a 6060 600a 0a3c 212d 2d20 656e  ils.```..<!-- en
-00001c90: 6420 6275 696c 642d 6169 2d73 6572 7669  d build-ai-servi
-00001ca0: 6365 7320 2d2d 3e0a 0a3e 202a 2a4e 6f74  ces -->..> **Not
-00001cb0: 652a 2a0a 3e20 496e 2061 206e 6f74 6562  e**.> In a noteb
-00001cc0: 6f6f 6b2c 2079 6f75 2063 616e 2774 2075  ook, you can't u
-00001cd0: 7365 2060 6465 706c 6f79 6d65 6e74 2e62  se `deployment.b
-00001ce0: 6c6f 636b 2829 6020 616e 6420 7468 656e  lock()` and then
-00001cf0: 206d 616b 6520 7265 7175 6573 7473 2074   make requests t
-00001d00: 6f20 7468 6520 636c 6965 6e74 2e20 506c  o the client. Pl
-00001d10: 6561 7365 2072 6566 6572 2074 6f20 7468  ease refer to th
-00001d20: 6520 436f 6c61 6220 6c69 6e6b 2061 626f  e Colab link abo
-00001d30: 7665 2066 6f72 2072 6570 726f 6475 6369  ve for reproduci
-00001d40: 626c 6520 4a75 7079 7465 7220 4e6f 7465  ble Jupyter Note
-00001d50: 626f 6f6b 2063 6f64 6520 736e 6970 7065  book code snippe
-00001d60: 7473 2e0a 0a23 2323 2042 7569 6c64 2061  ts...### Build a
-00001d70: 2070 6970 656c 696e 650a 0a3c 212d 2d20   pipeline..<!-- 
-00001d80: 7374 6172 7420 6275 696c 642d 7069 7065  start build-pipe
-00001d90: 6c69 6e65 7320 2d2d 3e0a 0a53 6f6d 6574  lines -->..Somet
-00001da0: 696d 6573 2079 6f75 2077 616e 7420 746f  imes you want to
-00001db0: 2063 6861 696e 206d 6963 726f 7365 7276   chain microserv
-00001dc0: 6963 6573 2074 6f67 6574 6865 7220 696e  ices together in
-00001dd0: 746f 2061 2070 6970 656c 696e 652e 2054  to a pipeline. T
-00001de0: 6861 7427 7320 7768 6572 6520 6120 5b46  hat's where a [F
-00001df0: 6c6f 775d 2868 7474 7073 3a2f 2f64 6f63  low](https://doc
-00001e00: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00001e10: 7473 2f66 6c6f 772f 2920 636f 6d65 7320  ts/flow/) comes 
-00001e20: 696e 2e0a 0a41 2046 6c6f 7720 6973 2061  in...A Flow is a
-00001e30: 205b 4441 475d 2868 7474 7073 3a2f 2f64   [DAG](https://d
-00001e40: 652e 7769 6b69 7065 6469 612e 6f72 672f  e.wikipedia.org/
-00001e50: 7769 6b69 2f44 4147 2920 7069 7065 6c69  wiki/DAG) pipeli
-00001e60: 6e65 2c20 636f 6d70 6f73 6564 206f 6620  ne, composed of 
-00001e70: 6120 7365 7420 6f66 2073 7465 7073 2c20  a set of steps, 
-00001e80: 4974 206f 7263 6865 7374 7261 7465 7320  It orchestrates 
-00001e90: 6120 7365 7420 6f66 205b 4578 6563 7574  a set of [Execut
-00001ea0: 6f72 735d 2868 7474 7073 3a2f 2f64 6f63  ors](https://doc
-00001eb0: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00001ec0: 7473 2f65 7865 6375 746f 722f 2920 616e  ts/executor/) an
-00001ed0: 6420 6120 5b47 6174 6577 6179 5d28 6874  d a [Gateway](ht
-00001ee0: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
-00001ef0: 6169 2f63 6f6e 6365 7074 732f 6761 7465  ai/concepts/gate
-00001f00: 7761 792f 2920 746f 206f 6666 6572 2061  way/) to offer a
-00001f10: 6e20 656e 642d 746f 2d65 6e64 2073 6572  n end-to-end ser
-00001f20: 7669 6365 2e0a 0a3e 202a 2a4e 6f74 652a  vice...> **Note*
-00001f30: 2a0a 3e20 4966 2079 6f75 206a 7573 7420  *.> If you just 
-00001f40: 7761 6e74 2074 6f20 7365 7276 6520 6120  want to serve a 
-00001f50: 7369 6e67 6c65 2045 7865 6375 746f 722c  single Executor,
-00001f60: 2079 6f75 2063 616e 2075 7365 2061 205b   you can use a [
-00001f70: 4465 706c 6f79 6d65 6e74 5d28 2362 7569  Deployment](#bui
-00001f80: 6c64 2d61 692d 2d6d 6c2d 7365 7276 6963  ld-ai--ml-servic
-00001f90: 6573 292e 0a0a 466f 7220 696e 7374 616e  es)...For instan
-00001fa0: 6365 2c20 6c65 7427 7320 636f 6d62 696e  ce, let's combin
-00001fb0: 6520 5b6f 7572 2053 7461 626c 654c 4d20  e [our StableLM 
-00001fc0: 6c61 6e67 7561 6765 206d 6f64 656c 5d28  language model](
-00001fd0: 2362 7569 6c64 2d61 692d 2d6d 6c2d 7365  #build-ai--ml-se
-00001fe0: 7276 6963 6573 2920 7769 7468 2061 2053  rvices) with a S
-00001ff0: 7461 626c 6520 4469 6666 7573 696f 6e20  table Diffusion 
-00002000: 696d 6167 6520 6765 6e65 7261 7469 6f6e  image generation
-00002010: 2073 6572 7669 6365 2066 726f 6d20 436d   service from Cm
-00002020: 6f6e 2041 4927 7320 5b45 7865 6375 746f  on AI's [Executo
-00002030: 7220 4875 625d 2868 7474 7073 3a2f 2f63  r Hub](https://c
-00002040: 6c6f 7564 2e63 6d6f 6e2e 6169 2f65 7865  loud.cmon.ai/exe
-00002050: 6375 746f 7273 292e 2043 6861 696e 696e  cutors). Chainin
-00002060: 6720 7468 6573 6520 7365 7276 6963 6573  g these services
-00002070: 2074 6f67 6574 6865 7220 696e 746f 2061   together into a
-00002080: 205b 466c 6f77 5d28 6874 7470 733a 2f2f   [Flow](https://
-00002090: 646f 6373 2e63 6d6f 6e2e 6169 2f63 6f6e  docs.cmon.ai/con
-000020a0: 6365 7074 732f 666c 6f77 2f29 2077 696c  cepts/flow/) wil
-000020b0: 6c20 6769 7665 2075 7320 6120 7365 7276  l give us a serv
-000020c0: 6963 6520 7468 6174 2077 696c 6c20 6765  ice that will ge
-000020d0: 6e65 7261 7465 2069 6d61 6765 7320 6261  nerate images ba
-000020e0: 7365 6420 6f6e 2061 2070 726f 6d70 7420  sed on a prompt 
-000020f0: 6765 6e65 7261 7465 6420 6279 2074 6865  generated by the
-00002100: 204c 4c4d 2e0a 0a21 5b5d 282e 2f2e 6769   LLM...![](./.gi
-00002110: 7468 7562 2f69 6d61 6765 732f 666c 6f77  thub/images/flow
-00002120: 2d64 6961 6772 616d 2e70 6e67 290a 0a42  -diagram.png)..B
-00002130: 7569 6c64 2074 6865 2046 6c6f 7720 7769  uild the Flow wi
-00002140: 7468 2065 6974 6865 7220 5079 7468 6f6e  th either Python
-00002150: 206f 7220 5941 4d4c 3a0a 0a3c 6469 7620   or YAML:..<div 
-00002160: 636c 6173 733d 2274 6162 6c65 2d77 7261  class="table-wra
-00002170: 7070 6572 223e 0a3c 7461 626c 653e 0a3c  pper">.<table>.<
-00002180: 7472 3e0a 3c74 683e 2050 7974 686f 6e20  tr>.<th> Python 
-00002190: 4150 493a 203c 636f 6465 3e66 6c6f 772e  API: <code>flow.
-000021a0: 7079 3c2f 636f 6465 3e20 3c2f 7468 3e20  py</code> </th> 
-000021b0: 0a3c 7468 3e20 5941 4d4c 3a20 3c63 6f64  .<th> YAML: <cod
-000021c0: 653e 666c 6f77 2e79 6d6c 3c2f 636f 6465  e>flow.yml</code
-000021d0: 3e20 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  > </th>.</tr>.<t
-000021e0: 723e 0a3c 7464 3e0a 0a60 6060 7079 7468  r>.<td>..```pyth
-000021f0: 6f6e 0a66 726f 6d20 636d 6f6e 2069 6d70  on.from cmon imp
-00002200: 6f72 7420 466c 6f77 0a66 726f 6d20 6578  ort Flow.from ex
-00002210: 6563 7574 6f72 2069 6d70 6f72 7420 5374  ecutor import St
-00002220: 6162 6c65 4c4d 0a0a 666c 6f77 203d 2028  ableLM..flow = (
-00002230: 0a20 2020 2046 6c6f 7728 290a 2020 2020  .    Flow().    
-00002240: 2e61 6464 2875 7365 733d 5374 6162 6c65  .add(uses=Stable
-00002250: 4c4d 2c20 7469 6d65 6f75 745f 7265 6164  LM, timeout_read
-00002260: 793d 2d31 2c20 706f 7274 3d31 3233 3435  y=-1, port=12345
-00002270: 290a 2020 2020 2e61 6464 280a 2020 2020  ).    .add(.    
-00002280: 2020 2020 7573 6573 3d27 636d 6f6e 6169      uses='cmonai
-00002290: 3a2f 2f63 6d6f 6e2d 6169 2f54 6578 7454  ://cmon-ai/TextT
-000022a0: 6f49 6d61 6765 272c 0a20 2020 2020 2020  oImage',.       
-000022b0: 2074 696d 656f 7574 5f72 6561 6479 3d2d   timeout_ready=-
-000022c0: 312c 0a20 2020 2020 2020 2069 6e73 7461  1,.        insta
-000022d0: 6c6c 5f72 6571 7569 7265 6d65 6e74 733d  ll_requirements=
-000022e0: 5472 7565 2c0a 2020 2020 290a 2920 2023  True,.    ).)  #
-000022f0: 2075 7365 2074 6865 2045 7865 6375 746f   use the Executo
-00002300: 7220 6672 6f6d 2043 6d6f 6e27 7320 4578  r from Cmon's Ex
-00002310: 6563 7574 6f72 2068 7562 0a0a 7769 7468  ecutor hub..with
-00002320: 2066 6c6f 773a 0a20 2020 2066 6c6f 772e   flow:.    flow.
-00002330: 626c 6f63 6b28 290a 6060 600a 0a3c 2f74  block().```..</t
-00002340: 643e 0a3c 7464 3e0a 0a60 6060 7961 6d6c  d>.<td>..```yaml
-00002350: 0a6a 7479 7065 3a20 466c 6f77 0a77 6974  .jtype: Flow.wit
-00002360: 683a 0a20 2020 2070 6f72 743a 2031 3233  h:.    port: 123
-00002370: 3435 0a65 7865 6375 746f 7273 3a0a 2020  45.executors:.  
-00002380: 2d20 7573 6573 3a20 5374 6162 6c65 4c4d  - uses: StableLM
-00002390: 0a20 2020 2074 696d 656f 7574 5f72 6561  .    timeout_rea
-000023a0: 6479 3a20 2d31 0a20 2020 2070 795f 6d6f  dy: -1.    py_mo
-000023b0: 6475 6c65 733a 0a20 2020 2020 202d 2065  dules:.      - e
-000023c0: 7865 6375 746f 722e 7079 0a20 202d 2075  xecutor.py.  - u
-000023d0: 7365 733a 2063 6d6f 6e61 693a 2f2f 636d  ses: cmonai://cm
-000023e0: 6f6e 2d61 692f 5465 7874 546f 496d 6167  on-ai/TextToImag
-000023f0: 650a 2020 2020 7469 6d65 6f75 745f 7265  e.    timeout_re
-00002400: 6164 793a 202d 310a 2020 2020 696e 7374  ady: -1.    inst
-00002410: 616c 6c5f 7265 7175 6972 656d 656e 7473  all_requirements
-00002420: 3a20 7472 7565 0a60 6060 0a0a 5468 656e  : true.```..Then
-00002430: 2072 756e 2074 6865 2059 414d 4c20 466c   run the YAML Fl
-00002440: 6f77 2077 6974 6820 7468 6520 434c 493a  ow with the CLI:
-00002450: 2060 636d 6f6e 2066 6c6f 7720 2d2d 7573   `cmon flow --us
-00002460: 6573 2066 6c6f 772e 796d 6c60 0a0a 3c2f  es flow.yml`..</
-00002470: 7464 3e0a 3c2f 7472 3e0a 3c2f 7461 626c  td>.</tr>.</tabl
-00002480: 653e 0a3c 2f64 6976 3e0a 0a54 6865 6e2c  e>.</div>..Then,
-00002490: 2075 7365 205b 436d 6f6e 2043 6c69 656e   use [Cmon Clien
-000024a0: 745d 2868 7474 7073 3a2f 2f64 6f63 732e  t](https://docs.
-000024b0: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-000024c0: 2f63 6c69 656e 742f 2920 746f 206d 616b  /client/) to mak
-000024d0: 6520 7265 7175 6573 7473 2074 6f20 7468  e requests to th
-000024e0: 6520 466c 6f77 3a0a 0a60 6060 7079 7468  e Flow:..```pyth
-000024f0: 6f6e 0a66 726f 6d20 636d 6f6e 2069 6d70  on.from cmon imp
-00002500: 6f72 7420 436c 6965 6e74 2c20 446f 6375  ort Client, Docu
-00002510: 6d65 6e74 0a0a 636c 6965 6e74 203d 2043  ment..client = C
-00002520: 6c69 656e 7428 706f 7274 3d31 3233 3435  lient(port=12345
-00002530: 290a 0a70 726f 6d70 7420 3d20 446f 6375  )..prompt = Docu
-00002540: 6d65 6e74 280a 2020 2020 7461 6773 203d  ment(.    tags =
-00002550: 207b 2770 726f 6d70 7427 3a20 2773 7567   {'prompt': 'sug
-00002560: 6765 7374 2061 6e20 696e 7465 7265 7374  gest an interest
-00002570: 696e 6720 696d 6167 6520 6765 6e65 7261  ing image genera
-00002580: 7469 6f6e 2070 726f 6d70 7420 666f 7220  tion prompt for 
-00002590: 6120 6d6f 6e61 206c 6973 6120 7661 7269  a mona lisa vari
-000025a0: 616e 7427 7d0a 290a 0a72 6573 706f 6e73  ant'}.)..respons
-000025b0: 6520 3d20 636c 6965 6e74 2e70 6f73 7428  e = client.post(
-000025c0: 6f6e 3d27 2f27 2c20 696e 7075 7473 3d5b  on='/', inputs=[
-000025d0: 7072 6f6d 7074 5d29 0a0a 7265 7370 6f6e  prompt])..respon
-000025e0: 7365 5b30 5d2e 6469 7370 6c61 7928 290a  se[0].display().
-000025f0: 6060 600a 0a21 5b5d 282e 2f2e 6769 7468  ```..![](./.gith
-00002600: 7562 2f69 6d61 6765 732f 6d6f 6e61 2d6c  ub/images/mona-l
-00002610: 6973 612e 706e 6729 0a0a 2323 2044 6570  isa.png)..## Dep
-00002620: 6c6f 7920 746f 2074 6865 2063 6c6f 7564  loy to the cloud
-00002630: 0a0a 596f 7520 6361 6e20 616c 736f 2064  ..You can also d
-00002640: 6570 6c6f 7920 6120 466c 6f77 2074 6f20  eploy a Flow to 
-00002650: 4a43 6c6f 7564 2e0a 0a46 6972 7374 2c20  JCloud...First, 
-00002660: 7475 726e 2074 6865 2060 666c 6f77 2e79  turn the `flow.y
-00002670: 6d6c 6020 6669 6c65 2069 6e74 6f20 6120  ml` file into a 
-00002680: 5b4a 436c 6f75 642d 636f 6d70 6174 6962  [JCloud-compatib
-00002690: 6c65 2059 414d 4c5d 2868 7474 7073 3a2f  le YAML](https:/
-000026a0: 2f64 6f63 732e 636d 6f6e 2e61 692f 636f  /docs.cmon.ai/co
-000026b0: 6e63 6570 7473 2f6a 636c 6f75 642f 7961  ncepts/jcloud/ya
-000026c0: 6d6c 2d73 7065 632f 2920 6279 2073 7065  ml-spec/) by spe
-000026d0: 6369 6679 696e 6720 7265 736f 7572 6365  cifying resource
-000026e0: 2072 6571 7569 7265 6d65 6e74 7320 616e   requirements an
-000026f0: 6420 7573 696e 6720 636f 6e74 6169 6e65  d using containe
-00002700: 7269 7a65 6420 4875 6220 4578 6563 7574  rized Hub Execut
-00002710: 6f72 732e 0a0a 5468 656e 2c20 7573 6520  ors...Then, use 
-00002720: 6063 6d6f 6e20 636c 6f75 6420 6465 706c  `cmon cloud depl
-00002730: 6f79 6020 636f 6d6d 616e 6420 746f 2064  oy` command to d
-00002740: 6570 6c6f 7920 746f 2074 6865 2063 6c6f  eploy to the clo
-00002750: 7564 3a0a 0a60 6060 7368 656c 6c0a 7767  ud:..```shell.wg
-00002760: 6574 2068 7474 7073 3a2f 2f72 6177 2e67  et https://raw.g
-00002770: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00002780: 2e63 6f6d 2f63 6d6f 6e2d 6169 2f63 6d6f  .com/cmon-ai/cmo
-00002790: 6e2f 6d61 7374 6572 2f2e 6769 7468 7562  n/master/.github
-000027a0: 2f67 6574 7469 6e67 2d73 7461 7274 6564  /getting-started
-000027b0: 2f6a 636c 6f75 642d 666c 6f77 2e79 6d6c  /jcloud-flow.yml
-000027c0: 0a63 6d6f 6e20 636c 6f75 6420 6465 706c  .cmon cloud depl
-000027d0: 6f79 206a 636c 6f75 642d 666c 6f77 2e79  oy jcloud-flow.y
-000027e0: 6d6c 0a60 6060 0a0a 3e20 2a2a 5761 726e  ml.```..> **Warn
-000027f0: 696e 672a 2a0a 3e0a 3e20 4d61 6b65 2073  ing**.>.> Make s
-00002800: 7572 6520 746f 2064 656c 6574 652f 636c  ure to delete/cl
-00002810: 6561 6e20 7570 2074 6865 2046 6c6f 7720  ean up the Flow 
-00002820: 6f6e 6365 2079 6f75 2061 7265 2064 6f6e  once you are don
-00002830: 6520 7769 7468 2074 6869 7320 7475 746f  e with this tuto
-00002840: 7269 616c 2074 6f20 7361 7665 2072 6573  rial to save res
-00002850: 6f75 7263 6573 2061 6e64 2063 7265 6469  ources and credi
-00002860: 7473 2e0a 0a52 6561 6420 6d6f 7265 2061  ts...Read more a
-00002870: 626f 7574 205b 6465 706c 6f79 696e 6720  bout [deploying 
-00002880: 466c 6f77 7320 746f 204a 436c 6f75 645d  Flows to JCloud]
-00002890: 2868 7474 7073 3a2f 2f64 6f63 732e 636d  (https://docs.cm
-000028a0: 6f6e 2e61 692f 636f 6e63 6570 7473 2f6a  on.ai/concepts/j
-000028b0: 636c 6f75 642f 2364 6570 6c6f 7929 2e0a  cloud/#deploy)..
-000028c0: 0a3c 212d 2d20 656e 6420 6275 696c 642d  .<!-- end build-
-000028d0: 7069 7065 6c69 6e65 7320 2d2d 3e0a 0a43  pipelines -->..C
-000028e0: 6865 636b 205b 7468 6520 6765 7474 696e  heck [the gettin
-000028f0: 672d 7374 6172 7465 6420 7072 6f6a 6563  g-started projec
-00002900: 7420 736f 7572 6365 2063 6f64 655d 2868  t source code](h
-00002910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002920: 6d2f 636d 6f6e 2d61 692f 636d 6f6e 2f74  m/cmon-ai/cmon/t
-00002930: 7265 652f 6d61 7374 6572 2f2e 6769 7468  ree/master/.gith
-00002940: 7562 2f67 6574 7469 6e67 2d73 7461 7274  ub/getting-start
-00002950: 6564 292e 0a0a 2323 2320 4561 7379 2073  ed)...### Easy s
-00002960: 6361 6c61 6269 6c69 7479 2061 6e64 2063  calability and c
-00002970: 6f6e 6375 7272 656e 6379 0a0a 5768 7920  oncurrency..Why 
-00002980: 6e6f 7420 6a75 7374 2075 7365 2073 7461  not just use sta
-00002990: 6e64 6172 6420 5079 7468 6f6e 2074 6f20  ndard Python to 
-000029a0: 6275 696c 6420 7468 6174 206d 6963 726f  build that micro
-000029b0: 7365 7276 6963 6520 616e 6420 7069 7065  service and pipe
-000029c0: 6c69 6e65 3f20 436d 6f6e 2061 6363 656c  line? Cmon accel
-000029d0: 6572 6174 6573 2074 696d 6520 746f 206d  erates time to m
-000029e0: 6172 6b65 7420 6f66 2079 6f75 7220 6170  arket of your ap
-000029f0: 706c 6963 6174 696f 6e20 6279 206d 616b  plication by mak
-00002a00: 696e 6720 6974 206d 6f72 6520 7363 616c  ing it more scal
-00002a10: 6162 6c65 2061 6e64 2063 6c6f 7564 2d6e  able and cloud-n
-00002a20: 6174 6976 652e 2043 6d6f 6e20 616c 736f  ative. Cmon also
-00002a30: 2068 616e 646c 6573 2074 6865 2069 6e66   handles the inf
-00002a40: 7261 7374 7275 6374 7572 6520 636f 6d70  rastructure comp
-00002a50: 6c65 7869 7479 2069 6e20 7072 6f64 7563  lexity in produc
-00002a60: 7469 6f6e 2061 6e64 206f 7468 6572 2044  tion and other D
-00002a70: 6179 2d32 206f 7065 7261 7469 6f6e 7320  ay-2 operations 
-00002a80: 736f 2074 6861 7420 796f 7520 6361 6e20  so that you can 
-00002a90: 666f 6375 7320 6f6e 2074 6865 2064 6174  focus on the dat
-00002aa0: 6120 6170 706c 6963 6174 696f 6e20 6974  a application it
-00002ab0: 7365 6c66 2e0a 0a49 6e63 7265 6173 6520  self...Increase 
-00002ac0: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
-00002ad0: 2773 2074 6872 6f75 6768 7075 7420 7769  's throughput wi
-00002ae0: 7468 2073 6361 6c61 6269 6c69 7479 2066  th scalability f
-00002af0: 6561 7475 7265 7320 6f75 7420 6f66 2074  eatures out of t
-00002b00: 6865 2062 6f78 2c20 6c69 6b65 205b 7265  he box, like [re
-00002b10: 706c 6963 6173 5d28 6874 7470 733a 2f2f  plicas](https://
-00002b20: 646f 6373 2e63 6d6f 6e2e 6169 2f63 6f6e  docs.cmon.ai/con
-00002b30: 6365 7074 732f 6f72 6368 6573 7472 6174  cepts/orchestrat
-00002b40: 696f 6e2f 7363 616c 652d 6f75 742f 2372  ion/scale-out/#r
-00002b50: 6570 6c69 6361 7465 2d65 7865 6375 746f  eplicate-executo
-00002b60: 7273 292c 205b 7368 6172 6473 5d28 6874  rs), [shards](ht
-00002b70: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
-00002b80: 6169 2f63 6f6e 6365 7074 732f 6f72 6368  ai/concepts/orch
-00002b90: 6573 7472 6174 696f 6e2f 7363 616c 652d  estration/scale-
-00002ba0: 6f75 742f 2363 7573 746f 6d69 7a65 2d70  out/#customize-p
-00002bb0: 6f6c 6c69 6e67 2d62 6568 6176 696f 7273  olling-behaviors
-00002bc0: 2920 616e 6420 5b64 796e 616d 6963 2062  ) and [dynamic b
-00002bd0: 6174 6368 696e 675d 2868 7474 7073 3a2f  atching](https:/
-00002be0: 2f64 6f63 732e 636d 6f6e 2e61 692f 636f  /docs.cmon.ai/co
-00002bf0: 6e63 6570 7473 2f73 6572 7669 6e67 2f65  ncepts/serving/e
-00002c00: 7865 6375 746f 722f 6479 6e61 6d69 632d  xecutor/dynamic-
-00002c10: 6261 7463 6869 6e67 2f29 2e0a 0a4c 6574  batching/)...Let
-00002c20: 2773 2073 6361 6c65 2061 2053 7461 626c  's scale a Stabl
-00002c30: 6520 4469 6666 7573 696f 6e20 4578 6563  e Diffusion Exec
-00002c40: 7574 6f72 2064 6570 6c6f 796d 656e 7420  utor deployment 
-00002c50: 7769 7468 2072 6570 6c69 6361 7320 616e  with replicas an
-00002c60: 6420 6479 6e61 6d69 6320 6261 7463 6869  d dynamic batchi
-00002c70: 6e67 3a0a 0a21 5b5d 282e 2f2e 6769 7468  ng:..![](./.gith
-00002c80: 7562 2f69 6d61 6765 732f 7363 616c 6564  ub/images/scaled
-00002c90: 2d64 6570 6c6f 796d 656e 742e 706e 6729  -deployment.png)
-00002ca0: 0a0a 2a20 4372 6561 7465 2074 776f 2072  ..* Create two r
-00002cb0: 6570 6c69 6361 732c 2077 6974 6820 5b61  eplicas, with [a
-00002cc0: 2047 5055 2061 7373 6967 6e65 6420 666f   GPU assigned fo
-00002cd0: 7220 6561 6368 5d28 6874 7470 733a 2f2f  r each](https://
-00002ce0: 646f 6373 2e63 6d6f 6e2e 6169 2f63 6f6e  docs.cmon.ai/con
-00002cf0: 6365 7074 732f 666c 6f77 2f73 6361 6c65  cepts/flow/scale
-00002d00: 2d6f 7574 2f23 7265 706c 6963 6174 652d  -out/#replicate-
-00002d10: 6f6e 2d6d 756c 7469 706c 652d 6770 7573  on-multiple-gpus
-00002d20: 292e 0a2a 2045 6e61 626c 6520 6479 6e61  )..* Enable dyna
-00002d30: 6d69 6320 6261 7463 6869 6e67 2074 6f20  mic batching to 
-00002d40: 7072 6f63 6573 7320 696e 636f 6d69 6e67  process incoming
-00002d50: 2070 6172 616c 6c65 6c20 7265 7175 6573   parallel reques
-00002d60: 7473 2074 6f67 6574 6865 7220 7769 7468  ts together with
-00002d70: 2074 6865 2073 616d 6520 6d6f 6465 6c20   the same model 
-00002d80: 696e 6665 7265 6e63 652e 0a0a 0a3c 6469  inference....<di
-00002d90: 7620 636c 6173 733d 2274 6162 6c65 2d77  v class="table-w
-00002da0: 7261 7070 6572 223e 0a3c 7461 626c 653e  rapper">.<table>
-00002db0: 0a3c 7472 3e0a 3c74 683e 204e 6f72 6d61  .<tr>.<th> Norma
-00002dc0: 6c20 4465 706c 6f79 6d65 6e74 203c 2f74  l Deployment </t
-00002dd0: 683e 200a 3c74 683e 2053 6361 6c65 6420  h> .<th> Scaled 
-00002de0: 4465 706c 6f79 6d65 6e74 203c 2f74 683e  Deployment </th>
-00002df0: 0a3c 2f74 723e 0a3c 7472 3e0a 3c74 643e  .</tr>.<tr>.<td>
-00002e00: 0a0a 6060 6079 616d 6c0a 6a74 7970 653a  ..```yaml.jtype:
-00002e10: 2044 6570 6c6f 796d 656e 740a 7769 7468   Deployment.with
-00002e20: 3a0a 2020 7469 6d65 6f75 745f 7265 6164  :.  timeout_read
-00002e30: 793a 202d 310a 2020 7573 6573 3a20 636d  y: -1.  uses: cm
-00002e40: 6f6e 6169 3a2f 2f63 6d6f 6e2d 6169 2f54  onai://cmon-ai/T
-00002e50: 6578 7454 6f49 6d61 6765 0a20 2069 6e73  extToImage.  ins
-00002e60: 7461 6c6c 5f72 6571 7569 7265 6d65 6e74  tall_requirement
-00002e70: 733a 2074 7275 650a 6060 600a 0a3c 2f74  s: true.```..</t
-00002e80: 643e 0a3c 7464 3e0a 0a60 6060 7961 6d6c  d>.<td>..```yaml
-00002e90: 0a6a 7479 7065 3a20 4465 706c 6f79 6d65  .jtype: Deployme
-00002ea0: 6e74 0a77 6974 683a 0a20 2074 696d 656f  nt.with:.  timeo
-00002eb0: 7574 5f72 6561 6479 3a20 2d31 0a20 2075  ut_ready: -1.  u
-00002ec0: 7365 733a 2063 6d6f 6e61 693a 2f2f 636d  ses: cmonai://cm
-00002ed0: 6f6e 2d61 692f 5465 7874 546f 496d 6167  on-ai/TextToImag
-00002ee0: 650a 2020 696e 7374 616c 6c5f 7265 7175  e.  install_requ
-00002ef0: 6972 656d 656e 7473 3a20 7472 7565 0a20  irements: true. 
-00002f00: 2065 6e76 3a0a 2020 2043 5544 415f 5649   env:.   CUDA_VI
-00002f10: 5349 424c 455f 4445 5649 4345 533a 2052  SIBLE_DEVICES: R
-00002f20: 520a 2020 7265 706c 6963 6173 3a20 320a  R.  replicas: 2.
-00002f30: 2020 7573 6573 5f64 796e 616d 6963 5f62    uses_dynamic_b
-00002f40: 6174 6368 696e 673a 2023 2063 6f6e 6669  atching: # confi
-00002f50: 6775 7265 2064 796e 616d 6963 2062 6174  gure dynamic bat
-00002f60: 6368 696e 670a 2020 2020 2f64 6566 6175  ching.    /defau
-00002f70: 6c74 3a0a 2020 2020 2020 7072 6566 6572  lt:.      prefer
-00002f80: 7265 645f 6261 7463 685f 7369 7a65 3a20  red_batch_size: 
-00002f90: 3130 0a20 2020 2020 2074 696d 656f 7574  10.      timeout
-00002fa0: 3a20 3230 300a 6060 600a 0a3c 2f74 643e  : 200.```..</td>
-00002fb0: 0a3c 2f74 723e 0a3c 2f74 6162 6c65 3e0a  .</tr>.</table>.
-00002fc0: 3c2f 6469 763e 0a0a 4173 7375 6d69 6e67  </div>..Assuming
-00002fd0: 2079 6f75 7220 6d61 6368 696e 6520 6861   your machine ha
-00002fe0: 7320 7477 6f20 4750 5573 2c20 7573 696e  s two GPUs, usin
-00002ff0: 6720 7468 6520 7363 616c 6564 2064 6570  g the scaled dep
-00003000: 6c6f 796d 656e 7420 5941 4d4c 2077 696c  loyment YAML wil
-00003010: 6c20 6769 7665 2062 6574 7465 7220 7468  l give better th
-00003020: 726f 7567 6870 7574 2063 6f6d 7061 7265  roughput compare
-00003030: 6420 746f 2074 6865 206e 6f72 6d61 6c20  d to the normal 
-00003040: 6465 706c 6f79 6d65 6e74 2e0a 0a54 6865  deployment...The
-00003050: 7365 2066 6561 7475 7265 7320 6170 706c  se features appl
-00003060: 7920 746f 2062 6f74 6820 5b44 6570 6c6f  y to both [Deplo
-00003070: 796d 656e 7420 5941 4d4c 5d28 6874 7470  yment YAML](http
-00003080: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-00003090: 2f63 6f6e 6365 7074 732f 6578 6563 7574  /concepts/execut
-000030a0: 6f72 2f64 6570 6c6f 796d 656e 742d 7961  or/deployment-ya
-000030b0: 6d6c 2d73 7065 632f 2364 6570 6c6f 796d  ml-spec/#deploym
-000030c0: 656e 742d 7961 6d6c 2d73 7065 6329 2061  ent-yaml-spec) a
-000030d0: 6e64 205b 466c 6f77 2059 414d 4c5d 2868  nd [Flow YAML](h
-000030e0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-000030f0: 2e61 692f 636f 6e63 6570 7473 2f66 6c6f  .ai/concepts/flo
-00003100: 772f 7961 6d6c 2d73 7065 632f 292e 2054  w/yaml-spec/). T
-00003110: 6861 6e6b 7320 746f 2074 6865 2059 414d  hanks to the YAM
-00003120: 4c20 7379 6e74 6178 2c20 796f 7520 6361  L syntax, you ca
-00003130: 6e20 696e 6a65 6374 2064 6570 6c6f 796d  n inject deploym
-00003140: 656e 7420 636f 6e66 6967 7572 6174 696f  ent configuratio
-00003150: 6e73 2072 6567 6172 646c 6573 7320 6f66  ns regardless of
-00003160: 2045 7865 6375 746f 7220 636f 6465 2e0a   Executor code..
-00003170: 0a23 2323 2047 6574 206f 6e20 7468 6520  .### Get on the 
-00003180: 6661 7374 206c 616e 6520 746f 2063 6c6f  fast lane to clo
-00003190: 7564 2d6e 6174 6976 650a 0a55 7369 6e67  ud-native..Using
-000031a0: 204b 7562 6572 6e65 7465 7320 7769 7468   Kubernetes with
-000031b0: 2043 6d6f 6e20 6973 2065 6173 793a 0a0a   Cmon is easy:..
-000031c0: 6060 6062 6173 680a 636d 6f6e 2065 7870  ```bash.cmon exp
-000031d0: 6f72 7420 6b75 6265 726e 6574 6573 2066  ort kubernetes f
-000031e0: 6c6f 772e 796d 6c20 2e2f 6d79 2d6b 3873  low.yml ./my-k8s
-000031f0: 0a6b 7562 6563 746c 2061 7070 6c79 202d  .kubectl apply -
-00003200: 5220 2d66 206d 792d 6b38 730a 6060 600a  R -f my-k8s.```.
-00003210: 0a41 6e64 2073 6f20 6973 2044 6f63 6b65  .And so is Docke
-00003220: 7220 436f 6d70 6f73 653a 0a0a 6060 6062  r Compose:..```b
-00003230: 6173 680a 636d 6f6e 2065 7870 6f72 7420  ash.cmon export 
-00003240: 646f 636b 6572 2d63 6f6d 706f 7365 2066  docker-compose f
-00003250: 6c6f 772e 796d 6c20 646f 636b 6572 2d63  low.yml docker-c
-00003260: 6f6d 706f 7365 2e79 6d6c 0a64 6f63 6b65  ompose.yml.docke
-00003270: 722d 636f 6d70 6f73 6520 7570 0a60 6060  r-compose up.```
-00003280: 0a0a 3e20 2a2a 4e6f 7465 2a2a 0a3e 2059  ..> **Note**.> Y
-00003290: 6f75 2063 616e 2061 6c73 6f20 6578 706f  ou can also expo
-000032a0: 7274 2044 6570 6c6f 796d 656e 7420 5941  rt Deployment YA
-000032b0: 4d4c 2074 6f20 5b4b 7562 6572 6e65 7465  ML to [Kubernete
-000032c0: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
-000032d0: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-000032e0: 2f65 7865 6375 746f 722f 7365 7276 652f  /executor/serve/
-000032f0: 2373 6572 7665 2d76 6961 2d6b 7562 6572  #serve-via-kuber
-00003300: 6e65 7465 7329 2061 6e64 205b 446f 636b  netes) and [Dock
-00003310: 6572 2043 6f6d 706f 7365 5d28 6874 7470  er Compose](http
-00003320: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-00003330: 2f63 6f6e 6365 7074 732f 6578 6563 7574  /concepts/execut
-00003340: 6f72 2f73 6572 7665 2f23 7365 7276 652d  or/serve/#serve-
-00003350: 7669 612d 646f 636b 6572 2d63 6f6d 706f  via-docker-compo
-00003360: 7365 292e 0a0a 5468 6174 2773 206e 6f74  se)...That's not
-00003370: 2061 6c6c 2e20 5765 2061 6c73 6f20 7375   all. We also su
-00003380: 7070 6f72 7420 5b4f 7065 6e54 656c 656d  pport [OpenTelem
-00003390: 6574 7279 2c20 5072 6f6d 6574 6865 7573  etry, Prometheus
-000033a0: 2c20 616e 6420 4a61 6567 6572 5d28 6874  , and Jaeger](ht
-000033b0: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
-000033c0: 6169 2f63 6c6f 7564 2d6e 6174 6976 656e  ai/cloud-nativen
-000033d0: 6573 732f 6f70 656e 7465 6c65 6d65 7472  ess/opentelemetr
-000033e0: 792f 292e 0a0a 5768 6174 2063 6c6f 7564  y/)...What cloud
-000033f0: 2d6e 6174 6976 6520 7465 6368 6e6f 6c6f  -native technolo
-00003400: 6779 2069 7320 7374 696c 6c20 6368 616c  gy is still chal
-00003410: 6c65 6e67 696e 6720 746f 2079 6f75 3f20  lenging to you? 
-00003420: 5b54 656c 6c20 7573 5d28 6874 7470 733a  [Tell us](https:
-00003430: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6d6f  //github.com/cmo
-00003440: 6e2d 6169 2f63 6d6f 6e2f 6973 7375 6573  n-ai/cmon/issues
-00003450: 2920 616e 6420 7765 276c 6c20 6861 6e64  ) and we'll hand
-00003460: 6c65 2074 6865 2063 6f6d 706c 6578 6974  le the complexit
-00003470: 7920 616e 6420 6d61 6b65 2069 7420 6561  y and make it ea
-00003480: 7379 2066 6f72 2079 6f75 2e0a 0a3c 212d  sy for you...<!-
-00003490: 2d20 7374 6172 7420 7375 7070 6f72 742d  - start support-
-000034a0: 7069 7463 6820 2d2d 3e0a 0a23 2320 5375  pitch -->..## Su
-000034b0: 7070 6f72 740a 0a2d 204a 6f69 6e20 6f75  pport..- Join ou
-000034c0: 7220 5b44 6973 636f 7264 2063 6f6d 6d75  r [Discord commu
-000034d0: 6e69 7479 5d28 6874 7470 733a 2f2f 6469  nity](https://di
-000034e0: 7363 6f72 642e 636d 6f6e 2e61 6929 2061  scord.cmon.ai) a
-000034f0: 6e64 2063 6861 7420 7769 7468 206f 7468  nd chat with oth
-00003500: 6572 2063 6f6d 6d75 6e69 7479 206d 656d  er community mem
-00003510: 6265 7273 2061 626f 7574 2069 6465 6173  bers about ideas
-00003520: 2e0a 2d20 5375 6273 6372 6962 6520 746f  ..- Subscribe to
-00003530: 2074 6865 206c 6174 6573 7420 7669 6465   the latest vide
-00003540: 6f20 7475 746f 7269 616c 7320 6f6e 206f  o tutorials on o
-00003550: 7572 205b 596f 7554 7562 6520 6368 616e  ur [YouTube chan
-00003560: 6e65 6c5d 2868 7474 7073 3a2f 2f79 6f75  nel](https://you
-00003570: 7475 6265 2e63 6f6d 2f63 2f63 6d6f 6e2d  tube.com/c/cmon-
-00003580: 6169 290a 0a23 2320 4a6f 696e 2055 730a  ai)..## Join Us.
-00003590: 0a43 6d6f 6e20 6973 2062 6163 6b65 6420  .Cmon is backed 
-000035a0: 6279 205b 436d 6f6e 2041 495d 2868 7474  by [Cmon AI](htt
-000035b0: 7073 3a2f 2f63 6d6f 6e2e 6169 2920 616e  ps://cmon.ai) an
-000035c0: 6420 6c69 6365 6e73 6564 2075 6e64 6572  d licensed under
-000035d0: 205b 4170 6163 6865 2d32 2e30 5d28 2e2f   [Apache-2.0](./
-000035e0: 4c49 4345 4e53 4529 2e0a 0a3c 212d 2d20  LICENSE)...<!-- 
-000035f0: 656e 6420 7375 7070 6f72 742d 7069 7463  end support-pitc
-00003600: 6820 2d2d 3e0a                           h -->.
+00000010: 223e 0d0a 3c21 2d2d 2073 7572 7665 7920  ">..<!-- survey 
+00000020: 6261 6e6e 6572 2073 7461 7274 202d 2d3e  banner start -->
+00000030: 0d0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000040: 3a2f 2f31 3073 7731 7463 706c 6434 2e74  ://10sw1tcpld4.t
+00000050: 7970 6566 6f72 6d2e 636f 6d2f 746f 2f45  ypeform.com/to/E
+00000060: 4741 4552 654d 373f 7574 6d5f 736f 7572  GAEReM7?utm_sour
+00000070: 6365 3d72 6561 646d 6526 7574 6d5f 6d65  ce=readme&utm_me
+00000080: 6469 756d 3d67 6974 6875 6226 7574 6d5f  dium=github&utm_
+00000090: 6361 6d70 6169 676e 3d75 7365 7225 3230  campaign=user%20
+000000a0: 6578 7065 7269 656e 6365 2675 746d 5f74  experience&utm_t
+000000b0: 6572 6d3d 6665 6232 3032 3326 7574 6d5f  erm=feb2023&utm_
+000000c0: 636f 6e74 656e 743d 7375 7276 6579 223e  content=survey">
+000000d0: 0d0a 2020 3c69 6d67 2073 7263 3d22 2e2f  ..  <img src="./
+000000e0: 2e67 6974 6875 622f 6261 6e6e 6572 2e73  .github/banner.s
+000000f0: 7667 3f72 6177 3d74 7275 6522 3e0d 0a3c  vg?raw=true">..<
+00000100: 2f61 3e0d 0a3c 212d 2d20 7375 7276 6579  /a>..<!-- survey
+00000110: 2062 616e 6e65 7220 7374 6172 7420 2d2d   banner start --
+00000120: 3e0d 0a0d 0a3c 7020 616c 6967 6e3d 2263  >....<p align="c
+00000130: 656e 7465 7222 3e0d 0a3c 6120 6872 6566  enter">..<a href
+00000140: 3d22 6874 7470 733a 2f2f 646f 6373 2e63  ="https://docs.c
+00000150: 6d6f 6e2e 7077 223e 3c69 6d67 2073 7263  mon.pw"><img src
+00000160: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000170: 2e63 6f6d 2f63 6d6f 6e2e 7077 2f63 6d6f  .com/cmon.pw/cmo
+00000180: 6e2f 626c 6f62 2f6d 6173 7465 722f 646f  n/blob/master/do
+00000190: 6373 2f5f 7374 6174 6963 2f6c 6f67 6f2d  cs/_static/logo-
+000001a0: 6c69 6768 742e 7376 673f 7261 773d 7472  light.svg?raw=tr
+000001b0: 7565 2220 616c 743d 2243 6d6f 6e20 6c6f  ue" alt="Cmon lo
+000001c0: 676f 3a20 4275 696c 6420 6d75 6c74 696d  go: Build multim
+000001d0: 6f64 616c 2041 4920 7365 7276 6963 6573  odal AI services
+000001e0: 2076 6961 2063 6c6f 7564 206e 6174 6976   via cloud nativ
+000001f0: 6520 7465 6368 6e6f 6c6f 6769 6573 20c2  e technologies .
+00000200: b720 4e65 7572 616c 2053 6561 7263 6820  . Neural Search 
+00000210: c2b7 2047 656e 6572 6174 6976 6520 4149  .. Generative AI
+00000220: 20c2 b720 436c 6f75 6420 4e61 7469 7665   .. Cloud Native
+00000230: 2220 7769 6474 683d 2231 3530 7078 223e  " width="150px">
+00000240: 3c2f 613e 0d0a 3c2f 703e 0d0a 0d0a 3c70  </a>..</p>....<p
+00000250: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000260: 0d0a 3c62 3e42 7569 6c64 206d 756c 7469  ..<b>Build multi
+00000270: 6d6f 6461 6c20 4149 2073 6572 7669 6365  modal AI service
+00000280: 7320 7769 7468 2063 6c6f 7564 206e 6174  s with cloud nat
+00000290: 6976 6520 7465 6368 6e6f 6c6f 6769 6573  ive technologies
+000002a0: 3c2f 623e 0d0a 3c2f 703e 0d0a 0d0a 3c70  </b>..</p>....<p
+000002b0: 2061 6c69 676e 3d63 656e 7465 723e 0d0a   align=center>..
+000002c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000002d0: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+000002e0: 742f 636d 6f6e 2f22 3e3c 696d 6720 616c  t/cmon/"><img al
+000002f0: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
+00000300: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000310: 732e 696f 2f70 7970 692f 762f 636d 6f6e  s.io/pypi/v/cmon
+00000320: 3f6c 6162 656c 3d52 656c 6561 7365 2673  ?label=Release&s
+00000330: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00000340: 223e 3c2f 613e 0d0a 3c21 2d2d 3c61 2068  "></a>..<!--<a h
+00000350: 7265 663d 2268 7474 7073 3a2f 2f63 6f64  ref="https://cod
+00000360: 6563 6f76 2e69 6f2f 6768 2f63 6d6f 6e2e  ecov.io/gh/cmon.
+00000370: 7077 2f63 6d6f 6e22 3e3c 696d 6720 616c  pw/cmon"><img al
+00000380: 743d 2243 6f64 6563 6f76 2062 7261 6e63  t="Codecov branc
+00000390: 6822 2073 7263 3d22 6874 7470 733a 2f2f  h" src="https://
+000003a0: 696d 672e 7368 6965 6c64 732e 696f 2f63  img.shields.io/c
+000003b0: 6f64 6563 6f76 2f63 2f67 6974 6875 622f  odecov/c/github/
+000003c0: 636d 6f6e 2e70 772f 636d 6f6e 2f6d 6173  cmon.pw/cmon/mas
+000003d0: 7465 723f 266c 6f67 6f3d 436f 6465 636f  ter?&logo=Codeco
+000003e0: 7626 6c6f 676f 436f 6c6f 723d 7768 6974  v&logoColor=whit
+000003f0: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
+00000400: 6172 6522 3e3c 2f61 3e2d 2d3e 0d0a 3c61  are"></a>-->..<a
+00000410: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00000420: 6973 636f 7264 2e63 6d6f 6e2e 7077 223e  iscord.cmon.pw">
+00000430: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000440: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000450: 2f64 6973 636f 7264 2f31 3130 3635 3432  /discord/1106542
+00000460: 3232 3031 3132 3330 3231 3330 3f6c 6f67  220112302130?log
+00000470: 6f3d 6469 7363 6f72 6426 6c6f 676f 436f  o=discord&logoCo
+00000480: 6c6f 723d 7768 6974 6526 7374 796c 653d  lor=white&style=
+00000490: 666c 6174 2d73 7175 6172 6522 3e3c 2f61  flat-square"></a
+000004a0: 3e0d 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
+000004b0: 733a 2f2f 7079 7069 7374 6174 732e 6f72  s://pypistats.or
+000004c0: 672f 7061 636b 6167 6573 2f63 6d6f 6e22  g/packages/cmon"
+000004d0: 3e3c 696d 6720 616c 743d 2250 7950 4920  ><img alt="PyPI 
+000004e0: 2d20 446f 776e 6c6f 6164 7320 6672 6f6d  - Downloads from
+000004f0: 206f 6666 6963 6961 6c20 7079 7069 7374   official pypist
+00000500: 6174 7322 2073 7263 3d22 6874 7470 733a  ats" src="https:
+00000510: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000520: 2f70 7970 692f 646d 2f63 6d6f 6e3f 7374  /pypi/dm/cmon?st
+00000530: 796c 653d 666c 6174 2d73 7175 6172 6522  yle=flat-square"
+00000540: 3e3c 2f61 3e0d 0a3c 6120 6872 6566 3d22  ></a>..<a href="
+00000550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000560: 6f6d 2f63 6d6f 6e2e 7077 2f63 6d6f 6e2f  om/cmon.pw/cmon/
+00000570: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000580: 732f 6364 2e79 6d6c 223e 3c69 6d67 2061  s/cd.yml"><img a
+00000590: 6c74 3d22 4769 7468 7562 2043 4420 7374  lt="Github CD st
+000005a0: 6174 7573 2220 7372 633d 2268 7474 7073  atus" src="https
+000005b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 636d  ://github.com/cm
+000005c0: 6f6e 2e70 772f 636d 6f6e 2f61 6374 696f  on.pw/cmon/actio
+000005d0: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 642e  ns/workflows/cd.
+000005e0: 796d 6c2f 6261 6467 652e 7376 6722 3e3c  yml/badge.svg"><
+000005f0: 2f61 3e0d 0a3c 2f70 3e0d 0a0d 0a3c 212d  /a>..</p>....<!-
+00000600: 2d20 7374 6172 7420 636d 6f6e 2d64 6573  - start cmon-des
+00000610: 6372 6970 7469 6f6e 202d 2d3e 0d0a 0d0a  cription -->....
+00000620: 436d 6f6e 206c 6574 7320 796f 7520 6275  Cmon lets you bu
+00000630: 696c 6420 6d75 6c74 696d 6f64 616c 205b  ild multimodal [
+00000640: 2a2a 4149 2073 6572 7669 6365 732a 2a5d  **AI services**]
+00000650: 2823 6275 696c 642d 6169 2d73 6572 7669  (#build-ai-servi
+00000660: 6365 7329 2061 6e64 205b 2a2a 7069 7065  ces) and [**pipe
+00000670: 6c69 6e65 732a 2a5d 2823 6275 696c 642d  lines**](#build-
+00000680: 612d 7069 7065 6c69 6e65 2920 7468 6174  a-pipeline) that
+00000690: 2063 6f6d 6d75 6e69 6361 7465 2076 6961   communicate via
+000006a0: 2067 5250 432c 2048 5454 5020 616e 6420   gRPC, HTTP and 
+000006b0: 5765 6253 6f63 6b65 7473 2c20 7468 656e  WebSockets, then
+000006c0: 2073 6361 6c65 2074 6865 6d20 7570 2061   scale them up a
+000006d0: 6e64 2064 6570 6c6f 7920 746f 2070 726f  nd deploy to pro
+000006e0: 6475 6374 696f 6e2e 2059 6f75 2063 616e  duction. You can
+000006f0: 2066 6f63 7573 206f 6e20 796f 7572 206c   focus on your l
+00000700: 6f67 6963 2061 6e64 2061 6c67 6f72 6974  ogic and algorit
+00000710: 686d 732c 2077 6974 686f 7574 2077 6f72  hms, without wor
+00000720: 7279 696e 6720 6162 6f75 7420 7468 6520  rying about the 
+00000730: 696e 6672 6173 7472 7563 7475 7265 2063  infrastructure c
+00000740: 6f6d 706c 6578 6974 792e 0d0a 0d0a 215b  omplexity.....![
+00000750: 5d28 2e2f 2e67 6974 6875 622f 696d 6167  ](./.github/imag
+00000760: 6573 2f62 7569 6c64 2d64 6570 6c6f 792e  es/build-deploy.
+00000770: 706e 6729 0d0a 0d0a 436d 6f6e 2070 726f  png)....Cmon pro
+00000780: 7669 6465 7320 6120 736d 6f6f 7468 2050  vides a smooth P
+00000790: 7974 686f 6e69 6320 6578 7065 7269 656e  ythonic experien
+000007a0: 6365 2074 7261 6e73 6974 696f 6e69 6e67  ce transitioning
+000007b0: 2066 726f 6d20 6c6f 6361 6c20 6465 706c   from local depl
+000007c0: 6f79 6d65 6e74 2074 6f20 6164 7661 6e63  oyment to advanc
+000007d0: 6564 206f 7263 6865 7374 7261 7469 6f6e  ed orchestration
+000007e0: 2066 7261 6d65 776f 726b 7320 6c69 6b65   frameworks like
+000007f0: 2044 6f63 6b65 722d 436f 6d70 6f73 652c   Docker-Compose,
+00000800: 204b 7562 6572 6e65 7465 732c 206f 7220   Kubernetes, or 
+00000810: 436d 6f6e 2041 4920 436c 6f75 642e 2043  Cmon AI Cloud. C
+00000820: 6d6f 6e20 6d61 6b65 7320 6164 7661 6e63  mon makes advanc
+00000830: 6564 2073 6f6c 7574 696f 6e20 656e 6769  ed solution engi
+00000840: 6e65 6572 696e 6720 616e 6420 636c 6f75  neering and clou
+00000850: 642d 6e61 7469 7665 2074 6563 686e 6f6c  d-native technol
+00000860: 6f67 6965 7320 6163 6365 7373 6962 6c65  ogies accessible
+00000870: 2074 6f20 6576 6572 7920 6465 7665 6c6f   to every develo
+00000880: 7065 722e 0d0a 0d0a 2d20 4275 696c 6420  per.....- Build 
+00000890: 6170 706c 6963 6174 696f 6e73 2066 6f72  applications for
+000008a0: 2061 6e79 205b 6461 7461 2074 7970 655d   any [data type]
+000008b0: 2868 7474 7073 3a2f 2f64 6f63 732e 646f  (https://docs.do
+000008c0: 6361 7272 6179 2e6f 7267 2f64 6174 615f  carray.org/data_
+000008d0: 7479 7065 732f 6669 7273 745f 7374 6570  types/first_step
+000008e0: 732f 292c 2061 6e79 206d 6169 6e73 7472  s/), any mainstr
+000008f0: 6561 6d20 5b64 6565 7020 6c65 6172 6e69  eam [deep learni
+00000900: 6e67 2066 7261 6d65 776f 726b 5d28 292c  ng framework](),
+00000910: 2061 6e64 2061 6e79 205b 7072 6f74 6f63   and any [protoc
+00000920: 6f6c 5d28 6874 7470 733a 2f2f 646f 6373  ol](https://docs
+00000930: 2e63 6d6f 6e2e 7077 2f63 6f6e 6365 7074  .cmon.pw/concept
+00000940: 732f 7365 7276 696e 672f 6761 7465 7761  s/serving/gatewa
+00000950: 792f 2373 6574 2d70 726f 746f 636f 6c2d  y/#set-protocol-
+00000960: 696e 2d70 7974 686f 6e29 2e0d 0a2d 2044  in-python)...- D
+00000970: 6573 6967 6e20 6869 6768 2d70 6572 666f  esign high-perfo
+00000980: 726d 616e 6365 206d 6963 726f 7365 7276  rmance microserv
+00000990: 6963 6573 2c20 7769 7468 205b 6561 7379  ices, with [easy
+000009a0: 2073 6361 6c69 6e67 5d28 6874 7470 733a   scaling](https:
+000009b0: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+000009c0: 6f6e 6365 7074 732f 6f72 6368 6573 7472  oncepts/orchestr
+000009d0: 6174 696f 6e2f 7363 616c 652d 6f75 742f  ation/scale-out/
+000009e0: 292c 2064 7570 6c65 7820 636c 6965 6e74  ), duplex client
+000009f0: 2d73 6572 7665 7220 7374 7265 616d 696e  -server streamin
+00000a00: 672c 2061 6e64 2061 7379 6e63 2f6e 6f6e  g, and async/non
+00000a10: 2d62 6c6f 636b 696e 6720 6461 7461 2070  -blocking data p
+00000a20: 726f 6365 7373 696e 6720 6f76 6572 2064  rocessing over d
+00000a30: 796e 616d 6963 2066 6c6f 7773 2e0d 0a2d  ynamic flows...-
+00000a40: 2044 6f63 6b65 7220 636f 6e74 6169 6e65   Docker containe
+00000a50: 7220 696e 7465 6772 6174 696f 6e20 7669  r integration vi
+00000a60: 6120 5b45 7865 6375 746f 7220 4875 625d  a [Executor Hub]
+00000a70: 2868 7474 7073 3a2f 2f63 6c6f 7564 2e63  (https://cloud.c
+00000a80: 6d6f 6e2e 7077 292c 204f 7065 6e54 656c  mon.pw), OpenTel
+00000a90: 656d 6574 7279 2f50 726f 6d65 7468 6575  emetry/Prometheu
+00000aa0: 7320 6f62 7365 7276 6162 696c 6974 792c  s observability,
+00000ab0: 2061 6e64 2066 6173 7420 4b75 6265 726e   and fast Kubern
+00000ac0: 6574 6573 2f44 6f63 6b65 722d 436f 6d70  etes/Docker-Comp
+00000ad0: 6f73 6520 6465 706c 6f79 6d65 6e74 2e0d  ose deployment..
+00000ae0: 0a2d 2043 5055 2f47 5055 2068 6f73 7469  .- CPU/GPU hosti
+00000af0: 6e67 2076 6961 205b 436d 6f6e 2041 4920  ng via [Cmon AI 
+00000b00: 436c 6f75 645d 2868 7474 7073 3a2f 2f63  Cloud](https://c
+00000b10: 6c6f 7564 2e63 6d6f 6e2e 7077 292e 0d0a  loud.cmon.pw)...
+00000b20: 0d0a 3c64 6574 6169 6c73 3e0d 0a20 2020  ..<details>..   
+00000b30: 203c 7375 6d6d 6172 793e 3c73 7472 6f6e   <summary><stron
+00000b40: 673e 5761 6974 2c20 686f 7720 6973 2043  g>Wait, how is C
+00000b50: 6d6f 6e20 6469 6666 6572 656e 7420 6672  mon different fr
+00000b60: 6f6d 2046 6173 7441 5049 3f3c 2f73 7472  om FastAPI?</str
+00000b70: 6f6e 673e 3c2f 7375 6d6d 6172 793e 0d0a  ong></summary>..
+00000b80: 436d 6f6e 2773 2076 616c 7565 2070 726f  Cmon's value pro
+00000b90: 706f 7369 7469 6f6e 206d 6179 2073 6565  position may see
+00000ba0: 6d20 7175 6974 6520 7369 6d69 6c61 7220  m quite similar 
+00000bb0: 746f 2074 6861 7420 6f66 2046 6173 7441  to that of FastA
+00000bc0: 5049 2e20 486f 7765 7665 722c 2074 6865  PI. However, the
+00000bd0: 7265 2061 7265 2073 6576 6572 616c 2066  re are several f
+00000be0: 756e 6461 6d65 6e74 616c 2064 6966 6665  undamental diffe
+00000bf0: 7265 6e63 6573 3a0d 0a0d 0a20 2a2a 4461  rences:.... **Da
+00000c00: 7461 2073 7472 7563 7475 7265 2061 6e64  ta structure and
+00000c10: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2070   communication p
+00000c20: 726f 746f 636f 6c73 2a2a 0d0a 2020 2d20  rotocols**..  - 
+00000c30: 4661 7374 4150 4920 636f 6d6d 756e 6963  FastAPI communic
+00000c40: 6174 696f 6e20 7265 6c69 6573 206f 6e20  ation relies on 
+00000c50: 5079 6461 6e74 6963 2061 6e64 2043 6d6f  Pydantic and Cmo
+00000c60: 6e20 7265 6c69 6573 206f 6e20 5b64 6f63  n relies on [doc
+00000c70: 6172 7261 795d 2868 7474 7073 3a2f 2f67  array](https://g
+00000c80: 6974 6875 622e 636f 6d2f 646f 6361 7272  ithub.com/docarr
+00000c90: 6179 2f64 6f63 6172 7261 7929 2061 6c6c  ay/docarray) all
+00000ca0: 6f77 696e 6720 436d 6f6e 2074 6f20 7375  owing Cmon to su
+00000cb0: 7070 6f72 7420 6d75 6c74 6970 6c65 2070  pport multiple p
+00000cc0: 726f 746f 636f 6c73 0d0a 2020 746f 2065  rotocols..  to e
+00000cd0: 7870 6f73 6520 6974 7320 7365 7276 6963  xpose its servic
+00000ce0: 6573 2e0d 0a0d 0a20 2a2a 4164 7661 6e63  es..... **Advanc
+00000cf0: 6564 206f 7263 6865 7374 7261 7469 6f6e  ed orchestration
+00000d00: 2061 6e64 2073 6361 6c69 6e67 2063 6170   and scaling cap
+00000d10: 6162 696c 6974 6965 732a 2a0d 0a20 202d  abilities**..  -
+00000d20: 2043 6d6f 6e20 6c65 7473 2079 6f75 2064   Cmon lets you d
+00000d30: 6570 6c6f 7920 6170 706c 6963 6174 696f  eploy applicatio
+00000d40: 6e73 2066 6f72 6d65 6420 6672 6f6d 206d  ns formed from m
+00000d50: 756c 7469 706c 6520 6d69 6372 6f73 6572  ultiple microser
+00000d60: 7669 6365 7320 7468 6174 2063 616e 2062  vices that can b
+00000d70: 6520 636f 6e74 6169 6e65 7269 7a65 6420  e containerized 
+00000d80: 616e 6420 7363 616c 6564 2069 6e64 6570  and scaled indep
+00000d90: 656e 6465 6e74 6c79 2e0d 0a20 202d 2043  endently...  - C
+00000da0: 6d6f 6e20 616c 6c6f 7773 2079 6f75 2074  mon allows you t
+00000db0: 6f20 6561 7369 6c79 2063 6f6e 7461 696e  o easily contain
+00000dc0: 6572 697a 6520 616e 6420 6f72 6368 6573  erize and orches
+00000dd0: 7472 6174 6520 796f 7572 2073 6572 7669  trate your servi
+00000de0: 6365 732c 2070 726f 7669 6469 6e67 2063  ces, providing c
+00000df0: 6f6e 6375 7272 656e 6379 2061 6e64 2073  oncurrency and s
+00000e00: 6361 6c61 6269 6c69 7479 2e0d 0a0d 0a20  calability..... 
+00000e10: 2a2a 4a6f 7572 6e65 7920 746f 2074 6865  **Journey to the
+00000e20: 2063 6c6f 7564 2a2a 0d0a 2020 2d20 436d   cloud**..  - Cm
+00000e30: 6f6e 2070 726f 7669 6465 7320 6120 736d  on provides a sm
+00000e40: 6f6f 7468 2074 7261 6e73 6974 696f 6e20  ooth transition 
+00000e50: 6672 6f6d 206c 6f63 616c 2064 6576 656c  from local devel
+00000e60: 6f70 6d65 6e74 2028 7573 696e 6720 5b64  opment (using [d
+00000e70: 6f63 6172 7261 795d 2868 7474 7073 3a2f  ocarray](https:/
+00000e80: 2f67 6974 6875 622e 636f 6d2f 646f 6361  /github.com/doca
+00000e90: 7272 6179 2f64 6f63 6172 7261 7929 2920  rray/docarray)) 
+00000ea0: 746f 206c 6f63 616c 2073 6572 7669 6e67  to local serving
+00000eb0: 2075 7369 6e67 2028 436d 6f6e 2773 206f   using (Cmon's o
+00000ec0: 7263 6865 7374 7261 7469 6f6e 206c 6179  rchestration lay
+00000ed0: 6572 290d 0a20 2074 6f20 6861 7669 6e67  er)..  to having
+00000ee0: 2070 726f 6475 6374 696f 6e2d 7265 6164   production-read
+00000ef0: 7920 7365 7276 6963 6573 2062 7920 7573  y services by us
+00000f00: 696e 6720 4b75 6265 726e 6574 6573 2063  ing Kubernetes c
+00000f10: 6170 6163 6974 7920 746f 206f 7263 6865  apacity to orche
+00000f20: 7374 7261 7465 2074 6865 206c 6966 6574  strate the lifet
+00000f30: 696d 6520 6f66 2063 6f6e 7461 696e 6572  ime of container
+00000f40: 732e 0d0a 2020 2d20 4279 2075 7369 6e67  s...  - By using
+00000f50: 205b 436d 6f6e 2041 4920 436c 6f75 645d   [Cmon AI Cloud]
+00000f60: 2868 7474 7073 3a2f 2f63 6c6f 7564 2e63  (https://cloud.c
+00000f70: 6d6f 6e2e 7077 2920 796f 7520 6861 7665  mon.pw) you have
+00000f80: 2061 6363 6573 7320 746f 2073 6361 6c61   access to scala
+00000f90: 626c 6520 616e 6420 7365 7276 6572 6c65  ble and serverle
+00000fa0: 7373 2064 6570 6c6f 796d 656e 7473 206f  ss deployments o
+00000fb0: 6620 796f 7572 2061 7070 6c69 6361 7469  f your applicati
+00000fc0: 6f6e 7320 696e 206f 6e65 2063 6f6d 6d61  ons in one comma
+00000fd0: 6e64 2e0d 0a3c 2f64 6574 6169 6c73 3e0d  nd...</details>.
+00000fe0: 0a0d 0a3c 212d 2d20 656e 6420 636d 6f6e  ...<!-- end cmon
+00000ff0: 2d64 6573 6372 6970 7469 6f6e 202d 2d3e  -description -->
+00001000: 0d0a 0d0a 2323 205b 446f 6375 6d65 6e74  ....## [Document
+00001010: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
+00001020: 6f63 732e 636d 6f6e 2e70 7729 0d0a 0d0a  ocs.cmon.pw)....
+00001030: 2323 2049 6e73 7461 6c6c 200d 0a0d 0a4e  ## Install ....N
+00001040: 6f74 653a 2028 5769 6e64 6f77 7329 206e  ote: (Windows) n
+00001050: 6f74 2073 7570 706f 7274 6564 2061 7420  ot supported at 
+00001060: 7468 6973 206d 6f6d 656e 7421 2059 6f75  this moment! You
+00001070: 206d 6179 2072 6571 7569 7265 2074 6f20   may require to 
+00001080: 696e 7374 616c 6c20 6974 206f 6e20 2857  install it on (W
+00001090: 534c 292e 0d0a 5b20 2055 5044 4154 4520  SL)...[  UPDATE 
+000010a0: 205d 203a 2057 696e 646f 7773 2053 7570   ] : Windows Sup
+000010b0: 706f 7274 2061 6464 6564 210d 0a0d 0a60  port added!....`
+000010c0: 6060 6261 7368 0d0a 7069 7020 696e 7374  ``bash..pip inst
+000010d0: 616c 6c20 636d 6f6e 2d61 690d 0a60 6060  all cmon-ai..```
+000010e0: 0d0a 0d0a 4669 6e64 206d 6f72 6520 696e  ....Find more in
+000010f0: 7374 616c 6c20 6f70 7469 6f6e 7320 6f6e  stall options on
+00001100: 205b 4170 706c 6520 5369 6c69 636f 6e5d   [Apple Silicon]
+00001110: 2868 7474 7073 3a2f 2f64 6f63 732e 636d  (https://docs.cm
+00001120: 6f6e 2e70 772f 6765 742d 7374 6172 7465  on.pw/get-starte
+00001130: 642f 696e 7374 616c 6c2f 6170 706c 652d  d/install/apple-
+00001140: 7369 6c69 636f 6e2d 6d31 2d6d 322f 290d  silicon-m1-m2/).
+00001150: 0a0d 0a0d 0a23 2320 4765 7420 5374 6172  .....## Get Star
+00001160: 7465 640d 0a0d 0a23 2323 2042 6173 6963  ted....### Basic
+00001170: 2043 6f6e 6365 7074 730d 0a0d 0a43 6d6f   Concepts....Cmo
+00001180: 6e20 6861 7320 666f 7572 2066 756e 6461  n has four funda
+00001190: 6d65 6e74 616c 2063 6f6e 6365 7074 733a  mental concepts:
+000011a0: 0d0a 0d0a 2d20 4120 5b2a 2a44 6f63 756d  ....- A [**Docum
+000011b0: 656e 742a 2a5d 2868 7474 7073 3a2f 2f64  ent**](https://d
+000011c0: 6f63 6172 7261 792e 636d 6f6e 2e70 772f  ocarray.cmon.pw/
+000011d0: 2920 2866 726f 6d20 5b64 6f63 6172 7261  ) (from [docarra
+000011e0: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
+000011f0: 622e 636f 6d2f 646f 6361 7272 6179 2f64  b.com/docarray/d
+00001200: 6f63 6172 7261 7929 2920 6973 2074 6865  ocarray)) is the
+00001210: 2069 6e70 7574 2f6f 7574 7075 7420 666f   input/output fo
+00001220: 726d 6174 2069 6e20 436d 6f6e 2e0d 0a2d  rmat in Cmon...-
+00001230: 2041 6e20 5b2a 2a45 7865 6375 746f 722a   An [**Executor*
+00001240: 2a5d 2868 7474 7073 3a2f 2f64 6f63 732e  *](https://docs.
+00001250: 636d 6f6e 2e70 772f 636f 6e63 6570 7473  cmon.pw/concepts
+00001260: 2f73 6572 7669 6e67 2f65 7865 6375 746f  /serving/executo
+00001270: 722f 2920 6973 2061 2050 7974 686f 6e20  r/) is a Python 
+00001280: 636c 6173 7320 7468 6174 2074 7261 6e73  class that trans
+00001290: 666f 726d 7320 616e 6420 7072 6f63 6573  forms and proces
+000012a0: 7365 7320 446f 6375 6d65 6e74 732e 0d0a  ses Documents...
+000012b0: 2d20 4120 5b2a 2a44 6570 6c6f 796d 656e  - A [**Deploymen
+000012c0: 742a 2a5d 2868 7474 7073 3a2f 2f64 6f63  t**](https://doc
+000012d0: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+000012e0: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
+000012f0: 2f64 6570 6c6f 796d 656e 7429 2073 6572  /deployment) ser
+00001300: 7665 7320 6120 7369 6e67 6c65 2045 7865  ves a single Exe
+00001310: 6375 746f 722c 2077 6869 6c65 2061 205b  cutor, while a [
+00001320: 2a2a 466c 6f77 2a2a 5d28 6874 7470 733a  **Flow**](https:
+00001330: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+00001340: 6f6e 6365 7074 732f 6f72 6368 6573 7472  oncepts/orchestr
+00001350: 6174 696f 6e2f 666c 6f77 2f29 2073 6572  ation/flow/) ser
+00001360: 7665 7320 4578 6563 7574 6f72 7320 6368  ves Executors ch
+00001370: 6169 6e65 6420 696e 746f 2061 2070 6970  ained into a pip
+00001380: 656c 696e 652e 0d0a 0d0a 0d0a 5b54 6865  eline.......[The
+00001390: 2066 756c 6c20 676c 6f73 7361 7279 2069   full glossary i
+000013a0: 7320 6578 706c 6169 6e65 6420 6865 7265  s explained here
+000013b0: 5d28 6874 7470 733a 2f2f 646f 6373 2e63  ](https://docs.c
+000013c0: 6d6f 6e2e 7077 2f63 6f6e 6365 7074 732f  mon.pw/concepts/
+000013d0: 7072 656c 696d 696e 6172 6965 732f 2329  preliminaries/#)
+000013e0: 2e0d 0a0d 0a23 2323 2042 7569 6c64 2041  .....### Build A
+000013f0: 4920 5365 7276 6963 6573 0d0a 3c21 2d2d  I Services..<!--
+00001400: 2073 7461 7274 2062 7569 6c64 2d61 692d   start build-ai-
+00001410: 7365 7276 6963 6573 202d 2d3e 0d0a 0d0a  services -->....
+00001420: 4c65 7427 7320 6275 696c 6420 6120 6661  Let's build a fa
+00001430: 7374 2c20 7265 6c69 6162 6c65 2061 6e64  st, reliable and
+00001440: 2073 6361 6c61 626c 6520 6752 5043 2d62   scalable gRPC-b
+00001450: 6173 6564 2041 4920 7365 7276 6963 652e  ased AI service.
+00001460: 2049 6e20 436d 6f6e 2077 6520 6361 6c6c   In Cmon we call
+00001470: 2074 6869 7320 616e 202a 2a5b 4578 6563   this an **[Exec
+00001480: 7574 6f72 5d28 6874 7470 733a 2f2f 646f  utor](https://do
+00001490: 6373 2e63 6d6f 6e2e 7077 2f63 6f6e 6365  cs.cmon.pw/conce
+000014a0: 7074 732f 6578 6563 7574 6f72 2f29 2a2a  pts/executor/)**
+000014b0: 2e20 4f75 7220 7369 6d70 6c65 2045 7865  . Our simple Exe
+000014c0: 6375 746f 7220 7769 6c6c 2077 7261 7020  cutor will wrap 
+000014d0: 7468 6520 5b53 7461 626c 654c 4d5d 2868  the [StableLM](h
+000014e0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+000014f0: 6365 2e63 6f2f 7374 6162 696c 6974 7961  ce.co/stabilitya
+00001500: 692f 7374 6162 6c65 6c6d 2d62 6173 652d  i/stablelm-base-
+00001510: 616c 7068 612d 3362 2920 4c4c 4d20 6672  alpha-3b) LLM fr
+00001520: 6f6d 2053 7461 6269 6c69 7479 2041 492e  om Stability AI.
+00001530: 2057 6527 6c6c 2074 6865 6e20 7573 6520   We'll then use 
+00001540: 6120 2a2a 4465 706c 6f79 6d65 6e74 2a2a  a **Deployment**
+00001550: 2074 6f20 7365 7276 6520 6974 2e0d 0a0d   to serve it....
+00001560: 0a21 5b5d 282e 2f2e 6769 7468 7562 2f69  .![](./.github/i
+00001570: 6d61 6765 732f 6465 706c 6f79 6d65 6e74  mages/deployment
+00001580: 2d64 6961 6772 616d 2e70 6e67 290d 0a0d  -diagram.png)...
+00001590: 0a3e 202a 2a4e 6f74 652a 2a0d 0a3e 2041  .> **Note**..> A
+000015a0: 2044 6570 6c6f 796d 656e 7420 7365 7276   Deployment serv
+000015b0: 6573 206a 7573 7420 6f6e 6520 4578 6563  es just one Exec
+000015c0: 7574 6f72 2e20 546f 2063 6f6d 6269 6e65  utor. To combine
+000015d0: 206d 756c 7469 706c 6520 4578 6563 7574   multiple Execut
+000015e0: 6f72 7320 696e 746f 2061 2070 6970 656c  ors into a pipel
+000015f0: 696e 6520 616e 6420 7365 7276 6520 7468  ine and serve th
+00001600: 6174 2c20 7573 6520 6120 5b46 6c6f 775d  at, use a [Flow]
+00001610: 2823 6275 696c 642d 612d 7069 7065 6c69  (#build-a-pipeli
+00001620: 6e65 292e 0d0a 0d0a 4c65 7427 7320 696d  ne).....Let's im
+00001630: 706c 656d 656e 7420 7468 6520 7365 7276  plement the serv
+00001640: 6963 6527 7320 6c6f 6769 633a 0d0a 0d0a  ice's logic:....
+00001650: 3c74 6162 6c65 3e0d 0a3c 7472 3e0d 0a3c  <table>..<tr>..<
+00001660: 7468 3e3c 636f 6465 3e65 7865 6375 746f  th><code>executo
+00001670: 722e 7079 3c2f 636f 6465 3e3c 2f74 683e  r.py</code></th>
+00001680: 200d 0a3c 7472 3e0d 0a3c 7464 3e0d 0a0d   ..<tr>..<td>...
+00001690: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+000016a0: 2063 6d6f 6e20 696d 706f 7274 2045 7865   cmon import Exe
+000016b0: 6375 746f 722c 2072 6571 7565 7374 730d  cutor, requests.
+000016c0: 0a66 726f 6d20 646f 6361 7272 6179 2069  .from docarray i
+000016d0: 6d70 6f72 7420 446f 6375 6d65 6e74 4172  mport DocumentAr
+000016e0: 7261 790d 0a0d 0a66 726f 6d20 7472 616e  ray....from tran
+000016f0: 7366 6f72 6d65 7273 2069 6d70 6f72 7420  sformers import 
+00001700: 7069 7065 6c69 6e65 0d0a 0d0a 0d0a 636c  pipeline......cl
+00001710: 6173 7320 5374 6162 6c65 4c4d 2845 7865  ass StableLM(Exe
+00001720: 6375 746f 7229 3a0d 0a0d 0a20 2020 2064  cutor):....    d
+00001730: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00001740: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+00001750: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00001760: 696e 6974 5f5f 282a 2a6b 7761 7267 7329  init__(**kwargs)
+00001770: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00001780: 656e 6572 6174 6f72 203d 2070 6970 656c  enerator = pipel
+00001790: 696e 6528 2774 6578 742d 6765 6e65 7261  ine('text-genera
+000017a0: 7469 6f6e 272c 206d 6f64 656c 3d27 7374  tion', model='st
+000017b0: 6162 6c65 6c6d 2d33 6227 290d 0a0d 0a20  ablelm-3b').... 
+000017c0: 2020 2040 7265 7175 6573 7473 0d0a 2020     @requests..  
+000017d0: 2020 6465 6620 6765 6e65 7261 7465 2873    def generate(s
+000017e0: 656c 662c 2064 6f63 733a 2044 6f63 756d  elf, docs: Docum
+000017f0: 656e 7441 7272 6179 2c20 2a2a 6b77 6172  entArray, **kwar
+00001800: 6773 293a 0d0a 2020 2020 2020 2020 6765  gs):..        ge
+00001810: 6e65 7261 7465 645f 7465 7874 203d 2073  nerated_text = s
+00001820: 656c 662e 6765 6e65 7261 746f 7228 646f  elf.generator(do
+00001830: 6373 2e74 6578 7473 290d 0a20 2020 2020  cs.texts)..     
+00001840: 2020 2064 6f63 732e 7465 7874 7320 3d20     docs.texts = 
+00001850: 5b67 656e 5b30 5d5b 2767 656e 6572 6174  [gen[0]['generat
+00001860: 6564 5f74 6578 7427 5d20 666f 7220 6765  ed_text'] for ge
+00001870: 6e20 696e 2067 656e 6572 6174 6564 5f74  n in generated_t
+00001880: 6578 745d 0d0a 6060 600d 0a0d 0a3c 2f74  ext]..```....</t
+00001890: 643e 0d0a 3c2f 7472 3e0d 0a3c 2f74 6162  d>..</tr>..</tab
+000018a0: 6c65 3e0d 0a0d 0a54 6865 6e20 7765 2064  le>....Then we d
+000018b0: 6570 6c6f 7920 6974 2077 6974 6820 6569  eploy it with ei
+000018c0: 7468 6572 2074 6865 2050 7974 686f 6e20  ther the Python 
+000018d0: 4150 4920 6f72 2059 414d 4c3a 0d0a 3c64  API or YAML:..<d
+000018e0: 6976 2063 6c61 7373 3d22 7461 626c 652d  iv class="table-
+000018f0: 7772 6170 7065 7222 3e0d 0a3c 7461 626c  wrapper">..<tabl
+00001900: 653e 0d0a 3c74 723e 0d0a 3c74 683e 2050  e>..<tr>..<th> P
+00001910: 7974 686f 6e20 4150 493a 203c 636f 6465  ython API: <code
+00001920: 3e64 6570 6c6f 796d 656e 742e 7079 3c2f  >deployment.py</
+00001930: 636f 6465 3e20 3c2f 7468 3e20 0d0a 3c74  code> </th> ..<t
+00001940: 683e 2059 414d 4c3a 203c 636f 6465 3e64  h> YAML: <code>d
+00001950: 6570 6c6f 796d 656e 742e 796d 6c3c 2f63  eployment.yml</c
+00001960: 6f64 653e 203c 2f74 683e 0d0a 3c2f 7472  ode> </th>..</tr
+00001970: 3e0d 0a3c 7472 3e0d 0a3c 7464 3e0d 0a0d  >..<tr>..<td>...
+00001980: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00001990: 2063 6d6f 6e20 696d 706f 7274 2044 6570   cmon import Dep
+000019a0: 6c6f 796d 656e 740d 0a66 726f 6d20 6578  loyment..from ex
+000019b0: 6563 7574 6f72 2069 6d70 6f72 7420 5374  ecutor import St
+000019c0: 6162 6c65 4c4d 0d0a 0d0a 6465 7020 3d20  ableLM....dep = 
+000019d0: 4465 706c 6f79 6d65 6e74 2875 7365 733d  Deployment(uses=
+000019e0: 5374 6162 6c65 4c4d 2c20 7469 6d65 6f75  StableLM, timeou
+000019f0: 745f 7265 6164 793d 2d31 2c20 706f 7274  t_ready=-1, port
+00001a00: 3d31 3233 3435 290d 0a0d 0a77 6974 6820  =12345)....with 
+00001a10: 6465 703a 0d0a 2020 2020 6465 702e 626c  dep:..    dep.bl
+00001a20: 6f63 6b28 290d 0a60 6060 0d0a 0d0a 3c2f  ock()..```....</
+00001a30: 7464 3e0d 0a3c 7464 3e0d 0a0d 0a60 6060  td>..<td>....```
+00001a40: 7961 6d6c 0d0a 6a74 7970 653a 2044 6570  yaml..jtype: Dep
+00001a50: 6c6f 796d 656e 740d 0a77 6974 683a 0d0a  loyment..with:..
+00001a60: 2020 7573 6573 3a20 5374 6162 6c65 4c4d    uses: StableLM
+00001a70: 0d0a 2020 7079 5f6d 6f64 756c 6573 3a0d  ..  py_modules:.
+00001a80: 0a20 2020 202d 2065 7865 6375 746f 722e  .    - executor.
+00001a90: 7079 0d0a 2020 7469 6d65 6f75 745f 7265  py..  timeout_re
+00001aa0: 6164 793a 202d 310d 0a20 2070 6f72 743a  ady: -1..  port:
+00001ab0: 2031 3233 3435 0d0a 6060 600d 0a0d 0a41   12345..```....A
+00001ac0: 6e64 2072 756e 2074 6865 2059 414d 4c20  nd run the YAML 
+00001ad0: 4465 706c 6f79 6d65 6e74 2077 6974 6820  Deployment with 
+00001ae0: 7468 6520 434c 493a 2060 636d 6f6e 2064  the CLI: `cmon d
+00001af0: 6570 6c6f 796d 656e 7420 2d2d 7573 6573  eployment --uses
+00001b00: 2064 6570 6c6f 796d 656e 742e 796d 6c60   deployment.yml`
+00001b10: 0d0a 0d0a 3c2f 7464 3e0d 0a3c 2f74 723e  ....</td>..</tr>
+00001b20: 0d0a 3c2f 7461 626c 653e 0d0a 3c2f 6469  ..</table>..</di
+00001b30: 763e 0d0a 0d0a 5573 6520 5b43 6d6f 6e20  v>....Use [Cmon 
+00001b40: 436c 6965 6e74 5d28 6874 7470 733a 2f2f  Client](https://
+00001b50: 646f 6373 2e63 6d6f 6e2e 7077 2f63 6f6e  docs.cmon.pw/con
+00001b60: 6365 7074 732f 636c 6965 6e74 2f29 2074  cepts/client/) t
+00001b70: 6f20 6d61 6b65 2072 6571 7565 7374 7320  o make requests 
+00001b80: 746f 2074 6865 2073 6572 7669 6365 3a0d  to the service:.
+00001b90: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
+00001ba0: 6f6d 2064 6f63 6172 7261 7920 696d 706f  om docarray impo
+00001bb0: 7274 2044 6f63 756d 656e 740d 0a66 726f  rt Document..fro
+00001bc0: 6d20 636d 6f6e 2069 6d70 6f72 7420 436c  m cmon import Cl
+00001bd0: 6965 6e74 0d0a 0d0a 7072 6f6d 7074 203d  ient....prompt =
+00001be0: 2044 6f63 756d 656e 7428 0d0a 2020 2020   Document(..    
+00001bf0: 7461 6773 203d 207b 2770 726f 6d70 7427  tags = {'prompt'
+00001c00: 3a20 2773 7567 6765 7374 2061 6e20 696e  : 'suggest an in
+00001c10: 7465 7265 7374 696e 6720 696d 6167 6520  teresting image 
+00001c20: 6765 6e65 7261 7469 6f6e 2070 726f 6d70  generation promp
+00001c30: 7420 666f 7220 6120 6d6f 6e61 206c 6973  t for a mona lis
+00001c40: 6120 7661 7269 616e 7427 7d0d 0a29 0d0a  a variant'}..)..
+00001c50: 0d0a 636c 6965 6e74 203d 2043 6c69 656e  ..client = Clien
+00001c60: 7428 706f 7274 3d31 3233 3435 2920 2023  t(port=12345)  #
+00001c70: 2075 7365 2070 6f72 7420 6672 6f6d 206f   use port from o
+00001c80: 7574 7075 7420 6162 6f76 650d 0a72 6573  utput above..res
+00001c90: 706f 6e73 6520 3d20 636c 6965 6e74 2e70  ponse = client.p
+00001ca0: 6f73 7428 6f6e 3d27 2f27 2c20 696e 7075  ost(on='/', inpu
+00001cb0: 7473 3d5b 7072 6f6d 7074 5d29 0d0a 0d0a  ts=[prompt])....
+00001cc0: 7072 696e 7428 7265 7370 6f6e 7365 5b30  print(response[0
+00001cd0: 5d2e 7465 7874 290d 0a60 6060 0d0a 0d0a  ].text)..```....
+00001ce0: 6060 6074 6578 740d 0a61 2073 7465 616d  ```text..a steam
+00001cf0: 7075 6e6b 2076 6572 7369 6f6e 206f 6620  punk version of 
+00001d00: 7468 6520 4d6f 6e61 204c 6973 612c 2069  the Mona Lisa, i
+00001d10: 6e63 6f72 706f 7261 7469 6e67 206d 6563  ncorporating mec
+00001d20: 6861 6e69 6361 6c20 6765 6172 732c 2062  hanical gears, b
+00001d30: 7261 7373 2065 6c65 6d65 6e74 732c 2061  rass elements, a
+00001d40: 6e64 2056 6963 746f 7269 616e 2065 7261  nd Victorian era
+00001d50: 2063 6c6f 7468 696e 6720 6465 7461 696c   clothing detail
+00001d60: 730d 0a60 6060 0d0a 0d0a 3c21 2d2d 2065  s..```....<!-- e
+00001d70: 6e64 2062 7569 6c64 2d61 692d 7365 7276  nd build-ai-serv
+00001d80: 6963 6573 202d 2d3e 0d0a 0d0a 3e20 2a2a  ices -->....> **
+00001d90: 4e6f 7465 2a2a 0d0a 3e20 496e 2061 206e  Note**..> In a n
+00001da0: 6f74 6562 6f6f 6b2c 2079 6f75 2063 616e  otebook, you can
+00001db0: 2774 2075 7365 2060 6465 706c 6f79 6d65  't use `deployme
+00001dc0: 6e74 2e62 6c6f 636b 2829 6020 616e 6420  nt.block()` and 
+00001dd0: 7468 656e 206d 616b 6520 7265 7175 6573  then make reques
+00001de0: 7473 2074 6f20 7468 6520 636c 6965 6e74  ts to the client
+00001df0: 2e20 506c 6561 7365 2072 6566 6572 2074  . Please refer t
+00001e00: 6f20 7468 6520 436f 6c61 6220 6c69 6e6b  o the Colab link
+00001e10: 2061 626f 7665 2066 6f72 2072 6570 726f   above for repro
+00001e20: 6475 6369 626c 6520 4a75 7079 7465 7220  ducible Jupyter 
+00001e30: 4e6f 7465 626f 6f6b 2063 6f64 6520 736e  Notebook code sn
+00001e40: 6970 7065 7473 2e0d 0a0d 0a23 2323 2042  ippets.....### B
+00001e50: 7569 6c64 2061 2070 6970 656c 696e 650d  uild a pipeline.
+00001e60: 0a0d 0a3c 212d 2d20 7374 6172 7420 6275  ...<!-- start bu
+00001e70: 696c 642d 7069 7065 6c69 6e65 7320 2d2d  ild-pipelines --
+00001e80: 3e0d 0a0d 0a53 6f6d 6574 696d 6573 2079  >....Sometimes y
+00001e90: 6f75 2077 616e 7420 746f 2063 6861 696e  ou want to chain
+00001ea0: 206d 6963 726f 7365 7276 6963 6573 2074   microservices t
+00001eb0: 6f67 6574 6865 7220 696e 746f 2061 2070  ogether into a p
+00001ec0: 6970 656c 696e 652e 2054 6861 7427 7320  ipeline. That's 
+00001ed0: 7768 6572 6520 6120 5b46 6c6f 775d 2868  where a [Flow](h
+00001ee0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
+00001ef0: 2e70 772f 636f 6e63 6570 7473 2f66 6c6f  .pw/concepts/flo
+00001f00: 772f 2920 636f 6d65 7320 696e 2e0d 0a0d  w/) comes in....
+00001f10: 0a41 2046 6c6f 7720 6973 2061 205b 4441  .A Flow is a [DA
+00001f20: 475d 2868 7474 7073 3a2f 2f64 652e 7769  G](https://de.wi
+00001f30: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00001f40: 2f44 4147 2920 7069 7065 6c69 6e65 2c20  /DAG) pipeline, 
+00001f50: 636f 6d70 6f73 6564 206f 6620 6120 7365  composed of a se
+00001f60: 7420 6f66 2073 7465 7073 2c20 4974 206f  t of steps, It o
+00001f70: 7263 6865 7374 7261 7465 7320 6120 7365  rchestrates a se
+00001f80: 7420 6f66 205b 4578 6563 7574 6f72 735d  t of [Executors]
+00001f90: 2868 7474 7073 3a2f 2f64 6f63 732e 636d  (https://docs.cm
+00001fa0: 6f6e 2e70 772f 636f 6e63 6570 7473 2f65  on.pw/concepts/e
+00001fb0: 7865 6375 746f 722f 2920 616e 6420 6120  xecutor/) and a 
+00001fc0: 5b47 6174 6577 6179 5d28 6874 7470 733a  [Gateway](https:
+00001fd0: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+00001fe0: 6f6e 6365 7074 732f 6761 7465 7761 792f  oncepts/gateway/
+00001ff0: 2920 746f 206f 6666 6572 2061 6e20 656e  ) to offer an en
+00002000: 642d 746f 2d65 6e64 2073 6572 7669 6365  d-to-end service
+00002010: 2e0d 0a0d 0a3e 202a 2a4e 6f74 652a 2a0d  .....> **Note**.
+00002020: 0a3e 2049 6620 796f 7520 6a75 7374 2077  .> If you just w
+00002030: 616e 7420 746f 2073 6572 7665 2061 2073  ant to serve a s
+00002040: 696e 676c 6520 4578 6563 7574 6f72 2c20  ingle Executor, 
+00002050: 796f 7520 6361 6e20 7573 6520 6120 5b44  you can use a [D
+00002060: 6570 6c6f 796d 656e 745d 2823 6275 696c  eployment](#buil
+00002070: 642d 6169 2d2d 6d6c 2d73 6572 7669 6365  d-ai--ml-service
+00002080: 7329 2e0d 0a0d 0a46 6f72 2069 6e73 7461  s).....For insta
+00002090: 6e63 652c 206c 6574 2773 2063 6f6d 6269  nce, let's combi
+000020a0: 6e65 205b 6f75 7220 5374 6162 6c65 4c4d  ne [our StableLM
+000020b0: 206c 616e 6775 6167 6520 6d6f 6465 6c5d   language model]
+000020c0: 2823 6275 696c 642d 6169 2d2d 6d6c 2d73  (#build-ai--ml-s
+000020d0: 6572 7669 6365 7329 2077 6974 6820 6120  ervices) with a 
+000020e0: 5374 6162 6c65 2044 6966 6675 7369 6f6e  Stable Diffusion
+000020f0: 2069 6d61 6765 2067 656e 6572 6174 696f   image generatio
+00002100: 6e20 7365 7276 6963 6520 6672 6f6d 2043  n service from C
+00002110: 6d6f 6e20 4149 2773 205b 4578 6563 7574  mon AI's [Execut
+00002120: 6f72 2048 7562 5d28 6874 7470 733a 2f2f  or Hub](https://
+00002130: 636c 6f75 642e 636d 6f6e 2e70 772f 6578  cloud.cmon.pw/ex
+00002140: 6563 7574 6f72 7329 2e20 4368 6169 6e69  ecutors). Chaini
+00002150: 6e67 2074 6865 7365 2073 6572 7669 6365  ng these service
+00002160: 7320 746f 6765 7468 6572 2069 6e74 6f20  s together into 
+00002170: 6120 5b46 6c6f 775d 2868 7474 7073 3a2f  a [Flow](https:/
+00002180: 2f64 6f63 732e 636d 6f6e 2e70 772f 636f  /docs.cmon.pw/co
+00002190: 6e63 6570 7473 2f66 6c6f 772f 2920 7769  ncepts/flow/) wi
+000021a0: 6c6c 2067 6976 6520 7573 2061 2073 6572  ll give us a ser
+000021b0: 7669 6365 2074 6861 7420 7769 6c6c 2067  vice that will g
+000021c0: 656e 6572 6174 6520 696d 6167 6573 2062  enerate images b
+000021d0: 6173 6564 206f 6e20 6120 7072 6f6d 7074  ased on a prompt
+000021e0: 2067 656e 6572 6174 6564 2062 7920 7468   generated by th
+000021f0: 6520 4c4c 4d2e 0d0a 0d0a 215b 5d28 2e2f  e LLM.....![](./
+00002200: 2e67 6974 6875 622f 696d 6167 6573 2f66  .github/images/f
+00002210: 6c6f 772d 6469 6167 7261 6d2e 706e 6729  low-diagram.png)
+00002220: 0d0a 0d0a 4275 696c 6420 7468 6520 466c  ....Build the Fl
+00002230: 6f77 2077 6974 6820 6569 7468 6572 2050  ow with either P
+00002240: 7974 686f 6e20 6f72 2059 414d 4c3a 0d0a  ython or YAML:..
+00002250: 0d0a 3c64 6976 2063 6c61 7373 3d22 7461  ..<div class="ta
+00002260: 626c 652d 7772 6170 7065 7222 3e0d 0a3c  ble-wrapper">..<
+00002270: 7461 626c 653e 0d0a 3c74 723e 0d0a 3c74  table>..<tr>..<t
+00002280: 683e 2050 7974 686f 6e20 4150 493a 203c  h> Python API: <
+00002290: 636f 6465 3e66 6c6f 772e 7079 3c2f 636f  code>flow.py</co
+000022a0: 6465 3e20 3c2f 7468 3e20 0d0a 3c74 683e  de> </th> ..<th>
+000022b0: 2059 414d 4c3a 203c 636f 6465 3e66 6c6f   YAML: <code>flo
+000022c0: 772e 796d 6c3c 2f63 6f64 653e 203c 2f74  w.yml</code> </t
+000022d0: 683e 0d0a 3c2f 7472 3e0d 0a3c 7472 3e0d  h>..</tr>..<tr>.
+000022e0: 0a3c 7464 3e0d 0a0d 0a60 6060 7079 7468  .<td>....```pyth
+000022f0: 6f6e 0d0a 6672 6f6d 2063 6d6f 6e20 696d  on..from cmon im
+00002300: 706f 7274 2046 6c6f 770d 0a66 726f 6d20  port Flow..from 
+00002310: 6578 6563 7574 6f72 2069 6d70 6f72 7420  executor import 
+00002320: 5374 6162 6c65 4c4d 0d0a 0d0a 666c 6f77  StableLM....flow
+00002330: 203d 2028 0d0a 2020 2020 466c 6f77 2829   = (..    Flow()
+00002340: 0d0a 2020 2020 2e61 6464 2875 7365 733d  ..    .add(uses=
+00002350: 5374 6162 6c65 4c4d 2c20 7469 6d65 6f75  StableLM, timeou
+00002360: 745f 7265 6164 793d 2d31 2c20 706f 7274  t_ready=-1, port
+00002370: 3d31 3233 3435 290d 0a20 2020 202e 6164  =12345)..    .ad
+00002380: 6428 0d0a 2020 2020 2020 2020 7573 6573  d(..        uses
+00002390: 3d27 636d 6f6e 6169 3a2f 2f63 6d6f 6e2e  ='cmonai://cmon.
+000023a0: 7077 2f54 6578 7454 6f49 6d61 6765 272c  pw/TextToImage',
+000023b0: 0d0a 2020 2020 2020 2020 7469 6d65 6f75  ..        timeou
+000023c0: 745f 7265 6164 793d 2d31 2c0d 0a20 2020  t_ready=-1,..   
+000023d0: 2020 2020 2069 6e73 7461 6c6c 5f72 6571       install_req
+000023e0: 7569 7265 6d65 6e74 733d 5472 7565 2c0d  uirements=True,.
+000023f0: 0a20 2020 2029 0d0a 2920 2023 2075 7365  .    )..)  # use
+00002400: 2074 6865 2045 7865 6375 746f 7220 6672   the Executor fr
+00002410: 6f6d 2043 6d6f 6e27 7320 4578 6563 7574  om Cmon's Execut
+00002420: 6f72 2068 7562 0d0a 0d0a 7769 7468 2066  or hub....with f
+00002430: 6c6f 773a 0d0a 2020 2020 666c 6f77 2e62  low:..    flow.b
+00002440: 6c6f 636b 2829 0d0a 6060 600d 0a0d 0a3c  lock()..```....<
+00002450: 2f74 643e 0d0a 3c74 643e 0d0a 0d0a 6060  /td>..<td>....``
+00002460: 6079 616d 6c0d 0a6a 7479 7065 3a20 466c  `yaml..jtype: Fl
+00002470: 6f77 0d0a 7769 7468 3a0d 0a20 2020 2070  ow..with:..    p
+00002480: 6f72 743a 2031 3233 3435 0d0a 6578 6563  ort: 12345..exec
+00002490: 7574 6f72 733a 0d0a 2020 2d20 7573 6573  utors:..  - uses
+000024a0: 3a20 5374 6162 6c65 4c4d 0d0a 2020 2020  : StableLM..    
+000024b0: 7469 6d65 6f75 745f 7265 6164 793a 202d  timeout_ready: -
+000024c0: 310d 0a20 2020 2070 795f 6d6f 6475 6c65  1..    py_module
+000024d0: 733a 0d0a 2020 2020 2020 2d20 6578 6563  s:..      - exec
+000024e0: 7574 6f72 2e70 790d 0a20 202d 2075 7365  utor.py..  - use
+000024f0: 733a 2063 6d6f 6e61 693a 2f2f 636d 6f6e  s: cmonai://cmon
+00002500: 2e70 772f 5465 7874 546f 496d 6167 650d  .pw/TextToImage.
+00002510: 0a20 2020 2074 696d 656f 7574 5f72 6561  .    timeout_rea
+00002520: 6479 3a20 2d31 0d0a 2020 2020 696e 7374  dy: -1..    inst
+00002530: 616c 6c5f 7265 7175 6972 656d 656e 7473  all_requirements
+00002540: 3a20 7472 7565 0d0a 6060 600d 0a0d 0a54  : true..```....T
+00002550: 6865 6e20 7275 6e20 7468 6520 5941 4d4c  hen run the YAML
+00002560: 2046 6c6f 7720 7769 7468 2074 6865 2043   Flow with the C
+00002570: 4c49 3a20 6063 6d6f 6e20 666c 6f77 202d  LI: `cmon flow -
+00002580: 2d75 7365 7320 666c 6f77 2e79 6d6c 600d  -uses flow.yml`.
+00002590: 0a0d 0a3c 2f74 643e 0d0a 3c2f 7472 3e0d  ...</td>..</tr>.
+000025a0: 0a3c 2f74 6162 6c65 3e0d 0a3c 2f64 6976  .</table>..</div
+000025b0: 3e0d 0a0d 0a54 6865 6e2c 2075 7365 205b  >....Then, use [
+000025c0: 436d 6f6e 2043 6c69 656e 745d 2868 7474  Cmon Client](htt
+000025d0: 7073 3a2f 2f64 6f63 732e 636d 6f6e 2e70  ps://docs.cmon.p
+000025e0: 772f 636f 6e63 6570 7473 2f63 6c69 656e  w/concepts/clien
+000025f0: 742f 2920 746f 206d 616b 6520 7265 7175  t/) to make requ
+00002600: 6573 7473 2074 6f20 7468 6520 466c 6f77  ests to the Flow
+00002610: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00002620: 6672 6f6d 2063 6d6f 6e20 696d 706f 7274  from cmon import
+00002630: 2043 6c69 656e 742c 2044 6f63 756d 656e   Client, Documen
+00002640: 740d 0a0d 0a63 6c69 656e 7420 3d20 436c  t....client = Cl
+00002650: 6965 6e74 2870 6f72 743d 3132 3334 3529  ient(port=12345)
+00002660: 0d0a 0d0a 7072 6f6d 7074 203d 2044 6f63  ....prompt = Doc
+00002670: 756d 656e 7428 0d0a 2020 2020 7461 6773  ument(..    tags
+00002680: 203d 207b 2770 726f 6d70 7427 3a20 2773   = {'prompt': 's
+00002690: 7567 6765 7374 2061 6e20 696e 7465 7265  uggest an intere
+000026a0: 7374 696e 6720 696d 6167 6520 6765 6e65  sting image gene
+000026b0: 7261 7469 6f6e 2070 726f 6d70 7420 666f  ration prompt fo
+000026c0: 7220 6120 6d6f 6e61 206c 6973 6120 7661  r a mona lisa va
+000026d0: 7269 616e 7427 7d0d 0a29 0d0a 0d0a 7265  riant'}..)....re
+000026e0: 7370 6f6e 7365 203d 2063 6c69 656e 742e  sponse = client.
+000026f0: 706f 7374 286f 6e3d 272f 272c 2069 6e70  post(on='/', inp
+00002700: 7574 733d 5b70 726f 6d70 745d 290d 0a0d  uts=[prompt])...
+00002710: 0a72 6573 706f 6e73 655b 305d 2e64 6973  .response[0].dis
+00002720: 706c 6179 2829 0d0a 6060 600d 0a0d 0a21  play()..```....!
+00002730: 5b5d 282e 2f2e 6769 7468 7562 2f69 6d61  [](./.github/ima
+00002740: 6765 732f 6d6f 6e61 2d6c 6973 612e 706e  ges/mona-lisa.pn
+00002750: 6729 0d0a 0d0a 2323 2044 6570 6c6f 7920  g)....## Deploy 
+00002760: 746f 2074 6865 2063 6c6f 7564 0d0a 0d0a  to the cloud....
+00002770: 596f 7520 6361 6e20 616c 736f 2064 6570  You can also dep
+00002780: 6c6f 7920 6120 466c 6f77 2074 6f20 4a43  loy a Flow to JC
+00002790: 6c6f 7564 2e0d 0a0d 0a46 6972 7374 2c20  loud.....First, 
+000027a0: 7475 726e 2074 6865 2060 666c 6f77 2e79  turn the `flow.y
+000027b0: 6d6c 6020 6669 6c65 2069 6e74 6f20 6120  ml` file into a 
+000027c0: 5b4a 436c 6f75 642d 636f 6d70 6174 6962  [JCloud-compatib
+000027d0: 6c65 2059 414d 4c5d 2868 7474 7073 3a2f  le YAML](https:/
+000027e0: 2f64 6f63 732e 636d 6f6e 2e70 772f 636f  /docs.cmon.pw/co
+000027f0: 6e63 6570 7473 2f6a 636c 6f75 642f 7961  ncepts/jcloud/ya
+00002800: 6d6c 2d73 7065 632f 2920 6279 2073 7065  ml-spec/) by spe
+00002810: 6369 6679 696e 6720 7265 736f 7572 6365  cifying resource
+00002820: 2072 6571 7569 7265 6d65 6e74 7320 616e   requirements an
+00002830: 6420 7573 696e 6720 636f 6e74 6169 6e65  d using containe
+00002840: 7269 7a65 6420 4875 6220 4578 6563 7574  rized Hub Execut
+00002850: 6f72 732e 0d0a 0d0a 5468 656e 2c20 7573  ors.....Then, us
+00002860: 6520 6063 6d6f 6e20 636c 6f75 6420 6465  e `cmon cloud de
+00002870: 706c 6f79 6020 636f 6d6d 616e 6420 746f  ploy` command to
+00002880: 2064 6570 6c6f 7920 746f 2074 6865 2063   deploy to the c
+00002890: 6c6f 7564 3a0d 0a0d 0a60 6060 7368 656c  loud:....```shel
+000028a0: 6c0d 0a77 6765 7420 6874 7470 733a 2f2f  l..wget https://
+000028b0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000028c0: 6e74 656e 742e 636f 6d2f 636d 6f6e 2e70  ntent.com/cmon.p
+000028d0: 772f 636d 6f6e 2f6d 6173 7465 722f 2e67  w/cmon/master/.g
+000028e0: 6974 6875 622f 6765 7474 696e 672d 7374  ithub/getting-st
+000028f0: 6172 7465 642f 6a63 6c6f 7564 2d66 6c6f  arted/jcloud-flo
+00002900: 772e 796d 6c0d 0a63 6d6f 6e20 636c 6f75  w.yml..cmon clou
+00002910: 6420 6465 706c 6f79 206a 636c 6f75 642d  d deploy jcloud-
+00002920: 666c 6f77 2e79 6d6c 0d0a 6060 600d 0a0d  flow.yml..```...
+00002930: 0a3e 202a 2a57 6172 6e69 6e67 2a2a 0d0a  .> **Warning**..
+00002940: 3e0d 0a3e 204d 616b 6520 7375 7265 2074  >..> Make sure t
+00002950: 6f20 6465 6c65 7465 2f63 6c65 616e 2075  o delete/clean u
+00002960: 7020 7468 6520 466c 6f77 206f 6e63 6520  p the Flow once 
+00002970: 796f 7520 6172 6520 646f 6e65 2077 6974  you are done wit
+00002980: 6820 7468 6973 2074 7574 6f72 6961 6c20  h this tutorial 
+00002990: 746f 2073 6176 6520 7265 736f 7572 6365  to save resource
+000029a0: 7320 616e 6420 6372 6564 6974 732e 0d0a  s and credits...
+000029b0: 0d0a 5265 6164 206d 6f72 6520 6162 6f75  ..Read more abou
+000029c0: 7420 5b64 6570 6c6f 7969 6e67 2046 6c6f  t [deploying Flo
+000029d0: 7773 2074 6f20 4a43 6c6f 7564 5d28 6874  ws to JCloud](ht
+000029e0: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
+000029f0: 7077 2f63 6f6e 6365 7074 732f 6a63 6c6f  pw/concepts/jclo
+00002a00: 7564 2f23 6465 706c 6f79 292e 0d0a 0d0a  ud/#deploy).....
+00002a10: 3c21 2d2d 2065 6e64 2062 7569 6c64 2d70  <!-- end build-p
+00002a20: 6970 656c 696e 6573 202d 2d3e 0d0a 0d0a  ipelines -->....
+00002a30: 4368 6563 6b20 5b74 6865 2067 6574 7469  Check [the getti
+00002a40: 6e67 2d73 7461 7274 6564 2070 726f 6a65  ng-started proje
+00002a50: 6374 2073 6f75 7263 6520 636f 6465 5d28  ct source code](
+00002a60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002a70: 6f6d 2f63 6d6f 6e2e 7077 2f63 6d6f 6e2f  om/cmon.pw/cmon/
+00002a80: 7472 6565 2f6d 6173 7465 722f 2e67 6974  tree/master/.git
+00002a90: 6875 622f 6765 7474 696e 672d 7374 6172  hub/getting-star
+00002aa0: 7465 6429 2e0d 0a0d 0a23 2323 2045 6173  ted).....### Eas
+00002ab0: 7920 7363 616c 6162 696c 6974 7920 616e  y scalability an
+00002ac0: 6420 636f 6e63 7572 7265 6e63 790d 0a0d  d concurrency...
+00002ad0: 0a57 6879 206e 6f74 206a 7573 7420 7573  .Why not just us
+00002ae0: 6520 7374 616e 6461 7264 2050 7974 686f  e standard Pytho
+00002af0: 6e20 746f 2062 7569 6c64 2074 6861 7420  n to build that 
+00002b00: 6d69 6372 6f73 6572 7669 6365 2061 6e64  microservice and
+00002b10: 2070 6970 656c 696e 653f 2043 6d6f 6e20   pipeline? Cmon 
+00002b20: 6163 6365 6c65 7261 7465 7320 7469 6d65  accelerates time
+00002b30: 2074 6f20 6d61 726b 6574 206f 6620 796f   to market of yo
+00002b40: 7572 2061 7070 6c69 6361 7469 6f6e 2062  ur application b
+00002b50: 7920 6d61 6b69 6e67 2069 7420 6d6f 7265  y making it more
+00002b60: 2073 6361 6c61 626c 6520 616e 6420 636c   scalable and cl
+00002b70: 6f75 642d 6e61 7469 7665 2e20 436d 6f6e  oud-native. Cmon
+00002b80: 2061 6c73 6f20 6861 6e64 6c65 7320 7468   also handles th
+00002b90: 6520 696e 6672 6173 7472 7563 7475 7265  e infrastructure
+00002ba0: 2063 6f6d 706c 6578 6974 7920 696e 2070   complexity in p
+00002bb0: 726f 6475 6374 696f 6e20 616e 6420 6f74  roduction and ot
+00002bc0: 6865 7220 4461 792d 3220 6f70 6572 6174  her Day-2 operat
+00002bd0: 696f 6e73 2073 6f20 7468 6174 2079 6f75  ions so that you
+00002be0: 2063 616e 2066 6f63 7573 206f 6e20 7468   can focus on th
+00002bf0: 6520 6461 7461 2061 7070 6c69 6361 7469  e data applicati
+00002c00: 6f6e 2069 7473 656c 662e 0d0a 0d0a 496e  on itself.....In
+00002c10: 6372 6561 7365 2079 6f75 7220 6170 706c  crease your appl
+00002c20: 6963 6174 696f 6e27 7320 7468 726f 7567  ication's throug
+00002c30: 6870 7574 2077 6974 6820 7363 616c 6162  hput with scalab
+00002c40: 696c 6974 7920 6665 6174 7572 6573 206f  ility features o
+00002c50: 7574 206f 6620 7468 6520 626f 782c 206c  ut of the box, l
+00002c60: 696b 6520 5b72 6570 6c69 6361 735d 2868  ike [replicas](h
+00002c70: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
+00002c80: 2e70 772f 636f 6e63 6570 7473 2f6f 7263  .pw/concepts/orc
+00002c90: 6865 7374 7261 7469 6f6e 2f73 6361 6c65  hestration/scale
+00002ca0: 2d6f 7574 2f23 7265 706c 6963 6174 652d  -out/#replicate-
+00002cb0: 6578 6563 7574 6f72 7329 2c20 5b73 6861  executors), [sha
+00002cc0: 7264 735d 2868 7474 7073 3a2f 2f64 6f63  rds](https://doc
+00002cd0: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+00002ce0: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
+00002cf0: 2f73 6361 6c65 2d6f 7574 2f23 6375 7374  /scale-out/#cust
+00002d00: 6f6d 697a 652d 706f 6c6c 696e 672d 6265  omize-polling-be
+00002d10: 6861 7669 6f72 7329 2061 6e64 205b 6479  haviors) and [dy
+00002d20: 6e61 6d69 6320 6261 7463 6869 6e67 5d28  namic batching](
+00002d30: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00002d40: 6e2e 7077 2f63 6f6e 6365 7074 732f 7365  n.pw/concepts/se
+00002d50: 7276 696e 672f 6578 6563 7574 6f72 2f64  rving/executor/d
+00002d60: 796e 616d 6963 2d62 6174 6368 696e 672f  ynamic-batching/
+00002d70: 292e 0d0a 0d0a 4c65 7427 7320 7363 616c  ).....Let's scal
+00002d80: 6520 6120 5374 6162 6c65 2044 6966 6675  e a Stable Diffu
+00002d90: 7369 6f6e 2045 7865 6375 746f 7220 6465  sion Executor de
+00002da0: 706c 6f79 6d65 6e74 2077 6974 6820 7265  ployment with re
+00002db0: 706c 6963 6173 2061 6e64 2064 796e 616d  plicas and dynam
+00002dc0: 6963 2062 6174 6368 696e 673a 0d0a 0d0a  ic batching:....
+00002dd0: 215b 5d28 2e2f 2e67 6974 6875 622f 696d  ![](./.github/im
+00002de0: 6167 6573 2f73 6361 6c65 642d 6465 706c  ages/scaled-depl
+00002df0: 6f79 6d65 6e74 2e70 6e67 290d 0a0d 0a2a  oyment.png)....*
+00002e00: 2043 7265 6174 6520 7477 6f20 7265 706c   Create two repl
+00002e10: 6963 6173 2c20 7769 7468 205b 6120 4750  icas, with [a GP
+00002e20: 5520 6173 7369 676e 6564 2066 6f72 2065  U assigned for e
+00002e30: 6163 685d 2868 7474 7073 3a2f 2f64 6f63  ach](https://doc
+00002e40: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+00002e50: 7473 2f66 6c6f 772f 7363 616c 652d 6f75  ts/flow/scale-ou
+00002e60: 742f 2372 6570 6c69 6361 7465 2d6f 6e2d  t/#replicate-on-
+00002e70: 6d75 6c74 6970 6c65 2d67 7075 7329 2e0d  multiple-gpus)..
+00002e80: 0a2a 2045 6e61 626c 6520 6479 6e61 6d69  .* Enable dynami
+00002e90: 6320 6261 7463 6869 6e67 2074 6f20 7072  c batching to pr
+00002ea0: 6f63 6573 7320 696e 636f 6d69 6e67 2070  ocess incoming p
+00002eb0: 6172 616c 6c65 6c20 7265 7175 6573 7473  arallel requests
+00002ec0: 2074 6f67 6574 6865 7220 7769 7468 2074   together with t
+00002ed0: 6865 2073 616d 6520 6d6f 6465 6c20 696e  he same model in
+00002ee0: 6665 7265 6e63 652e 0d0a 0d0a 0d0a 3c64  ference.......<d
+00002ef0: 6976 2063 6c61 7373 3d22 7461 626c 652d  iv class="table-
+00002f00: 7772 6170 7065 7222 3e0d 0a3c 7461 626c  wrapper">..<tabl
+00002f10: 653e 0d0a 3c74 723e 0d0a 3c74 683e 204e  e>..<tr>..<th> N
+00002f20: 6f72 6d61 6c20 4465 706c 6f79 6d65 6e74  ormal Deployment
+00002f30: 203c 2f74 683e 200d 0a3c 7468 3e20 5363   </th> ..<th> Sc
+00002f40: 616c 6564 2044 6570 6c6f 796d 656e 7420  aled Deployment 
+00002f50: 3c2f 7468 3e0d 0a3c 2f74 723e 0d0a 3c74  </th>..</tr>..<t
+00002f60: 723e 0d0a 3c74 643e 0d0a 0d0a 6060 6079  r>..<td>....```y
+00002f70: 616d 6c0d 0a6a 7479 7065 3a20 4465 706c  aml..jtype: Depl
+00002f80: 6f79 6d65 6e74 0d0a 7769 7468 3a0d 0a20  oyment..with:.. 
+00002f90: 2074 696d 656f 7574 5f72 6561 6479 3a20   timeout_ready: 
+00002fa0: 2d31 0d0a 2020 7573 6573 3a20 636d 6f6e  -1..  uses: cmon
+00002fb0: 6169 3a2f 2f63 6d6f 6e2e 7077 2f54 6578  ai://cmon.pw/Tex
+00002fc0: 7454 6f49 6d61 6765 0d0a 2020 696e 7374  tToImage..  inst
+00002fd0: 616c 6c5f 7265 7175 6972 656d 656e 7473  all_requirements
+00002fe0: 3a20 7472 7565 0d0a 6060 600d 0a0d 0a3c  : true..```....<
+00002ff0: 2f74 643e 0d0a 3c74 643e 0d0a 0d0a 6060  /td>..<td>....``
+00003000: 6079 616d 6c0d 0a6a 7479 7065 3a20 4465  `yaml..jtype: De
+00003010: 706c 6f79 6d65 6e74 0d0a 7769 7468 3a0d  ployment..with:.
+00003020: 0a20 2074 696d 656f 7574 5f72 6561 6479  .  timeout_ready
+00003030: 3a20 2d31 0d0a 2020 7573 6573 3a20 636d  : -1..  uses: cm
+00003040: 6f6e 6169 3a2f 2f63 6d6f 6e2e 7077 2f54  onai://cmon.pw/T
+00003050: 6578 7454 6f49 6d61 6765 0d0a 2020 696e  extToImage..  in
+00003060: 7374 616c 6c5f 7265 7175 6972 656d 656e  stall_requiremen
+00003070: 7473 3a20 7472 7565 0d0a 2020 656e 763a  ts: true..  env:
+00003080: 0d0a 2020 2043 5544 415f 5649 5349 424c  ..   CUDA_VISIBL
+00003090: 455f 4445 5649 4345 533a 2052 520d 0a20  E_DEVICES: RR.. 
+000030a0: 2072 6570 6c69 6361 733a 2032 0d0a 2020   replicas: 2..  
+000030b0: 7573 6573 5f64 796e 616d 6963 5f62 6174  uses_dynamic_bat
+000030c0: 6368 696e 673a 2023 2063 6f6e 6669 6775  ching: # configu
+000030d0: 7265 2064 796e 616d 6963 2062 6174 6368  re dynamic batch
+000030e0: 696e 670d 0a20 2020 202f 6465 6661 756c  ing..    /defaul
+000030f0: 743a 0d0a 2020 2020 2020 7072 6566 6572  t:..      prefer
+00003100: 7265 645f 6261 7463 685f 7369 7a65 3a20  red_batch_size: 
+00003110: 3130 0d0a 2020 2020 2020 7469 6d65 6f75  10..      timeou
+00003120: 743a 2032 3030 0d0a 6060 600d 0a0d 0a3c  t: 200..```....<
+00003130: 2f74 643e 0d0a 3c2f 7472 3e0d 0a3c 2f74  /td>..</tr>..</t
+00003140: 6162 6c65 3e0d 0a3c 2f64 6976 3e0d 0a0d  able>..</div>...
+00003150: 0a41 7373 756d 696e 6720 796f 7572 206d  .Assuming your m
+00003160: 6163 6869 6e65 2068 6173 2074 776f 2047  achine has two G
+00003170: 5055 732c 2075 7369 6e67 2074 6865 2073  PUs, using the s
+00003180: 6361 6c65 6420 6465 706c 6f79 6d65 6e74  caled deployment
+00003190: 2059 414d 4c20 7769 6c6c 2067 6976 6520   YAML will give 
+000031a0: 6265 7474 6572 2074 6872 6f75 6768 7075  better throughpu
+000031b0: 7420 636f 6d70 6172 6564 2074 6f20 7468  t compared to th
+000031c0: 6520 6e6f 726d 616c 2064 6570 6c6f 796d  e normal deploym
+000031d0: 656e 742e 0d0a 0d0a 5468 6573 6520 6665  ent.....These fe
+000031e0: 6174 7572 6573 2061 7070 6c79 2074 6f20  atures apply to 
+000031f0: 626f 7468 205b 4465 706c 6f79 6d65 6e74  both [Deployment
+00003200: 2059 414d 4c5d 2868 7474 7073 3a2f 2f64   YAML](https://d
+00003210: 6f63 732e 636d 6f6e 2e70 772f 636f 6e63  ocs.cmon.pw/conc
+00003220: 6570 7473 2f65 7865 6375 746f 722f 6465  epts/executor/de
+00003230: 706c 6f79 6d65 6e74 2d79 616d 6c2d 7370  ployment-yaml-sp
+00003240: 6563 2f23 6465 706c 6f79 6d65 6e74 2d79  ec/#deployment-y
+00003250: 616d 6c2d 7370 6563 2920 616e 6420 5b46  aml-spec) and [F
+00003260: 6c6f 7720 5941 4d4c 5d28 6874 7470 733a  low YAML](https:
+00003270: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+00003280: 6f6e 6365 7074 732f 666c 6f77 2f79 616d  oncepts/flow/yam
+00003290: 6c2d 7370 6563 2f29 2e20 5468 616e 6b73  l-spec/). Thanks
+000032a0: 2074 6f20 7468 6520 5941 4d4c 2073 796e   to the YAML syn
+000032b0: 7461 782c 2079 6f75 2063 616e 2069 6e6a  tax, you can inj
+000032c0: 6563 7420 6465 706c 6f79 6d65 6e74 2063  ect deployment c
+000032d0: 6f6e 6669 6775 7261 7469 6f6e 7320 7265  onfigurations re
+000032e0: 6761 7264 6c65 7373 206f 6620 4578 6563  gardless of Exec
+000032f0: 7574 6f72 2063 6f64 652e 0d0a 0d0a 2323  utor code.....##
+00003300: 2320 4765 7420 6f6e 2074 6865 2066 6173  # Get on the fas
+00003310: 7420 6c61 6e65 2074 6f20 636c 6f75 642d  t lane to cloud-
+00003320: 6e61 7469 7665 0d0a 0d0a 5573 696e 6720  native....Using 
+00003330: 4b75 6265 726e 6574 6573 2077 6974 6820  Kubernetes with 
+00003340: 436d 6f6e 2069 7320 6561 7379 3a0d 0a0d  Cmon is easy:...
+00003350: 0a60 6060 6261 7368 0d0a 636d 6f6e 2065  .```bash..cmon e
+00003360: 7870 6f72 7420 6b75 6265 726e 6574 6573  xport kubernetes
+00003370: 2066 6c6f 772e 796d 6c20 2e2f 6d79 2d6b   flow.yml ./my-k
+00003380: 3873 0d0a 6b75 6265 6374 6c20 6170 706c  8s..kubectl appl
+00003390: 7920 2d52 202d 6620 6d79 2d6b 3873 0d0a  y -R -f my-k8s..
+000033a0: 6060 600d 0a0d 0a41 6e64 2073 6f20 6973  ```....And so is
+000033b0: 2044 6f63 6b65 7220 436f 6d70 6f73 653a   Docker Compose:
+000033c0: 0d0a 0d0a 6060 6062 6173 680d 0a63 6d6f  ....```bash..cmo
+000033d0: 6e20 6578 706f 7274 2064 6f63 6b65 722d  n export docker-
+000033e0: 636f 6d70 6f73 6520 666c 6f77 2e79 6d6c  compose flow.yml
+000033f0: 2064 6f63 6b65 722d 636f 6d70 6f73 652e   docker-compose.
+00003400: 796d 6c0d 0a64 6f63 6b65 722d 636f 6d70  yml..docker-comp
+00003410: 6f73 6520 7570 0d0a 6060 600d 0a0d 0a3e  ose up..```....>
+00003420: 202a 2a4e 6f74 652a 2a0d 0a3e 2059 6f75   **Note**..> You
+00003430: 2063 616e 2061 6c73 6f20 6578 706f 7274   can also export
+00003440: 2044 6570 6c6f 796d 656e 7420 5941 4d4c   Deployment YAML
+00003450: 2074 6f20 5b4b 7562 6572 6e65 7465 735d   to [Kubernetes]
+00003460: 2868 7474 7073 3a2f 2f64 6f63 732e 636d  (https://docs.cm
+00003470: 6f6e 2e70 772f 636f 6e63 6570 7473 2f65  on.pw/concepts/e
+00003480: 7865 6375 746f 722f 7365 7276 652f 2373  xecutor/serve/#s
+00003490: 6572 7665 2d76 6961 2d6b 7562 6572 6e65  erve-via-kuberne
+000034a0: 7465 7329 2061 6e64 205b 446f 636b 6572  tes) and [Docker
+000034b0: 2043 6f6d 706f 7365 5d28 6874 7470 733a   Compose](https:
+000034c0: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+000034d0: 6f6e 6365 7074 732f 6578 6563 7574 6f72  oncepts/executor
+000034e0: 2f73 6572 7665 2f23 7365 7276 652d 7669  /serve/#serve-vi
+000034f0: 612d 646f 636b 6572 2d63 6f6d 706f 7365  a-docker-compose
+00003500: 292e 0d0a 0d0a 5468 6174 2773 206e 6f74  ).....That's not
+00003510: 2061 6c6c 2e20 5765 2061 6c73 6f20 7375   all. We also su
+00003520: 7070 6f72 7420 5b4f 7065 6e54 656c 656d  pport [OpenTelem
+00003530: 6574 7279 2c20 5072 6f6d 6574 6865 7573  etry, Prometheus
+00003540: 2c20 616e 6420 4a61 6567 6572 5d28 6874  , and Jaeger](ht
+00003550: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
+00003560: 7077 2f63 6c6f 7564 2d6e 6174 6976 656e  pw/cloud-nativen
+00003570: 6573 732f 6f70 656e 7465 6c65 6d65 7472  ess/opentelemetr
+00003580: 792f 292e 0d0a 0d0a 5768 6174 2063 6c6f  y/).....What clo
+00003590: 7564 2d6e 6174 6976 6520 7465 6368 6e6f  ud-native techno
+000035a0: 6c6f 6779 2069 7320 7374 696c 6c20 6368  logy is still ch
+000035b0: 616c 6c65 6e67 696e 6720 746f 2079 6f75  allenging to you
+000035c0: 3f20 5b54 656c 6c20 7573 5d28 6874 7470  ? [Tell us](http
+000035d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+000035e0: 6d6f 6e2e 7077 2f63 6d6f 6e2f 6973 7375  mon.pw/cmon/issu
+000035f0: 6573 2920 616e 6420 7765 276c 6c20 6861  es) and we'll ha
+00003600: 6e64 6c65 2074 6865 2063 6f6d 706c 6578  ndle the complex
+00003610: 6974 7920 616e 6420 6d61 6b65 2069 7420  ity and make it 
+00003620: 6561 7379 2066 6f72 2079 6f75 2e0d 0a0d  easy for you....
+00003630: 0a3c 212d 2d20 7374 6172 7420 7375 7070  .<!-- start supp
+00003640: 6f72 742d 7069 7463 6820 2d2d 3e0d 0a0d  ort-pitch -->...
+00003650: 0a23 2320 5375 7070 6f72 740d 0a0d 0a2d  .## Support....-
+00003660: 204a 6f69 6e20 6f75 7220 5b44 6973 636f   Join our [Disco
+00003670: 7264 2063 6f6d 6d75 6e69 7479 5d28 6874  rd community](ht
+00003680: 7470 733a 2f2f 6469 7363 6f72 642e 636d  tps://discord.cm
+00003690: 6f6e 2e70 7729 2061 6e64 2063 6861 7420  on.pw) and chat 
+000036a0: 7769 7468 206f 7468 6572 2063 6f6d 6d75  with other commu
+000036b0: 6e69 7479 206d 656d 6265 7273 2061 626f  nity members abo
+000036c0: 7574 2069 6465 6173 2e0d 0a2d 2053 7562  ut ideas...- Sub
+000036d0: 7363 7269 6265 2074 6f20 7468 6520 6c61  scribe to the la
+000036e0: 7465 7374 2076 6964 656f 2074 7574 6f72  test video tutor
+000036f0: 6961 6c73 206f 6e20 6f75 7220 5b59 6f75  ials on our [You
+00003700: 5475 6265 2063 6861 6e6e 656c 5d28 6874  Tube channel](ht
+00003710: 7470 733a 2f2f 796f 7574 7562 652e 636f  tps://youtube.co
+00003720: 6d2f 632f 636d 6f6e 2e70 7729 0d0a 0d0a  m/c/cmon.pw)....
+00003730: 2323 204a 6f69 6e20 5573 0d0a 0d0a 436d  ## Join Us....Cm
+00003740: 6f6e 2069 7320 6261 636b 6564 2062 7920  on is backed by 
+00003750: 5b43 6d6f 6e20 4149 5d28 6874 7470 733a  [Cmon AI](https:
+00003760: 2f2f 636d 6f6e 2e70 7729 2061 6e64 206c  //cmon.pw) and l
+00003770: 6963 656e 7365 6420 756e 6465 7220 5b41  icensed under [A
+00003780: 7061 6368 652d 322e 305d 282e 2f4c 4943  pache-2.0](./LIC
+00003790: 454e 5345 292e 0d0a 0d0a 3c21 2d2d 2065  ENSE).....<!-- e
+000037a0: 6e64 2073 7570 706f 7274 2d70 6974 6368  nd support-pitch
+000037b0: 202d 2d3e 0d0a                            -->..
```

### Comparing `cmon-ai-0.38.5/cmon/__init__.py` & `cmon-ai-0.42.6/cmon/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/checker.py` & `cmon-ai-0.42.6/cmon/checker.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/__init__.py` & `cmon-ai-0.42.6/cmon/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/__init__.py` & `cmon-ai-0.42.6/cmon/clients/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/grpc.py` & `cmon-ai-0.42.6/cmon/clients/base/grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/helper.py` & `cmon-ai-0.42.6/cmon/clients/base/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/http.py` & `cmon-ai-0.42.6/cmon/clients/base/http.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/retry.py` & `cmon-ai-0.42.6/cmon/clients/base/retry.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/stream_rpc.py` & `cmon-ai-0.42.6/cmon/clients/base/stream_rpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/unary_rpc.py` & `cmon-ai-0.42.6/cmon/clients/base/unary_rpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/base/websocket.py` & `cmon-ai-0.42.6/cmon/clients/base/websocket.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/grpc.py` & `cmon-ai-0.42.6/cmon/clients/grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/helper.py` & `cmon-ai-0.42.6/cmon/clients/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/http.py` & `cmon-ai-0.42.6/cmon/clients/http.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/mixin.py` & `cmon-ai-0.42.6/cmon/clients/mixin.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/request/__init__.py` & `cmon-ai-0.42.6/cmon/clients/request/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/request/asyncio.py` & `cmon-ai-0.42.6/cmon/clients/request/asyncio.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/request/helper.py` & `cmon-ai-0.42.6/cmon/clients/request/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/clients/websocket.py` & `cmon-ai-0.42.6/cmon/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/constants.py` & `cmon-ai-0.42.6/cmon/constants.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/enums.py` & `cmon-ai-0.42.6/cmon/enums.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/excepts.py` & `cmon-ai-0.42.6/cmon/excepts.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/exporter.py` & `cmon-ai-0.42.6/cmon/exporter.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/helper.py` & `cmon-ai-0.42.6/cmon/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -972,15 +972,15 @@
             'platform-version': platform.version(),
             'architecture': platform.machine(),
             'processor': platform.processor(),
             'uid': getnode(),
             'session-id': str(random_uuid(use_uuid1=True)),
             'uptime': __uptime__,
             'ci-vendor': get_ci_vendor() or __unset_msg__,
-            'internal': 'cmon-ai'
+            'internal': 'cmon.pw'
             in os.getenv('GITHUB_ACTION_REPOSITORY', __unset_msg__),
         }
 
         env_info = {k: os.getenv(k, __unset_msg__) for k in __cmon_env__}
         full_version = info, env_info
     except Exception as e:
         default_logger.error(str(e))
@@ -1640,15 +1640,15 @@
     :param kwargs: Extra kwargs to be passed to the data sent
     """
 
     if 'CMON_OPTOUT_TELEMETRY' in os.environ:
         return
 
     def _telemetry():
-        url = 'https://telemetry.cmon.ai/'
+        url = 'https://telemetry.cmon.pw/'
         try:
             from cmon.helper import get_full_version
 
             metas, _ = get_full_version()
             data = base64.urlsafe_b64encode(
                 json.dumps(
                     {**metas, 'event': f'{obj_cls_name}.{event}', **kwargs}
```

### Comparing `cmon-ai-0.38.5/cmon/importer.py` & `cmon-ai-0.42.6/cmon/importer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/__init__.py` & `cmon-ai-0.42.6/cmon/jaml/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/helper.py` & `cmon-ai-0.42.6/cmon/jaml/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/parsers/__init__.py` & `cmon-ai-0.42.6/cmon/jaml/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/parsers/base.py` & `cmon-ai-0.42.6/cmon/jaml/parsers/base.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/parsers/deployment/legacy.py` & `cmon-ai-0.42.6/cmon/jaml/parsers/deployment/legacy.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/parsers/executor/legacy.py` & `cmon-ai-0.42.6/cmon/jaml/parsers/executor/legacy.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/parsers/flow/v1.py` & `cmon-ai-0.42.6/cmon/jaml/parsers/flow/v1.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/jaml/parsers/gateway/legacy.py` & `cmon-ai-0.42.6/cmon/jaml/parsers/gateway/legacy.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/logging/formatter.py` & `cmon-ai-0.42.6/cmon/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/logging/logger.py` & `cmon-ai-0.42.6/cmon/logging/logger.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/logging/profile.py` & `cmon-ai-0.42.6/cmon/logging/profile.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/__init__.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,15 @@
 
               When not given, then the default naming strategy will apply.
         :param native: If set, only native Executors is allowed, and the Executor is always run inside WorkerRuntime.
         :param no_reduce: Disable the built-in reduction mechanism. Set this if the reduction is to be handled by the Executor itself by operating on a `docs_matrix` or `docs_map`
         :param output_array_type: The type of array `tensor` and `embedding` will be serialized to.
 
           Supports the same types as `docarray.to_protobuf(.., ndarray_type=...)`, which can be found
-          `here <https://docarray.cmon.ai/fundamentals/document/serialization/#from-to-protobuf>`.
+          `here <https://docarray.cmon.pw/fundamentals/document/serialization/#from-to-protobuf>`.
           Defaults to retaining whatever type is returned by the Executor.
         :param polling: The polling strategy of the Deployment and its endpoints (when `shards>1`).
               Can be defined for all endpoints of a Deployment or by endpoint.
               Define per Deployment:
               - ANY: only one (whoever is idle) Pod polls the message
               - ALL: all Pods poll the message (like a broadcast)
               Define per Endpoint:
@@ -383,23 +383,23 @@
         :param prefer_platform: The preferred target Docker platform. (e.g. "linux/amd64", "linux/arm64")
         :param protocol: Communication protocol of the server exposed by the Executor. This can be a single value or a list of protocols, depending on your chosen Gateway. Choose the convenient protocols from: ['GRPC', 'HTTP', 'WEBSOCKET'].
         :param py_modules: The customized python modules need to be imported before loading the executor
 
           Note that the recommended way is to only import a single module - a simple python file, if your
           executor can be defined in a single file, or an ``__init__.py`` file if you have multiple files,
           which should be structured as a python package. For more details, please see the
-          `Executor cookbook <https://docs.cmon.ai/concepts/executor/executor-files/>`__
+          `Executor cookbook <https://docs.cmon.pw/concepts/executor/executor-files/>`__
         :param quiet: If set, then no log will be emitted from this object.
         :param quiet_error: If set, then exception stack information will not be added to the log
         :param raft_configuration: Dictionary of kwargs arguments that will be passed to the RAFT node as configuration options when starting the RAFT node.
         :param reload: If set, the Executor will restart while serving if YAML configuration source or Executor modules are changed. If YAML configuration is changed, the whole deployment is reloaded and new processes will be restarted. If only Python modules of the Executor have changed, they will be reloaded to the interpreter without restarting process.
         :param replicas: The number of replicas in the deployment
         :param retries: Number of retries per gRPC call. If <0 it defaults to max(3, num_replicas)
         :param runtime_cls: The runtime class to run inside the Pod
-        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.ai/concepts/flow/create-flow/#complex-flow-topologies
+        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.pw/concepts/flow/create-flow/#complex-flow-topologies
         :param ssl_certfile: the path to the certificate file
         :param ssl_keyfile: the path to the key file
         :param stateful: If set, start consensus module to make sure write operations are properly replicated between all the replicas
         :param timeout_ctrl: The timeout in milliseconds of the control request, -1 for waiting forever
         :param timeout_ready: The timeout in milliseconds of a Pod waits for the runtime to be ready, -1 for waiting forever
         :param timeout_send: The timeout in milliseconds used when sending data requests to Executors, -1 means no timeout, disabled by default
         :param title: The title of this HTTP server. It will be used in automatics docs such as Swagger UI.
@@ -431,15 +431,15 @@
           More details can be found in Uvicorn docs: https://www.uvicorn.org/settings/
         :param volumes: The path on the host to be mounted inside the container.
 
           Note,
           - If separated by `:`, then the first part will be considered as the local host path and the second part is the path in the container system.
           - If no split provided, then the basename of that directory will be mounted into container's root path, e.g. `--volumes="/user/test/my-workspace"` will be mounted into `/my-workspace` inside the container.
           - All volumes are mounted with read-write mode.
-        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `DocArray query condition <https://docarray.cmon.ai/fundamentals/documentarray/find/#query-by-conditions>`
+        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `docarray query condition <https://docarray.cmon.pw/fundamentals/documentarray/find/#query-by-conditions>`
         :param workspace: The working directory for any IO operations in this object. If not set, then derive from its parent `workspace`.
 
         .. # noqa: DAR202
         .. # noqa: DAR101
         .. # noqa: DAR003
         """
```

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/config/docker_compose.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/config/docker_compose.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/config/helper.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/config/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8s.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8s.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_deployment.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/config/k8slib/kubernetes_tools.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/deployments/install_requirements_helper.py` & `cmon-ai-0.42.6/cmon/orchestrate/deployments/install_requirements_helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/flow/asyncio.py` & `cmon-ai-0.42.6/cmon/orchestrate/flow/asyncio.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/flow/base.py` & `cmon-ai-0.42.6/cmon/orchestrate/flow/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -952,15 +952,15 @@
 
               When not given, then the default naming strategy will apply.
         :param native: If set, only native Executors is allowed, and the Executor is always run inside WorkerRuntime.
         :param no_reduce: Disable the built-in reduction mechanism. Set this if the reduction is to be handled by the Executor itself by operating on a `docs_matrix` or `docs_map`
         :param output_array_type: The type of array `tensor` and `embedding` will be serialized to.
 
           Supports the same types as `docarray.to_protobuf(.., ndarray_type=...)`, which can be found
-          `here <https://docarray.cmon.ai/fundamentals/document/serialization/#from-to-protobuf>`.
+          `here <https://docarray.cmon.pw/fundamentals/document/serialization/#from-to-protobuf>`.
           Defaults to retaining whatever type is returned by the Executor.
         :param polling: The polling strategy of the Deployment and its endpoints (when `shards>1`).
               Can be defined for all endpoints of a Deployment or by endpoint.
               Define per Deployment:
               - ANY: only one (whoever is idle) Pod polls the message
               - ALL: all Pods poll the message (like a broadcast)
               Define per Endpoint:
@@ -971,23 +971,23 @@
         :param prefer_platform: The preferred target Docker platform. (e.g. "linux/amd64", "linux/arm64")
         :param protocol: Communication protocol of the server exposed by the Executor. This can be a single value or a list of protocols, depending on your chosen Gateway. Choose the convenient protocols from: ['GRPC', 'HTTP', 'WEBSOCKET'].
         :param py_modules: The customized python modules need to be imported before loading the executor
 
           Note that the recommended way is to only import a single module - a simple python file, if your
           executor can be defined in a single file, or an ``__init__.py`` file if you have multiple files,
           which should be structured as a python package. For more details, please see the
-          `Executor cookbook <https://docs.cmon.ai/concepts/executor/executor-files/>`__
+          `Executor cookbook <https://docs.cmon.pw/concepts/executor/executor-files/>`__
         :param quiet: If set, then no log will be emitted from this object.
         :param quiet_error: If set, then exception stack information will not be added to the log
         :param raft_configuration: Dictionary of kwargs arguments that will be passed to the RAFT node as configuration options when starting the RAFT node.
         :param reload: If set, the Executor will restart while serving if YAML configuration source or Executor modules are changed. If YAML configuration is changed, the whole deployment is reloaded and new processes will be restarted. If only Python modules of the Executor have changed, they will be reloaded to the interpreter without restarting process.
         :param replicas: The number of replicas in the deployment
         :param retries: Number of retries per gRPC call. If <0 it defaults to max(3, num_replicas)
         :param runtime_cls: The runtime class to run inside the Pod
-        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.ai/concepts/flow/create-flow/#complex-flow-topologies
+        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.pw/concepts/flow/create-flow/#complex-flow-topologies
         :param ssl_certfile: the path to the certificate file
         :param ssl_keyfile: the path to the key file
         :param stateful: If set, start consensus module to make sure write operations are properly replicated between all the replicas
         :param timeout_ctrl: The timeout in milliseconds of the control request, -1 for waiting forever
         :param timeout_ready: The timeout in milliseconds of a Pod waits for the runtime to be ready, -1 for waiting forever
         :param timeout_send: The timeout in milliseconds used when sending data requests to Executors, -1 means no timeout, disabled by default
         :param title: The title of this HTTP server. It will be used in automatics docs such as Swagger UI.
@@ -1019,15 +1019,15 @@
           More details can be found in Uvicorn docs: https://www.uvicorn.org/settings/
         :param volumes: The path on the host to be mounted inside the container.
 
           Note,
           - If separated by `:`, then the first part will be considered as the local host path and the second part is the path in the container system.
           - If no split provided, then the basename of that directory will be mounted into container's root path, e.g. `--volumes="/user/test/my-workspace"` will be mounted into `/my-workspace` inside the container.
           - All volumes are mounted with read-write mode.
-        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `DocArray query condition <https://docarray.cmon.ai/fundamentals/documentarray/find/#query-by-conditions>`
+        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `docarray query condition <https://docarray.cmon.pw/fundamentals/documentarray/find/#query-by-conditions>`
         :param workspace: The working directory for any IO operations in this object. If not set, then derive from its parent `workspace`.
         :return: a (new) Flow object with modification
 
         .. # noqa: DAR202
         .. # noqa: DAR101
         .. # noqa: DAR003
         """
@@ -1115,15 +1115,15 @@
 
               When not given, then the default naming strategy will apply.
         :param native: If set, only native Executors is allowed, and the Executor is always run inside WorkerRuntime.
         :param no_reduce: Disable the built-in reduction mechanism. Set this if the reduction is to be handled by the Executor itself by operating on a `docs_matrix` or `docs_map`
         :param output_array_type: The type of array `tensor` and `embedding` will be serialized to.
 
           Supports the same types as `docarray.to_protobuf(.., ndarray_type=...)`, which can be found
-          `here <https://docarray.cmon.ai/fundamentals/document/serialization/#from-to-protobuf>`.
+          `here <https://docarray.cmon.pw/fundamentals/document/serialization/#from-to-protobuf>`.
           Defaults to retaining whatever type is returned by the Executor.
         :param polling: The polling strategy of the Deployment and its endpoints (when `shards>1`).
               Can be defined for all endpoints of a Deployment or by endpoint.
               Define per Deployment:
               - ANY: only one (whoever is idle) Pod polls the message
               - ALL: all Pods poll the message (like a broadcast)
               Define per Endpoint:
@@ -1134,23 +1134,23 @@
         :param prefer_platform: The preferred target Docker platform. (e.g. "linux/amd64", "linux/arm64")
         :param protocol: Communication protocol of the server exposed by the Executor. This can be a single value or a list of protocols, depending on your chosen Gateway. Choose the convenient protocols from: ['GRPC', 'HTTP', 'WEBSOCKET'].
         :param py_modules: The customized python modules need to be imported before loading the executor
 
           Note that the recommended way is to only import a single module - a simple python file, if your
           executor can be defined in a single file, or an ``__init__.py`` file if you have multiple files,
           which should be structured as a python package. For more details, please see the
-          `Executor cookbook <https://docs.cmon.ai/concepts/executor/executor-files/>`__
+          `Executor cookbook <https://docs.cmon.pw/concepts/executor/executor-files/>`__
         :param quiet: If set, then no log will be emitted from this object.
         :param quiet_error: If set, then exception stack information will not be added to the log
         :param raft_configuration: Dictionary of kwargs arguments that will be passed to the RAFT node as configuration options when starting the RAFT node.
         :param reload: If set, the Executor will restart while serving if YAML configuration source or Executor modules are changed. If YAML configuration is changed, the whole deployment is reloaded and new processes will be restarted. If only Python modules of the Executor have changed, they will be reloaded to the interpreter without restarting process.
         :param replicas: The number of replicas in the deployment
         :param retries: Number of retries per gRPC call. If <0 it defaults to max(3, num_replicas)
         :param runtime_cls: The runtime class to run inside the Pod
-        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.ai/concepts/flow/create-flow/#complex-flow-topologies
+        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.pw/concepts/flow/create-flow/#complex-flow-topologies
         :param ssl_certfile: the path to the certificate file
         :param ssl_keyfile: the path to the key file
         :param stateful: If set, start consensus module to make sure write operations are properly replicated between all the replicas
         :param timeout_ctrl: The timeout in milliseconds of the control request, -1 for waiting forever
         :param timeout_ready: The timeout in milliseconds of a Pod waits for the runtime to be ready, -1 for waiting forever
         :param timeout_send: The timeout in milliseconds used when sending data requests to Executors, -1 means no timeout, disabled by default
         :param title: The title of this HTTP server. It will be used in automatics docs such as Swagger UI.
@@ -1182,15 +1182,15 @@
           More details can be found in Uvicorn docs: https://www.uvicorn.org/settings/
         :param volumes: The path on the host to be mounted inside the container.
 
           Note,
           - If separated by `:`, then the first part will be considered as the local host path and the second part is the path in the container system.
           - If no split provided, then the basename of that directory will be mounted into container's root path, e.g. `--volumes="/user/test/my-workspace"` will be mounted into `/my-workspace` inside the container.
           - All volumes are mounted with read-write mode.
-        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `DocArray query condition <https://docarray.cmon.ai/fundamentals/documentarray/find/#query-by-conditions>`
+        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `docarray query condition <https://docarray.cmon.pw/fundamentals/documentarray/find/#query-by-conditions>`
         :param workspace: The working directory for any IO operations in this object. If not set, then derive from its parent `workspace`.
         :param needs: the name of the Deployment(s) that this Deployment receives data from. One can also use "gateway" to indicate the connection with the gateway.
         :param deployment_role: the role of the Deployment, used for visualization and route planning
         :param copy_flow: when set to true, then always copy the current Flow and do the modification on top of it then return, otherwise, do in-line modification
         :param kwargs: other keyword-value arguments that the Deployment CLI supports
         :return: a (new) Flow object with modification
         :return: a (new) Flow object with modification
@@ -2003,15 +2003,15 @@
             )  # can't use logger here see : https://github.com/Textualize/rich/discussions/2024
             self.logger.debug(
                 f'{self.num_deployments} Deployments (i.e. {self.num_pods} Pods) are running in this Flow'
             )
 
             if 'CMON_HIDE_SURVEY' not in os.environ:
                 print(
-                    'Do you love open source? Help us improve [link=https://github.com/cmon-ai/cmon]Cmon[/link] in just 1 minute and 30 seconds by taking our survey: https://10sw1tcpld4.typeform.com/cmonsurveyfeb23?utm_source=cmon '
+                    'Do you love open source? Help us improve [link=https://github.com/cmon.pw/cmon]Cmon[/link] in just 1 minute and 30 seconds by taking our survey: https://10sw1tcpld4.typeform.com/cmonsurveyfeb23?utm_source=cmon '
                     '(Set environment variable CMON_HIDE_SURVEY=1 to hide this message.)'
                 )
 
     @property
     def num_deployments(self) -> int:
         """Get the number of Deployments in this Flow
```

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/flow/builder.py` & `cmon-ai-0.42.6/cmon/orchestrate/flow/builder.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/helper.py` & `cmon-ai-0.42.6/cmon/orchestrate/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/orchestrator.py` & `cmon-ai-0.42.6/cmon/orchestrate/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/pods/__init__.py` & `cmon-ai-0.42.6/cmon/orchestrate/pods/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/pods/container.py` & `cmon-ai-0.42.6/cmon/orchestrate/pods/container.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/pods/container_helper.py` & `cmon-ai-0.42.6/cmon/orchestrate/pods/container_helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/pods/factory.py` & `cmon-ai-0.42.6/cmon/orchestrate/pods/factory.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/orchestrate/pods/helper.py` & `cmon-ai-0.42.6/cmon/orchestrate/pods/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/__init__.py` & `cmon-ai-0.42.6/cmon/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/base.py` & `cmon-ai-0.42.6/cmon/parsers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     :return: the parser
     """
     from cmon import __version__
     from cmon.helper import colored, format_full_version_info, get_full_version
 
     # create the top-level parser
     urls = {
-        'Code': ('💻', 'https://oss.cmon.ai'),
-        'Docs': ('📖', 'https://docs.cmon.ai'),
-        'Help': ('💬', 'https://discord.cmon.ai'),
-        'Hiring!': ('🙌', 'https://jobs.cmon.ai'),
+        'Code': ('💻', 'https://oss.cmon.pw'),
+        'Docs': ('📖', 'https://docs.cmon.pw'),
+        'Help': ('💬', 'https://discord.cmon.pw'),
+        'Hiring!': ('🙌', 'https://jobs.cmon.pw'),
     }
     url_str = '\n'.join(
         f'- {v[0]:<10} {k:10.10}\t{colored(v[1], "cyan", attrs=["underline"])}'
         for k, v in urls.items()
     )
 
     parser = argparse.ArgumentParser(
```

### Comparing `cmon-ai-0.38.5/cmon/parsers/client.py` & `cmon-ai-0.42.6/cmon/parsers/client.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/create.py` & `cmon-ai-0.42.6/cmon/parsers/create.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/deprecated.py` & `cmon-ai-0.42.6/cmon/parsers/deprecated.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/export.py` & `cmon-ai-0.42.6/cmon/parsers/export.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/flow.py` & `cmon-ai-0.42.6/cmon/parsers/flow.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/helper.py` & `cmon-ai-0.42.6/cmon/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/base.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     )
 
     gp.add_argument(
         '--shards',
         type=int,
         default=1,
         help='The number of shards in the deployment running at the same time. For more details check '
-        'https://docs.cmon.ai/concepts/flow/create-flow/#complex-flow-topologies',
+        'https://docs.cmon.pw/concepts/flow/create-flow/#complex-flow-topologies',
     )
 
     gp.add_argument(
         '--replicas',
         type=int,
         default=1,
         help='The number of replicas in the deployment',
```

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/deployment.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     gp.add_argument(
         '--when',
         action=KVAppendAction,
         metavar='KEY: VALUE',
         nargs='*',
         help='The condition that the documents need to fulfill before reaching the Executor.'
-        'The condition can be defined in the form of a `DocArray query condition <https://docarray.cmon.ai/fundamentals/documentarray/find/#query-by-conditions>`',
+        'The condition can be defined in the form of a `docarray query condition <https://docarray.cmon.pw/fundamentals/documentarray/find/#query-by-conditions>`',
     )
 
     gp.add_argument(
         '--external',
         action='store_true',
         default=False,
         help='The Deployment will be considered an external Deployment that has been started independently from the Flow.'
```

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/pod.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/pod.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/container.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/container.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/grpc_channel.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/grpc_channel.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/head.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/head.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/remote.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/remote.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/runtime.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/runtime.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/parsers/orchestrate/runtimes/worker.py` & `cmon-ai-0.42.6/cmon/parsers/orchestrate/runtimes/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,27 +79,27 @@
         metavar='PATH',
         help='''
 The customized python modules need to be imported before loading the executor
 
 Note that the recommended way is to only import a single module - a simple python file, if your
 executor can be defined in a single file, or an ``__init__.py`` file if you have multiple files,
 which should be structured as a python package. For more details, please see the
-`Executor cookbook <https://docs.cmon.ai/concepts/executor/executor-files/>`__
+`Executor cookbook <https://docs.cmon.pw/concepts/executor/executor-files/>`__
 ''',
     )
 
     gp.add_argument(
         '--output-array-type',
         type=str,
         default=None,
         help='''
 The type of array `tensor` and `embedding` will be serialized to.
 
 Supports the same types as `docarray.to_protobuf(.., ndarray_type=...)`, which can be found 
-`here <https://docarray.cmon.ai/fundamentals/document/serialization/#from-to-protobuf>`.
+`here <https://docarray.cmon.pw/fundamentals/document/serialization/#from-to-protobuf>`.
 Defaults to retaining whatever type is returned by the Executor.
 ''',
     )
 
     gp.add_argument(
         '--exit-on-exceptions',
         type=str,
```

### Comparing `cmon-ai-0.38.5/cmon/parsers/ping.py` & `cmon-ai-0.42.6/cmon/parsers/ping.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v1/pb/cmon_pb2.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v1/pb/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v1/pb/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v1/pb2/cmon_pb2.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v1/pb2/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v1/pb2/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v2/pb/cmon_pb2.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v2/pb/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v2/pb/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v2/pb2/cmon_pb2.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v2/pb2/cmon_pb2.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py` & `cmon-ai-0.42.6/cmon/proto/docarray_v2/pb2/cmon_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/proto/serializer.py` & `cmon-ai-0.42.6/cmon/proto/serializer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/Python.gitignore` & `cmon-ai-0.42.6/cmon/resources/Python.gitignore`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/ci-vendors.json` & `cmon-ai-0.42.6/cmon/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/completions/cmon.bash` & `cmon-ai-0.42.6/cmon/resources/completions/cmon.bash`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/completions/cmon.fish` & `cmon-ai-0.42.6/cmon/resources/completions/cmon.fish`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/extra-requirements.txt` & `cmon-ai-0.42.6/cmon/resources/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/health_check/gateway.py` & `cmon-ai-0.42.6/cmon/resources/health_check/gateway.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/health_check/pod.py` & `cmon-ai-0.42.6/cmon/resources/health_check/pod.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-executor.yml` & `cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-executor.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-gateway.yml` & `cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-gateway.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-uses-after.yml` & `cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-uses-after.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-uses-before-after.yml` & `cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-uses-before-after.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/k8s/template/deployment-uses-before.yml` & `cmon-ai-0.42.6/cmon/resources/k8s/template/deployment-uses-before.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/k8s/template/statefulset-executor.yml` & `cmon-ai-0.42.6/cmon/resources/k8s/template/statefulset-executor.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/logging.default.yml` & `cmon-ai-0.42.6/cmon/resources/logging.default.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/logging.docker.yml` & `cmon-ai-0.42.6/cmon/resources/logging.docker.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/logging.quiet.yml` & `cmon-ai-0.42.6/cmon/resources/logging.quiet.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/resources/logging.remote.yml` & `cmon-ai-0.42.6/cmon/resources/logging.remote.yml`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/schemas/__init__.py` & `cmon-ai-0.42.6/cmon/schemas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         schema_metas,
         schema_deployment,
         IMPORTED.schema_executors,
     ]:
         definitions.update(s)
 
     return {
-        '$id': f'https://api.cmon.ai/schemas/{__version__}.json',
+        '$id': f'https://api.cmon.pw/schemas/{__version__}.json',
         '$schema': 'http://json-schema.org/draft-07/schema#',
         'description': 'The YAML schema of Cmon objects (Flow, Executor).',
         'type': 'object',
         'oneOf': [{'$ref': '#/definitions/Cmon::Flow'}]
         + [{"$ref": f"#/definitions/{k}"} for k in IMPORTED.schema_executors.keys()],
         'definitions': definitions,
     }
```

### Comparing `cmon-ai-0.38.5/cmon/schemas/deployment.py` & `cmon-ai-0.42.6/cmon/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/schemas/flow.py` & `cmon-ai-0.42.6/cmon/schemas/flow.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/schemas/helper.py` & `cmon-ai-0.42.6/cmon/schemas/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/schemas/meta.py` & `cmon-ai-0.42.6/cmon/schemas/meta.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/README.md` & `cmon-ai-0.42.6/cmon/serve/consensus/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Raft implementation for Cmon Docarray
+# Raft implementation for Cmon docarray
 
 ## Setup Go
 
 The default project and folder setup is for the Go project files. Install the Go version >= 1.19. To install all dependencies run:
 
 ```shell
 go get
```

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/add_voter.go` & `cmon-ai-0.42.6/cmon/serve/consensus/add_voter.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon-go-proto/cmon.pb.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon-go-proto/cmon.pb.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon-go-proto/cmon_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon.proto` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon.proto`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/cmonraft.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/cmonraft.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/executor_connection.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/executor_connection.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/fsm.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/fsm.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/rpc.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/rpc.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/cmon_raft/snapshot.go` & `cmon-ai-0.42.6/cmon/serve/consensus/cmon_raft/snapshot.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/docarray-go-proto/docarray.pb.go` & `cmon-ai-0.42.6/cmon/serve/consensus/docarray-go-proto/docarray.pb.go`

 * *Files 2% similar despite different names*

```diff
@@ -257,23 +257,23 @@
 	//	*NodeProto_Text
 	//	*NodeProto_Integer
 	//	*NodeProto_Float
 	//	*NodeProto_Boolean
 	//	*NodeProto_Blob
 	//	*NodeProto_Ndarray
 	//	*NodeProto_Doc
-	//	*NodeProto_DocArray
+	//	*NodeProto_docarray
 	//	*NodeProto_List
 	//	*NodeProto_Set
 	//	*NodeProto_Tuple
 	//	*NodeProto_Dict
 	Content isNodeProto_Content `protobuf_oneof:"content"`
-	// Types that are assignable to DocarrayType:
+	// Types that are assignable to docarrayType:
 	//	*NodeProto_Type
-	DocarrayType isNodeProto_DocarrayType `protobuf_oneof:"docarray_type"`
+	docarrayType isNodeProto_docarrayType `protobuf_oneof:"docarray_type"`
 }
 
 func (x *NodeProto) Reset() {
 	*x = NodeProto{}
 	if protoimpl.UnsafeEnabled {
 		mi := &file_docarray_proto_msgTypes[4]
 		ms := protoimpl.X.MessageStateOf(protoimpl.Pointer(x))
@@ -356,17 +356,17 @@
 func (x *NodeProto) GetDoc() *DocProto {
 	if x, ok := x.GetContent().(*NodeProto_Doc); ok {
 		return x.Doc
 	}
 	return nil
 }
 
-func (x *NodeProto) GetDocArray() *DocListProto {
-	if x, ok := x.GetContent().(*NodeProto_DocArray); ok {
-		return x.DocArray
+func (x *NodeProto) Getdocarray() *DocListProto {
+	if x, ok := x.GetContent().(*NodeProto_docarray); ok {
+		return x.docarray
 	}
 	return nil
 }
 
 func (x *NodeProto) GetList() *ListOfAnyProto {
 	if x, ok := x.GetContent().(*NodeProto_List); ok {
 		return x.List
@@ -391,23 +391,23 @@
 func (x *NodeProto) GetDict() *DictOfAnyProto {
 	if x, ok := x.GetContent().(*NodeProto_Dict); ok {
 		return x.Dict
 	}
 	return nil
 }
 
-func (m *NodeProto) GetDocarrayType() isNodeProto_DocarrayType {
+func (m *NodeProto) GetdocarrayType() isNodeProto_docarrayType {
 	if m != nil {
-		return m.DocarrayType
+		return m.docarrayType
 	}
 	return nil
 }
 
 func (x *NodeProto) GetType() string {
-	if x, ok := x.GetDocarrayType().(*NodeProto_Type); ok {
+	if x, ok := x.GetdocarrayType().(*NodeProto_Type); ok {
 		return x.Type
 	}
 	return ""
 }
 
 type isNodeProto_Content interface {
 	isNodeProto_Content()
@@ -444,17 +444,17 @@
 }
 
 type NodeProto_Doc struct {
 	// a sub Document
 	Doc *DocProto `protobuf:"bytes,7,opt,name=doc,proto3,oneof"`
 }
 
-type NodeProto_DocArray struct {
-	// a sub DocArray
-	DocArray *DocListProto `protobuf:"bytes,8,opt,name=doc_array,json=docArray,proto3,oneof"`
+type NodeProto_docarray struct {
+	// a sub docarray
+	docarray *DocListProto `protobuf:"bytes,8,opt,name=doc_array,json=docarray,proto3,oneof"`
 }
 
 type NodeProto_List struct {
 	//any list
 	List *ListOfAnyProto `protobuf:"bytes,9,opt,name=list,proto3,oneof"`
 }
 
@@ -483,33 +483,33 @@
 
 func (*NodeProto_Blob) isNodeProto_Content() {}
 
 func (*NodeProto_Ndarray) isNodeProto_Content() {}
 
 func (*NodeProto_Doc) isNodeProto_Content() {}
 
-func (*NodeProto_DocArray) isNodeProto_Content() {}
+func (*NodeProto_docarray) isNodeProto_Content() {}
 
 func (*NodeProto_List) isNodeProto_Content() {}
 
 func (*NodeProto_Set) isNodeProto_Content() {}
 
 func (*NodeProto_Tuple) isNodeProto_Content() {}
 
 func (*NodeProto_Dict) isNodeProto_Content() {}
 
-type isNodeProto_DocarrayType interface {
-	isNodeProto_DocarrayType()
+type isNodeProto_docarrayType interface {
+	isNodeProto_docarrayType()
 }
 
 type NodeProto_Type struct {
 	Type string `protobuf:"bytes,13,opt,name=type,proto3,oneof"`
 }
 
-func (*NodeProto_Type) isNodeProto_DocarrayType() {}
+func (*NodeProto_Type) isNodeProto_docarrayType() {}
 
 //*
 // Represents a Document
 type DocProto struct {
 	state         protoimpl.MessageState
 	sizeCache     protoimpl.SizeCache
 	unknownFields protoimpl.UnknownFields
@@ -693,69 +693,69 @@
 func (x *DocListProto) GetDocs() []*DocProto {
 	if x != nil {
 		return x.Docs
 	}
 	return nil
 }
 
-type ListOfDocArrayProto struct {
+type ListOfdocarrayProto struct {
 	state         protoimpl.MessageState
 	sizeCache     protoimpl.SizeCache
 	unknownFields protoimpl.UnknownFields
 
 	Data []*DocListProto `protobuf:"bytes,1,rep,name=data,proto3" json:"data,omitempty"`
 }
 
-func (x *ListOfDocArrayProto) Reset() {
-	*x = ListOfDocArrayProto{}
+func (x *ListOfdocarrayProto) Reset() {
+	*x = ListOfdocarrayProto{}
 	if protoimpl.UnsafeEnabled {
 		mi := &file_docarray_proto_msgTypes[9]
 		ms := protoimpl.X.MessageStateOf(protoimpl.Pointer(x))
 		ms.StoreMessageInfo(mi)
 	}
 }
 
-func (x *ListOfDocArrayProto) String() string {
+func (x *ListOfdocarrayProto) String() string {
 	return protoimpl.X.MessageStringOf(x)
 }
 
-func (*ListOfDocArrayProto) ProtoMessage() {}
+func (*ListOfdocarrayProto) ProtoMessage() {}
 
-func (x *ListOfDocArrayProto) ProtoReflect() protoreflect.Message {
+func (x *ListOfdocarrayProto) ProtoReflect() protoreflect.Message {
 	mi := &file_docarray_proto_msgTypes[9]
 	if protoimpl.UnsafeEnabled && x != nil {
 		ms := protoimpl.X.MessageStateOf(protoimpl.Pointer(x))
 		if ms.LoadMessageInfo() == nil {
 			ms.StoreMessageInfo(mi)
 		}
 		return ms
 	}
 	return mi.MessageOf(x)
 }
 
-// Deprecated: Use ListOfDocArrayProto.ProtoReflect.Descriptor instead.
-func (*ListOfDocArrayProto) Descriptor() ([]byte, []int) {
+// Deprecated: Use ListOfdocarrayProto.ProtoReflect.Descriptor instead.
+func (*ListOfdocarrayProto) Descriptor() ([]byte, []int) {
 	return file_docarray_proto_rawDescGZIP(), []int{9}
 }
 
-func (x *ListOfDocArrayProto) GetData() []*DocListProto {
+func (x *ListOfdocarrayProto) GetData() []*DocListProto {
 	if x != nil {
 		return x.Data
 	}
 	return nil
 }
 
 type DocVecProto struct {
 	state         protoimpl.MessageState
 	sizeCache     protoimpl.SizeCache
 	unknownFields protoimpl.UnknownFields
 
 	TensorColumns  map[string]*NdArrayProto        `protobuf:"bytes,1,rep,name=tensor_columns,json=tensorColumns,proto3" json:"tensor_columns,omitempty" protobuf_key:"bytes,1,opt,name=key,proto3" protobuf_val:"bytes,2,opt,name=value,proto3"`      // a dict of document columns
 	DocColumns     map[string]*DocVecProto         `protobuf:"bytes,2,rep,name=doc_columns,json=docColumns,proto3" json:"doc_columns,omitempty" protobuf_key:"bytes,1,opt,name=key,proto3" protobuf_val:"bytes,2,opt,name=value,proto3"`               // a dict of tensor columns
-	DocsVecColumns map[string]*ListOfDocArrayProto `protobuf:"bytes,3,rep,name=docs_vec_columns,json=docsVecColumns,proto3" json:"docs_vec_columns,omitempty" protobuf_key:"bytes,1,opt,name=key,proto3" protobuf_val:"bytes,2,opt,name=value,proto3"` // a dict of document array columns
+	DocsVecColumns map[string]*ListOfdocarrayProto `protobuf:"bytes,3,rep,name=docs_vec_columns,json=docsVecColumns,proto3" json:"docs_vec_columns,omitempty" protobuf_key:"bytes,1,opt,name=key,proto3" protobuf_val:"bytes,2,opt,name=value,proto3"` // a dict of document array columns
 	AnyColumns     map[string]*ListOfAnyProto      `protobuf:"bytes,4,rep,name=any_columns,json=anyColumns,proto3" json:"any_columns,omitempty" protobuf_key:"bytes,1,opt,name=key,proto3" protobuf_val:"bytes,2,opt,name=value,proto3"`               // a dict of any columns. Used for the rest of the data
 }
 
 func (x *DocVecProto) Reset() {
 	*x = DocVecProto{}
 	if protoimpl.UnsafeEnabled {
 		mi := &file_docarray_proto_msgTypes[10]
@@ -797,15 +797,15 @@
 func (x *DocVecProto) GetDocColumns() map[string]*DocVecProto {
 	if x != nil {
 		return x.DocColumns
 	}
 	return nil
 }
 
-func (x *DocVecProto) GetDocsVecColumns() map[string]*ListOfDocArrayProto {
+func (x *DocVecProto) GetDocsVecColumns() map[string]*ListOfdocarrayProto {
 	if x != nil {
 		return x.DocsVecColumns
 	}
 	return nil
 }
 
 func (x *DocVecProto) GetAnyColumns() map[string]*ListOfAnyProto {
@@ -975,15 +975,15 @@
 	(*KeyValuePair)(nil),        // 2: docarray.KeyValuePair
 	(*GenericDictValue)(nil),    // 3: docarray.GenericDictValue
 	(*NodeProto)(nil),           // 4: docarray.NodeProto
 	(*DocProto)(nil),            // 5: docarray.DocProto
 	(*DictOfAnyProto)(nil),      // 6: docarray.DictOfAnyProto
 	(*ListOfAnyProto)(nil),      // 7: docarray.ListOfAnyProto
 	(*DocListProto)(nil),        // 8: docarray.DocListProto
-	(*ListOfDocArrayProto)(nil), // 9: docarray.ListOfDocArrayProto
+	(*ListOfdocarrayProto)(nil), // 9: docarray.ListOfdocarrayProto
 	(*DocVecProto)(nil),         // 10: docarray.DocVecProto
 	nil,                         // 11: docarray.DocProto.DataEntry
 	nil,                         // 12: docarray.DictOfAnyProto.DataEntry
 	nil,                         // 13: docarray.DocVecProto.TensorColumnsEntry
 	nil,                         // 14: docarray.DocVecProto.DocColumnsEntry
 	nil,                         // 15: docarray.DocVecProto.DocsVecColumnsEntry
 	nil,                         // 16: docarray.DocVecProto.AnyColumnsEntry
@@ -1003,24 +1003,24 @@
 	7,  // 9: docarray.NodeProto.set:type_name -> docarray.ListOfAnyProto
 	7,  // 10: docarray.NodeProto.tuple:type_name -> docarray.ListOfAnyProto
 	6,  // 11: docarray.NodeProto.dict:type_name -> docarray.DictOfAnyProto
 	11, // 12: docarray.DocProto.data:type_name -> docarray.DocProto.DataEntry
 	12, // 13: docarray.DictOfAnyProto.data:type_name -> docarray.DictOfAnyProto.DataEntry
 	4,  // 14: docarray.ListOfAnyProto.data:type_name -> docarray.NodeProto
 	5,  // 15: docarray.DocListProto.docs:type_name -> docarray.DocProto
-	8,  // 16: docarray.ListOfDocArrayProto.data:type_name -> docarray.DocListProto
+	8,  // 16: docarray.ListOfdocarrayProto.data:type_name -> docarray.DocListProto
 	13, // 17: docarray.DocVecProto.tensor_columns:type_name -> docarray.DocVecProto.TensorColumnsEntry
 	14, // 18: docarray.DocVecProto.doc_columns:type_name -> docarray.DocVecProto.DocColumnsEntry
 	15, // 19: docarray.DocVecProto.docs_vec_columns:type_name -> docarray.DocVecProto.DocsVecColumnsEntry
 	16, // 20: docarray.DocVecProto.any_columns:type_name -> docarray.DocVecProto.AnyColumnsEntry
 	4,  // 21: docarray.DocProto.DataEntry.value:type_name -> docarray.NodeProto
 	4,  // 22: docarray.DictOfAnyProto.DataEntry.value:type_name -> docarray.NodeProto
 	1,  // 23: docarray.DocVecProto.TensorColumnsEntry.value:type_name -> docarray.NdArrayProto
 	10, // 24: docarray.DocVecProto.DocColumnsEntry.value:type_name -> docarray.DocVecProto
-	9,  // 25: docarray.DocVecProto.DocsVecColumnsEntry.value:type_name -> docarray.ListOfDocArrayProto
+	9,  // 25: docarray.DocVecProto.DocsVecColumnsEntry.value:type_name -> docarray.ListOfdocarrayProto
 	7,  // 26: docarray.DocVecProto.AnyColumnsEntry.value:type_name -> docarray.ListOfAnyProto
 	27, // [27:27] is the sub-list for method output_type
 	27, // [27:27] is the sub-list for method input_type
 	27, // [27:27] is the sub-list for extension type_name
 	27, // [27:27] is the sub-list for extension extendee
 	0,  // [0:27] is the sub-list for field type_name
 }
@@ -1136,15 +1136,15 @@
 			case 2:
 				return &v.unknownFields
 			default:
 				return nil
 			}
 		}
 		file_docarray_proto_msgTypes[9].Exporter = func(v interface{}, i int) interface{} {
-			switch v := v.(*ListOfDocArrayProto); i {
+			switch v := v.(*ListOfdocarrayProto); i {
 			case 0:
 				return &v.state
 			case 1:
 				return &v.sizeCache
 			case 2:
 				return &v.unknownFields
 			default:
@@ -1168,15 +1168,15 @@
 		(*NodeProto_Text)(nil),
 		(*NodeProto_Integer)(nil),
 		(*NodeProto_Float)(nil),
 		(*NodeProto_Boolean)(nil),
 		(*NodeProto_Blob)(nil),
 		(*NodeProto_Ndarray)(nil),
 		(*NodeProto_Doc)(nil),
-		(*NodeProto_DocArray)(nil),
+		(*NodeProto_docarray)(nil),
 		(*NodeProto_List)(nil),
 		(*NodeProto_Set)(nil),
 		(*NodeProto_Tuple)(nil),
 		(*NodeProto_Dict)(nil),
 		(*NodeProto_Type)(nil),
 	}
 	type x struct{}
```

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/docarray.proto` & `cmon-ai-0.42.6/cmon/serve/consensus/docarray.proto`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     bool boolean = 4;
     // a bytes representation
     bytes blob = 5;
     // the ndarray of the image/audio/video document
     NdArrayProto ndarray = 6;
     // a sub Document
     DocProto doc = 7;
-    // a sub DocArray
+    // a sub docarray
     DocListProto doc_array = 8;
     //any list
     ListOfAnyProto list = 9;
     //any set
     ListOfAnyProto set = 10;
     //any tuple
     ListOfAnyProto tuple = 11;
@@ -94,17 +94,17 @@
 }
 
 message DocListProto {
   repeated DocProto docs = 1; // a list of Documents
 }
 
 
-message ListOfDocArrayProto {
+message ListOfdocarrayProto {
   repeated DocListProto data = 1;
 }
 
 message DocVecProto{
   map<string, NdArrayProto> tensor_columns = 1; // a dict of document columns
   map<string, DocVecProto> doc_columns = 2; // a dict of tensor columns
-  map<string, ListOfDocArrayProto> docs_vec_columns = 3; // a dict of document array columns
+  map<string, ListOfdocarrayProto> docs_vec_columns = 3; // a dict of document array columns
   map<string, ListOfAnyProto> any_columns = 4; // a dict of any columns. Used for the rest of the data
 }
```

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/go.mod` & `cmon-ai-0.42.6/cmon/serve/consensus/go.mod`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/go.sum` & `cmon-ai-0.42.6/cmon/serve/consensus/go.sum`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/jraft.go` & `cmon-ai-0.42.6/cmon/serve/consensus/jraft.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/jraft.h` & `cmon-ai-0.42.6/cmon/serve/consensus/jraft.h`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/run.go` & `cmon-ai-0.42.6/cmon/serve/consensus/run.go`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/consensus/scripts/protogen.sh` & `cmon-ai-0.42.6/cmon/serve/consensus/scripts/protogen.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #/bin/sh
 
 set -e
 
 # This script is used to generate gRPC client stubs from the proto files.
 
 GO_MODULE="jraft"
-DOCARRAY_PROTO="docarray.proto"
-DOCARRAY_DIR="../../docarray"
-DOCARRAY_PACKAGE="$GO_MODULE/docarray"
+docarray_PROTO="docarray.proto"
+docarray_DIR="../../docarray"
+docarray_PACKAGE="$GO_MODULE/docarray"
 
 CMON_PROTO="cmon.proto"
 CMON_DIR="../../cmon"
 CMON_PACKAGE="$GO_MODULE/cmon-go-proto"
 
 
 cd cmon/proto
 if ! $(grep -q '^option go_package = ' docarray.proto);then
-       awk '/package docarray;/{print; print "option go_package = \"'${DOCARRAY_PACKAGE}'\";";next}1' docarray.proto > temp.proto
+       awk '/package docarray;/{print; print "option go_package = \"'${docarray_PACKAGE}'\";";next}1' docarray.proto > temp.proto
        mv temp.proto docarray.proto
 fi
-protoc --go_out=${DOCARRAY_DIR} \
+protoc --go_out=${docarray_DIR} \
        --go_opt=paths=source_relative \
-       --go_opt=M${DOCARRAY_PROTO}=${DOCARRAY_PACKAGE} \
-       --go-grpc_out=${DOCARRAY_DIR} \
+       --go_opt=M${docarray_PROTO}=${docarray_PACKAGE} \
+       --go-grpc_out=${docarray_DIR} \
        --go-grpc_opt=paths=source_relative \
        --experimental_allow_proto3_optional \
-       ${DOCARRAY_PROTO} 
+       ${docarray_PROTO} 
 
 if ! $(grep -q '^option go_package = ' cmon.proto);then
        awk '/package cmon;/{print; print "option go_package = \"'${CMON_PACKAGE}'\";";next}1' cmon.proto > temp.proto
        mv temp.proto cmon.proto
 fi
 protoc --go_out=${CMON_DIR} \
        --go_opt=paths=source_relative \
```

### Comparing `cmon-ai-0.38.5/cmon/serve/executors/__init__.py` & `cmon-ai-0.42.6/cmon/serve/executors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,15 +793,15 @@
 
               When not given, then the default naming strategy will apply.
         :param native: If set, only native Executors is allowed, and the Executor is always run inside WorkerRuntime.
         :param no_reduce: Disable the built-in reduction mechanism. Set this if the reduction is to be handled by the Executor itself by operating on a `docs_matrix` or `docs_map`
         :param output_array_type: The type of array `tensor` and `embedding` will be serialized to.
 
           Supports the same types as `docarray.to_protobuf(.., ndarray_type=...)`, which can be found
-          `here <https://docarray.cmon.ai/fundamentals/document/serialization/#from-to-protobuf>`.
+          `here <https://docarray.cmon.pw/fundamentals/document/serialization/#from-to-protobuf>`.
           Defaults to retaining whatever type is returned by the Executor.
         :param polling: The polling strategy of the Deployment and its endpoints (when `shards>1`).
               Can be defined for all endpoints of a Deployment or by endpoint.
               Define per Deployment:
               - ANY: only one (whoever is idle) Pod polls the message
               - ALL: all Pods poll the message (like a broadcast)
               Define per Endpoint:
@@ -812,23 +812,23 @@
         :param prefer_platform: The preferred target Docker platform. (e.g. "linux/amd64", "linux/arm64")
         :param protocol: Communication protocol of the server exposed by the Executor. This can be a single value or a list of protocols, depending on your chosen Gateway. Choose the convenient protocols from: ['GRPC', 'HTTP', 'WEBSOCKET'].
         :param py_modules: The customized python modules need to be imported before loading the executor
 
           Note that the recommended way is to only import a single module - a simple python file, if your
           executor can be defined in a single file, or an ``__init__.py`` file if you have multiple files,
           which should be structured as a python package. For more details, please see the
-          `Executor cookbook <https://docs.cmon.ai/concepts/executor/executor-files/>`__
+          `Executor cookbook <https://docs.cmon.pw/concepts/executor/executor-files/>`__
         :param quiet: If set, then no log will be emitted from this object.
         :param quiet_error: If set, then exception stack information will not be added to the log
         :param raft_configuration: Dictionary of kwargs arguments that will be passed to the RAFT node as configuration options when starting the RAFT node.
         :param reload: If set, the Executor will restart while serving if YAML configuration source or Executor modules are changed. If YAML configuration is changed, the whole deployment is reloaded and new processes will be restarted. If only Python modules of the Executor have changed, they will be reloaded to the interpreter without restarting process.
         :param replicas: The number of replicas in the deployment
         :param retries: Number of retries per gRPC call. If <0 it defaults to max(3, num_replicas)
         :param runtime_cls: The runtime class to run inside the Pod
-        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.ai/concepts/flow/create-flow/#complex-flow-topologies
+        :param shards: The number of shards in the deployment running at the same time. For more details check https://docs.cmon.pw/concepts/flow/create-flow/#complex-flow-topologies
         :param ssl_certfile: the path to the certificate file
         :param ssl_keyfile: the path to the key file
         :param stateful: If set, start consensus module to make sure write operations are properly replicated between all the replicas
         :param timeout_ctrl: The timeout in milliseconds of the control request, -1 for waiting forever
         :param timeout_ready: The timeout in milliseconds of a Pod waits for the runtime to be ready, -1 for waiting forever
         :param timeout_send: The timeout in milliseconds used when sending data requests to Executors, -1 means no timeout, disabled by default
         :param title: The title of this HTTP server. It will be used in automatics docs such as Swagger UI.
@@ -860,15 +860,15 @@
           More details can be found in Uvicorn docs: https://www.uvicorn.org/settings/
         :param volumes: The path on the host to be mounted inside the container.
 
           Note,
           - If separated by `:`, then the first part will be considered as the local host path and the second part is the path in the container system.
           - If no split provided, then the basename of that directory will be mounted into container's root path, e.g. `--volumes="/user/test/my-workspace"` will be mounted into `/my-workspace` inside the container.
           - All volumes are mounted with read-write mode.
-        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `DocArray query condition <https://docarray.cmon.ai/fundamentals/documentarray/find/#query-by-conditions>`
+        :param when: The condition that the documents need to fulfill before reaching the Executor.The condition can be defined in the form of a `docarray query condition <https://docarray.cmon.pw/fundamentals/documentarray/find/#query-by-conditions>`
         :param workspace: The working directory for any IO operations in this object. If not set, then derive from its parent `workspace`.
 
         .. # noqa: DAR202
         .. # noqa: DAR101
         .. # noqa: DAR003
         """
 
@@ -891,20 +891,20 @@
         :param uses_metas: dictionary of parameters to overwrite from the default config's metas field
         :param uses_requests: dictionary of parameters to overwrite from the default config's requests field
         :param reload: If set, the Executor reloads the modules as they change
         :param stop_event: a threading event or a multiprocessing event that once set will resume the control Flow
             to main thread.
         :param uses_dynamic_batching: dictionary of parameters to overwrite from the default config's dynamic_batching field
         :param reload: a flag indicating if the Executor should watch the Python files of its implementation to reload the code live while serving.
-        :param kwargs: other kwargs accepted by the Flow, full list can be found `here <https://docs.cmon.ai/api/cmon.orchestrate.flow.base/>`
+        :param kwargs: other kwargs accepted by the Flow, full list can be found `here <https://docs.cmon.pw/api/cmon.orchestrate.flow.base/>`
 
         """
         warnings.warn(
             f'Executor.serve() is no more supported and will be deprecated soon. Use Deployment to serve an Executor instead: '
-            f'https://docs.cmon.ai/concepts/executor/serve/',
+            f'https://docs.cmon.pw/concepts/executor/serve/',
             DeprecationWarning,
         )
         from cmon.orchestrate.deployments import Deployment
 
         dep = Deployment(
             uses=cls,
             uses_with=uses_with,
@@ -949,19 +949,19 @@
         :param output_base_path: The base path where to dump all the yaml files
         :param k8s_namespace: The name of the k8s namespace to set for the configurations. If None, the name of the Flow will be used.
         :param executor_type: The type of Executor. Can be external or shared. External Executors include the Gateway. Shared Executors don't. Defaults to External
         :param uses_with: dictionary of parameters to overwrite from the default config's with field
         :param uses_metas: dictionary of parameters to overwrite from the default config's metas field
         :param uses_requests: dictionary of parameters to overwrite from the default config's requests field
         :param uses_dynamic_batching: dictionary of parameters to overwrite from the default config's dynamic_batching field
-        :param kwargs: other kwargs accepted by the Flow, full list can be found `here <https://docs.cmon.ai/api/cmon.orchestrate.flow.base/>`
+        :param kwargs: other kwargs accepted by the Flow, full list can be found `here <https://docs.cmon.pw/api/cmon.orchestrate.flow.base/>`
         """
         warnings.warn(
             f'Executor.to_kubernetes_yaml() is no more supported and will be deprecated soon. Use Deployment to export kubernetes YAML files: '
-            f'https://docs.cmon.ai/concepts/executor/serve/#serve-via-kubernetes',
+            f'https://docs.cmon.pw/concepts/executor/serve/#serve-via-kubernetes',
             DeprecationWarning,
         )
         from cmon.orchestrate.flow.base import Flow
 
         Flow(**kwargs).add(
             uses=uses,
             uses_with=uses_with,
@@ -997,20 +997,20 @@
         :param output_path: The output path for the yaml file
         :param network_name: The name of the network that will be used by the deployment name
         :param executor_type: The type of Executor. Can be external or shared. External Executors include the Gateway. Shared Executors don't. Defaults to External
         :param uses_with: dictionary of parameters to overwrite from the default config's with field
         :param uses_metas: dictionary of parameters to overwrite from the default config's metas field
         :param uses_requests: dictionary of parameters to overwrite from the default config's requests field
         :param uses_dynamic_batching: dictionary of parameters to overwrite from the default config's requests field
-        :param kwargs: other kwargs accepted by the Flow, full list can be found `here <https://docs.cmon.ai/api/cmon.orchestrate.flow.base/>`
+        :param kwargs: other kwargs accepted by the Flow, full list can be found `here <https://docs.cmon.pw/api/cmon.orchestrate.flow.base/>`
         """
 
         warnings.warn(
             f'Executor.to_docker_compose_yaml() is no more supported and will be deprecated soon. Use Deployment to export docker compose YAML files: '
-            f'https://docs.cmon.ai/concepts/executor/serve/#serve-via-docker-compose',
+            f'https://docs.cmon.pw/concepts/executor/serve/#serve-via-docker-compose',
             DeprecationWarning,
         )
 
         from cmon.orchestrate.flow.base import Flow
 
         f = Flow(**kwargs).add(
             uses=uses,
```

### Comparing `cmon-ai-0.38.5/cmon/serve/executors/decorators.py` & `cmon-ai-0.42.6/cmon/serve/executors/decorators.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/executors/metas.py` & `cmon-ai-0.42.6/cmon/serve/executors/metas.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/executors/run.py` & `cmon-ai-0.42.6/cmon/serve/executors/run.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/helper.py` & `cmon-ai-0.42.6/cmon/serve/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/instrumentation/__init__.py` & `cmon-ai-0.42.6/cmon/serve/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/monitoring.py` & `cmon-ai-0.42.6/cmon/serve/monitoring.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/__init__.py` & `cmon-ai-0.42.6/cmon/serve/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/connection_pool_map.py` & `cmon-ai-0.42.6/cmon/serve/networking/connection_pool_map.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/connection_stub.py` & `cmon-ai-0.42.6/cmon/serve/networking/connection_stub.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/instrumentation.py` & `cmon-ai-0.42.6/cmon/serve/networking/instrumentation.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/replica_list.py` & `cmon-ai-0.42.6/cmon/serve/networking/replica_list.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/sse.py` & `cmon-ai-0.42.6/cmon/serve/networking/sse.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/networking/utils.py` & `cmon-ai-0.42.6/cmon/serve/networking/utils.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/asyncio.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/asyncio.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/async_request_response_handling.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/async_request_response_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/gateway.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/graph/topology_graph.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/graph/topology_graph.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/health_model.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/health_model.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http_fastapi_app.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http_fastapi_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
             if not docarray_v2:
                 from docarray.document.strawberry_type import (
                     JSONScalar,
                     StrawberryDocument,
                     StrawberryDocumentInput,
                 )
             else:
-                raise NotImplementedError('GraphQL is not yet supported for DocArrayV2')
+                raise NotImplementedError('GraphQL is not yet supported for docarrayV2')
 
             async def get_docs_from_endpoint(
                     data, target_executor, parameters, exec_endpoint
             ):
                 req_generator_input = {
                     'data': [asdict(d) for d in data],
                     'target_executor': target_executor,
```

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/http_fastapi_app_docarrayv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
     if expose_graphql_endpoint:
         logger.error(f' GraphQL endpoint is not enabled when using docarray >0.30')
     with ImportExtensions(required=True):
         from fastapi import FastAPI, Response, HTTPException
         from fastapi.middleware.cors import CORSMiddleware
         import pydantic
-    from docarray.base_doc.docarray_response import DocArrayResponse
+    from docarray.base_doc.docarray_response import docarrayResponse
     from docarray import DocList, BaseDoc
 
     from cmon import __version__
 
     app = FastAPI(
         title=title or 'My Cmon Service',
         description=description
@@ -168,15 +168,15 @@
         return header_dict
 
     def add_route(endpoint_path, input_model, output_model, input_doc_list_model=None, output_doc_list_model=None):
         app_kwargs = dict(path=f'/{endpoint_path.strip("/")}',
                           methods=['POST'],
                           summary=f'Endpoint {endpoint_path}',
                           response_model=output_model, )
-        app_kwargs['response_class'] = DocArrayResponse
+        app_kwargs['response_class'] = docarrayResponse
 
         @app.api_route(
             **app_kwargs
         )
         async def post(body: input_model, response: Response):
             docs = DocList[input_doc_list_model](body.data)
             target_executor = None
```

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/models.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
                 PydanticDocumentArray,
                 Dict[str, PydanticDocumentArray],
             ]
         ] = Field(
             None,
             example=[
                 {'text': 'hello, world!'},
-                {'uri': 'https://docs.cmon.ai/_static/logo-light.svg'},
+                {'uri': 'https://docs.cmon.pw/_static/logo-light.svg'},
             ],
             description=DESCRIPTION_DATA,
         )
         target_executor: Optional[str] = Field(
             None,
             example='',
             description=DESCRIPTION_TARGET_EXEC,
```

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/request_handling.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/request_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/streamer.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/streamer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/gateway/websocket_fastapi_app.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/gateway/websocket_fastapi_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                             if request['data'] is not None and 'docs' in request['data']:
                                 req_generator_input['data'] = req_generator_input['data'][
                                     'docs'
                                 ]
                             for data_request in request_generator(**req_generator_input):
                                 yield data_request
                         else:
-                            raise RuntimeError(f' DocArray v2 is not compatible with {WebsocketSubProtocols.JSON} subprotocol')
+                            raise RuntimeError(f' docarray v2 is not compatible with {WebsocketSubProtocols.JSON} subprotocol')
                 elif isinstance(request, bytes):
                     if request == bytes(True):
                         break
                     else:
                         yield DataRequest(request)
 
         try:
```

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/head/request_handling.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/head/request_handling.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/helper.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/monitoring.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/monitoring.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/servers/__init__.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/servers/composite.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/servers/composite.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/servers/grpc.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/servers/grpc.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/servers/http.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/servers/http.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/servers/load_balancer.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/servers/load_balancer.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/servers/websocket.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/servers/websocket.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/worker/batch_queue.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/worker/batch_queue.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/worker/http_fastapi_app.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/worker/http_fastapi_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,17 +74,17 @@
         app_kwargs = dict(
             path=f'/{endpoint_path.strip("/")}',
             methods=['POST'],
             summary=f'Endpoint {endpoint_path}',
             response_model=output_model,
         )
         if docarray_v2:
-            from docarray.base_doc.docarray_response import DocArrayResponse
+            from docarray.base_doc.docarray_response import docarrayResponse
 
-            app_kwargs['response_class'] = DocArrayResponse
+            app_kwargs['response_class'] = docarrayResponse
 
         @app.api_route(**app_kwargs)
         async def post(body: input_model, response: Response):
 
             req = DataRequest()
             if not docarray_v2:
                 req.data.docs = DocumentArray.from_pydantic_model(body.data)
```

### Comparing `cmon-ai-0.38.5/cmon/serve/runtimes/worker/request_handling.py` & `cmon-ai-0.42.6/cmon/serve/runtimes/worker/request_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,15 +739,15 @@
         docs_map = {}
         docs_matrix = []
         for req in requests:
             docs_matrix.append(req.docs)
             docs_map[req.last_executor] = req.docs
 
         # to unify all length=0 DocumentArray (or any other results) will simply considered as None
-        # otherwise, the executor has to handle [None, None, None] or [DocArray(0), DocArray(0), DocArray(0)]
+        # otherwise, the executor has to handle [None, None, None] or [docarray(0), docarray(0), docarray(0)]
         len_r = sum(len(r) for r in docs_matrix)
         if len_r == 0:
             docs_matrix = None
 
         return docs_matrix, docs_map
 
     @staticmethod
```

### Comparing `cmon-ai-0.38.5/cmon/serve/stream/__init__.py` & `cmon-ai-0.42.6/cmon/serve/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/serve/stream/helper.py` & `cmon-ai-0.42.6/cmon/serve/stream/helper.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/types/mixin.py` & `cmon-ai-0.42.6/cmon/types/mixin.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/types/request/__init__.py` & `cmon-ai-0.42.6/cmon/types/request/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/types/request/data.py` & `cmon-ai-0.42.6/cmon/types/request/data.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon/types/request/status.py` & `cmon-ai-0.42.6/cmon/types/request/status.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon_ai.egg-info/PKG-INFO` & `cmon-ai-0.42.6/cmon_ai.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,989 +1,1019 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 636d 6f6e  : 2.1.Name: cmon
-00000020: 2d61 690a 5665 7273 696f 6e3a 2030 2e33  -ai.Version: 0.3
-00000030: 382e 350a 5375 6d6d 6172 793a 2042 7569  8.5.Summary: Bui
-00000040: 6c64 206d 756c 7469 6d6f 6461 6c20 4149  ld multimodal AI
-00000050: 2073 6572 7669 6365 7320 7669 6120 636c   services via cl
-00000060: 6f75 6420 6e61 7469 7665 2074 6563 686e  oud native techn
-00000070: 6f6c 6f67 6965 7320 c2b7 204e 6575 7261  ologies .. Neura
-00000080: 6c20 5365 6172 6368 20c2 b720 4765 6e65  l Search .. Gene
-00000090: 7261 7469 7665 2041 4920 c2b7 204d 4c4f  rative AI .. MLO
-000000a0: 7073 0a48 6f6d 652d 7061 6765 3a20 6874  ps.Home-page: ht
-000000b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000000c0: 2f61 6c69 6e6f 6f72 6979 616e 2f43 6d6f  /alinooriyan/Cmo
-000000d0: 6e2d 4149 0a44 6f77 6e6c 6f61 642d 5552  n-AI.Download-UR
-000000e0: 4c3a 2068 7474 7073 3a2f 2f67 6974 6875  L: https://githu
-000000f0: 622e 636f 6d2f 616c 696e 6f6f 7269 7961  b.com/alinooriya
-00000100: 6e2f 436d 6f6e 2d41 492f 6172 6368 6976  n/Cmon-AI/archiv
-00000110: 652f 7265 6673 2f74 6167 732f 4149 2e7a  e/refs/tags/AI.z
-00000120: 6970 0a41 7574 686f 723a 2043 6d6f 6e20  ip.Author: Cmon 
-00000130: 4149 0a41 7574 686f 722d 656d 6169 6c3a  AI.Author-email:
-00000140: 2068 656c 6c6f 4063 6d6f 6e2e 6169 0a4c   hello@cmon.ai.L
-00000150: 6963 656e 7365 3a20 4170 6163 6865 2032  icense: Apache 2
-00000160: 2e30 0a50 726f 6a65 6374 2d55 524c 3a20  .0.Project-URL: 
-00000170: 446f 6375 6d65 6e74 6174 696f 6e2c 2068  Documentation, h
-00000180: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00000190: 2e70 770a 5072 6f6a 6563 742d 5552 4c3a  .pw.Project-URL:
-000001a0: 2053 6f75 7263 652c 2068 7474 7073 3a2f   Source, https:/
-000001b0: 2f67 6974 6875 622e 636f 6d2f 616c 696e  /github.com/alin
-000001c0: 6f6f 7269 7961 6e2f 636d 6f6e 2d61 692f  ooriyan/cmon-ai/
-000001d0: 0a50 726f 6a65 6374 2d55 524c 3a20 5472  .Project-URL: Tr
-000001e0: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
-000001f0: 6974 6875 622e 636f 6d2f 616c 696e 6f6f  ithub.com/alinoo
-00000200: 7269 7961 6e2f 636d 6f6e 2d61 692f 6973  riyan/cmon-ai/is
-00000210: 7375 6573 0a4b 6579 776f 7264 733a 2063  sues.Keywords: c
-00000220: 6d6f 6e20 636c 6f75 642d 6e61 7469 7665  mon cloud-native
-00000230: 2063 726f 7373 2d6d 6f64 616c 206d 756c   cross-modal mul
-00000240: 7469 6d6f 6461 6c20 6e65 7572 616c 2d73  timodal neural-s
-00000250: 6561 7263 6820 7175 6572 7920 7365 6172  earch query sear
-00000260: 6368 2069 6e64 6578 2065 6c61 7374 6963  ch index elastic
-00000270: 206e 6575 7261 6c2d 6e65 7477 6f72 6b20   neural-network 
-00000280: 656e 636f 6469 6e67 2065 6d62 6564 6469  encoding embeddi
-00000290: 6e67 2073 6572 7669 6e67 2064 6f63 6b65  ng serving docke
-000002a0: 7220 636f 6e74 6169 6e65 7220 696d 6167  r container imag
-000002b0: 6520 7669 6465 6f20 6175 6469 6f20 6465  e video audio de
-000002c0: 6570 2d6c 6561 726e 696e 6720 6d6c 6f70  ep-learning mlop
-000002d0: 730a 436c 6173 7369 6669 6572 3a20 4465  s.Classifier: De
-000002e0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-000002f0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
-00000300: 6f6e 2f53 7461 626c 650a 436c 6173 7369  on/Stable.Classi
-00000310: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000320: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000330: 6f70 6572 730a 436c 6173 7369 6669 6572  opers.Classifier
-00000340: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000350: 6e63 6520 3a3a 2045 6475 6361 7469 6f6e  nce :: Education
-00000360: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-00000370: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000380: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-00000390: 6368 0a43 6c61 7373 6966 6965 723a 2050  ch.Classifier: P
-000003a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000003b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000003c0: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
-000003d0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000003e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000003f0: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
-00000400: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000410: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000420: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
-00000430: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000440: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000450: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-00000460: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000470: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000480: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
-00000490: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000004a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000004b0: 3a3a 2055 6e69 7820 5368 656c 6c0a 436c  :: Unix Shell.Cl
-000004c0: 6173 7369 6669 6572 3a20 456e 7669 726f  assifier: Enviro
-000004d0: 6e6d 656e 7420 3a3a 2043 6f6e 736f 6c65  nment :: Console
-000004e0: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
-000004f0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-00000500: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
-00000510: 6f66 7477 6172 6520 4c69 6365 6e73 650a  oftware License.
-00000520: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000530: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000540: 4f53 2049 6e64 6570 656e 6465 6e74 0a43  OS Independent.C
-00000550: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000560: 203a 3a20 4461 7461 6261 7365 203a 3a20   :: Database :: 
-00000570: 4461 7461 6261 7365 2045 6e67 696e 6573  Database Engines
-00000580: 2f53 6572 7665 7273 0a43 6c61 7373 6966  /Servers.Classif
-00000590: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
-000005a0: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-000005b0: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
-000005c0: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
-000005d0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-000005e0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-000005f0: 2057 5757 2f48 5454 5020 3a3a 2049 6e64   WWW/HTTP :: Ind
-00000600: 6578 696e 672f 5365 6172 6368 0a43 6c61  exing/Search.Cla
-00000610: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000620: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
-00000630: 696e 6565 7269 6e67 203a 3a20 496d 6167  ineering :: Imag
-00000640: 6520 5265 636f 676e 6974 696f 6e0a 436c  e Recognition.Cl
-00000650: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00000660: 3a3a 204d 756c 7469 6d65 6469 6120 3a3a  :: Multimedia ::
-00000670: 2056 6964 656f 0a43 6c61 7373 6966 6965   Video.Classifie
-00000680: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-00000690: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-000006a0: 6e67 0a43 6c61 7373 6966 6965 723a 2054  ng.Classifier: T
-000006b0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-000006c0: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-000006d0: 3a20 4d61 7468 656d 6174 6963 730a 436c  : Mathematics.Cl
-000006e0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-000006f0: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000700: 6c6f 706d 656e 740a 436c 6173 7369 6669  lopment.Classifi
-00000710: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-00000720: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000730: 7420 3a3a 204c 6962 7261 7269 6573 0a43  t :: Libraries.C
-00000740: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000750: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000760: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000770: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
-00000780: 4d6f 6475 6c65 730a 4465 7363 7269 7074  Modules.Descript
-00000790: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000007a0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000007b0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000007c0: 4345 4e53 450a 0a3c 7020 616c 6967 6e3d  CENSE..<p align=
-000007d0: 2263 656e 7465 7222 3e0a 3c21 2d2d 2073  "center">.<!-- s
-000007e0: 7572 7665 7920 6261 6e6e 6572 2073 7461  urvey banner sta
-000007f0: 7274 202d 2d3e 0a3c 6120 6872 6566 3d22  rt -->.<a href="
-00000800: 6874 7470 733a 2f2f 3130 7377 3174 6370  https://10sw1tcp
-00000810: 6c64 342e 7479 7065 666f 726d 2e63 6f6d  ld4.typeform.com
-00000820: 2f74 6f2f 4547 4145 5265 4d37 3f75 746d  /to/EGAEReM7?utm
-00000830: 5f73 6f75 7263 653d 7265 6164 6d65 2675  _source=readme&u
-00000840: 746d 5f6d 6564 6975 6d3d 6769 7468 7562  tm_medium=github
-00000850: 2675 746d 5f63 616d 7061 6967 6e3d 7573  &utm_campaign=us
-00000860: 6572 2532 3065 7870 6572 6965 6e63 6526  er%20experience&
-00000870: 7574 6d5f 7465 726d 3d66 6562 3230 3233  utm_term=feb2023
-00000880: 2675 746d 5f63 6f6e 7465 6e74 3d73 7572  &utm_content=sur
-00000890: 7665 7922 3e0a 2020 3c69 6d67 2073 7263  vey">.  <img src
-000008a0: 3d22 2e2f 2e67 6974 6875 622f 6261 6e6e  ="./.github/bann
-000008b0: 6572 2e73 7667 3f72 6177 3d74 7275 6522  er.svg?raw=true"
-000008c0: 3e0a 3c2f 613e 0a3c 212d 2d20 7375 7276  >.</a>.<!-- surv
-000008d0: 6579 2062 616e 6e65 7220 7374 6172 7420  ey banner start 
-000008e0: 2d2d 3e0a 0a3c 7020 616c 6967 6e3d 2263  -->..<p align="c
-000008f0: 656e 7465 7222 3e0a 3c61 2068 7265 663d  enter">.<a href=
-00000900: 2268 7474 7073 3a2f 2f64 6f63 732e 636d  "https://docs.cm
-00000910: 6f6e 2e61 6922 3e3c 696d 6720 7372 633d  on.ai"><img src=
-00000920: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00000930: 636f 6d2f 636d 6f6e 2d61 692f 636d 6f6e  com/cmon-ai/cmon
-00000940: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
-00000950: 732f 5f73 7461 7469 632f 6c6f 676f 2d6c  s/_static/logo-l
-00000960: 6967 6874 2e73 7667 3f72 6177 3d74 7275  ight.svg?raw=tru
-00000970: 6522 2061 6c74 3d22 436d 6f6e 206c 6f67  e" alt="Cmon log
-00000980: 6f3a 2042 7569 6c64 206d 756c 7469 6d6f  o: Build multimo
-00000990: 6461 6c20 4149 2073 6572 7669 6365 7320  dal AI services 
-000009a0: 7669 6120 636c 6f75 6420 6e61 7469 7665  via cloud native
-000009b0: 2074 6563 686e 6f6c 6f67 6965 7320 c2b7   technologies ..
-000009c0: 204e 6575 7261 6c20 5365 6172 6368 20c2   Neural Search .
-000009d0: b720 4765 6e65 7261 7469 7665 2041 4920  . Generative AI 
-000009e0: c2b7 2043 6c6f 7564 204e 6174 6976 6522  .. Cloud Native"
-000009f0: 2077 6964 7468 3d22 3135 3070 7822 3e3c   width="150px"><
-00000a00: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
-00000a10: 676e 3d22 6365 6e74 6572 223e 0a3c 623e  gn="center">.<b>
-00000a20: 4275 696c 6420 6d75 6c74 696d 6f64 616c  Build multimodal
-00000a30: 2041 4920 7365 7276 6963 6573 2077 6974   AI services wit
-00000a40: 6820 636c 6f75 6420 6e61 7469 7665 2074  h cloud native t
-00000a50: 6563 686e 6f6c 6f67 6965 733c 2f62 3e0a  echnologies</b>.
-00000a60: 3c2f 703e 0a0a 3c70 2061 6c69 676e 3d63  </p>..<p align=c
-00000a70: 656e 7465 723e 0a3c 6120 6872 6566 3d22  enter>.<a href="
-00000a80: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000a90: 2f70 726f 6a65 6374 2f63 6d6f 6e2f 223e  /project/cmon/">
-00000aa0: 3c69 6d67 2061 6c74 3d22 5079 5049 2220  <img alt="PyPI" 
-00000ab0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000ac0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000ad0: 2f76 2f63 6d6f 6e3f 6c61 6265 6c3d 5265  /v/cmon?label=Re
-00000ae0: 6c65 6173 6526 7374 796c 653d 666c 6174  lease&style=flat
-00000af0: 2d73 7175 6172 6522 3e3c 2f61 3e0a 3c21  -square"></a>.<!
-00000b00: 2d2d 3c61 2068 7265 663d 2268 7474 7073  --<a href="https
-00000b10: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000b20: 2f63 6d6f 6e2d 6169 2f63 6d6f 6e22 3e3c  /cmon-ai/cmon"><
-00000b30: 696d 6720 616c 743d 2243 6f64 6563 6f76  img alt="Codecov
-00000b40: 2062 7261 6e63 6822 2073 7263 3d22 6874   branch" src="ht
-00000b50: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000b60: 732e 696f 2f63 6f64 6563 6f76 2f63 2f67  s.io/codecov/c/g
-00000b70: 6974 6875 622f 636d 6f6e 2d61 692f 636d  ithub/cmon-ai/cm
-00000b80: 6f6e 2f6d 6173 7465 723f 266c 6f67 6f3d  on/master?&logo=
-00000b90: 436f 6465 636f 7626 6c6f 676f 436f 6c6f  Codecov&logoColo
-00000ba0: 723d 7768 6974 6526 7374 796c 653d 666c  r=white&style=fl
-00000bb0: 6174 2d73 7175 6172 6522 3e3c 2f61 3e2d  at-square"></a>-
-00000bc0: 2d3e 0a3c 6120 6872 6566 3d22 6874 7470  ->.<a href="http
-00000bd0: 733a 2f2f 6469 7363 6f72 642e 636d 6f6e  s://discord.cmon
-00000be0: 2e61 6922 3e3c 696d 6720 7372 633d 2268  .ai"><img src="h
-00000bf0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000c00: 6473 2e69 6f2f 6469 7363 6f72 642f 3131  ds.io/discord/11
-00000c10: 3036 3534 3232 3230 3131 3233 3032 3133  0654222011230213
-00000c20: 303f 6c6f 676f 3d64 6973 636f 7264 266c  0?logo=discord&l
-00000c30: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2673  ogoColor=white&s
-00000c40: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000c50: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00000c60: 6874 7470 733a 2f2f 7079 7069 7374 6174  https://pypistat
-00000c70: 732e 6f72 672f 7061 636b 6167 6573 2f63  s.org/packages/c
-00000c80: 6d6f 6e22 3e3c 696d 6720 616c 743d 2250  mon"><img alt="P
-00000c90: 7950 4920 2d20 446f 776e 6c6f 6164 7320  yPI - Downloads 
-00000ca0: 6672 6f6d 206f 6666 6963 6961 6c20 7079  from official py
-00000cb0: 7069 7374 6174 7322 2073 7263 3d22 6874  pistats" src="ht
-00000cc0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000cd0: 732e 696f 2f70 7970 692f 646d 2f63 6d6f  s.io/pypi/dm/cmo
-00000ce0: 6e3f 7374 796c 653d 666c 6174 2d73 7175  n?style=flat-squ
-00000cf0: 6172 6522 3e3c 2f61 3e0a 3c61 2068 7265  are"></a>.<a hre
-00000d00: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000d10: 622e 636f 6d2f 636d 6f6e 2d61 692f 636d  b.com/cmon-ai/cm
-00000d20: 6f6e 2f61 6374 696f 6e73 2f77 6f72 6b66  on/actions/workf
-00000d30: 6c6f 7773 2f63 642e 796d 6c22 3e3c 696d  lows/cd.yml"><im
-00000d40: 6720 616c 743d 2247 6974 6875 6220 4344  g alt="Github CD
-00000d50: 2073 7461 7475 7322 2073 7263 3d22 6874   status" src="ht
-00000d60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000d70: 2f63 6d6f 6e2d 6169 2f63 6d6f 6e2f 6163  /cmon-ai/cmon/ac
-00000d80: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000d90: 6364 2e79 6d6c 2f62 6164 6765 2e73 7667  cd.yml/badge.svg
-00000da0: 223e 3c2f 613e 0a3c 2f70 3e0a 0a3c 212d  "></a>.</p>..<!-
-00000db0: 2d20 7374 6172 7420 636d 6f6e 2d64 6573  - start cmon-des
-00000dc0: 6372 6970 7469 6f6e 202d 2d3e 0a0a 436d  cription -->..Cm
-00000dd0: 6f6e 206c 6574 7320 796f 7520 6275 696c  on lets you buil
-00000de0: 6420 6d75 6c74 696d 6f64 616c 205b 2a2a  d multimodal [**
-00000df0: 4149 2073 6572 7669 6365 732a 2a5d 2823  AI services**](#
-00000e00: 6275 696c 642d 6169 2d73 6572 7669 6365  build-ai-service
-00000e10: 7329 2061 6e64 205b 2a2a 7069 7065 6c69  s) and [**pipeli
-00000e20: 6e65 732a 2a5d 2823 6275 696c 642d 612d  nes**](#build-a-
-00000e30: 7069 7065 6c69 6e65 2920 7468 6174 2063  pipeline) that c
-00000e40: 6f6d 6d75 6e69 6361 7465 2076 6961 2067  ommunicate via g
-00000e50: 5250 432c 2048 5454 5020 616e 6420 5765  RPC, HTTP and We
-00000e60: 6253 6f63 6b65 7473 2c20 7468 656e 2073  bSockets, then s
-00000e70: 6361 6c65 2074 6865 6d20 7570 2061 6e64  cale them up and
-00000e80: 2064 6570 6c6f 7920 746f 2070 726f 6475   deploy to produ
-00000e90: 6374 696f 6e2e 2059 6f75 2063 616e 2066  ction. You can f
-00000ea0: 6f63 7573 206f 6e20 796f 7572 206c 6f67  ocus on your log
-00000eb0: 6963 2061 6e64 2061 6c67 6f72 6974 686d  ic and algorithm
-00000ec0: 732c 2077 6974 686f 7574 2077 6f72 7279  s, without worry
-00000ed0: 696e 6720 6162 6f75 7420 7468 6520 696e  ing about the in
-00000ee0: 6672 6173 7472 7563 7475 7265 2063 6f6d  frastructure com
-00000ef0: 706c 6578 6974 792e 0a0a 215b 5d28 2e2f  plexity...![](./
-00000f00: 2e67 6974 6875 622f 696d 6167 6573 2f62  .github/images/b
-00000f10: 7569 6c64 2d64 6570 6c6f 792e 706e 6729  uild-deploy.png)
-00000f20: 0a0a 436d 6f6e 2070 726f 7669 6465 7320  ..Cmon provides 
-00000f30: 6120 736d 6f6f 7468 2050 7974 686f 6e69  a smooth Pythoni
-00000f40: 6320 6578 7065 7269 656e 6365 2074 7261  c experience tra
-00000f50: 6e73 6974 696f 6e69 6e67 2066 726f 6d20  nsitioning from 
-00000f60: 6c6f 6361 6c20 6465 706c 6f79 6d65 6e74  local deployment
-00000f70: 2074 6f20 6164 7661 6e63 6564 206f 7263   to advanced orc
-00000f80: 6865 7374 7261 7469 6f6e 2066 7261 6d65  hestration frame
-00000f90: 776f 726b 7320 6c69 6b65 2044 6f63 6b65  works like Docke
-00000fa0: 722d 436f 6d70 6f73 652c 204b 7562 6572  r-Compose, Kuber
-00000fb0: 6e65 7465 732c 206f 7220 436d 6f6e 2041  netes, or Cmon A
-00000fc0: 4920 436c 6f75 642e 2043 6d6f 6e20 6d61  I Cloud. Cmon ma
-00000fd0: 6b65 7320 6164 7661 6e63 6564 2073 6f6c  kes advanced sol
-00000fe0: 7574 696f 6e20 656e 6769 6e65 6572 696e  ution engineerin
-00000ff0: 6720 616e 6420 636c 6f75 642d 6e61 7469  g and cloud-nati
-00001000: 7665 2074 6563 686e 6f6c 6f67 6965 7320  ve technologies 
-00001010: 6163 6365 7373 6962 6c65 2074 6f20 6576  accessible to ev
-00001020: 6572 7920 6465 7665 6c6f 7065 722e 0a0a  ery developer...
-00001030: 2d20 4275 696c 6420 6170 706c 6963 6174  - Build applicat
-00001040: 696f 6e73 2066 6f72 2061 6e79 205b 6461  ions for any [da
-00001050: 7461 2074 7970 655d 2868 7474 7073 3a2f  ta type](https:/
-00001060: 2f64 6f63 732e 646f 6361 7272 6179 2e6f  /docs.docarray.o
-00001070: 7267 2f64 6174 615f 7479 7065 732f 6669  rg/data_types/fi
-00001080: 7273 745f 7374 6570 732f 292c 2061 6e79  rst_steps/), any
-00001090: 206d 6169 6e73 7472 6561 6d20 5b64 6565   mainstream [dee
-000010a0: 7020 6c65 6172 6e69 6e67 2066 7261 6d65  p learning frame
-000010b0: 776f 726b 5d28 292c 2061 6e64 2061 6e79  work](), and any
-000010c0: 205b 7072 6f74 6f63 6f6c 5d28 6874 7470   [protocol](http
-000010d0: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-000010e0: 2f63 6f6e 6365 7074 732f 7365 7276 696e  /concepts/servin
-000010f0: 672f 6761 7465 7761 792f 2373 6574 2d70  g/gateway/#set-p
-00001100: 726f 746f 636f 6c2d 696e 2d70 7974 686f  rotocol-in-pytho
-00001110: 6e29 2e0a 2d20 4465 7369 676e 2068 6967  n)..- Design hig
-00001120: 682d 7065 7266 6f72 6d61 6e63 6520 6d69  h-performance mi
-00001130: 6372 6f73 6572 7669 6365 732c 2077 6974  croservices, wit
-00001140: 6820 5b65 6173 7920 7363 616c 696e 675d  h [easy scaling]
-00001150: 2868 7474 7073 3a2f 2f64 6f63 732e 636d  (https://docs.cm
-00001160: 6f6e 2e61 692f 636f 6e63 6570 7473 2f6f  on.ai/concepts/o
-00001170: 7263 6865 7374 7261 7469 6f6e 2f73 6361  rchestration/sca
-00001180: 6c65 2d6f 7574 2f29 2c20 6475 706c 6578  le-out/), duplex
-00001190: 2063 6c69 656e 742d 7365 7276 6572 2073   client-server s
-000011a0: 7472 6561 6d69 6e67 2c20 616e 6420 6173  treaming, and as
-000011b0: 796e 632f 6e6f 6e2d 626c 6f63 6b69 6e67  ync/non-blocking
-000011c0: 2064 6174 6120 7072 6f63 6573 7369 6e67   data processing
-000011d0: 206f 7665 7220 6479 6e61 6d69 6320 666c   over dynamic fl
-000011e0: 6f77 732e 0a2d 2044 6f63 6b65 7220 636f  ows..- Docker co
-000011f0: 6e74 6169 6e65 7220 696e 7465 6772 6174  ntainer integrat
-00001200: 696f 6e20 7669 6120 5b45 7865 6375 746f  ion via [Executo
-00001210: 7220 4875 625d 2868 7474 7073 3a2f 2f63  r Hub](https://c
-00001220: 6c6f 7564 2e63 6d6f 6e2e 6169 292c 204f  loud.cmon.ai), O
-00001230: 7065 6e54 656c 656d 6574 7279 2f50 726f  penTelemetry/Pro
-00001240: 6d65 7468 6575 7320 6f62 7365 7276 6162  metheus observab
-00001250: 696c 6974 792c 2061 6e64 2066 6173 7420  ility, and fast 
-00001260: 4b75 6265 726e 6574 6573 2f44 6f63 6b65  Kubernetes/Docke
-00001270: 722d 436f 6d70 6f73 6520 6465 706c 6f79  r-Compose deploy
-00001280: 6d65 6e74 2e0a 2d20 4350 552f 4750 5520  ment..- CPU/GPU 
-00001290: 686f 7374 696e 6720 7669 6120 5b43 6d6f  hosting via [Cmo
-000012a0: 6e20 4149 2043 6c6f 7564 5d28 6874 7470  n AI Cloud](http
-000012b0: 733a 2f2f 636c 6f75 642e 636d 6f6e 2e61  s://cloud.cmon.a
-000012c0: 6929 2e0a 0a3c 6465 7461 696c 733e 0a20  i)...<details>. 
-000012d0: 2020 203c 7375 6d6d 6172 793e 3c73 7472     <summary><str
-000012e0: 6f6e 673e 5761 6974 2c20 686f 7720 6973  ong>Wait, how is
-000012f0: 2043 6d6f 6e20 6469 6666 6572 656e 7420   Cmon different 
-00001300: 6672 6f6d 2046 6173 7441 5049 3f3c 2f73  from FastAPI?</s
-00001310: 7472 6f6e 673e 3c2f 7375 6d6d 6172 793e  trong></summary>
-00001320: 0a43 6d6f 6e27 7320 7661 6c75 6520 7072  .Cmon's value pr
-00001330: 6f70 6f73 6974 696f 6e20 6d61 7920 7365  oposition may se
-00001340: 656d 2071 7569 7465 2073 696d 696c 6172  em quite similar
-00001350: 2074 6f20 7468 6174 206f 6620 4661 7374   to that of Fast
-00001360: 4150 492e 2048 6f77 6576 6572 2c20 7468  API. However, th
-00001370: 6572 6520 6172 6520 7365 7665 7261 6c20  ere are several 
-00001380: 6675 6e64 616d 656e 7461 6c20 6469 6666  fundamental diff
-00001390: 6572 656e 6365 733a 0a0a 202a 2a44 6174  erences:.. **Dat
-000013a0: 6120 7374 7275 6374 7572 6520 616e 6420  a structure and 
-000013b0: 636f 6d6d 756e 6963 6174 696f 6e20 7072  communication pr
-000013c0: 6f74 6f63 6f6c 732a 2a0a 2020 2d20 4661  otocols**.  - Fa
-000013d0: 7374 4150 4920 636f 6d6d 756e 6963 6174  stAPI communicat
-000013e0: 696f 6e20 7265 6c69 6573 206f 6e20 5079  ion relies on Py
-000013f0: 6461 6e74 6963 2061 6e64 2043 6d6f 6e20  dantic and Cmon 
-00001400: 7265 6c69 6573 206f 6e20 5b44 6f63 4172  relies on [DocAr
-00001410: 7261 795d 2868 7474 7073 3a2f 2f67 6974  ray](https://git
-00001420: 6875 622e 636f 6d2f 646f 6361 7272 6179  hub.com/docarray
-00001430: 2f64 6f63 6172 7261 7929 2061 6c6c 6f77  /docarray) allow
-00001440: 696e 6720 436d 6f6e 2074 6f20 7375 7070  ing Cmon to supp
-00001450: 6f72 7420 6d75 6c74 6970 6c65 2070 726f  ort multiple pro
-00001460: 746f 636f 6c73 0a20 2074 6f20 6578 706f  tocols.  to expo
-00001470: 7365 2069 7473 2073 6572 7669 6365 732e  se its services.
-00001480: 0a0a 202a 2a41 6476 616e 6365 6420 6f72  .. **Advanced or
-00001490: 6368 6573 7472 6174 696f 6e20 616e 6420  chestration and 
-000014a0: 7363 616c 696e 6720 6361 7061 6269 6c69  scaling capabili
-000014b0: 7469 6573 2a2a 0a20 202d 2043 6d6f 6e20  ties**.  - Cmon 
-000014c0: 6c65 7473 2079 6f75 2064 6570 6c6f 7920  lets you deploy 
-000014d0: 6170 706c 6963 6174 696f 6e73 2066 6f72  applications for
-000014e0: 6d65 6420 6672 6f6d 206d 756c 7469 706c  med from multipl
-000014f0: 6520 6d69 6372 6f73 6572 7669 6365 7320  e microservices 
-00001500: 7468 6174 2063 616e 2062 6520 636f 6e74  that can be cont
-00001510: 6169 6e65 7269 7a65 6420 616e 6420 7363  ainerized and sc
-00001520: 616c 6564 2069 6e64 6570 656e 6465 6e74  aled independent
-00001530: 6c79 2e0a 2020 2d20 436d 6f6e 2061 6c6c  ly..  - Cmon all
-00001540: 6f77 7320 796f 7520 746f 2065 6173 696c  ows you to easil
-00001550: 7920 636f 6e74 6169 6e65 7269 7a65 2061  y containerize a
-00001560: 6e64 206f 7263 6865 7374 7261 7465 2079  nd orchestrate y
-00001570: 6f75 7220 7365 7276 6963 6573 2c20 7072  our services, pr
-00001580: 6f76 6964 696e 6720 636f 6e63 7572 7265  oviding concurre
-00001590: 6e63 7920 616e 6420 7363 616c 6162 696c  ncy and scalabil
-000015a0: 6974 792e 0a0a 202a 2a4a 6f75 726e 6579  ity... **Journey
-000015b0: 2074 6f20 7468 6520 636c 6f75 642a 2a0a   to the cloud**.
-000015c0: 2020 2d20 436d 6f6e 2070 726f 7669 6465    - Cmon provide
-000015d0: 7320 6120 736d 6f6f 7468 2074 7261 6e73  s a smooth trans
-000015e0: 6974 696f 6e20 6672 6f6d 206c 6f63 616c  ition from local
-000015f0: 2064 6576 656c 6f70 6d65 6e74 2028 7573   development (us
-00001600: 696e 6720 5b44 6f63 4172 7261 795d 2868  ing [DocArray](h
-00001610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001620: 6d2f 646f 6361 7272 6179 2f64 6f63 6172  m/docarray/docar
-00001630: 7261 7929 2920 746f 206c 6f63 616c 2073  ray)) to local s
-00001640: 6572 7669 6e67 2075 7369 6e67 2028 436d  erving using (Cm
-00001650: 6f6e 2773 206f 7263 6865 7374 7261 7469  on's orchestrati
-00001660: 6f6e 206c 6179 6572 290a 2020 746f 2068  on layer).  to h
-00001670: 6176 696e 6720 7072 6f64 7563 7469 6f6e  aving production
-00001680: 2d72 6561 6479 2073 6572 7669 6365 7320  -ready services 
-00001690: 6279 2075 7369 6e67 204b 7562 6572 6e65  by using Kuberne
-000016a0: 7465 7320 6361 7061 6369 7479 2074 6f20  tes capacity to 
-000016b0: 6f72 6368 6573 7472 6174 6520 7468 6520  orchestrate the 
-000016c0: 6c69 6665 7469 6d65 206f 6620 636f 6e74  lifetime of cont
-000016d0: 6169 6e65 7273 2e0a 2020 2d20 4279 2075  ainers..  - By u
-000016e0: 7369 6e67 205b 436d 6f6e 2041 4920 436c  sing [Cmon AI Cl
-000016f0: 6f75 645d 2868 7474 7073 3a2f 2f63 6c6f  oud](https://clo
-00001700: 7564 2e63 6d6f 6e2e 6169 2920 796f 7520  ud.cmon.ai) you 
-00001710: 6861 7665 2061 6363 6573 7320 746f 2073  have access to s
-00001720: 6361 6c61 626c 6520 616e 6420 7365 7276  calable and serv
-00001730: 6572 6c65 7373 2064 6570 6c6f 796d 656e  erless deploymen
-00001740: 7473 206f 6620 796f 7572 2061 7070 6c69  ts of your appli
-00001750: 6361 7469 6f6e 7320 696e 206f 6e65 2063  cations in one c
-00001760: 6f6d 6d61 6e64 2e0a 3c2f 6465 7461 696c  ommand..</detail
-00001770: 733e 0a0a 3c21 2d2d 2065 6e64 2063 6d6f  s>..<!-- end cmo
-00001780: 6e2d 6465 7363 7269 7074 696f 6e20 2d2d  n-description --
-00001790: 3e0a 0a23 2320 5b44 6f63 756d 656e 7461  >..## [Documenta
-000017a0: 7469 6f6e 5d28 6874 7470 733a 2f2f 646f  tion](https://do
-000017b0: 6373 2e63 6d6f 6e2e 6169 290a 0a23 2320  cs.cmon.ai)..## 
-000017c0: 496e 7374 616c 6c20 0a0a 4e6f 7465 3a20  Install ..Note: 
-000017d0: 2857 696e 646f 7773 2920 6e6f 7420 7375  (Windows) not su
-000017e0: 7070 6f72 7465 6420 6174 2074 6869 7320  pported at this 
-000017f0: 6d6f 6d65 6e74 2120 596f 7520 6d61 7920  moment! You may 
-00001800: 7265 7175 6972 6520 746f 2069 6e73 7461  require to insta
-00001810: 6c6c 2069 7420 6f6e 2028 5753 4c29 2e0a  ll it on (WSL)..
-00001820: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-00001830: 7461 6c6c 2063 6d6f 6e0a 6060 600a 0a46  tall cmon.```..F
-00001840: 696e 6420 6d6f 7265 2069 6e73 7461 6c6c  ind more install
-00001850: 206f 7074 696f 6e73 206f 6e20 5b41 7070   options on [App
-00001860: 6c65 2053 696c 6963 6f6e 5d28 6874 7470  le Silicon](http
-00001870: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-00001880: 2f67 6574 2d73 7461 7274 6564 2f69 6e73  /get-started/ins
-00001890: 7461 6c6c 2f61 7070 6c65 2d73 696c 6963  tall/apple-silic
-000018a0: 6f6e 2d6d 312d 6d32 2f29 0a0a 0a23 2320  on-m1-m2/)...## 
-000018b0: 4765 7420 5374 6172 7465 640a 0a23 2323  Get Started..###
-000018c0: 2042 6173 6963 2043 6f6e 6365 7074 730a   Basic Concepts.
-000018d0: 0a43 6d6f 6e20 6861 7320 666f 7572 2066  .Cmon has four f
-000018e0: 756e 6461 6d65 6e74 616c 2063 6f6e 6365  undamental conce
-000018f0: 7074 733a 0a0a 2d20 4120 5b2a 2a44 6f63  pts:..- A [**Doc
-00001900: 756d 656e 742a 2a5d 2868 7474 7073 3a2f  ument**](https:/
-00001910: 2f64 6f63 6172 7261 792e 636d 6f6e 2e61  /docarray.cmon.a
-00001920: 692f 2920 2866 726f 6d20 5b44 6f63 4172  i/) (from [DocAr
-00001930: 7261 795d 2868 7474 7073 3a2f 2f67 6974  ray](https://git
-00001940: 6875 622e 636f 6d2f 646f 6361 7272 6179  hub.com/docarray
-00001950: 2f64 6f63 6172 7261 7929 2920 6973 2074  /docarray)) is t
-00001960: 6865 2069 6e70 7574 2f6f 7574 7075 7420  he input/output 
-00001970: 666f 726d 6174 2069 6e20 436d 6f6e 2e0a  format in Cmon..
-00001980: 2d20 416e 205b 2a2a 4578 6563 7574 6f72  - An [**Executor
-00001990: 2a2a 5d28 6874 7470 733a 2f2f 646f 6373  **](https://docs
-000019a0: 2e63 6d6f 6e2e 6169 2f63 6f6e 6365 7074  .cmon.ai/concept
-000019b0: 732f 7365 7276 696e 672f 6578 6563 7574  s/serving/execut
-000019c0: 6f72 2f29 2069 7320 6120 5079 7468 6f6e  or/) is a Python
-000019d0: 2063 6c61 7373 2074 6861 7420 7472 616e   class that tran
-000019e0: 7366 6f72 6d73 2061 6e64 2070 726f 6365  sforms and proce
-000019f0: 7373 6573 2044 6f63 756d 656e 7473 2e0a  sses Documents..
-00001a00: 2d20 4120 5b2a 2a44 6570 6c6f 796d 656e  - A [**Deploymen
-00001a10: 742a 2a5d 2868 7474 7073 3a2f 2f64 6f63  t**](https://doc
-00001a20: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00001a30: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
-00001a40: 2f64 6570 6c6f 796d 656e 7429 2073 6572  /deployment) ser
-00001a50: 7665 7320 6120 7369 6e67 6c65 2045 7865  ves a single Exe
-00001a60: 6375 746f 722c 2077 6869 6c65 2061 205b  cutor, while a [
-00001a70: 2a2a 466c 6f77 2a2a 5d28 6874 7470 733a  **Flow**](https:
-00001a80: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-00001a90: 6f6e 6365 7074 732f 6f72 6368 6573 7472  oncepts/orchestr
-00001aa0: 6174 696f 6e2f 666c 6f77 2f29 2073 6572  ation/flow/) ser
-00001ab0: 7665 7320 4578 6563 7574 6f72 7320 6368  ves Executors ch
-00001ac0: 6169 6e65 6420 696e 746f 2061 2070 6970  ained into a pip
-00001ad0: 656c 696e 652e 0a0a 0a5b 5468 6520 6675  eline....[The fu
-00001ae0: 6c6c 2067 6c6f 7373 6172 7920 6973 2065  ll glossary is e
-00001af0: 7870 6c61 696e 6564 2068 6572 655d 2868  xplained here](h
-00001b00: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00001b10: 2e61 692f 636f 6e63 6570 7473 2f70 7265  .ai/concepts/pre
-00001b20: 6c69 6d69 6e61 7269 6573 2f23 292e 0a0a  liminaries/#)...
-00001b30: 2323 2320 4275 696c 6420 4149 2053 6572  ### Build AI Ser
-00001b40: 7669 6365 730a 3c21 2d2d 2073 7461 7274  vices.<!-- start
-00001b50: 2062 7569 6c64 2d61 692d 7365 7276 6963   build-ai-servic
-00001b60: 6573 202d 2d3e 0a0a 4c65 7427 7320 6275  es -->..Let's bu
-00001b70: 696c 6420 6120 6661 7374 2c20 7265 6c69  ild a fast, reli
-00001b80: 6162 6c65 2061 6e64 2073 6361 6c61 626c  able and scalabl
-00001b90: 6520 6752 5043 2d62 6173 6564 2041 4920  e gRPC-based AI 
-00001ba0: 7365 7276 6963 652e 2049 6e20 436d 6f6e  service. In Cmon
-00001bb0: 2077 6520 6361 6c6c 2074 6869 7320 616e   we call this an
-00001bc0: 202a 2a5b 4578 6563 7574 6f72 5d28 6874   **[Executor](ht
-00001bd0: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
-00001be0: 6169 2f63 6f6e 6365 7074 732f 6578 6563  ai/concepts/exec
-00001bf0: 7574 6f72 2f29 2a2a 2e20 4f75 7220 7369  utor/)**. Our si
-00001c00: 6d70 6c65 2045 7865 6375 746f 7220 7769  mple Executor wi
-00001c10: 6c6c 2077 7261 7020 7468 6520 5b53 7461  ll wrap the [Sta
-00001c20: 626c 654c 4d5d 2868 7474 7073 3a2f 2f68  bleLM](https://h
-00001c30: 7567 6769 6e67 6661 6365 2e63 6f2f 7374  uggingface.co/st
-00001c40: 6162 696c 6974 7961 692f 7374 6162 6c65  abilityai/stable
-00001c50: 6c6d 2d62 6173 652d 616c 7068 612d 3362  lm-base-alpha-3b
-00001c60: 2920 4c4c 4d20 6672 6f6d 2053 7461 6269  ) LLM from Stabi
-00001c70: 6c69 7479 2041 492e 2057 6527 6c6c 2074  lity AI. We'll t
-00001c80: 6865 6e20 7573 6520 6120 2a2a 4465 706c  hen use a **Depl
-00001c90: 6f79 6d65 6e74 2a2a 2074 6f20 7365 7276  oyment** to serv
-00001ca0: 6520 6974 2e0a 0a21 5b5d 282e 2f2e 6769  e it...![](./.gi
-00001cb0: 7468 7562 2f69 6d61 6765 732f 6465 706c  thub/images/depl
-00001cc0: 6f79 6d65 6e74 2d64 6961 6772 616d 2e70  oyment-diagram.p
-00001cd0: 6e67 290a 0a3e 202a 2a4e 6f74 652a 2a0a  ng)..> **Note**.
-00001ce0: 3e20 4120 4465 706c 6f79 6d65 6e74 2073  > A Deployment s
-00001cf0: 6572 7665 7320 6a75 7374 206f 6e65 2045  erves just one E
-00001d00: 7865 6375 746f 722e 2054 6f20 636f 6d62  xecutor. To comb
-00001d10: 696e 6520 6d75 6c74 6970 6c65 2045 7865  ine multiple Exe
-00001d20: 6375 746f 7273 2069 6e74 6f20 6120 7069  cutors into a pi
-00001d30: 7065 6c69 6e65 2061 6e64 2073 6572 7665  peline and serve
-00001d40: 2074 6861 742c 2075 7365 2061 205b 466c   that, use a [Fl
-00001d50: 6f77 5d28 2362 7569 6c64 2d61 2d70 6970  ow](#build-a-pip
-00001d60: 656c 696e 6529 2e0a 0a4c 6574 2773 2069  eline)...Let's i
-00001d70: 6d70 6c65 6d65 6e74 2074 6865 2073 6572  mplement the ser
-00001d80: 7669 6365 2773 206c 6f67 6963 3a0a 0a3c  vice's logic:..<
-00001d90: 7461 626c 653e 0a3c 7472 3e0a 3c74 683e  table>.<tr>.<th>
-00001da0: 3c63 6f64 653e 6578 6563 7574 6f72 2e70  <code>executor.p
-00001db0: 793c 2f63 6f64 653e 3c2f 7468 3e20 0a3c  y</code></th> .<
-00001dc0: 7472 3e0a 3c74 643e 0a0a 6060 6070 7974  tr>.<td>..```pyt
-00001dd0: 686f 6e0a 6672 6f6d 2063 6d6f 6e20 696d  hon.from cmon im
-00001de0: 706f 7274 2045 7865 6375 746f 722c 2072  port Executor, r
-00001df0: 6571 7565 7374 730a 6672 6f6d 2064 6f63  equests.from doc
-00001e00: 6172 7261 7920 696d 706f 7274 2044 6f63  array import Doc
-00001e10: 756d 656e 7441 7272 6179 0a0a 6672 6f6d  umentArray..from
-00001e20: 2074 7261 6e73 666f 726d 6572 7320 696d   transformers im
-00001e30: 706f 7274 2070 6970 656c 696e 650a 0a0a  port pipeline...
-00001e40: 636c 6173 7320 5374 6162 6c65 4c4d 2845  class StableLM(E
-00001e50: 7865 6375 746f 7229 3a0a 0a20 2020 2064  xecutor):..    d
-00001e60: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00001e70: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00001e80: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001e90: 6e69 745f 5f28 2a2a 6b77 6172 6773 290a  nit__(**kwargs).
-00001ea0: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
-00001eb0: 6572 6174 6f72 203d 2070 6970 656c 696e  erator = pipelin
-00001ec0: 6528 2774 6578 742d 6765 6e65 7261 7469  e('text-generati
-00001ed0: 6f6e 272c 206d 6f64 656c 3d27 7374 6162  on', model='stab
-00001ee0: 6c65 6c6d 2d33 6227 290a 0a20 2020 2040  lelm-3b')..    @
-00001ef0: 7265 7175 6573 7473 0a20 2020 2064 6566  requests.    def
-00001f00: 2067 656e 6572 6174 6528 7365 6c66 2c20   generate(self, 
-00001f10: 646f 6373 3a20 446f 6375 6d65 6e74 4172  docs: DocumentAr
-00001f20: 7261 792c 202a 2a6b 7761 7267 7329 3a0a  ray, **kwargs):.
-00001f30: 2020 2020 2020 2020 6765 6e65 7261 7465          generate
-00001f40: 645f 7465 7874 203d 2073 656c 662e 6765  d_text = self.ge
-00001f50: 6e65 7261 746f 7228 646f 6373 2e74 6578  nerator(docs.tex
-00001f60: 7473 290a 2020 2020 2020 2020 646f 6373  ts).        docs
-00001f70: 2e74 6578 7473 203d 205b 6765 6e5b 305d  .texts = [gen[0]
-00001f80: 5b27 6765 6e65 7261 7465 645f 7465 7874  ['generated_text
-00001f90: 275d 2066 6f72 2067 656e 2069 6e20 6765  '] for gen in ge
-00001fa0: 6e65 7261 7465 645f 7465 7874 5d0a 6060  nerated_text].``
-00001fb0: 600a 0a3c 2f74 643e 0a3c 2f74 723e 0a3c  `..</td>.</tr>.<
-00001fc0: 2f74 6162 6c65 3e0a 0a54 6865 6e20 7765  /table>..Then we
-00001fd0: 2064 6570 6c6f 7920 6974 2077 6974 6820   deploy it with 
-00001fe0: 6569 7468 6572 2074 6865 2050 7974 686f  either the Pytho
-00001ff0: 6e20 4150 4920 6f72 2059 414d 4c3a 0a3c  n API or YAML:.<
-00002000: 6469 7620 636c 6173 733d 2274 6162 6c65  div class="table
-00002010: 2d77 7261 7070 6572 223e 0a3c 7461 626c  -wrapper">.<tabl
-00002020: 653e 0a3c 7472 3e0a 3c74 683e 2050 7974  e>.<tr>.<th> Pyt
-00002030: 686f 6e20 4150 493a 203c 636f 6465 3e64  hon API: <code>d
-00002040: 6570 6c6f 796d 656e 742e 7079 3c2f 636f  eployment.py</co
-00002050: 6465 3e20 3c2f 7468 3e20 0a3c 7468 3e20  de> </th> .<th> 
-00002060: 5941 4d4c 3a20 3c63 6f64 653e 6465 706c  YAML: <code>depl
-00002070: 6f79 6d65 6e74 2e79 6d6c 3c2f 636f 6465  oyment.yml</code
-00002080: 3e20 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  > </th>.</tr>.<t
-00002090: 723e 0a3c 7464 3e0a 0a60 6060 7079 7468  r>.<td>..```pyth
-000020a0: 6f6e 0a66 726f 6d20 636d 6f6e 2069 6d70  on.from cmon imp
-000020b0: 6f72 7420 4465 706c 6f79 6d65 6e74 0a66  ort Deployment.f
-000020c0: 726f 6d20 6578 6563 7574 6f72 2069 6d70  rom executor imp
-000020d0: 6f72 7420 5374 6162 6c65 4c4d 0a0a 6465  ort StableLM..de
-000020e0: 7020 3d20 4465 706c 6f79 6d65 6e74 2875  p = Deployment(u
-000020f0: 7365 733d 5374 6162 6c65 4c4d 2c20 7469  ses=StableLM, ti
-00002100: 6d65 6f75 745f 7265 6164 793d 2d31 2c20  meout_ready=-1, 
-00002110: 706f 7274 3d31 3233 3435 290a 0a77 6974  port=12345)..wit
-00002120: 6820 6465 703a 0a20 2020 2064 6570 2e62  h dep:.    dep.b
-00002130: 6c6f 636b 2829 0a60 6060 0a0a 3c2f 7464  lock().```..</td
-00002140: 3e0a 3c74 643e 0a0a 6060 6079 616d 6c0a  >.<td>..```yaml.
-00002150: 6a74 7970 653a 2044 6570 6c6f 796d 656e  jtype: Deploymen
-00002160: 740a 7769 7468 3a0a 2020 7573 6573 3a20  t.with:.  uses: 
-00002170: 5374 6162 6c65 4c4d 0a20 2070 795f 6d6f  StableLM.  py_mo
-00002180: 6475 6c65 733a 0a20 2020 202d 2065 7865  dules:.    - exe
-00002190: 6375 746f 722e 7079 0a20 2074 696d 656f  cutor.py.  timeo
-000021a0: 7574 5f72 6561 6479 3a20 2d31 0a20 2070  ut_ready: -1.  p
-000021b0: 6f72 743a 2031 3233 3435 0a60 6060 0a0a  ort: 12345.```..
-000021c0: 416e 6420 7275 6e20 7468 6520 5941 4d4c  And run the YAML
-000021d0: 2044 6570 6c6f 796d 656e 7420 7769 7468   Deployment with
-000021e0: 2074 6865 2043 4c49 3a20 6063 6d6f 6e20   the CLI: `cmon 
-000021f0: 6465 706c 6f79 6d65 6e74 202d 2d75 7365  deployment --use
-00002200: 7320 6465 706c 6f79 6d65 6e74 2e79 6d6c  s deployment.yml
-00002210: 600a 0a3c 2f74 643e 0a3c 2f74 723e 0a3c  `..</td>.</tr>.<
-00002220: 2f74 6162 6c65 3e0a 3c2f 6469 763e 0a0a  /table>.</div>..
-00002230: 5573 6520 5b43 6d6f 6e20 436c 6965 6e74  Use [Cmon Client
-00002240: 5d28 6874 7470 733a 2f2f 646f 6373 2e63  ](https://docs.c
-00002250: 6d6f 6e2e 6169 2f63 6f6e 6365 7074 732f  mon.ai/concepts/
-00002260: 636c 6965 6e74 2f29 2074 6f20 6d61 6b65  client/) to make
-00002270: 2072 6571 7565 7374 7320 746f 2074 6865   requests to the
-00002280: 2073 6572 7669 6365 3a0a 0a60 6060 7079   service:..```py
-00002290: 7468 6f6e 0a66 726f 6d20 646f 6361 7272  thon.from docarr
-000022a0: 6179 2069 6d70 6f72 7420 446f 6375 6d65  ay import Docume
-000022b0: 6e74 0a66 726f 6d20 636d 6f6e 2069 6d70  nt.from cmon imp
-000022c0: 6f72 7420 436c 6965 6e74 0a0a 7072 6f6d  ort Client..prom
-000022d0: 7074 203d 2044 6f63 756d 656e 7428 0a20  pt = Document(. 
-000022e0: 2020 2074 6167 7320 3d20 7b27 7072 6f6d     tags = {'prom
-000022f0: 7074 273a 2027 7375 6767 6573 7420 616e  pt': 'suggest an
-00002300: 2069 6e74 6572 6573 7469 6e67 2069 6d61   interesting ima
-00002310: 6765 2067 656e 6572 6174 696f 6e20 7072  ge generation pr
-00002320: 6f6d 7074 2066 6f72 2061 206d 6f6e 6120  ompt for a mona 
-00002330: 6c69 7361 2076 6172 6961 6e74 277d 0a29  lisa variant'}.)
-00002340: 0a0a 636c 6965 6e74 203d 2043 6c69 656e  ..client = Clien
-00002350: 7428 706f 7274 3d31 3233 3435 2920 2023  t(port=12345)  #
-00002360: 2075 7365 2070 6f72 7420 6672 6f6d 206f   use port from o
-00002370: 7574 7075 7420 6162 6f76 650a 7265 7370  utput above.resp
-00002380: 6f6e 7365 203d 2063 6c69 656e 742e 706f  onse = client.po
-00002390: 7374 286f 6e3d 272f 272c 2069 6e70 7574  st(on='/', input
-000023a0: 733d 5b70 726f 6d70 745d 290a 0a70 7269  s=[prompt])..pri
-000023b0: 6e74 2872 6573 706f 6e73 655b 305d 2e74  nt(response[0].t
-000023c0: 6578 7429 0a60 6060 0a0a 6060 6074 6578  ext).```..```tex
-000023d0: 740a 6120 7374 6561 6d70 756e 6b20 7665  t.a steampunk ve
-000023e0: 7273 696f 6e20 6f66 2074 6865 204d 6f6e  rsion of the Mon
-000023f0: 6120 4c69 7361 2c20 696e 636f 7270 6f72  a Lisa, incorpor
-00002400: 6174 696e 6720 6d65 6368 616e 6963 616c  ating mechanical
-00002410: 2067 6561 7273 2c20 6272 6173 7320 656c   gears, brass el
-00002420: 656d 656e 7473 2c20 616e 6420 5669 6374  ements, and Vict
-00002430: 6f72 6961 6e20 6572 6120 636c 6f74 6869  orian era clothi
-00002440: 6e67 2064 6574 6169 6c73 0a60 6060 0a0a  ng details.```..
-00002450: 3c21 2d2d 2065 6e64 2062 7569 6c64 2d61  <!-- end build-a
-00002460: 692d 7365 7276 6963 6573 202d 2d3e 0a0a  i-services -->..
-00002470: 3e20 2a2a 4e6f 7465 2a2a 0a3e 2049 6e20  > **Note**.> In 
-00002480: 6120 6e6f 7465 626f 6f6b 2c20 796f 7520  a notebook, you 
-00002490: 6361 6e27 7420 7573 6520 6064 6570 6c6f  can't use `deplo
-000024a0: 796d 656e 742e 626c 6f63 6b28 2960 2061  yment.block()` a
-000024b0: 6e64 2074 6865 6e20 6d61 6b65 2072 6571  nd then make req
-000024c0: 7565 7374 7320 746f 2074 6865 2063 6c69  uests to the cli
-000024d0: 656e 742e 2050 6c65 6173 6520 7265 6665  ent. Please refe
-000024e0: 7220 746f 2074 6865 2043 6f6c 6162 206c  r to the Colab l
-000024f0: 696e 6b20 6162 6f76 6520 666f 7220 7265  ink above for re
-00002500: 7072 6f64 7563 6962 6c65 204a 7570 7974  producible Jupyt
-00002510: 6572 204e 6f74 6562 6f6f 6b20 636f 6465  er Notebook code
-00002520: 2073 6e69 7070 6574 732e 0a0a 2323 2320   snippets...### 
-00002530: 4275 696c 6420 6120 7069 7065 6c69 6e65  Build a pipeline
-00002540: 0a0a 3c21 2d2d 2073 7461 7274 2062 7569  ..<!-- start bui
-00002550: 6c64 2d70 6970 656c 696e 6573 202d 2d3e  ld-pipelines -->
-00002560: 0a0a 536f 6d65 7469 6d65 7320 796f 7520  ..Sometimes you 
-00002570: 7761 6e74 2074 6f20 6368 6169 6e20 6d69  want to chain mi
-00002580: 6372 6f73 6572 7669 6365 7320 746f 6765  croservices toge
-00002590: 7468 6572 2069 6e74 6f20 6120 7069 7065  ther into a pipe
-000025a0: 6c69 6e65 2e20 5468 6174 2773 2077 6865  line. That's whe
-000025b0: 7265 2061 205b 466c 6f77 5d28 6874 7470  re a [Flow](http
-000025c0: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-000025d0: 2f63 6f6e 6365 7074 732f 666c 6f77 2f29  /concepts/flow/)
-000025e0: 2063 6f6d 6573 2069 6e2e 0a0a 4120 466c   comes in...A Fl
-000025f0: 6f77 2069 7320 6120 5b44 4147 5d28 6874  ow is a [DAG](ht
-00002600: 7470 733a 2f2f 6465 2e77 696b 6970 6564  tps://de.wikiped
-00002610: 6961 2e6f 7267 2f77 696b 692f 4441 4729  ia.org/wiki/DAG)
-00002620: 2070 6970 656c 696e 652c 2063 6f6d 706f   pipeline, compo
-00002630: 7365 6420 6f66 2061 2073 6574 206f 6620  sed of a set of 
-00002640: 7374 6570 732c 2049 7420 6f72 6368 6573  steps, It orches
-00002650: 7472 6174 6573 2061 2073 6574 206f 6620  trates a set of 
-00002660: 5b45 7865 6375 746f 7273 5d28 6874 7470  [Executors](http
-00002670: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 6169  s://docs.cmon.ai
-00002680: 2f63 6f6e 6365 7074 732f 6578 6563 7574  /concepts/execut
-00002690: 6f72 2f29 2061 6e64 2061 205b 4761 7465  or/) and a [Gate
-000026a0: 7761 795d 2868 7474 7073 3a2f 2f64 6f63  way](https://doc
-000026b0: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-000026c0: 7473 2f67 6174 6577 6179 2f29 2074 6f20  ts/gateway/) to 
-000026d0: 6f66 6665 7220 616e 2065 6e64 2d74 6f2d  offer an end-to-
-000026e0: 656e 6420 7365 7276 6963 652e 0a0a 3e20  end service...> 
-000026f0: 2a2a 4e6f 7465 2a2a 0a3e 2049 6620 796f  **Note**.> If yo
-00002700: 7520 6a75 7374 2077 616e 7420 746f 2073  u just want to s
-00002710: 6572 7665 2061 2073 696e 676c 6520 4578  erve a single Ex
-00002720: 6563 7574 6f72 2c20 796f 7520 6361 6e20  ecutor, you can 
-00002730: 7573 6520 6120 5b44 6570 6c6f 796d 656e  use a [Deploymen
-00002740: 745d 2823 6275 696c 642d 6169 2d2d 6d6c  t](#build-ai--ml
-00002750: 2d73 6572 7669 6365 7329 2e0a 0a46 6f72  -services)...For
-00002760: 2069 6e73 7461 6e63 652c 206c 6574 2773   instance, let's
-00002770: 2063 6f6d 6269 6e65 205b 6f75 7220 5374   combine [our St
-00002780: 6162 6c65 4c4d 206c 616e 6775 6167 6520  ableLM language 
-00002790: 6d6f 6465 6c5d 2823 6275 696c 642d 6169  model](#build-ai
-000027a0: 2d2d 6d6c 2d73 6572 7669 6365 7329 2077  --ml-services) w
-000027b0: 6974 6820 6120 5374 6162 6c65 2044 6966  ith a Stable Dif
-000027c0: 6675 7369 6f6e 2069 6d61 6765 2067 656e  fusion image gen
-000027d0: 6572 6174 696f 6e20 7365 7276 6963 6520  eration service 
-000027e0: 6672 6f6d 2043 6d6f 6e20 4149 2773 205b  from Cmon AI's [
-000027f0: 4578 6563 7574 6f72 2048 7562 5d28 6874  Executor Hub](ht
-00002800: 7470 733a 2f2f 636c 6f75 642e 636d 6f6e  tps://cloud.cmon
-00002810: 2e61 692f 6578 6563 7574 6f72 7329 2e20  .ai/executors). 
-00002820: 4368 6169 6e69 6e67 2074 6865 7365 2073  Chaining these s
-00002830: 6572 7669 6365 7320 746f 6765 7468 6572  ervices together
-00002840: 2069 6e74 6f20 6120 5b46 6c6f 775d 2868   into a [Flow](h
-00002850: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-00002860: 2e61 692f 636f 6e63 6570 7473 2f66 6c6f  .ai/concepts/flo
-00002870: 772f 2920 7769 6c6c 2067 6976 6520 7573  w/) will give us
-00002880: 2061 2073 6572 7669 6365 2074 6861 7420   a service that 
-00002890: 7769 6c6c 2067 656e 6572 6174 6520 696d  will generate im
-000028a0: 6167 6573 2062 6173 6564 206f 6e20 6120  ages based on a 
-000028b0: 7072 6f6d 7074 2067 656e 6572 6174 6564  prompt generated
-000028c0: 2062 7920 7468 6520 4c4c 4d2e 0a0a 215b   by the LLM...![
-000028d0: 5d28 2e2f 2e67 6974 6875 622f 696d 6167  ](./.github/imag
-000028e0: 6573 2f66 6c6f 772d 6469 6167 7261 6d2e  es/flow-diagram.
-000028f0: 706e 6729 0a0a 4275 696c 6420 7468 6520  png)..Build the 
-00002900: 466c 6f77 2077 6974 6820 6569 7468 6572  Flow with either
-00002910: 2050 7974 686f 6e20 6f72 2059 414d 4c3a   Python or YAML:
-00002920: 0a0a 3c64 6976 2063 6c61 7373 3d22 7461  ..<div class="ta
-00002930: 626c 652d 7772 6170 7065 7222 3e0a 3c74  ble-wrapper">.<t
-00002940: 6162 6c65 3e0a 3c74 723e 0a3c 7468 3e20  able>.<tr>.<th> 
-00002950: 5079 7468 6f6e 2041 5049 3a20 3c63 6f64  Python API: <cod
-00002960: 653e 666c 6f77 2e70 793c 2f63 6f64 653e  e>flow.py</code>
-00002970: 203c 2f74 683e 200a 3c74 683e 2059 414d   </th> .<th> YAM
-00002980: 4c3a 203c 636f 6465 3e66 6c6f 772e 796d  L: <code>flow.ym
-00002990: 6c3c 2f63 6f64 653e 203c 2f74 683e 0a3c  l</code> </th>.<
-000029a0: 2f74 723e 0a3c 7472 3e0a 3c74 643e 0a0a  /tr>.<tr>.<td>..
-000029b0: 6060 6070 7974 686f 6e0a 6672 6f6d 2063  ```python.from c
-000029c0: 6d6f 6e20 696d 706f 7274 2046 6c6f 770a  mon import Flow.
-000029d0: 6672 6f6d 2065 7865 6375 746f 7220 696d  from executor im
-000029e0: 706f 7274 2053 7461 626c 654c 4d0a 0a66  port StableLM..f
-000029f0: 6c6f 7720 3d20 280a 2020 2020 466c 6f77  low = (.    Flow
-00002a00: 2829 0a20 2020 202e 6164 6428 7573 6573  ().    .add(uses
-00002a10: 3d53 7461 626c 654c 4d2c 2074 696d 656f  =StableLM, timeo
-00002a20: 7574 5f72 6561 6479 3d2d 312c 2070 6f72  ut_ready=-1, por
-00002a30: 743d 3132 3334 3529 0a20 2020 202e 6164  t=12345).    .ad
-00002a40: 6428 0a20 2020 2020 2020 2075 7365 733d  d(.        uses=
-00002a50: 2763 6d6f 6e61 693a 2f2f 636d 6f6e 2d61  'cmonai://cmon-a
-00002a60: 692f 5465 7874 546f 496d 6167 6527 2c0a  i/TextToImage',.
-00002a70: 2020 2020 2020 2020 7469 6d65 6f75 745f          timeout_
-00002a80: 7265 6164 793d 2d31 2c0a 2020 2020 2020  ready=-1,.      
-00002a90: 2020 696e 7374 616c 6c5f 7265 7175 6972    install_requir
-00002aa0: 656d 656e 7473 3d54 7275 652c 0a20 2020  ements=True,.   
-00002ab0: 2029 0a29 2020 2320 7573 6520 7468 6520   ).)  # use the 
-00002ac0: 4578 6563 7574 6f72 2066 726f 6d20 436d  Executor from Cm
-00002ad0: 6f6e 2773 2045 7865 6375 746f 7220 6875  on's Executor hu
-00002ae0: 620a 0a77 6974 6820 666c 6f77 3a0a 2020  b..with flow:.  
-00002af0: 2020 666c 6f77 2e62 6c6f 636b 2829 0a60    flow.block().`
-00002b00: 6060 0a0a 3c2f 7464 3e0a 3c74 643e 0a0a  ``..</td>.<td>..
-00002b10: 6060 6079 616d 6c0a 6a74 7970 653a 2046  ```yaml.jtype: F
-00002b20: 6c6f 770a 7769 7468 3a0a 2020 2020 706f  low.with:.    po
-00002b30: 7274 3a20 3132 3334 350a 6578 6563 7574  rt: 12345.execut
-00002b40: 6f72 733a 0a20 202d 2075 7365 733a 2053  ors:.  - uses: S
-00002b50: 7461 626c 654c 4d0a 2020 2020 7469 6d65  tableLM.    time
-00002b60: 6f75 745f 7265 6164 793a 202d 310a 2020  out_ready: -1.  
-00002b70: 2020 7079 5f6d 6f64 756c 6573 3a0a 2020    py_modules:.  
-00002b80: 2020 2020 2d20 6578 6563 7574 6f72 2e70      - executor.p
-00002b90: 790a 2020 2d20 7573 6573 3a20 636d 6f6e  y.  - uses: cmon
-00002ba0: 6169 3a2f 2f63 6d6f 6e2d 6169 2f54 6578  ai://cmon-ai/Tex
-00002bb0: 7454 6f49 6d61 6765 0a20 2020 2074 696d  tToImage.    tim
-00002bc0: 656f 7574 5f72 6561 6479 3a20 2d31 0a20  eout_ready: -1. 
-00002bd0: 2020 2069 6e73 7461 6c6c 5f72 6571 7569     install_requi
-00002be0: 7265 6d65 6e74 733a 2074 7275 650a 6060  rements: true.``
-00002bf0: 600a 0a54 6865 6e20 7275 6e20 7468 6520  `..Then run the 
-00002c00: 5941 4d4c 2046 6c6f 7720 7769 7468 2074  YAML Flow with t
-00002c10: 6865 2043 4c49 3a20 6063 6d6f 6e20 666c  he CLI: `cmon fl
-00002c20: 6f77 202d 2d75 7365 7320 666c 6f77 2e79  ow --uses flow.y
-00002c30: 6d6c 600a 0a3c 2f74 643e 0a3c 2f74 723e  ml`..</td>.</tr>
-00002c40: 0a3c 2f74 6162 6c65 3e0a 3c2f 6469 763e  .</table>.</div>
-00002c50: 0a0a 5468 656e 2c20 7573 6520 5b43 6d6f  ..Then, use [Cmo
-00002c60: 6e20 436c 6965 6e74 5d28 6874 7470 733a  n Client](https:
-00002c70: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-00002c80: 6f6e 6365 7074 732f 636c 6965 6e74 2f29  oncepts/client/)
-00002c90: 2074 6f20 6d61 6b65 2072 6571 7565 7374   to make request
-00002ca0: 7320 746f 2074 6865 2046 6c6f 773a 0a0a  s to the Flow:..
-00002cb0: 6060 6070 7974 686f 6e0a 6672 6f6d 2063  ```python.from c
-00002cc0: 6d6f 6e20 696d 706f 7274 2043 6c69 656e  mon import Clien
-00002cd0: 742c 2044 6f63 756d 656e 740a 0a63 6c69  t, Document..cli
-00002ce0: 656e 7420 3d20 436c 6965 6e74 2870 6f72  ent = Client(por
-00002cf0: 743d 3132 3334 3529 0a0a 7072 6f6d 7074  t=12345)..prompt
-00002d00: 203d 2044 6f63 756d 656e 7428 0a20 2020   = Document(.   
-00002d10: 2074 6167 7320 3d20 7b27 7072 6f6d 7074   tags = {'prompt
-00002d20: 273a 2027 7375 6767 6573 7420 616e 2069  ': 'suggest an i
-00002d30: 6e74 6572 6573 7469 6e67 2069 6d61 6765  nteresting image
-00002d40: 2067 656e 6572 6174 696f 6e20 7072 6f6d   generation prom
-00002d50: 7074 2066 6f72 2061 206d 6f6e 6120 6c69  pt for a mona li
-00002d60: 7361 2076 6172 6961 6e74 277d 0a29 0a0a  sa variant'}.)..
-00002d70: 7265 7370 6f6e 7365 203d 2063 6c69 656e  response = clien
-00002d80: 742e 706f 7374 286f 6e3d 272f 272c 2069  t.post(on='/', i
-00002d90: 6e70 7574 733d 5b70 726f 6d70 745d 290a  nputs=[prompt]).
-00002da0: 0a72 6573 706f 6e73 655b 305d 2e64 6973  .response[0].dis
-00002db0: 706c 6179 2829 0a60 6060 0a0a 215b 5d28  play().```..![](
-00002dc0: 2e2f 2e67 6974 6875 622f 696d 6167 6573  ./.github/images
-00002dd0: 2f6d 6f6e 612d 6c69 7361 2e70 6e67 290a  /mona-lisa.png).
-00002de0: 0a23 2320 4465 706c 6f79 2074 6f20 7468  .## Deploy to th
-00002df0: 6520 636c 6f75 640a 0a59 6f75 2063 616e  e cloud..You can
-00002e00: 2061 6c73 6f20 6465 706c 6f79 2061 2046   also deploy a F
-00002e10: 6c6f 7720 746f 204a 436c 6f75 642e 0a0a  low to JCloud...
-00002e20: 4669 7273 742c 2074 7572 6e20 7468 6520  First, turn the 
-00002e30: 6066 6c6f 772e 796d 6c60 2066 696c 6520  `flow.yml` file 
-00002e40: 696e 746f 2061 205b 4a43 6c6f 7564 2d63  into a [JCloud-c
-00002e50: 6f6d 7061 7469 626c 6520 5941 4d4c 5d28  ompatible YAML](
-00002e60: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
-00002e70: 6e2e 6169 2f63 6f6e 6365 7074 732f 6a63  n.ai/concepts/jc
-00002e80: 6c6f 7564 2f79 616d 6c2d 7370 6563 2f29  loud/yaml-spec/)
-00002e90: 2062 7920 7370 6563 6966 7969 6e67 2072   by specifying r
-00002ea0: 6573 6f75 7263 6520 7265 7175 6972 656d  esource requirem
-00002eb0: 656e 7473 2061 6e64 2075 7369 6e67 2063  ents and using c
-00002ec0: 6f6e 7461 696e 6572 697a 6564 2048 7562  ontainerized Hub
-00002ed0: 2045 7865 6375 746f 7273 2e0a 0a54 6865   Executors...The
-00002ee0: 6e2c 2075 7365 2060 636d 6f6e 2063 6c6f  n, use `cmon clo
-00002ef0: 7564 2064 6570 6c6f 7960 2063 6f6d 6d61  ud deploy` comma
-00002f00: 6e64 2074 6f20 6465 706c 6f79 2074 6f20  nd to deploy to 
-00002f10: 7468 6520 636c 6f75 643a 0a0a 6060 6073  the cloud:..```s
-00002f20: 6865 6c6c 0a77 6765 7420 6874 7470 733a  hell.wget https:
-00002f30: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00002f40: 636f 6e74 656e 742e 636f 6d2f 636d 6f6e  content.com/cmon
-00002f50: 2d61 692f 636d 6f6e 2f6d 6173 7465 722f  -ai/cmon/master/
-00002f60: 2e67 6974 6875 622f 6765 7474 696e 672d  .github/getting-
-00002f70: 7374 6172 7465 642f 6a63 6c6f 7564 2d66  started/jcloud-f
-00002f80: 6c6f 772e 796d 6c0a 636d 6f6e 2063 6c6f  low.yml.cmon clo
-00002f90: 7564 2064 6570 6c6f 7920 6a63 6c6f 7564  ud deploy jcloud
-00002fa0: 2d66 6c6f 772e 796d 6c0a 6060 600a 0a3e  -flow.yml.```..>
-00002fb0: 202a 2a57 6172 6e69 6e67 2a2a 0a3e 0a3e   **Warning**.>.>
-00002fc0: 204d 616b 6520 7375 7265 2074 6f20 6465   Make sure to de
-00002fd0: 6c65 7465 2f63 6c65 616e 2075 7020 7468  lete/clean up th
-00002fe0: 6520 466c 6f77 206f 6e63 6520 796f 7520  e Flow once you 
-00002ff0: 6172 6520 646f 6e65 2077 6974 6820 7468  are done with th
-00003000: 6973 2074 7574 6f72 6961 6c20 746f 2073  is tutorial to s
-00003010: 6176 6520 7265 736f 7572 6365 7320 616e  ave resources an
-00003020: 6420 6372 6564 6974 732e 0a0a 5265 6164  d credits...Read
-00003030: 206d 6f72 6520 6162 6f75 7420 5b64 6570   more about [dep
-00003040: 6c6f 7969 6e67 2046 6c6f 7773 2074 6f20  loying Flows to 
-00003050: 4a43 6c6f 7564 5d28 6874 7470 733a 2f2f  JCloud](https://
-00003060: 646f 6373 2e63 6d6f 6e2e 6169 2f63 6f6e  docs.cmon.ai/con
-00003070: 6365 7074 732f 6a63 6c6f 7564 2f23 6465  cepts/jcloud/#de
-00003080: 706c 6f79 292e 0a0a 3c21 2d2d 2065 6e64  ploy)...<!-- end
-00003090: 2062 7569 6c64 2d70 6970 656c 696e 6573   build-pipelines
-000030a0: 202d 2d3e 0a0a 4368 6563 6b20 5b74 6865   -->..Check [the
-000030b0: 2067 6574 7469 6e67 2d73 7461 7274 6564   getting-started
-000030c0: 2070 726f 6a65 6374 2073 6f75 7263 6520   project source 
-000030d0: 636f 6465 5d28 6874 7470 733a 2f2f 6769  code](https://gi
-000030e0: 7468 7562 2e63 6f6d 2f63 6d6f 6e2d 6169  thub.com/cmon-ai
-000030f0: 2f63 6d6f 6e2f 7472 6565 2f6d 6173 7465  /cmon/tree/maste
-00003100: 722f 2e67 6974 6875 622f 6765 7474 696e  r/.github/gettin
-00003110: 672d 7374 6172 7465 6429 2e0a 0a23 2323  g-started)...###
-00003120: 2045 6173 7920 7363 616c 6162 696c 6974   Easy scalabilit
-00003130: 7920 616e 6420 636f 6e63 7572 7265 6e63  y and concurrenc
-00003140: 790a 0a57 6879 206e 6f74 206a 7573 7420  y..Why not just 
-00003150: 7573 6520 7374 616e 6461 7264 2050 7974  use standard Pyt
-00003160: 686f 6e20 746f 2062 7569 6c64 2074 6861  hon to build tha
-00003170: 7420 6d69 6372 6f73 6572 7669 6365 2061  t microservice a
-00003180: 6e64 2070 6970 656c 696e 653f 2043 6d6f  nd pipeline? Cmo
-00003190: 6e20 6163 6365 6c65 7261 7465 7320 7469  n accelerates ti
-000031a0: 6d65 2074 6f20 6d61 726b 6574 206f 6620  me to market of 
-000031b0: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
-000031c0: 2062 7920 6d61 6b69 6e67 2069 7420 6d6f   by making it mo
-000031d0: 7265 2073 6361 6c61 626c 6520 616e 6420  re scalable and 
-000031e0: 636c 6f75 642d 6e61 7469 7665 2e20 436d  cloud-native. Cm
-000031f0: 6f6e 2061 6c73 6f20 6861 6e64 6c65 7320  on also handles 
-00003200: 7468 6520 696e 6672 6173 7472 7563 7475  the infrastructu
-00003210: 7265 2063 6f6d 706c 6578 6974 7920 696e  re complexity in
-00003220: 2070 726f 6475 6374 696f 6e20 616e 6420   production and 
-00003230: 6f74 6865 7220 4461 792d 3220 6f70 6572  other Day-2 oper
-00003240: 6174 696f 6e73 2073 6f20 7468 6174 2079  ations so that y
-00003250: 6f75 2063 616e 2066 6f63 7573 206f 6e20  ou can focus on 
-00003260: 7468 6520 6461 7461 2061 7070 6c69 6361  the data applica
-00003270: 7469 6f6e 2069 7473 656c 662e 0a0a 496e  tion itself...In
-00003280: 6372 6561 7365 2079 6f75 7220 6170 706c  crease your appl
-00003290: 6963 6174 696f 6e27 7320 7468 726f 7567  ication's throug
-000032a0: 6870 7574 2077 6974 6820 7363 616c 6162  hput with scalab
-000032b0: 696c 6974 7920 6665 6174 7572 6573 206f  ility features o
-000032c0: 7574 206f 6620 7468 6520 626f 782c 206c  ut of the box, l
-000032d0: 696b 6520 5b72 6570 6c69 6361 735d 2868  ike [replicas](h
-000032e0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-000032f0: 2e61 692f 636f 6e63 6570 7473 2f6f 7263  .ai/concepts/orc
-00003300: 6865 7374 7261 7469 6f6e 2f73 6361 6c65  hestration/scale
-00003310: 2d6f 7574 2f23 7265 706c 6963 6174 652d  -out/#replicate-
-00003320: 6578 6563 7574 6f72 7329 2c20 5b73 6861  executors), [sha
-00003330: 7264 735d 2868 7474 7073 3a2f 2f64 6f63  rds](https://doc
-00003340: 732e 636d 6f6e 2e61 692f 636f 6e63 6570  s.cmon.ai/concep
-00003350: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
-00003360: 2f73 6361 6c65 2d6f 7574 2f23 6375 7374  /scale-out/#cust
-00003370: 6f6d 697a 652d 706f 6c6c 696e 672d 6265  omize-polling-be
-00003380: 6861 7669 6f72 7329 2061 6e64 205b 6479  haviors) and [dy
-00003390: 6e61 6d69 6320 6261 7463 6869 6e67 5d28  namic batching](
-000033a0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
-000033b0: 6e2e 6169 2f63 6f6e 6365 7074 732f 7365  n.ai/concepts/se
-000033c0: 7276 696e 672f 6578 6563 7574 6f72 2f64  rving/executor/d
-000033d0: 796e 616d 6963 2d62 6174 6368 696e 672f  ynamic-batching/
-000033e0: 292e 0a0a 4c65 7427 7320 7363 616c 6520  )...Let's scale 
-000033f0: 6120 5374 6162 6c65 2044 6966 6675 7369  a Stable Diffusi
-00003400: 6f6e 2045 7865 6375 746f 7220 6465 706c  on Executor depl
-00003410: 6f79 6d65 6e74 2077 6974 6820 7265 706c  oyment with repl
-00003420: 6963 6173 2061 6e64 2064 796e 616d 6963  icas and dynamic
-00003430: 2062 6174 6368 696e 673a 0a0a 215b 5d28   batching:..![](
-00003440: 2e2f 2e67 6974 6875 622f 696d 6167 6573  ./.github/images
-00003450: 2f73 6361 6c65 642d 6465 706c 6f79 6d65  /scaled-deployme
-00003460: 6e74 2e70 6e67 290a 0a2a 2043 7265 6174  nt.png)..* Creat
-00003470: 6520 7477 6f20 7265 706c 6963 6173 2c20  e two replicas, 
-00003480: 7769 7468 205b 6120 4750 5520 6173 7369  with [a GPU assi
-00003490: 676e 6564 2066 6f72 2065 6163 685d 2868  gned for each](h
-000034a0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
-000034b0: 2e61 692f 636f 6e63 6570 7473 2f66 6c6f  .ai/concepts/flo
-000034c0: 772f 7363 616c 652d 6f75 742f 2372 6570  w/scale-out/#rep
-000034d0: 6c69 6361 7465 2d6f 6e2d 6d75 6c74 6970  licate-on-multip
-000034e0: 6c65 2d67 7075 7329 2e0a 2a20 456e 6162  le-gpus)..* Enab
-000034f0: 6c65 2064 796e 616d 6963 2062 6174 6368  le dynamic batch
-00003500: 696e 6720 746f 2070 726f 6365 7373 2069  ing to process i
-00003510: 6e63 6f6d 696e 6720 7061 7261 6c6c 656c  ncoming parallel
-00003520: 2072 6571 7565 7374 7320 746f 6765 7468   requests togeth
-00003530: 6572 2077 6974 6820 7468 6520 7361 6d65  er with the same
-00003540: 206d 6f64 656c 2069 6e66 6572 656e 6365   model inference
-00003550: 2e0a 0a0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
-00003560: 7461 626c 652d 7772 6170 7065 7222 3e0a  table-wrapper">.
-00003570: 3c74 6162 6c65 3e0a 3c74 723e 0a3c 7468  <table>.<tr>.<th
-00003580: 3e20 4e6f 726d 616c 2044 6570 6c6f 796d  > Normal Deploym
-00003590: 656e 7420 3c2f 7468 3e20 0a3c 7468 3e20  ent </th> .<th> 
-000035a0: 5363 616c 6564 2044 6570 6c6f 796d 656e  Scaled Deploymen
-000035b0: 7420 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74  t </th>.</tr>.<t
-000035c0: 723e 0a3c 7464 3e0a 0a60 6060 7961 6d6c  r>.<td>..```yaml
-000035d0: 0a6a 7479 7065 3a20 4465 706c 6f79 6d65  .jtype: Deployme
-000035e0: 6e74 0a77 6974 683a 0a20 2074 696d 656f  nt.with:.  timeo
-000035f0: 7574 5f72 6561 6479 3a20 2d31 0a20 2075  ut_ready: -1.  u
-00003600: 7365 733a 2063 6d6f 6e61 693a 2f2f 636d  ses: cmonai://cm
-00003610: 6f6e 2d61 692f 5465 7874 546f 496d 6167  on-ai/TextToImag
-00003620: 650a 2020 696e 7374 616c 6c5f 7265 7175  e.  install_requ
-00003630: 6972 656d 656e 7473 3a20 7472 7565 0a60  irements: true.`
-00003640: 6060 0a0a 3c2f 7464 3e0a 3c74 643e 0a0a  ``..</td>.<td>..
-00003650: 6060 6079 616d 6c0a 6a74 7970 653a 2044  ```yaml.jtype: D
-00003660: 6570 6c6f 796d 656e 740a 7769 7468 3a0a  eployment.with:.
-00003670: 2020 7469 6d65 6f75 745f 7265 6164 793a    timeout_ready:
-00003680: 202d 310a 2020 7573 6573 3a20 636d 6f6e   -1.  uses: cmon
-00003690: 6169 3a2f 2f63 6d6f 6e2d 6169 2f54 6578  ai://cmon-ai/Tex
-000036a0: 7454 6f49 6d61 6765 0a20 2069 6e73 7461  tToImage.  insta
-000036b0: 6c6c 5f72 6571 7569 7265 6d65 6e74 733a  ll_requirements:
-000036c0: 2074 7275 650a 2020 656e 763a 0a20 2020   true.  env:.   
-000036d0: 4355 4441 5f56 4953 4942 4c45 5f44 4556  CUDA_VISIBLE_DEV
-000036e0: 4943 4553 3a20 5252 0a20 2072 6570 6c69  ICES: RR.  repli
-000036f0: 6361 733a 2032 0a20 2075 7365 735f 6479  cas: 2.  uses_dy
-00003700: 6e61 6d69 635f 6261 7463 6869 6e67 3a20  namic_batching: 
-00003710: 2320 636f 6e66 6967 7572 6520 6479 6e61  # configure dyna
-00003720: 6d69 6320 6261 7463 6869 6e67 0a20 2020  mic batching.   
-00003730: 202f 6465 6661 756c 743a 0a20 2020 2020   /default:.     
-00003740: 2070 7265 6665 7272 6564 5f62 6174 6368   preferred_batch
-00003750: 5f73 697a 653a 2031 300a 2020 2020 2020  _size: 10.      
-00003760: 7469 6d65 6f75 743a 2032 3030 0a60 6060  timeout: 200.```
-00003770: 0a0a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c2f  ..</td>.</tr>.</
-00003780: 7461 626c 653e 0a3c 2f64 6976 3e0a 0a41  table>.</div>..A
-00003790: 7373 756d 696e 6720 796f 7572 206d 6163  ssuming your mac
-000037a0: 6869 6e65 2068 6173 2074 776f 2047 5055  hine has two GPU
-000037b0: 732c 2075 7369 6e67 2074 6865 2073 6361  s, using the sca
-000037c0: 6c65 6420 6465 706c 6f79 6d65 6e74 2059  led deployment Y
-000037d0: 414d 4c20 7769 6c6c 2067 6976 6520 6265  AML will give be
-000037e0: 7474 6572 2074 6872 6f75 6768 7075 7420  tter throughput 
-000037f0: 636f 6d70 6172 6564 2074 6f20 7468 6520  compared to the 
-00003800: 6e6f 726d 616c 2064 6570 6c6f 796d 656e  normal deploymen
-00003810: 742e 0a0a 5468 6573 6520 6665 6174 7572  t...These featur
-00003820: 6573 2061 7070 6c79 2074 6f20 626f 7468  es apply to both
-00003830: 205b 4465 706c 6f79 6d65 6e74 2059 414d   [Deployment YAM
-00003840: 4c5d 2868 7474 7073 3a2f 2f64 6f63 732e  L](https://docs.
-00003850: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-00003860: 2f65 7865 6375 746f 722f 6465 706c 6f79  /executor/deploy
-00003870: 6d65 6e74 2d79 616d 6c2d 7370 6563 2f23  ment-yaml-spec/#
-00003880: 6465 706c 6f79 6d65 6e74 2d79 616d 6c2d  deployment-yaml-
-00003890: 7370 6563 2920 616e 6420 5b46 6c6f 7720  spec) and [Flow 
-000038a0: 5941 4d4c 5d28 6874 7470 733a 2f2f 646f  YAML](https://do
-000038b0: 6373 2e63 6d6f 6e2e 6169 2f63 6f6e 6365  cs.cmon.ai/conce
-000038c0: 7074 732f 666c 6f77 2f79 616d 6c2d 7370  pts/flow/yaml-sp
-000038d0: 6563 2f29 2e20 5468 616e 6b73 2074 6f20  ec/). Thanks to 
-000038e0: 7468 6520 5941 4d4c 2073 796e 7461 782c  the YAML syntax,
-000038f0: 2079 6f75 2063 616e 2069 6e6a 6563 7420   you can inject 
-00003900: 6465 706c 6f79 6d65 6e74 2063 6f6e 6669  deployment confi
-00003910: 6775 7261 7469 6f6e 7320 7265 6761 7264  gurations regard
-00003920: 6c65 7373 206f 6620 4578 6563 7574 6f72  less of Executor
-00003930: 2063 6f64 652e 0a0a 2323 2320 4765 7420   code...### Get 
-00003940: 6f6e 2074 6865 2066 6173 7420 6c61 6e65  on the fast lane
-00003950: 2074 6f20 636c 6f75 642d 6e61 7469 7665   to cloud-native
-00003960: 0a0a 5573 696e 6720 4b75 6265 726e 6574  ..Using Kubernet
-00003970: 6573 2077 6974 6820 436d 6f6e 2069 7320  es with Cmon is 
-00003980: 6561 7379 3a0a 0a60 6060 6261 7368 0a63  easy:..```bash.c
-00003990: 6d6f 6e20 6578 706f 7274 206b 7562 6572  mon export kuber
-000039a0: 6e65 7465 7320 666c 6f77 2e79 6d6c 202e  netes flow.yml .
-000039b0: 2f6d 792d 6b38 730a 6b75 6265 6374 6c20  /my-k8s.kubectl 
-000039c0: 6170 706c 7920 2d52 202d 6620 6d79 2d6b  apply -R -f my-k
-000039d0: 3873 0a60 6060 0a0a 416e 6420 736f 2069  8s.```..And so i
-000039e0: 7320 446f 636b 6572 2043 6f6d 706f 7365  s Docker Compose
-000039f0: 3a0a 0a60 6060 6261 7368 0a63 6d6f 6e20  :..```bash.cmon 
-00003a00: 6578 706f 7274 2064 6f63 6b65 722d 636f  export docker-co
-00003a10: 6d70 6f73 6520 666c 6f77 2e79 6d6c 2064  mpose flow.yml d
-00003a20: 6f63 6b65 722d 636f 6d70 6f73 652e 796d  ocker-compose.ym
-00003a30: 6c0a 646f 636b 6572 2d63 6f6d 706f 7365  l.docker-compose
-00003a40: 2075 700a 6060 600a 0a3e 202a 2a4e 6f74   up.```..> **Not
-00003a50: 652a 2a0a 3e20 596f 7520 6361 6e20 616c  e**.> You can al
-00003a60: 736f 2065 7870 6f72 7420 4465 706c 6f79  so export Deploy
-00003a70: 6d65 6e74 2059 414d 4c20 746f 205b 4b75  ment YAML to [Ku
-00003a80: 6265 726e 6574 6573 5d28 6874 7470 733a  bernetes](https:
-00003a90: 2f2f 646f 6373 2e63 6d6f 6e2e 6169 2f63  //docs.cmon.ai/c
-00003aa0: 6f6e 6365 7074 732f 6578 6563 7574 6f72  oncepts/executor
-00003ab0: 2f73 6572 7665 2f23 7365 7276 652d 7669  /serve/#serve-vi
-00003ac0: 612d 6b75 6265 726e 6574 6573 2920 616e  a-kubernetes) an
-00003ad0: 6420 5b44 6f63 6b65 7220 436f 6d70 6f73  d [Docker Compos
-00003ae0: 655d 2868 7474 7073 3a2f 2f64 6f63 732e  e](https://docs.
-00003af0: 636d 6f6e 2e61 692f 636f 6e63 6570 7473  cmon.ai/concepts
-00003b00: 2f65 7865 6375 746f 722f 7365 7276 652f  /executor/serve/
-00003b10: 2373 6572 7665 2d76 6961 2d64 6f63 6b65  #serve-via-docke
-00003b20: 722d 636f 6d70 6f73 6529 2e0a 0a54 6861  r-compose)...Tha
-00003b30: 7427 7320 6e6f 7420 616c 6c2e 2057 6520  t's not all. We 
-00003b40: 616c 736f 2073 7570 706f 7274 205b 4f70  also support [Op
-00003b50: 656e 5465 6c65 6d65 7472 792c 2050 726f  enTelemetry, Pro
-00003b60: 6d65 7468 6575 732c 2061 6e64 204a 6165  metheus, and Jae
-00003b70: 6765 725d 2868 7474 7073 3a2f 2f64 6f63  ger](https://doc
-00003b80: 732e 636d 6f6e 2e61 692f 636c 6f75 642d  s.cmon.ai/cloud-
-00003b90: 6e61 7469 7665 6e65 7373 2f6f 7065 6e74  nativeness/opent
-00003ba0: 656c 656d 6574 7279 2f29 2e0a 0a57 6861  elemetry/)...Wha
-00003bb0: 7420 636c 6f75 642d 6e61 7469 7665 2074  t cloud-native t
-00003bc0: 6563 686e 6f6c 6f67 7920 6973 2073 7469  echnology is sti
-00003bd0: 6c6c 2063 6861 6c6c 656e 6769 6e67 2074  ll challenging t
-00003be0: 6f20 796f 753f 205b 5465 6c6c 2075 735d  o you? [Tell us]
-00003bf0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003c00: 636f 6d2f 636d 6f6e 2d61 692f 636d 6f6e  com/cmon-ai/cmon
-00003c10: 2f69 7373 7565 7329 2061 6e64 2077 6527  /issues) and we'
-00003c20: 6c6c 2068 616e 646c 6520 7468 6520 636f  ll handle the co
-00003c30: 6d70 6c65 7869 7479 2061 6e64 206d 616b  mplexity and mak
-00003c40: 6520 6974 2065 6173 7920 666f 7220 796f  e it easy for yo
-00003c50: 752e 0a0a 3c21 2d2d 2073 7461 7274 2073  u...<!-- start s
-00003c60: 7570 706f 7274 2d70 6974 6368 202d 2d3e  upport-pitch -->
-00003c70: 0a0a 2323 2053 7570 706f 7274 0a0a 2d20  ..## Support..- 
-00003c80: 4a6f 696e 206f 7572 205b 4469 7363 6f72  Join our [Discor
-00003c90: 6420 636f 6d6d 756e 6974 795d 2868 7474  d community](htt
-00003ca0: 7073 3a2f 2f64 6973 636f 7264 2e63 6d6f  ps://discord.cmo
-00003cb0: 6e2e 6169 2920 616e 6420 6368 6174 2077  n.ai) and chat w
-00003cc0: 6974 6820 6f74 6865 7220 636f 6d6d 756e  ith other commun
-00003cd0: 6974 7920 6d65 6d62 6572 7320 6162 6f75  ity members abou
-00003ce0: 7420 6964 6561 732e 0a2d 2053 7562 7363  t ideas..- Subsc
-00003cf0: 7269 6265 2074 6f20 7468 6520 6c61 7465  ribe to the late
-00003d00: 7374 2076 6964 656f 2074 7574 6f72 6961  st video tutoria
-00003d10: 6c73 206f 6e20 6f75 7220 5b59 6f75 5475  ls on our [YouTu
-00003d20: 6265 2063 6861 6e6e 656c 5d28 6874 7470  be channel](http
-00003d30: 733a 2f2f 796f 7574 7562 652e 636f 6d2f  s://youtube.com/
-00003d40: 632f 636d 6f6e 2d61 6929 0a0a 2323 204a  c/cmon-ai)..## J
-00003d50: 6f69 6e20 5573 0a0a 436d 6f6e 2069 7320  oin Us..Cmon is 
-00003d60: 6261 636b 6564 2062 7920 5b43 6d6f 6e20  backed by [Cmon 
-00003d70: 4149 5d28 6874 7470 733a 2f2f 636d 6f6e  AI](https://cmon
-00003d80: 2e61 6929 2061 6e64 206c 6963 656e 7365  .ai) and license
-00003d90: 6420 756e 6465 7220 5b41 7061 6368 652d  d under [Apache-
-00003da0: 322e 305d 282e 2f4c 4943 454e 5345 292e  2.0](./LICENSE).
-00003db0: 0a0a 3c21 2d2d 2065 6e64 2073 7570 706f  ..<!-- end suppo
-00003dc0: 7274 2d70 6974 6368 202d 2d3e 0a         rt-pitch -->.
+00000010: 3a20 322e 310d 0a4e 616d 653a 2063 6d6f  : 2.1..Name: cmo
+00000020: 6e2d 6169 0d0a 5665 7273 696f 6e3a 2030  n-ai..Version: 0
+00000030: 2e34 322e 360d 0a53 756d 6d61 7279 3a20  .42.6..Summary: 
+00000040: 4275 696c 6420 6d75 6c74 696d 6f64 616c  Build multimodal
+00000050: 2041 4920 7365 7276 6963 6573 2076 6961   AI services via
+00000060: 2063 6c6f 7564 206e 6174 6976 6520 7465   cloud native te
+00000070: 6368 6e6f 6c6f 6769 6573 20c2 b720 4e65  chnologies .. Ne
+00000080: 7572 616c 2053 6561 7263 6820 c2b7 2047  ural Search .. G
+00000090: 656e 6572 6174 6976 6520 4149 20c2 b720  enerative AI .. 
+000000a0: 4d4c 4f70 730d 0a48 6f6d 652d 7061 6765  MLOps..Home-page
+000000b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000c0: 2e63 6f6d 2f6f 7065 6e61 692d 6165 2f43  .com/openai-ae/C
+000000d0: 6d6f 6e2d 4149 2d4c 6962 7261 7279 0d0a  mon-AI-Library..
+000000e0: 446f 776e 6c6f 6164 2d55 524c 3a20 6874  Download-URL: ht
+000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000100: 2f6f 7065 6e61 692d 6165 2f43 6d6f 6e2d  /openai-ae/Cmon-
+00000110: 4149 2d4c 6962 7261 7279 2f61 7263 6869  AI-Library/archi
+00000120: 7665 2f72 6566 732f 7461 6773 2f41 492e  ve/refs/tags/AI.
+00000130: 7a69 700d 0a41 7574 686f 723a 2043 6d6f  zip..Author: Cmo
+00000140: 6e20 4149 0d0a 4175 7468 6f72 2d65 6d61  n AI..Author-ema
+00000150: 696c 3a20 6865 6c6c 6f40 636d 6f6e 2e70  il: hello@cmon.p
+00000160: 770d 0a4c 6963 656e 7365 3a20 4170 6163  w..License: Apac
+00000170: 6865 2032 2e30 0d0a 5072 6f6a 6563 742d  he 2.0..Project-
+00000180: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
+00000190: 6f6e 2c20 6874 7470 733a 2f2f 646f 6373  on, https://docs
+000001a0: 2e63 6d6f 6e2e 7077 0d0a 5072 6f6a 6563  .cmon.pw..Projec
+000001b0: 742d 5552 4c3a 2053 6f75 7263 652c 2068  t-URL: Source, h
+000001c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001d0: 6d2f 6f70 656e 6169 2d61 652f 636d 6f6e  m/openai-ae/cmon
+000001e0: 2d61 692f 0d0a 5072 6f6a 6563 742d 5552  -ai/..Project-UR
+000001f0: 4c3a 2054 7261 636b 6572 2c20 6874 7470  L: Tracker, http
+00000200: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000210: 7065 6e61 692d 6165 2f63 6d6f 6e2d 6169  penai-ae/cmon-ai
+00000220: 2f69 7373 7565 730d 0a4b 6579 776f 7264  /issues..Keyword
+00000230: 733a 2063 6d6f 6e20 636c 6f75 642d 6e61  s: cmon cloud-na
+00000240: 7469 7665 2063 726f 7373 2d6d 6f64 616c  tive cross-modal
+00000250: 206d 756c 7469 6d6f 6461 6c20 6e65 7572   multimodal neur
+00000260: 616c 2d73 6561 7263 6820 7175 6572 7920  al-search query 
+00000270: 7365 6172 6368 2069 6e64 6578 2065 6c61  search index ela
+00000280: 7374 6963 206e 6575 7261 6c2d 6e65 7477  stic neural-netw
+00000290: 6f72 6b20 656e 636f 6469 6e67 2065 6d62  ork encoding emb
+000002a0: 6564 6469 6e67 2073 6572 7669 6e67 2064  edding serving d
+000002b0: 6f63 6b65 7220 636f 6e74 6169 6e65 7220  ocker container 
+000002c0: 696d 6167 6520 7669 6465 6f20 6175 6469  image video audi
+000002d0: 6f20 6465 6570 2d6c 6561 726e 696e 6720  o deep-learning 
+000002e0: 6d6c 6f70 730d 0a43 6c61 7373 6966 6965  mlops..Classifie
+000002f0: 723a 2044 6576 656c 6f70 6d65 6e74 2053  r: Development S
+00000300: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
+00000310: 6475 6374 696f 6e2f 5374 6162 6c65 0d0a  duction/Stable..
+00000320: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000330: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000340: 2044 6576 656c 6f70 6572 730d 0a43 6c61   Developers..Cla
+00000350: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000360: 6420 4175 6469 656e 6365 203a 3a20 4564  d Audience :: Ed
+00000370: 7563 6174 696f 6e0d 0a43 6c61 7373 6966  ucation..Classif
+00000380: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
+00000390: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
+000003a0: 652f 5265 7365 6172 6368 0d0a 436c 6173  e/Research..Clas
+000003b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000003c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000003d0: 5079 7468 6f6e 203a 3a20 332e 370d 0a43  Python :: 3.7..C
+000003e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000003f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000400: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000410: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000420: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000430: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000440: 332e 390d 0a43 6c61 7373 6966 6965 723a  3.9..Classifier:
+00000450: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000460: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000470: 3a3a 2033 2e31 300d 0a43 6c61 7373 6966  :: 3.10..Classif
+00000480: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000490: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000004a0: 686f 6e20 3a3a 2033 2e31 310d 0a43 6c61  hon :: 3.11..Cla
+000004b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000004c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000004d0: 2055 6e69 7820 5368 656c 6c0d 0a43 6c61   Unix Shell..Cla
+000004e0: 7373 6966 6965 723a 2045 6e76 6972 6f6e  ssifier: Environ
+000004f0: 6d65 6e74 203a 3a20 436f 6e73 6f6c 650d  ment :: Console.
+00000500: 0a43 6c61 7373 6966 6965 723a 204c 6963  .Classifier: Lic
+00000510: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+00000520: 6f76 6564 203a 3a20 4170 6163 6865 2053  oved :: Apache S
+00000530: 6f66 7477 6172 6520 4c69 6365 6e73 650d  oftware License.
+00000540: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000550: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000560: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000570: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+00000580: 6963 203a 3a20 4461 7461 6261 7365 203a  ic :: Database :
+00000590: 3a20 4461 7461 6261 7365 2045 6e67 696e  : Database Engin
+000005a0: 6573 2f53 6572 7665 7273 0d0a 436c 6173  es/Servers..Clas
+000005b0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000005c0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+000005d0: 6e65 6572 696e 6720 3a3a 2041 7274 6966  neering :: Artif
+000005e0: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+000005f0: 6365 0d0a 436c 6173 7369 6669 6572 3a20  ce..Classifier: 
+00000600: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+00000610: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
+00000620: 2049 6e64 6578 696e 672f 5365 6172 6368   Indexing/Search
+00000630: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
+00000640: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
+00000650: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
+00000660: 2049 6d61 6765 2052 6563 6f67 6e69 7469   Image Recogniti
+00000670: 6f6e 0d0a 436c 6173 7369 6669 6572 3a20  on..Classifier: 
+00000680: 546f 7069 6320 3a3a 204d 756c 7469 6d65  Topic :: Multime
+00000690: 6469 6120 3a3a 2056 6964 656f 0d0a 436c  dia :: Video..Cl
+000006a0: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+000006b0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+000006c0: 6769 6e65 6572 696e 670d 0a43 6c61 7373  gineering..Class
+000006d0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+000006e0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+000006f0: 6565 7269 6e67 203a 3a20 4d61 7468 656d  eering :: Mathem
+00000700: 6174 6963 730d 0a43 6c61 7373 6966 6965  atics..Classifie
+00000710: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+00000720: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000730: 0d0a 436c 6173 7369 6669 6572 3a20 546f  ..Classifier: To
+00000740: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000750: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000760: 6962 7261 7269 6573 0d0a 436c 6173 7369  ibraries..Classi
+00000770: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000780: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000790: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+000007a0: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
+000007b0: 6573 0d0a 4465 7363 7269 7074 696f 6e2d  es..Description-
+000007c0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+000007d0: 7874 2f6d 6172 6b64 6f77 6e0d 0a4c 6963  xt/markdown..Lic
+000007e0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+000007f0: 5345 0d0a 0d0a 3c70 2061 6c69 676e 3d22  SE....<p align="
+00000800: 6365 6e74 6572 223e 0d0a 3c21 2d2d 2073  center">..<!-- s
+00000810: 7572 7665 7920 6261 6e6e 6572 2073 7461  urvey banner sta
+00000820: 7274 202d 2d3e 0d0a 3c61 2068 7265 663d  rt -->..<a href=
+00000830: 2268 7474 7073 3a2f 2f31 3073 7731 7463  "https://10sw1tc
+00000840: 706c 6434 2e74 7970 6566 6f72 6d2e 636f  pld4.typeform.co
+00000850: 6d2f 746f 2f45 4741 4552 654d 373f 7574  m/to/EGAEReM7?ut
+00000860: 6d5f 736f 7572 6365 3d72 6561 646d 6526  m_source=readme&
+00000870: 7574 6d5f 6d65 6469 756d 3d67 6974 6875  utm_medium=githu
+00000880: 6226 7574 6d5f 6361 6d70 6169 676e 3d75  b&utm_campaign=u
+00000890: 7365 7225 3230 6578 7065 7269 656e 6365  ser%20experience
+000008a0: 2675 746d 5f74 6572 6d3d 6665 6232 3032  &utm_term=feb202
+000008b0: 3326 7574 6d5f 636f 6e74 656e 743d 7375  3&utm_content=su
+000008c0: 7276 6579 223e 0d0a 2020 3c69 6d67 2073  rvey">..  <img s
+000008d0: 7263 3d22 2e2f 2e67 6974 6875 622f 6261  rc="./.github/ba
+000008e0: 6e6e 6572 2e73 7667 3f72 6177 3d74 7275  nner.svg?raw=tru
+000008f0: 6522 3e0d 0a3c 2f61 3e0d 0a3c 212d 2d20  e">..</a>..<!-- 
+00000900: 7375 7276 6579 2062 616e 6e65 7220 7374  survey banner st
+00000910: 6172 7420 2d2d 3e0d 0a0d 0a3c 7020 616c  art -->....<p al
+00000920: 6967 6e3d 2263 656e 7465 7222 3e0d 0a3c  ign="center">..<
+00000930: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000940: 646f 6373 2e63 6d6f 6e2e 7077 223e 3c69  docs.cmon.pw"><i
+00000950: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000960: 6769 7468 7562 2e63 6f6d 2f63 6d6f 6e2e  github.com/cmon.
+00000970: 7077 2f63 6d6f 6e2f 626c 6f62 2f6d 6173  pw/cmon/blob/mas
+00000980: 7465 722f 646f 6373 2f5f 7374 6174 6963  ter/docs/_static
+00000990: 2f6c 6f67 6f2d 6c69 6768 742e 7376 673f  /logo-light.svg?
+000009a0: 7261 773d 7472 7565 2220 616c 743d 2243  raw=true" alt="C
+000009b0: 6d6f 6e20 6c6f 676f 3a20 4275 696c 6420  mon logo: Build 
+000009c0: 6d75 6c74 696d 6f64 616c 2041 4920 7365  multimodal AI se
+000009d0: 7276 6963 6573 2076 6961 2063 6c6f 7564  rvices via cloud
+000009e0: 206e 6174 6976 6520 7465 6368 6e6f 6c6f   native technolo
+000009f0: 6769 6573 20c2 b720 4e65 7572 616c 2053  gies .. Neural S
+00000a00: 6561 7263 6820 c2b7 2047 656e 6572 6174  earch .. Generat
+00000a10: 6976 6520 4149 20c2 b720 436c 6f75 6420  ive AI .. Cloud 
+00000a20: 4e61 7469 7665 2220 7769 6474 683d 2231  Native" width="1
+00000a30: 3530 7078 223e 3c2f 613e 0d0a 3c2f 703e  50px"></a>..</p>
+00000a40: 0d0a 0d0a 3c70 2061 6c69 676e 3d22 6365  ....<p align="ce
+00000a50: 6e74 6572 223e 0d0a 3c62 3e42 7569 6c64  nter">..<b>Build
+00000a60: 206d 756c 7469 6d6f 6461 6c20 4149 2073   multimodal AI s
+00000a70: 6572 7669 6365 7320 7769 7468 2063 6c6f  ervices with clo
+00000a80: 7564 206e 6174 6976 6520 7465 6368 6e6f  ud native techno
+00000a90: 6c6f 6769 6573 3c2f 623e 0d0a 3c2f 703e  logies</b>..</p>
+00000aa0: 0d0a 0d0a 3c70 2061 6c69 676e 3d63 656e  ....<p align=cen
+00000ab0: 7465 723e 0d0a 3c61 2068 7265 663d 2268  ter>..<a href="h
+00000ac0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000ad0: 7072 6f6a 6563 742f 636d 6f6e 2f22 3e3c  project/cmon/"><
+00000ae0: 696d 6720 616c 743d 2250 7950 4922 2073  img alt="PyPI" s
+00000af0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000b00: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000b10: 762f 636d 6f6e 3f6c 6162 656c 3d52 656c  v/cmon?label=Rel
+00000b20: 6561 7365 2673 7479 6c65 3d66 6c61 742d  ease&style=flat-
+00000b30: 7371 7561 7265 223e 3c2f 613e 0d0a 3c21  square"></a>..<!
+00000b40: 2d2d 3c61 2068 7265 663d 2268 7474 7073  --<a href="https
+00000b50: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00000b60: 2f63 6d6f 6e2e 7077 2f63 6d6f 6e22 3e3c  /cmon.pw/cmon"><
+00000b70: 696d 6720 616c 743d 2243 6f64 6563 6f76  img alt="Codecov
+00000b80: 2062 7261 6e63 6822 2073 7263 3d22 6874   branch" src="ht
+00000b90: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000ba0: 732e 696f 2f63 6f64 6563 6f76 2f63 2f67  s.io/codecov/c/g
+00000bb0: 6974 6875 622f 636d 6f6e 2e70 772f 636d  ithub/cmon.pw/cm
+00000bc0: 6f6e 2f6d 6173 7465 723f 266c 6f67 6f3d  on/master?&logo=
+00000bd0: 436f 6465 636f 7626 6c6f 676f 436f 6c6f  Codecov&logoColo
+00000be0: 723d 7768 6974 6526 7374 796c 653d 666c  r=white&style=fl
+00000bf0: 6174 2d73 7175 6172 6522 3e3c 2f61 3e2d  at-square"></a>-
+00000c00: 2d3e 0d0a 3c61 2068 7265 663d 2268 7474  ->..<a href="htt
+00000c10: 7073 3a2f 2f64 6973 636f 7264 2e63 6d6f  ps://discord.cmo
+00000c20: 6e2e 7077 223e 3c69 6d67 2073 7263 3d22  n.pw"><img src="
+00000c30: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000c40: 6c64 732e 696f 2f64 6973 636f 7264 2f31  lds.io/discord/1
+00000c50: 3130 3635 3432 3232 3031 3132 3330 3231  1065422201123021
+00000c60: 3330 3f6c 6f67 6f3d 6469 7363 6f72 6426  30?logo=discord&
+00000c70: 6c6f 676f 436f 6c6f 723d 7768 6974 6526  logoColor=white&
+00000c80: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
+00000c90: 6522 3e3c 2f61 3e0d 0a3c 6120 6872 6566  e"></a>..<a href
+00000ca0: 3d22 6874 7470 733a 2f2f 7079 7069 7374  ="https://pypist
+00000cb0: 6174 732e 6f72 672f 7061 636b 6167 6573  ats.org/packages
+00000cc0: 2f63 6d6f 6e22 3e3c 696d 6720 616c 743d  /cmon"><img alt=
+00000cd0: 2250 7950 4920 2d20 446f 776e 6c6f 6164  "PyPI - Download
+00000ce0: 7320 6672 6f6d 206f 6666 6963 6961 6c20  s from official 
+00000cf0: 7079 7069 7374 6174 7322 2073 7263 3d22  pypistats" src="
+00000d00: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000d10: 6c64 732e 696f 2f70 7970 692f 646d 2f63  lds.io/pypi/dm/c
+00000d20: 6d6f 6e3f 7374 796c 653d 666c 6174 2d73  mon?style=flat-s
+00000d30: 7175 6172 6522 3e3c 2f61 3e0d 0a3c 6120  quare"></a>..<a 
+00000d40: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000d50: 7468 7562 2e63 6f6d 2f63 6d6f 6e2e 7077  thub.com/cmon.pw
+00000d60: 2f63 6d6f 6e2f 6163 7469 6f6e 732f 776f  /cmon/actions/wo
+00000d70: 726b 666c 6f77 732f 6364 2e79 6d6c 223e  rkflows/cd.yml">
+00000d80: 3c69 6d67 2061 6c74 3d22 4769 7468 7562  <img alt="Github
+00000d90: 2043 4420 7374 6174 7573 2220 7372 633d   CD status" src=
+00000da0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000db0: 636f 6d2f 636d 6f6e 2e70 772f 636d 6f6e  com/cmon.pw/cmon
+00000dc0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000dd0: 7773 2f63 642e 796d 6c2f 6261 6467 652e  ws/cd.yml/badge.
+00000de0: 7376 6722 3e3c 2f61 3e0d 0a3c 2f70 3e0d  svg"></a>..</p>.
+00000df0: 0a0d 0a3c 212d 2d20 7374 6172 7420 636d  ...<!-- start cm
+00000e00: 6f6e 2d64 6573 6372 6970 7469 6f6e 202d  on-description -
+00000e10: 2d3e 0d0a 0d0a 436d 6f6e 206c 6574 7320  ->....Cmon lets 
+00000e20: 796f 7520 6275 696c 6420 6d75 6c74 696d  you build multim
+00000e30: 6f64 616c 205b 2a2a 4149 2073 6572 7669  odal [**AI servi
+00000e40: 6365 732a 2a5d 2823 6275 696c 642d 6169  ces**](#build-ai
+00000e50: 2d73 6572 7669 6365 7329 2061 6e64 205b  -services) and [
+00000e60: 2a2a 7069 7065 6c69 6e65 732a 2a5d 2823  **pipelines**](#
+00000e70: 6275 696c 642d 612d 7069 7065 6c69 6e65  build-a-pipeline
+00000e80: 2920 7468 6174 2063 6f6d 6d75 6e69 6361  ) that communica
+00000e90: 7465 2076 6961 2067 5250 432c 2048 5454  te via gRPC, HTT
+00000ea0: 5020 616e 6420 5765 6253 6f63 6b65 7473  P and WebSockets
+00000eb0: 2c20 7468 656e 2073 6361 6c65 2074 6865  , then scale the
+00000ec0: 6d20 7570 2061 6e64 2064 6570 6c6f 7920  m up and deploy 
+00000ed0: 746f 2070 726f 6475 6374 696f 6e2e 2059  to production. Y
+00000ee0: 6f75 2063 616e 2066 6f63 7573 206f 6e20  ou can focus on 
+00000ef0: 796f 7572 206c 6f67 6963 2061 6e64 2061  your logic and a
+00000f00: 6c67 6f72 6974 686d 732c 2077 6974 686f  lgorithms, witho
+00000f10: 7574 2077 6f72 7279 696e 6720 6162 6f75  ut worrying abou
+00000f20: 7420 7468 6520 696e 6672 6173 7472 7563  t the infrastruc
+00000f30: 7475 7265 2063 6f6d 706c 6578 6974 792e  ture complexity.
+00000f40: 0d0a 0d0a 215b 5d28 2e2f 2e67 6974 6875  ....![](./.githu
+00000f50: 622f 696d 6167 6573 2f62 7569 6c64 2d64  b/images/build-d
+00000f60: 6570 6c6f 792e 706e 6729 0d0a 0d0a 436d  eploy.png)....Cm
+00000f70: 6f6e 2070 726f 7669 6465 7320 6120 736d  on provides a sm
+00000f80: 6f6f 7468 2050 7974 686f 6e69 6320 6578  ooth Pythonic ex
+00000f90: 7065 7269 656e 6365 2074 7261 6e73 6974  perience transit
+00000fa0: 696f 6e69 6e67 2066 726f 6d20 6c6f 6361  ioning from loca
+00000fb0: 6c20 6465 706c 6f79 6d65 6e74 2074 6f20  l deployment to 
+00000fc0: 6164 7661 6e63 6564 206f 7263 6865 7374  advanced orchest
+00000fd0: 7261 7469 6f6e 2066 7261 6d65 776f 726b  ration framework
+00000fe0: 7320 6c69 6b65 2044 6f63 6b65 722d 436f  s like Docker-Co
+00000ff0: 6d70 6f73 652c 204b 7562 6572 6e65 7465  mpose, Kubernete
+00001000: 732c 206f 7220 436d 6f6e 2041 4920 436c  s, or Cmon AI Cl
+00001010: 6f75 642e 2043 6d6f 6e20 6d61 6b65 7320  oud. Cmon makes 
+00001020: 6164 7661 6e63 6564 2073 6f6c 7574 696f  advanced solutio
+00001030: 6e20 656e 6769 6e65 6572 696e 6720 616e  n engineering an
+00001040: 6420 636c 6f75 642d 6e61 7469 7665 2074  d cloud-native t
+00001050: 6563 686e 6f6c 6f67 6965 7320 6163 6365  echnologies acce
+00001060: 7373 6962 6c65 2074 6f20 6576 6572 7920  ssible to every 
+00001070: 6465 7665 6c6f 7065 722e 0d0a 0d0a 2d20  developer.....- 
+00001080: 4275 696c 6420 6170 706c 6963 6174 696f  Build applicatio
+00001090: 6e73 2066 6f72 2061 6e79 205b 6461 7461  ns for any [data
+000010a0: 2074 7970 655d 2868 7474 7073 3a2f 2f64   type](https://d
+000010b0: 6f63 732e 646f 6361 7272 6179 2e6f 7267  ocs.docarray.org
+000010c0: 2f64 6174 615f 7479 7065 732f 6669 7273  /data_types/firs
+000010d0: 745f 7374 6570 732f 292c 2061 6e79 206d  t_steps/), any m
+000010e0: 6169 6e73 7472 6561 6d20 5b64 6565 7020  ainstream [deep 
+000010f0: 6c65 6172 6e69 6e67 2066 7261 6d65 776f  learning framewo
+00001100: 726b 5d28 292c 2061 6e64 2061 6e79 205b  rk](), and any [
+00001110: 7072 6f74 6f63 6f6c 5d28 6874 7470 733a  protocol](https:
+00001120: 2f2f 646f 6373 2e63 6d6f 6e2e 7077 2f63  //docs.cmon.pw/c
+00001130: 6f6e 6365 7074 732f 7365 7276 696e 672f  oncepts/serving/
+00001140: 6761 7465 7761 792f 2373 6574 2d70 726f  gateway/#set-pro
+00001150: 746f 636f 6c2d 696e 2d70 7974 686f 6e29  tocol-in-python)
+00001160: 2e0d 0a2d 2044 6573 6967 6e20 6869 6768  ...- Design high
+00001170: 2d70 6572 666f 726d 616e 6365 206d 6963  -performance mic
+00001180: 726f 7365 7276 6963 6573 2c20 7769 7468  roservices, with
+00001190: 205b 6561 7379 2073 6361 6c69 6e67 5d28   [easy scaling](
+000011a0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+000011b0: 6e2e 7077 2f63 6f6e 6365 7074 732f 6f72  n.pw/concepts/or
+000011c0: 6368 6573 7472 6174 696f 6e2f 7363 616c  chestration/scal
+000011d0: 652d 6f75 742f 292c 2064 7570 6c65 7820  e-out/), duplex 
+000011e0: 636c 6965 6e74 2d73 6572 7665 7220 7374  client-server st
+000011f0: 7265 616d 696e 672c 2061 6e64 2061 7379  reaming, and asy
+00001200: 6e63 2f6e 6f6e 2d62 6c6f 636b 696e 6720  nc/non-blocking 
+00001210: 6461 7461 2070 726f 6365 7373 696e 6720  data processing 
+00001220: 6f76 6572 2064 796e 616d 6963 2066 6c6f  over dynamic flo
+00001230: 7773 2e0d 0a2d 2044 6f63 6b65 7220 636f  ws...- Docker co
+00001240: 6e74 6169 6e65 7220 696e 7465 6772 6174  ntainer integrat
+00001250: 696f 6e20 7669 6120 5b45 7865 6375 746f  ion via [Executo
+00001260: 7220 4875 625d 2868 7474 7073 3a2f 2f63  r Hub](https://c
+00001270: 6c6f 7564 2e63 6d6f 6e2e 7077 292c 204f  loud.cmon.pw), O
+00001280: 7065 6e54 656c 656d 6574 7279 2f50 726f  penTelemetry/Pro
+00001290: 6d65 7468 6575 7320 6f62 7365 7276 6162  metheus observab
+000012a0: 696c 6974 792c 2061 6e64 2066 6173 7420  ility, and fast 
+000012b0: 4b75 6265 726e 6574 6573 2f44 6f63 6b65  Kubernetes/Docke
+000012c0: 722d 436f 6d70 6f73 6520 6465 706c 6f79  r-Compose deploy
+000012d0: 6d65 6e74 2e0d 0a2d 2043 5055 2f47 5055  ment...- CPU/GPU
+000012e0: 2068 6f73 7469 6e67 2076 6961 205b 436d   hosting via [Cm
+000012f0: 6f6e 2041 4920 436c 6f75 645d 2868 7474  on AI Cloud](htt
+00001300: 7073 3a2f 2f63 6c6f 7564 2e63 6d6f 6e2e  ps://cloud.cmon.
+00001310: 7077 292e 0d0a 0d0a 3c64 6574 6169 6c73  pw).....<details
+00001320: 3e0d 0a20 2020 203c 7375 6d6d 6172 793e  >..    <summary>
+00001330: 3c73 7472 6f6e 673e 5761 6974 2c20 686f  <strong>Wait, ho
+00001340: 7720 6973 2043 6d6f 6e20 6469 6666 6572  w is Cmon differ
+00001350: 656e 7420 6672 6f6d 2046 6173 7441 5049  ent from FastAPI
+00001360: 3f3c 2f73 7472 6f6e 673e 3c2f 7375 6d6d  ?</strong></summ
+00001370: 6172 793e 0d0a 436d 6f6e 2773 2076 616c  ary>..Cmon's val
+00001380: 7565 2070 726f 706f 7369 7469 6f6e 206d  ue proposition m
+00001390: 6179 2073 6565 6d20 7175 6974 6520 7369  ay seem quite si
+000013a0: 6d69 6c61 7220 746f 2074 6861 7420 6f66  milar to that of
+000013b0: 2046 6173 7441 5049 2e20 486f 7765 7665   FastAPI. Howeve
+000013c0: 722c 2074 6865 7265 2061 7265 2073 6576  r, there are sev
+000013d0: 6572 616c 2066 756e 6461 6d65 6e74 616c  eral fundamental
+000013e0: 2064 6966 6665 7265 6e63 6573 3a0d 0a0d   differences:...
+000013f0: 0a20 2a2a 4461 7461 2073 7472 7563 7475  . **Data structu
+00001400: 7265 2061 6e64 2063 6f6d 6d75 6e69 6361  re and communica
+00001410: 7469 6f6e 2070 726f 746f 636f 6c73 2a2a  tion protocols**
+00001420: 0d0a 2020 2d20 4661 7374 4150 4920 636f  ..  - FastAPI co
+00001430: 6d6d 756e 6963 6174 696f 6e20 7265 6c69  mmunication reli
+00001440: 6573 206f 6e20 5079 6461 6e74 6963 2061  es on Pydantic a
+00001450: 6e64 2043 6d6f 6e20 7265 6c69 6573 206f  nd Cmon relies o
+00001460: 6e20 5b64 6f63 6172 7261 795d 2868 7474  n [docarray](htt
+00001470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001480: 646f 6361 7272 6179 2f64 6f63 6172 7261  docarray/docarra
+00001490: 7929 2061 6c6c 6f77 696e 6720 436d 6f6e  y) allowing Cmon
+000014a0: 2074 6f20 7375 7070 6f72 7420 6d75 6c74   to support mult
+000014b0: 6970 6c65 2070 726f 746f 636f 6c73 0d0a  iple protocols..
+000014c0: 2020 746f 2065 7870 6f73 6520 6974 7320    to expose its 
+000014d0: 7365 7276 6963 6573 2e0d 0a0d 0a20 2a2a  services..... **
+000014e0: 4164 7661 6e63 6564 206f 7263 6865 7374  Advanced orchest
+000014f0: 7261 7469 6f6e 2061 6e64 2073 6361 6c69  ration and scali
+00001500: 6e67 2063 6170 6162 696c 6974 6965 732a  ng capabilities*
+00001510: 2a0d 0a20 202d 2043 6d6f 6e20 6c65 7473  *..  - Cmon lets
+00001520: 2079 6f75 2064 6570 6c6f 7920 6170 706c   you deploy appl
+00001530: 6963 6174 696f 6e73 2066 6f72 6d65 6420  ications formed 
+00001540: 6672 6f6d 206d 756c 7469 706c 6520 6d69  from multiple mi
+00001550: 6372 6f73 6572 7669 6365 7320 7468 6174  croservices that
+00001560: 2063 616e 2062 6520 636f 6e74 6169 6e65   can be containe
+00001570: 7269 7a65 6420 616e 6420 7363 616c 6564  rized and scaled
+00001580: 2069 6e64 6570 656e 6465 6e74 6c79 2e0d   independently..
+00001590: 0a20 202d 2043 6d6f 6e20 616c 6c6f 7773  .  - Cmon allows
+000015a0: 2079 6f75 2074 6f20 6561 7369 6c79 2063   you to easily c
+000015b0: 6f6e 7461 696e 6572 697a 6520 616e 6420  ontainerize and 
+000015c0: 6f72 6368 6573 7472 6174 6520 796f 7572  orchestrate your
+000015d0: 2073 6572 7669 6365 732c 2070 726f 7669   services, provi
+000015e0: 6469 6e67 2063 6f6e 6375 7272 656e 6379  ding concurrency
+000015f0: 2061 6e64 2073 6361 6c61 6269 6c69 7479   and scalability
+00001600: 2e0d 0a0d 0a20 2a2a 4a6f 7572 6e65 7920  ..... **Journey 
+00001610: 746f 2074 6865 2063 6c6f 7564 2a2a 0d0a  to the cloud**..
+00001620: 2020 2d20 436d 6f6e 2070 726f 7669 6465    - Cmon provide
+00001630: 7320 6120 736d 6f6f 7468 2074 7261 6e73  s a smooth trans
+00001640: 6974 696f 6e20 6672 6f6d 206c 6f63 616c  ition from local
+00001650: 2064 6576 656c 6f70 6d65 6e74 2028 7573   development (us
+00001660: 696e 6720 5b64 6f63 6172 7261 795d 2868  ing [docarray](h
+00001670: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001680: 6d2f 646f 6361 7272 6179 2f64 6f63 6172  m/docarray/docar
+00001690: 7261 7929 2920 746f 206c 6f63 616c 2073  ray)) to local s
+000016a0: 6572 7669 6e67 2075 7369 6e67 2028 436d  erving using (Cm
+000016b0: 6f6e 2773 206f 7263 6865 7374 7261 7469  on's orchestrati
+000016c0: 6f6e 206c 6179 6572 290d 0a20 2074 6f20  on layer)..  to 
+000016d0: 6861 7669 6e67 2070 726f 6475 6374 696f  having productio
+000016e0: 6e2d 7265 6164 7920 7365 7276 6963 6573  n-ready services
+000016f0: 2062 7920 7573 696e 6720 4b75 6265 726e   by using Kubern
+00001700: 6574 6573 2063 6170 6163 6974 7920 746f  etes capacity to
+00001710: 206f 7263 6865 7374 7261 7465 2074 6865   orchestrate the
+00001720: 206c 6966 6574 696d 6520 6f66 2063 6f6e   lifetime of con
+00001730: 7461 696e 6572 732e 0d0a 2020 2d20 4279  tainers...  - By
+00001740: 2075 7369 6e67 205b 436d 6f6e 2041 4920   using [Cmon AI 
+00001750: 436c 6f75 645d 2868 7474 7073 3a2f 2f63  Cloud](https://c
+00001760: 6c6f 7564 2e63 6d6f 6e2e 7077 2920 796f  loud.cmon.pw) yo
+00001770: 7520 6861 7665 2061 6363 6573 7320 746f  u have access to
+00001780: 2073 6361 6c61 626c 6520 616e 6420 7365   scalable and se
+00001790: 7276 6572 6c65 7373 2064 6570 6c6f 796d  rverless deploym
+000017a0: 656e 7473 206f 6620 796f 7572 2061 7070  ents of your app
+000017b0: 6c69 6361 7469 6f6e 7320 696e 206f 6e65  lications in one
+000017c0: 2063 6f6d 6d61 6e64 2e0d 0a3c 2f64 6574   command...</det
+000017d0: 6169 6c73 3e0d 0a0d 0a3c 212d 2d20 656e  ails>....<!-- en
+000017e0: 6420 636d 6f6e 2d64 6573 6372 6970 7469  d cmon-descripti
+000017f0: 6f6e 202d 2d3e 0d0a 0d0a 2323 205b 446f  on -->....## [Do
+00001800: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00001810: 7073 3a2f 2f64 6f63 732e 636d 6f6e 2e70  ps://docs.cmon.p
+00001820: 7729 0d0a 0d0a 2323 2049 6e73 7461 6c6c  w)....## Install
+00001830: 200d 0a0d 0a4e 6f74 653a 2028 5769 6e64   ....Note: (Wind
+00001840: 6f77 7329 206e 6f74 2073 7570 706f 7274  ows) not support
+00001850: 6564 2061 7420 7468 6973 206d 6f6d 656e  ed at this momen
+00001860: 7421 2059 6f75 206d 6179 2072 6571 7569  t! You may requi
+00001870: 7265 2074 6f20 696e 7374 616c 6c20 6974  re to install it
+00001880: 206f 6e20 2857 534c 292e 0d0a 5b20 2055   on (WSL)...[  U
+00001890: 5044 4154 4520 205d 203a 2057 696e 646f  PDATE  ] : Windo
+000018a0: 7773 2053 7570 706f 7274 2061 6464 6564  ws Support added
+000018b0: 210d 0a0d 0a60 6060 6261 7368 0d0a 7069  !....```bash..pi
+000018c0: 7020 696e 7374 616c 6c20 636d 6f6e 2d61  p install cmon-a
+000018d0: 690d 0a60 6060 0d0a 0d0a 4669 6e64 206d  i..```....Find m
+000018e0: 6f72 6520 696e 7374 616c 6c20 6f70 7469  ore install opti
+000018f0: 6f6e 7320 6f6e 205b 4170 706c 6520 5369  ons on [Apple Si
+00001900: 6c69 636f 6e5d 2868 7474 7073 3a2f 2f64  licon](https://d
+00001910: 6f63 732e 636d 6f6e 2e70 772f 6765 742d  ocs.cmon.pw/get-
+00001920: 7374 6172 7465 642f 696e 7374 616c 6c2f  started/install/
+00001930: 6170 706c 652d 7369 6c69 636f 6e2d 6d31  apple-silicon-m1
+00001940: 2d6d 322f 290d 0a0d 0a0d 0a23 2320 4765  -m2/)......## Ge
+00001950: 7420 5374 6172 7465 640d 0a0d 0a23 2323  t Started....###
+00001960: 2042 6173 6963 2043 6f6e 6365 7074 730d   Basic Concepts.
+00001970: 0a0d 0a43 6d6f 6e20 6861 7320 666f 7572  ...Cmon has four
+00001980: 2066 756e 6461 6d65 6e74 616c 2063 6f6e   fundamental con
+00001990: 6365 7074 733a 0d0a 0d0a 2d20 4120 5b2a  cepts:....- A [*
+000019a0: 2a44 6f63 756d 656e 742a 2a5d 2868 7474  *Document**](htt
+000019b0: 7073 3a2f 2f64 6f63 6172 7261 792e 636d  ps://docarray.cm
+000019c0: 6f6e 2e70 772f 2920 2866 726f 6d20 5b64  on.pw/) (from [d
+000019d0: 6f63 6172 7261 795d 2868 7474 7073 3a2f  ocarray](https:/
+000019e0: 2f67 6974 6875 622e 636f 6d2f 646f 6361  /github.com/doca
+000019f0: 7272 6179 2f64 6f63 6172 7261 7929 2920  rray/docarray)) 
+00001a00: 6973 2074 6865 2069 6e70 7574 2f6f 7574  is the input/out
+00001a10: 7075 7420 666f 726d 6174 2069 6e20 436d  put format in Cm
+00001a20: 6f6e 2e0d 0a2d 2041 6e20 5b2a 2a45 7865  on...- An [**Exe
+00001a30: 6375 746f 722a 2a5d 2868 7474 7073 3a2f  cutor**](https:/
+00001a40: 2f64 6f63 732e 636d 6f6e 2e70 772f 636f  /docs.cmon.pw/co
+00001a50: 6e63 6570 7473 2f73 6572 7669 6e67 2f65  ncepts/serving/e
+00001a60: 7865 6375 746f 722f 2920 6973 2061 2050  xecutor/) is a P
+00001a70: 7974 686f 6e20 636c 6173 7320 7468 6174  ython class that
+00001a80: 2074 7261 6e73 666f 726d 7320 616e 6420   transforms and 
+00001a90: 7072 6f63 6573 7365 7320 446f 6375 6d65  processes Docume
+00001aa0: 6e74 732e 0d0a 2d20 4120 5b2a 2a44 6570  nts...- A [**Dep
+00001ab0: 6c6f 796d 656e 742a 2a5d 2868 7474 7073  loyment**](https
+00001ac0: 3a2f 2f64 6f63 732e 636d 6f6e 2e70 772f  ://docs.cmon.pw/
+00001ad0: 636f 6e63 6570 7473 2f6f 7263 6865 7374  concepts/orchest
+00001ae0: 7261 7469 6f6e 2f64 6570 6c6f 796d 656e  ration/deploymen
+00001af0: 7429 2073 6572 7665 7320 6120 7369 6e67  t) serves a sing
+00001b00: 6c65 2045 7865 6375 746f 722c 2077 6869  le Executor, whi
+00001b10: 6c65 2061 205b 2a2a 466c 6f77 2a2a 5d28  le a [**Flow**](
+00001b20: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00001b30: 6e2e 7077 2f63 6f6e 6365 7074 732f 6f72  n.pw/concepts/or
+00001b40: 6368 6573 7472 6174 696f 6e2f 666c 6f77  chestration/flow
+00001b50: 2f29 2073 6572 7665 7320 4578 6563 7574  /) serves Execut
+00001b60: 6f72 7320 6368 6169 6e65 6420 696e 746f  ors chained into
+00001b70: 2061 2070 6970 656c 696e 652e 0d0a 0d0a   a pipeline.....
+00001b80: 0d0a 5b54 6865 2066 756c 6c20 676c 6f73  ..[The full glos
+00001b90: 7361 7279 2069 7320 6578 706c 6169 6e65  sary is explaine
+00001ba0: 6420 6865 7265 5d28 6874 7470 733a 2f2f  d here](https://
+00001bb0: 646f 6373 2e63 6d6f 6e2e 7077 2f63 6f6e  docs.cmon.pw/con
+00001bc0: 6365 7074 732f 7072 656c 696d 696e 6172  cepts/preliminar
+00001bd0: 6965 732f 2329 2e0d 0a0d 0a23 2323 2042  ies/#).....### B
+00001be0: 7569 6c64 2041 4920 5365 7276 6963 6573  uild AI Services
+00001bf0: 0d0a 3c21 2d2d 2073 7461 7274 2062 7569  ..<!-- start bui
+00001c00: 6c64 2d61 692d 7365 7276 6963 6573 202d  ld-ai-services -
+00001c10: 2d3e 0d0a 0d0a 4c65 7427 7320 6275 696c  ->....Let's buil
+00001c20: 6420 6120 6661 7374 2c20 7265 6c69 6162  d a fast, reliab
+00001c30: 6c65 2061 6e64 2073 6361 6c61 626c 6520  le and scalable 
+00001c40: 6752 5043 2d62 6173 6564 2041 4920 7365  gRPC-based AI se
+00001c50: 7276 6963 652e 2049 6e20 436d 6f6e 2077  rvice. In Cmon w
+00001c60: 6520 6361 6c6c 2074 6869 7320 616e 202a  e call this an *
+00001c70: 2a5b 4578 6563 7574 6f72 5d28 6874 7470  *[Executor](http
+00001c80: 733a 2f2f 646f 6373 2e63 6d6f 6e2e 7077  s://docs.cmon.pw
+00001c90: 2f63 6f6e 6365 7074 732f 6578 6563 7574  /concepts/execut
+00001ca0: 6f72 2f29 2a2a 2e20 4f75 7220 7369 6d70  or/)**. Our simp
+00001cb0: 6c65 2045 7865 6375 746f 7220 7769 6c6c  le Executor will
+00001cc0: 2077 7261 7020 7468 6520 5b53 7461 626c   wrap the [Stabl
+00001cd0: 654c 4d5d 2868 7474 7073 3a2f 2f68 7567  eLM](https://hug
+00001ce0: 6769 6e67 6661 6365 2e63 6f2f 7374 6162  gingface.co/stab
+00001cf0: 696c 6974 7961 692f 7374 6162 6c65 6c6d  ilityai/stablelm
+00001d00: 2d62 6173 652d 616c 7068 612d 3362 2920  -base-alpha-3b) 
+00001d10: 4c4c 4d20 6672 6f6d 2053 7461 6269 6c69  LLM from Stabili
+00001d20: 7479 2041 492e 2057 6527 6c6c 2074 6865  ty AI. We'll the
+00001d30: 6e20 7573 6520 6120 2a2a 4465 706c 6f79  n use a **Deploy
+00001d40: 6d65 6e74 2a2a 2074 6f20 7365 7276 6520  ment** to serve 
+00001d50: 6974 2e0d 0a0d 0a21 5b5d 282e 2f2e 6769  it.....![](./.gi
+00001d60: 7468 7562 2f69 6d61 6765 732f 6465 706c  thub/images/depl
+00001d70: 6f79 6d65 6e74 2d64 6961 6772 616d 2e70  oyment-diagram.p
+00001d80: 6e67 290d 0a0d 0a3e 202a 2a4e 6f74 652a  ng)....> **Note*
+00001d90: 2a0d 0a3e 2041 2044 6570 6c6f 796d 656e  *..> A Deploymen
+00001da0: 7420 7365 7276 6573 206a 7573 7420 6f6e  t serves just on
+00001db0: 6520 4578 6563 7574 6f72 2e20 546f 2063  e Executor. To c
+00001dc0: 6f6d 6269 6e65 206d 756c 7469 706c 6520  ombine multiple 
+00001dd0: 4578 6563 7574 6f72 7320 696e 746f 2061  Executors into a
+00001de0: 2070 6970 656c 696e 6520 616e 6420 7365   pipeline and se
+00001df0: 7276 6520 7468 6174 2c20 7573 6520 6120  rve that, use a 
+00001e00: 5b46 6c6f 775d 2823 6275 696c 642d 612d  [Flow](#build-a-
+00001e10: 7069 7065 6c69 6e65 292e 0d0a 0d0a 4c65  pipeline).....Le
+00001e20: 7427 7320 696d 706c 656d 656e 7420 7468  t's implement th
+00001e30: 6520 7365 7276 6963 6527 7320 6c6f 6769  e service's logi
+00001e40: 633a 0d0a 0d0a 3c74 6162 6c65 3e0d 0a3c  c:....<table>..<
+00001e50: 7472 3e0d 0a3c 7468 3e3c 636f 6465 3e65  tr>..<th><code>e
+00001e60: 7865 6375 746f 722e 7079 3c2f 636f 6465  xecutor.py</code
+00001e70: 3e3c 2f74 683e 200d 0a3c 7472 3e0d 0a3c  ></th> ..<tr>..<
+00001e80: 7464 3e0d 0a0d 0a60 6060 7079 7468 6f6e  td>....```python
+00001e90: 0d0a 6672 6f6d 2063 6d6f 6e20 696d 706f  ..from cmon impo
+00001ea0: 7274 2045 7865 6375 746f 722c 2072 6571  rt Executor, req
+00001eb0: 7565 7374 730d 0a66 726f 6d20 646f 6361  uests..from doca
+00001ec0: 7272 6179 2069 6d70 6f72 7420 446f 6375  rray import Docu
+00001ed0: 6d65 6e74 4172 7261 790d 0a0d 0a66 726f  mentArray....fro
+00001ee0: 6d20 7472 616e 7366 6f72 6d65 7273 2069  m transformers i
+00001ef0: 6d70 6f72 7420 7069 7065 6c69 6e65 0d0a  mport pipeline..
+00001f00: 0d0a 0d0a 636c 6173 7320 5374 6162 6c65  ....class Stable
+00001f10: 4c4d 2845 7865 6375 746f 7229 3a0d 0a0d  LM(Executor):...
+00001f20: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001f30: 5f28 7365 6c66 2c20 2a2a 6b77 6172 6773  _(self, **kwargs
+00001f40: 293a 0d0a 2020 2020 2020 2020 7375 7065  ):..        supe
+00001f50: 7228 292e 5f5f 696e 6974 5f5f 282a 2a6b  r().__init__(**k
+00001f60: 7761 7267 7329 0d0a 2020 2020 2020 2020  wargs)..        
+00001f70: 7365 6c66 2e67 656e 6572 6174 6f72 203d  self.generator =
+00001f80: 2070 6970 656c 696e 6528 2774 6578 742d   pipeline('text-
+00001f90: 6765 6e65 7261 7469 6f6e 272c 206d 6f64  generation', mod
+00001fa0: 656c 3d27 7374 6162 6c65 6c6d 2d33 6227  el='stablelm-3b'
+00001fb0: 290d 0a0d 0a20 2020 2040 7265 7175 6573  )....    @reques
+00001fc0: 7473 0d0a 2020 2020 6465 6620 6765 6e65  ts..    def gene
+00001fd0: 7261 7465 2873 656c 662c 2064 6f63 733a  rate(self, docs:
+00001fe0: 2044 6f63 756d 656e 7441 7272 6179 2c20   DocumentArray, 
+00001ff0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+00002000: 2020 2020 6765 6e65 7261 7465 645f 7465      generated_te
+00002010: 7874 203d 2073 656c 662e 6765 6e65 7261  xt = self.genera
+00002020: 746f 7228 646f 6373 2e74 6578 7473 290d  tor(docs.texts).
+00002030: 0a20 2020 2020 2020 2064 6f63 732e 7465  .        docs.te
+00002040: 7874 7320 3d20 5b67 656e 5b30 5d5b 2767  xts = [gen[0]['g
+00002050: 656e 6572 6174 6564 5f74 6578 7427 5d20  enerated_text'] 
+00002060: 666f 7220 6765 6e20 696e 2067 656e 6572  for gen in gener
+00002070: 6174 6564 5f74 6578 745d 0d0a 6060 600d  ated_text]..```.
+00002080: 0a0d 0a3c 2f74 643e 0d0a 3c2f 7472 3e0d  ...</td>..</tr>.
+00002090: 0a3c 2f74 6162 6c65 3e0d 0a0d 0a54 6865  .</table>....The
+000020a0: 6e20 7765 2064 6570 6c6f 7920 6974 2077  n we deploy it w
+000020b0: 6974 6820 6569 7468 6572 2074 6865 2050  ith either the P
+000020c0: 7974 686f 6e20 4150 4920 6f72 2059 414d  ython API or YAM
+000020d0: 4c3a 0d0a 3c64 6976 2063 6c61 7373 3d22  L:..<div class="
+000020e0: 7461 626c 652d 7772 6170 7065 7222 3e0d  table-wrapper">.
+000020f0: 0a3c 7461 626c 653e 0d0a 3c74 723e 0d0a  .<table>..<tr>..
+00002100: 3c74 683e 2050 7974 686f 6e20 4150 493a  <th> Python API:
+00002110: 203c 636f 6465 3e64 6570 6c6f 796d 656e   <code>deploymen
+00002120: 742e 7079 3c2f 636f 6465 3e20 3c2f 7468  t.py</code> </th
+00002130: 3e20 0d0a 3c74 683e 2059 414d 4c3a 203c  > ..<th> YAML: <
+00002140: 636f 6465 3e64 6570 6c6f 796d 656e 742e  code>deployment.
+00002150: 796d 6c3c 2f63 6f64 653e 203c 2f74 683e  yml</code> </th>
+00002160: 0d0a 3c2f 7472 3e0d 0a3c 7472 3e0d 0a3c  ..</tr>..<tr>..<
+00002170: 7464 3e0d 0a0d 0a60 6060 7079 7468 6f6e  td>....```python
+00002180: 0d0a 6672 6f6d 2063 6d6f 6e20 696d 706f  ..from cmon impo
+00002190: 7274 2044 6570 6c6f 796d 656e 740d 0a66  rt Deployment..f
+000021a0: 726f 6d20 6578 6563 7574 6f72 2069 6d70  rom executor imp
+000021b0: 6f72 7420 5374 6162 6c65 4c4d 0d0a 0d0a  ort StableLM....
+000021c0: 6465 7020 3d20 4465 706c 6f79 6d65 6e74  dep = Deployment
+000021d0: 2875 7365 733d 5374 6162 6c65 4c4d 2c20  (uses=StableLM, 
+000021e0: 7469 6d65 6f75 745f 7265 6164 793d 2d31  timeout_ready=-1
+000021f0: 2c20 706f 7274 3d31 3233 3435 290d 0a0d  , port=12345)...
+00002200: 0a77 6974 6820 6465 703a 0d0a 2020 2020  .with dep:..    
+00002210: 6465 702e 626c 6f63 6b28 290d 0a60 6060  dep.block()..```
+00002220: 0d0a 0d0a 3c2f 7464 3e0d 0a3c 7464 3e0d  ....</td>..<td>.
+00002230: 0a0d 0a60 6060 7961 6d6c 0d0a 6a74 7970  ...```yaml..jtyp
+00002240: 653a 2044 6570 6c6f 796d 656e 740d 0a77  e: Deployment..w
+00002250: 6974 683a 0d0a 2020 7573 6573 3a20 5374  ith:..  uses: St
+00002260: 6162 6c65 4c4d 0d0a 2020 7079 5f6d 6f64  ableLM..  py_mod
+00002270: 756c 6573 3a0d 0a20 2020 202d 2065 7865  ules:..    - exe
+00002280: 6375 746f 722e 7079 0d0a 2020 7469 6d65  cutor.py..  time
+00002290: 6f75 745f 7265 6164 793a 202d 310d 0a20  out_ready: -1.. 
+000022a0: 2070 6f72 743a 2031 3233 3435 0d0a 6060   port: 12345..``
+000022b0: 600d 0a0d 0a41 6e64 2072 756e 2074 6865  `....And run the
+000022c0: 2059 414d 4c20 4465 706c 6f79 6d65 6e74   YAML Deployment
+000022d0: 2077 6974 6820 7468 6520 434c 493a 2060   with the CLI: `
+000022e0: 636d 6f6e 2064 6570 6c6f 796d 656e 7420  cmon deployment 
+000022f0: 2d2d 7573 6573 2064 6570 6c6f 796d 656e  --uses deploymen
+00002300: 742e 796d 6c60 0d0a 0d0a 3c2f 7464 3e0d  t.yml`....</td>.
+00002310: 0a3c 2f74 723e 0d0a 3c2f 7461 626c 653e  .</tr>..</table>
+00002320: 0d0a 3c2f 6469 763e 0d0a 0d0a 5573 6520  ..</div>....Use 
+00002330: 5b43 6d6f 6e20 436c 6965 6e74 5d28 6874  [Cmon Client](ht
+00002340: 7470 733a 2f2f 646f 6373 2e63 6d6f 6e2e  tps://docs.cmon.
+00002350: 7077 2f63 6f6e 6365 7074 732f 636c 6965  pw/concepts/clie
+00002360: 6e74 2f29 2074 6f20 6d61 6b65 2072 6571  nt/) to make req
+00002370: 7565 7374 7320 746f 2074 6865 2073 6572  uests to the ser
+00002380: 7669 6365 3a0d 0a0d 0a60 6060 7079 7468  vice:....```pyth
+00002390: 6f6e 0d0a 6672 6f6d 2064 6f63 6172 7261  on..from docarra
+000023a0: 7920 696d 706f 7274 2044 6f63 756d 656e  y import Documen
+000023b0: 740d 0a66 726f 6d20 636d 6f6e 2069 6d70  t..from cmon imp
+000023c0: 6f72 7420 436c 6965 6e74 0d0a 0d0a 7072  ort Client....pr
+000023d0: 6f6d 7074 203d 2044 6f63 756d 656e 7428  ompt = Document(
+000023e0: 0d0a 2020 2020 7461 6773 203d 207b 2770  ..    tags = {'p
+000023f0: 726f 6d70 7427 3a20 2773 7567 6765 7374  rompt': 'suggest
+00002400: 2061 6e20 696e 7465 7265 7374 696e 6720   an interesting 
+00002410: 696d 6167 6520 6765 6e65 7261 7469 6f6e  image generation
+00002420: 2070 726f 6d70 7420 666f 7220 6120 6d6f   prompt for a mo
+00002430: 6e61 206c 6973 6120 7661 7269 616e 7427  na lisa variant'
+00002440: 7d0d 0a29 0d0a 0d0a 636c 6965 6e74 203d  }..)....client =
+00002450: 2043 6c69 656e 7428 706f 7274 3d31 3233   Client(port=123
+00002460: 3435 2920 2023 2075 7365 2070 6f72 7420  45)  # use port 
+00002470: 6672 6f6d 206f 7574 7075 7420 6162 6f76  from output abov
+00002480: 650d 0a72 6573 706f 6e73 6520 3d20 636c  e..response = cl
+00002490: 6965 6e74 2e70 6f73 7428 6f6e 3d27 2f27  ient.post(on='/'
+000024a0: 2c20 696e 7075 7473 3d5b 7072 6f6d 7074  , inputs=[prompt
+000024b0: 5d29 0d0a 0d0a 7072 696e 7428 7265 7370  ])....print(resp
+000024c0: 6f6e 7365 5b30 5d2e 7465 7874 290d 0a60  onse[0].text)..`
+000024d0: 6060 0d0a 0d0a 6060 6074 6578 740d 0a61  ``....```text..a
+000024e0: 2073 7465 616d 7075 6e6b 2076 6572 7369   steampunk versi
+000024f0: 6f6e 206f 6620 7468 6520 4d6f 6e61 204c  on of the Mona L
+00002500: 6973 612c 2069 6e63 6f72 706f 7261 7469  isa, incorporati
+00002510: 6e67 206d 6563 6861 6e69 6361 6c20 6765  ng mechanical ge
+00002520: 6172 732c 2062 7261 7373 2065 6c65 6d65  ars, brass eleme
+00002530: 6e74 732c 2061 6e64 2056 6963 746f 7269  nts, and Victori
+00002540: 616e 2065 7261 2063 6c6f 7468 696e 6720  an era clothing 
+00002550: 6465 7461 696c 730d 0a60 6060 0d0a 0d0a  details..```....
+00002560: 3c21 2d2d 2065 6e64 2062 7569 6c64 2d61  <!-- end build-a
+00002570: 692d 7365 7276 6963 6573 202d 2d3e 0d0a  i-services -->..
+00002580: 0d0a 3e20 2a2a 4e6f 7465 2a2a 0d0a 3e20  ..> **Note**..> 
+00002590: 496e 2061 206e 6f74 6562 6f6f 6b2c 2079  In a notebook, y
+000025a0: 6f75 2063 616e 2774 2075 7365 2060 6465  ou can't use `de
+000025b0: 706c 6f79 6d65 6e74 2e62 6c6f 636b 2829  ployment.block()
+000025c0: 6020 616e 6420 7468 656e 206d 616b 6520  ` and then make 
+000025d0: 7265 7175 6573 7473 2074 6f20 7468 6520  requests to the 
+000025e0: 636c 6965 6e74 2e20 506c 6561 7365 2072  client. Please r
+000025f0: 6566 6572 2074 6f20 7468 6520 436f 6c61  efer to the Cola
+00002600: 6220 6c69 6e6b 2061 626f 7665 2066 6f72  b link above for
+00002610: 2072 6570 726f 6475 6369 626c 6520 4a75   reproducible Ju
+00002620: 7079 7465 7220 4e6f 7465 626f 6f6b 2063  pyter Notebook c
+00002630: 6f64 6520 736e 6970 7065 7473 2e0d 0a0d  ode snippets....
+00002640: 0a23 2323 2042 7569 6c64 2061 2070 6970  .### Build a pip
+00002650: 656c 696e 650d 0a0d 0a3c 212d 2d20 7374  eline....<!-- st
+00002660: 6172 7420 6275 696c 642d 7069 7065 6c69  art build-pipeli
+00002670: 6e65 7320 2d2d 3e0d 0a0d 0a53 6f6d 6574  nes -->....Somet
+00002680: 696d 6573 2079 6f75 2077 616e 7420 746f  imes you want to
+00002690: 2063 6861 696e 206d 6963 726f 7365 7276   chain microserv
+000026a0: 6963 6573 2074 6f67 6574 6865 7220 696e  ices together in
+000026b0: 746f 2061 2070 6970 656c 696e 652e 2054  to a pipeline. T
+000026c0: 6861 7427 7320 7768 6572 6520 6120 5b46  hat's where a [F
+000026d0: 6c6f 775d 2868 7474 7073 3a2f 2f64 6f63  low](https://doc
+000026e0: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+000026f0: 7473 2f66 6c6f 772f 2920 636f 6d65 7320  ts/flow/) comes 
+00002700: 696e 2e0d 0a0d 0a41 2046 6c6f 7720 6973  in.....A Flow is
+00002710: 2061 205b 4441 475d 2868 7474 7073 3a2f   a [DAG](https:/
+00002720: 2f64 652e 7769 6b69 7065 6469 612e 6f72  /de.wikipedia.or
+00002730: 672f 7769 6b69 2f44 4147 2920 7069 7065  g/wiki/DAG) pipe
+00002740: 6c69 6e65 2c20 636f 6d70 6f73 6564 206f  line, composed o
+00002750: 6620 6120 7365 7420 6f66 2073 7465 7073  f a set of steps
+00002760: 2c20 4974 206f 7263 6865 7374 7261 7465  , It orchestrate
+00002770: 7320 6120 7365 7420 6f66 205b 4578 6563  s a set of [Exec
+00002780: 7574 6f72 735d 2868 7474 7073 3a2f 2f64  utors](https://d
+00002790: 6f63 732e 636d 6f6e 2e70 772f 636f 6e63  ocs.cmon.pw/conc
+000027a0: 6570 7473 2f65 7865 6375 746f 722f 2920  epts/executor/) 
+000027b0: 616e 6420 6120 5b47 6174 6577 6179 5d28  and a [Gateway](
+000027c0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+000027d0: 6e2e 7077 2f63 6f6e 6365 7074 732f 6761  n.pw/concepts/ga
+000027e0: 7465 7761 792f 2920 746f 206f 6666 6572  teway/) to offer
+000027f0: 2061 6e20 656e 642d 746f 2d65 6e64 2073   an end-to-end s
+00002800: 6572 7669 6365 2e0d 0a0d 0a3e 202a 2a4e  ervice.....> **N
+00002810: 6f74 652a 2a0d 0a3e 2049 6620 796f 7520  ote**..> If you 
+00002820: 6a75 7374 2077 616e 7420 746f 2073 6572  just want to ser
+00002830: 7665 2061 2073 696e 676c 6520 4578 6563  ve a single Exec
+00002840: 7574 6f72 2c20 796f 7520 6361 6e20 7573  utor, you can us
+00002850: 6520 6120 5b44 6570 6c6f 796d 656e 745d  e a [Deployment]
+00002860: 2823 6275 696c 642d 6169 2d2d 6d6c 2d73  (#build-ai--ml-s
+00002870: 6572 7669 6365 7329 2e0d 0a0d 0a46 6f72  ervices).....For
+00002880: 2069 6e73 7461 6e63 652c 206c 6574 2773   instance, let's
+00002890: 2063 6f6d 6269 6e65 205b 6f75 7220 5374   combine [our St
+000028a0: 6162 6c65 4c4d 206c 616e 6775 6167 6520  ableLM language 
+000028b0: 6d6f 6465 6c5d 2823 6275 696c 642d 6169  model](#build-ai
+000028c0: 2d2d 6d6c 2d73 6572 7669 6365 7329 2077  --ml-services) w
+000028d0: 6974 6820 6120 5374 6162 6c65 2044 6966  ith a Stable Dif
+000028e0: 6675 7369 6f6e 2069 6d61 6765 2067 656e  fusion image gen
+000028f0: 6572 6174 696f 6e20 7365 7276 6963 6520  eration service 
+00002900: 6672 6f6d 2043 6d6f 6e20 4149 2773 205b  from Cmon AI's [
+00002910: 4578 6563 7574 6f72 2048 7562 5d28 6874  Executor Hub](ht
+00002920: 7470 733a 2f2f 636c 6f75 642e 636d 6f6e  tps://cloud.cmon
+00002930: 2e70 772f 6578 6563 7574 6f72 7329 2e20  .pw/executors). 
+00002940: 4368 6169 6e69 6e67 2074 6865 7365 2073  Chaining these s
+00002950: 6572 7669 6365 7320 746f 6765 7468 6572  ervices together
+00002960: 2069 6e74 6f20 6120 5b46 6c6f 775d 2868   into a [Flow](h
+00002970: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
+00002980: 2e70 772f 636f 6e63 6570 7473 2f66 6c6f  .pw/concepts/flo
+00002990: 772f 2920 7769 6c6c 2067 6976 6520 7573  w/) will give us
+000029a0: 2061 2073 6572 7669 6365 2074 6861 7420   a service that 
+000029b0: 7769 6c6c 2067 656e 6572 6174 6520 696d  will generate im
+000029c0: 6167 6573 2062 6173 6564 206f 6e20 6120  ages based on a 
+000029d0: 7072 6f6d 7074 2067 656e 6572 6174 6564  prompt generated
+000029e0: 2062 7920 7468 6520 4c4c 4d2e 0d0a 0d0a   by the LLM.....
+000029f0: 215b 5d28 2e2f 2e67 6974 6875 622f 696d  ![](./.github/im
+00002a00: 6167 6573 2f66 6c6f 772d 6469 6167 7261  ages/flow-diagra
+00002a10: 6d2e 706e 6729 0d0a 0d0a 4275 696c 6420  m.png)....Build 
+00002a20: 7468 6520 466c 6f77 2077 6974 6820 6569  the Flow with ei
+00002a30: 7468 6572 2050 7974 686f 6e20 6f72 2059  ther Python or Y
+00002a40: 414d 4c3a 0d0a 0d0a 3c64 6976 2063 6c61  AML:....<div cla
+00002a50: 7373 3d22 7461 626c 652d 7772 6170 7065  ss="table-wrappe
+00002a60: 7222 3e0d 0a3c 7461 626c 653e 0d0a 3c74  r">..<table>..<t
+00002a70: 723e 0d0a 3c74 683e 2050 7974 686f 6e20  r>..<th> Python 
+00002a80: 4150 493a 203c 636f 6465 3e66 6c6f 772e  API: <code>flow.
+00002a90: 7079 3c2f 636f 6465 3e20 3c2f 7468 3e20  py</code> </th> 
+00002aa0: 0d0a 3c74 683e 2059 414d 4c3a 203c 636f  ..<th> YAML: <co
+00002ab0: 6465 3e66 6c6f 772e 796d 6c3c 2f63 6f64  de>flow.yml</cod
+00002ac0: 653e 203c 2f74 683e 0d0a 3c2f 7472 3e0d  e> </th>..</tr>.
+00002ad0: 0a3c 7472 3e0d 0a3c 7464 3e0d 0a0d 0a60  .<tr>..<td>....`
+00002ae0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2063  ``python..from c
+00002af0: 6d6f 6e20 696d 706f 7274 2046 6c6f 770d  mon import Flow.
+00002b00: 0a66 726f 6d20 6578 6563 7574 6f72 2069  .from executor i
+00002b10: 6d70 6f72 7420 5374 6162 6c65 4c4d 0d0a  mport StableLM..
+00002b20: 0d0a 666c 6f77 203d 2028 0d0a 2020 2020  ..flow = (..    
+00002b30: 466c 6f77 2829 0d0a 2020 2020 2e61 6464  Flow()..    .add
+00002b40: 2875 7365 733d 5374 6162 6c65 4c4d 2c20  (uses=StableLM, 
+00002b50: 7469 6d65 6f75 745f 7265 6164 793d 2d31  timeout_ready=-1
+00002b60: 2c20 706f 7274 3d31 3233 3435 290d 0a20  , port=12345).. 
+00002b70: 2020 202e 6164 6428 0d0a 2020 2020 2020     .add(..      
+00002b80: 2020 7573 6573 3d27 636d 6f6e 6169 3a2f    uses='cmonai:/
+00002b90: 2f63 6d6f 6e2e 7077 2f54 6578 7454 6f49  /cmon.pw/TextToI
+00002ba0: 6d61 6765 272c 0d0a 2020 2020 2020 2020  mage',..        
+00002bb0: 7469 6d65 6f75 745f 7265 6164 793d 2d31  timeout_ready=-1
+00002bc0: 2c0d 0a20 2020 2020 2020 2069 6e73 7461  ,..        insta
+00002bd0: 6c6c 5f72 6571 7569 7265 6d65 6e74 733d  ll_requirements=
+00002be0: 5472 7565 2c0d 0a20 2020 2029 0d0a 2920  True,..    )..) 
+00002bf0: 2023 2075 7365 2074 6865 2045 7865 6375   # use the Execu
+00002c00: 746f 7220 6672 6f6d 2043 6d6f 6e27 7320  tor from Cmon's 
+00002c10: 4578 6563 7574 6f72 2068 7562 0d0a 0d0a  Executor hub....
+00002c20: 7769 7468 2066 6c6f 773a 0d0a 2020 2020  with flow:..    
+00002c30: 666c 6f77 2e62 6c6f 636b 2829 0d0a 6060  flow.block()..``
+00002c40: 600d 0a0d 0a3c 2f74 643e 0d0a 3c74 643e  `....</td>..<td>
+00002c50: 0d0a 0d0a 6060 6079 616d 6c0d 0a6a 7479  ....```yaml..jty
+00002c60: 7065 3a20 466c 6f77 0d0a 7769 7468 3a0d  pe: Flow..with:.
+00002c70: 0a20 2020 2070 6f72 743a 2031 3233 3435  .    port: 12345
+00002c80: 0d0a 6578 6563 7574 6f72 733a 0d0a 2020  ..executors:..  
+00002c90: 2d20 7573 6573 3a20 5374 6162 6c65 4c4d  - uses: StableLM
+00002ca0: 0d0a 2020 2020 7469 6d65 6f75 745f 7265  ..    timeout_re
+00002cb0: 6164 793a 202d 310d 0a20 2020 2070 795f  ady: -1..    py_
+00002cc0: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
+00002cd0: 2d20 6578 6563 7574 6f72 2e70 790d 0a20  - executor.py.. 
+00002ce0: 202d 2075 7365 733a 2063 6d6f 6e61 693a   - uses: cmonai:
+00002cf0: 2f2f 636d 6f6e 2e70 772f 5465 7874 546f  //cmon.pw/TextTo
+00002d00: 496d 6167 650d 0a20 2020 2074 696d 656f  Image..    timeo
+00002d10: 7574 5f72 6561 6479 3a20 2d31 0d0a 2020  ut_ready: -1..  
+00002d20: 2020 696e 7374 616c 6c5f 7265 7175 6972    install_requir
+00002d30: 656d 656e 7473 3a20 7472 7565 0d0a 6060  ements: true..``
+00002d40: 600d 0a0d 0a54 6865 6e20 7275 6e20 7468  `....Then run th
+00002d50: 6520 5941 4d4c 2046 6c6f 7720 7769 7468  e YAML Flow with
+00002d60: 2074 6865 2043 4c49 3a20 6063 6d6f 6e20   the CLI: `cmon 
+00002d70: 666c 6f77 202d 2d75 7365 7320 666c 6f77  flow --uses flow
+00002d80: 2e79 6d6c 600d 0a0d 0a3c 2f74 643e 0d0a  .yml`....</td>..
+00002d90: 3c2f 7472 3e0d 0a3c 2f74 6162 6c65 3e0d  </tr>..</table>.
+00002da0: 0a3c 2f64 6976 3e0d 0a0d 0a54 6865 6e2c  .</div>....Then,
+00002db0: 2075 7365 205b 436d 6f6e 2043 6c69 656e   use [Cmon Clien
+00002dc0: 745d 2868 7474 7073 3a2f 2f64 6f63 732e  t](https://docs.
+00002dd0: 636d 6f6e 2e70 772f 636f 6e63 6570 7473  cmon.pw/concepts
+00002de0: 2f63 6c69 656e 742f 2920 746f 206d 616b  /client/) to mak
+00002df0: 6520 7265 7175 6573 7473 2074 6f20 7468  e requests to th
+00002e00: 6520 466c 6f77 3a0d 0a0d 0a60 6060 7079  e Flow:....```py
+00002e10: 7468 6f6e 0d0a 6672 6f6d 2063 6d6f 6e20  thon..from cmon 
+00002e20: 696d 706f 7274 2043 6c69 656e 742c 2044  import Client, D
+00002e30: 6f63 756d 656e 740d 0a0d 0a63 6c69 656e  ocument....clien
+00002e40: 7420 3d20 436c 6965 6e74 2870 6f72 743d  t = Client(port=
+00002e50: 3132 3334 3529 0d0a 0d0a 7072 6f6d 7074  12345)....prompt
+00002e60: 203d 2044 6f63 756d 656e 7428 0d0a 2020   = Document(..  
+00002e70: 2020 7461 6773 203d 207b 2770 726f 6d70    tags = {'promp
+00002e80: 7427 3a20 2773 7567 6765 7374 2061 6e20  t': 'suggest an 
+00002e90: 696e 7465 7265 7374 696e 6720 696d 6167  interesting imag
+00002ea0: 6520 6765 6e65 7261 7469 6f6e 2070 726f  e generation pro
+00002eb0: 6d70 7420 666f 7220 6120 6d6f 6e61 206c  mpt for a mona l
+00002ec0: 6973 6120 7661 7269 616e 7427 7d0d 0a29  isa variant'}..)
+00002ed0: 0d0a 0d0a 7265 7370 6f6e 7365 203d 2063  ....response = c
+00002ee0: 6c69 656e 742e 706f 7374 286f 6e3d 272f  lient.post(on='/
+00002ef0: 272c 2069 6e70 7574 733d 5b70 726f 6d70  ', inputs=[promp
+00002f00: 745d 290d 0a0d 0a72 6573 706f 6e73 655b  t])....response[
+00002f10: 305d 2e64 6973 706c 6179 2829 0d0a 6060  0].display()..``
+00002f20: 600d 0a0d 0a21 5b5d 282e 2f2e 6769 7468  `....![](./.gith
+00002f30: 7562 2f69 6d61 6765 732f 6d6f 6e61 2d6c  ub/images/mona-l
+00002f40: 6973 612e 706e 6729 0d0a 0d0a 2323 2044  isa.png)....## D
+00002f50: 6570 6c6f 7920 746f 2074 6865 2063 6c6f  eploy to the clo
+00002f60: 7564 0d0a 0d0a 596f 7520 6361 6e20 616c  ud....You can al
+00002f70: 736f 2064 6570 6c6f 7920 6120 466c 6f77  so deploy a Flow
+00002f80: 2074 6f20 4a43 6c6f 7564 2e0d 0a0d 0a46   to JCloud.....F
+00002f90: 6972 7374 2c20 7475 726e 2074 6865 2060  irst, turn the `
+00002fa0: 666c 6f77 2e79 6d6c 6020 6669 6c65 2069  flow.yml` file i
+00002fb0: 6e74 6f20 6120 5b4a 436c 6f75 642d 636f  nto a [JCloud-co
+00002fc0: 6d70 6174 6962 6c65 2059 414d 4c5d 2868  mpatible YAML](h
+00002fd0: 7474 7073 3a2f 2f64 6f63 732e 636d 6f6e  ttps://docs.cmon
+00002fe0: 2e70 772f 636f 6e63 6570 7473 2f6a 636c  .pw/concepts/jcl
+00002ff0: 6f75 642f 7961 6d6c 2d73 7065 632f 2920  oud/yaml-spec/) 
+00003000: 6279 2073 7065 6369 6679 696e 6720 7265  by specifying re
+00003010: 736f 7572 6365 2072 6571 7569 7265 6d65  source requireme
+00003020: 6e74 7320 616e 6420 7573 696e 6720 636f  nts and using co
+00003030: 6e74 6169 6e65 7269 7a65 6420 4875 6220  ntainerized Hub 
+00003040: 4578 6563 7574 6f72 732e 0d0a 0d0a 5468  Executors.....Th
+00003050: 656e 2c20 7573 6520 6063 6d6f 6e20 636c  en, use `cmon cl
+00003060: 6f75 6420 6465 706c 6f79 6020 636f 6d6d  oud deploy` comm
+00003070: 616e 6420 746f 2064 6570 6c6f 7920 746f  and to deploy to
+00003080: 2074 6865 2063 6c6f 7564 3a0d 0a0d 0a60   the cloud:....`
+00003090: 6060 7368 656c 6c0d 0a77 6765 7420 6874  ``shell..wget ht
+000030a0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+000030b0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000030c0: 636d 6f6e 2e70 772f 636d 6f6e 2f6d 6173  cmon.pw/cmon/mas
+000030d0: 7465 722f 2e67 6974 6875 622f 6765 7474  ter/.github/gett
+000030e0: 696e 672d 7374 6172 7465 642f 6a63 6c6f  ing-started/jclo
+000030f0: 7564 2d66 6c6f 772e 796d 6c0d 0a63 6d6f  ud-flow.yml..cmo
+00003100: 6e20 636c 6f75 6420 6465 706c 6f79 206a  n cloud deploy j
+00003110: 636c 6f75 642d 666c 6f77 2e79 6d6c 0d0a  cloud-flow.yml..
+00003120: 6060 600d 0a0d 0a3e 202a 2a57 6172 6e69  ```....> **Warni
+00003130: 6e67 2a2a 0d0a 3e0d 0a3e 204d 616b 6520  ng**..>..> Make 
+00003140: 7375 7265 2074 6f20 6465 6c65 7465 2f63  sure to delete/c
+00003150: 6c65 616e 2075 7020 7468 6520 466c 6f77  lean up the Flow
+00003160: 206f 6e63 6520 796f 7520 6172 6520 646f   once you are do
+00003170: 6e65 2077 6974 6820 7468 6973 2074 7574  ne with this tut
+00003180: 6f72 6961 6c20 746f 2073 6176 6520 7265  orial to save re
+00003190: 736f 7572 6365 7320 616e 6420 6372 6564  sources and cred
+000031a0: 6974 732e 0d0a 0d0a 5265 6164 206d 6f72  its.....Read mor
+000031b0: 6520 6162 6f75 7420 5b64 6570 6c6f 7969  e about [deployi
+000031c0: 6e67 2046 6c6f 7773 2074 6f20 4a43 6c6f  ng Flows to JClo
+000031d0: 7564 5d28 6874 7470 733a 2f2f 646f 6373  ud](https://docs
+000031e0: 2e63 6d6f 6e2e 7077 2f63 6f6e 6365 7074  .cmon.pw/concept
+000031f0: 732f 6a63 6c6f 7564 2f23 6465 706c 6f79  s/jcloud/#deploy
+00003200: 292e 0d0a 0d0a 3c21 2d2d 2065 6e64 2062  ).....<!-- end b
+00003210: 7569 6c64 2d70 6970 656c 696e 6573 202d  uild-pipelines -
+00003220: 2d3e 0d0a 0d0a 4368 6563 6b20 5b74 6865  ->....Check [the
+00003230: 2067 6574 7469 6e67 2d73 7461 7274 6564   getting-started
+00003240: 2070 726f 6a65 6374 2073 6f75 7263 6520   project source 
+00003250: 636f 6465 5d28 6874 7470 733a 2f2f 6769  code](https://gi
+00003260: 7468 7562 2e63 6f6d 2f63 6d6f 6e2e 7077  thub.com/cmon.pw
+00003270: 2f63 6d6f 6e2f 7472 6565 2f6d 6173 7465  /cmon/tree/maste
+00003280: 722f 2e67 6974 6875 622f 6765 7474 696e  r/.github/gettin
+00003290: 672d 7374 6172 7465 6429 2e0d 0a0d 0a23  g-started).....#
+000032a0: 2323 2045 6173 7920 7363 616c 6162 696c  ## Easy scalabil
+000032b0: 6974 7920 616e 6420 636f 6e63 7572 7265  ity and concurre
+000032c0: 6e63 790d 0a0d 0a57 6879 206e 6f74 206a  ncy....Why not j
+000032d0: 7573 7420 7573 6520 7374 616e 6461 7264  ust use standard
+000032e0: 2050 7974 686f 6e20 746f 2062 7569 6c64   Python to build
+000032f0: 2074 6861 7420 6d69 6372 6f73 6572 7669   that microservi
+00003300: 6365 2061 6e64 2070 6970 656c 696e 653f  ce and pipeline?
+00003310: 2043 6d6f 6e20 6163 6365 6c65 7261 7465   Cmon accelerate
+00003320: 7320 7469 6d65 2074 6f20 6d61 726b 6574  s time to market
+00003330: 206f 6620 796f 7572 2061 7070 6c69 6361   of your applica
+00003340: 7469 6f6e 2062 7920 6d61 6b69 6e67 2069  tion by making i
+00003350: 7420 6d6f 7265 2073 6361 6c61 626c 6520  t more scalable 
+00003360: 616e 6420 636c 6f75 642d 6e61 7469 7665  and cloud-native
+00003370: 2e20 436d 6f6e 2061 6c73 6f20 6861 6e64  . Cmon also hand
+00003380: 6c65 7320 7468 6520 696e 6672 6173 7472  les the infrastr
+00003390: 7563 7475 7265 2063 6f6d 706c 6578 6974  ucture complexit
+000033a0: 7920 696e 2070 726f 6475 6374 696f 6e20  y in production 
+000033b0: 616e 6420 6f74 6865 7220 4461 792d 3220  and other Day-2 
+000033c0: 6f70 6572 6174 696f 6e73 2073 6f20 7468  operations so th
+000033d0: 6174 2079 6f75 2063 616e 2066 6f63 7573  at you can focus
+000033e0: 206f 6e20 7468 6520 6461 7461 2061 7070   on the data app
+000033f0: 6c69 6361 7469 6f6e 2069 7473 656c 662e  lication itself.
+00003400: 0d0a 0d0a 496e 6372 6561 7365 2079 6f75  ....Increase you
+00003410: 7220 6170 706c 6963 6174 696f 6e27 7320  r application's 
+00003420: 7468 726f 7567 6870 7574 2077 6974 6820  throughput with 
+00003430: 7363 616c 6162 696c 6974 7920 6665 6174  scalability feat
+00003440: 7572 6573 206f 7574 206f 6620 7468 6520  ures out of the 
+00003450: 626f 782c 206c 696b 6520 5b72 6570 6c69  box, like [repli
+00003460: 6361 735d 2868 7474 7073 3a2f 2f64 6f63  cas](https://doc
+00003470: 732e 636d 6f6e 2e70 772f 636f 6e63 6570  s.cmon.pw/concep
+00003480: 7473 2f6f 7263 6865 7374 7261 7469 6f6e  ts/orchestration
+00003490: 2f73 6361 6c65 2d6f 7574 2f23 7265 706c  /scale-out/#repl
+000034a0: 6963 6174 652d 6578 6563 7574 6f72 7329  icate-executors)
+000034b0: 2c20 5b73 6861 7264 735d 2868 7474 7073  , [shards](https
+000034c0: 3a2f 2f64 6f63 732e 636d 6f6e 2e70 772f  ://docs.cmon.pw/
+000034d0: 636f 6e63 6570 7473 2f6f 7263 6865 7374  concepts/orchest
+000034e0: 7261 7469 6f6e 2f73 6361 6c65 2d6f 7574  ration/scale-out
+000034f0: 2f23 6375 7374 6f6d 697a 652d 706f 6c6c  /#customize-poll
+00003500: 696e 672d 6265 6861 7669 6f72 7329 2061  ing-behaviors) a
+00003510: 6e64 205b 6479 6e61 6d69 6320 6261 7463  nd [dynamic batc
+00003520: 6869 6e67 5d28 6874 7470 733a 2f2f 646f  hing](https://do
+00003530: 6373 2e63 6d6f 6e2e 7077 2f63 6f6e 6365  cs.cmon.pw/conce
+00003540: 7074 732f 7365 7276 696e 672f 6578 6563  pts/serving/exec
+00003550: 7574 6f72 2f64 796e 616d 6963 2d62 6174  utor/dynamic-bat
+00003560: 6368 696e 672f 292e 0d0a 0d0a 4c65 7427  ching/).....Let'
+00003570: 7320 7363 616c 6520 6120 5374 6162 6c65  s scale a Stable
+00003580: 2044 6966 6675 7369 6f6e 2045 7865 6375   Diffusion Execu
+00003590: 746f 7220 6465 706c 6f79 6d65 6e74 2077  tor deployment w
+000035a0: 6974 6820 7265 706c 6963 6173 2061 6e64  ith replicas and
+000035b0: 2064 796e 616d 6963 2062 6174 6368 696e   dynamic batchin
+000035c0: 673a 0d0a 0d0a 215b 5d28 2e2f 2e67 6974  g:....![](./.git
+000035d0: 6875 622f 696d 6167 6573 2f73 6361 6c65  hub/images/scale
+000035e0: 642d 6465 706c 6f79 6d65 6e74 2e70 6e67  d-deployment.png
+000035f0: 290d 0a0d 0a2a 2043 7265 6174 6520 7477  )....* Create tw
+00003600: 6f20 7265 706c 6963 6173 2c20 7769 7468  o replicas, with
+00003610: 205b 6120 4750 5520 6173 7369 676e 6564   [a GPU assigned
+00003620: 2066 6f72 2065 6163 685d 2868 7474 7073   for each](https
+00003630: 3a2f 2f64 6f63 732e 636d 6f6e 2e70 772f  ://docs.cmon.pw/
+00003640: 636f 6e63 6570 7473 2f66 6c6f 772f 7363  concepts/flow/sc
+00003650: 616c 652d 6f75 742f 2372 6570 6c69 6361  ale-out/#replica
+00003660: 7465 2d6f 6e2d 6d75 6c74 6970 6c65 2d67  te-on-multiple-g
+00003670: 7075 7329 2e0d 0a2a 2045 6e61 626c 6520  pus)...* Enable 
+00003680: 6479 6e61 6d69 6320 6261 7463 6869 6e67  dynamic batching
+00003690: 2074 6f20 7072 6f63 6573 7320 696e 636f   to process inco
+000036a0: 6d69 6e67 2070 6172 616c 6c65 6c20 7265  ming parallel re
+000036b0: 7175 6573 7473 2074 6f67 6574 6865 7220  quests together 
+000036c0: 7769 7468 2074 6865 2073 616d 6520 6d6f  with the same mo
+000036d0: 6465 6c20 696e 6665 7265 6e63 652e 0d0a  del inference...
+000036e0: 0d0a 0d0a 3c64 6976 2063 6c61 7373 3d22  ....<div class="
+000036f0: 7461 626c 652d 7772 6170 7065 7222 3e0d  table-wrapper">.
+00003700: 0a3c 7461 626c 653e 0d0a 3c74 723e 0d0a  .<table>..<tr>..
+00003710: 3c74 683e 204e 6f72 6d61 6c20 4465 706c  <th> Normal Depl
+00003720: 6f79 6d65 6e74 203c 2f74 683e 200d 0a3c  oyment </th> ..<
+00003730: 7468 3e20 5363 616c 6564 2044 6570 6c6f  th> Scaled Deplo
+00003740: 796d 656e 7420 3c2f 7468 3e0d 0a3c 2f74  yment </th>..</t
+00003750: 723e 0d0a 3c74 723e 0d0a 3c74 643e 0d0a  r>..<tr>..<td>..
+00003760: 0d0a 6060 6079 616d 6c0d 0a6a 7479 7065  ..```yaml..jtype
+00003770: 3a20 4465 706c 6f79 6d65 6e74 0d0a 7769  : Deployment..wi
+00003780: 7468 3a0d 0a20 2074 696d 656f 7574 5f72  th:..  timeout_r
+00003790: 6561 6479 3a20 2d31 0d0a 2020 7573 6573  eady: -1..  uses
+000037a0: 3a20 636d 6f6e 6169 3a2f 2f63 6d6f 6e2e  : cmonai://cmon.
+000037b0: 7077 2f54 6578 7454 6f49 6d61 6765 0d0a  pw/TextToImage..
+000037c0: 2020 696e 7374 616c 6c5f 7265 7175 6972    install_requir
+000037d0: 656d 656e 7473 3a20 7472 7565 0d0a 6060  ements: true..``
+000037e0: 600d 0a0d 0a3c 2f74 643e 0d0a 3c74 643e  `....</td>..<td>
+000037f0: 0d0a 0d0a 6060 6079 616d 6c0d 0a6a 7479  ....```yaml..jty
+00003800: 7065 3a20 4465 706c 6f79 6d65 6e74 0d0a  pe: Deployment..
+00003810: 7769 7468 3a0d 0a20 2074 696d 656f 7574  with:..  timeout
+00003820: 5f72 6561 6479 3a20 2d31 0d0a 2020 7573  _ready: -1..  us
+00003830: 6573 3a20 636d 6f6e 6169 3a2f 2f63 6d6f  es: cmonai://cmo
+00003840: 6e2e 7077 2f54 6578 7454 6f49 6d61 6765  n.pw/TextToImage
+00003850: 0d0a 2020 696e 7374 616c 6c5f 7265 7175  ..  install_requ
+00003860: 6972 656d 656e 7473 3a20 7472 7565 0d0a  irements: true..
+00003870: 2020 656e 763a 0d0a 2020 2043 5544 415f    env:..   CUDA_
+00003880: 5649 5349 424c 455f 4445 5649 4345 533a  VISIBLE_DEVICES:
+00003890: 2052 520d 0a20 2072 6570 6c69 6361 733a   RR..  replicas:
+000038a0: 2032 0d0a 2020 7573 6573 5f64 796e 616d   2..  uses_dynam
+000038b0: 6963 5f62 6174 6368 696e 673a 2023 2063  ic_batching: # c
+000038c0: 6f6e 6669 6775 7265 2064 796e 616d 6963  onfigure dynamic
+000038d0: 2062 6174 6368 696e 670d 0a20 2020 202f   batching..    /
+000038e0: 6465 6661 756c 743a 0d0a 2020 2020 2020  default:..      
+000038f0: 7072 6566 6572 7265 645f 6261 7463 685f  preferred_batch_
+00003900: 7369 7a65 3a20 3130 0d0a 2020 2020 2020  size: 10..      
+00003910: 7469 6d65 6f75 743a 2032 3030 0d0a 6060  timeout: 200..``
+00003920: 600d 0a0d 0a3c 2f74 643e 0d0a 3c2f 7472  `....</td>..</tr
+00003930: 3e0d 0a3c 2f74 6162 6c65 3e0d 0a3c 2f64  >..</table>..</d
+00003940: 6976 3e0d 0a0d 0a41 7373 756d 696e 6720  iv>....Assuming 
+00003950: 796f 7572 206d 6163 6869 6e65 2068 6173  your machine has
+00003960: 2074 776f 2047 5055 732c 2075 7369 6e67   two GPUs, using
+00003970: 2074 6865 2073 6361 6c65 6420 6465 706c   the scaled depl
+00003980: 6f79 6d65 6e74 2059 414d 4c20 7769 6c6c  oyment YAML will
+00003990: 2067 6976 6520 6265 7474 6572 2074 6872   give better thr
+000039a0: 6f75 6768 7075 7420 636f 6d70 6172 6564  oughput compared
+000039b0: 2074 6f20 7468 6520 6e6f 726d 616c 2064   to the normal d
+000039c0: 6570 6c6f 796d 656e 742e 0d0a 0d0a 5468  eployment.....Th
+000039d0: 6573 6520 6665 6174 7572 6573 2061 7070  ese features app
+000039e0: 6c79 2074 6f20 626f 7468 205b 4465 706c  ly to both [Depl
+000039f0: 6f79 6d65 6e74 2059 414d 4c5d 2868 7474  oyment YAML](htt
+00003a00: 7073 3a2f 2f64 6f63 732e 636d 6f6e 2e70  ps://docs.cmon.p
+00003a10: 772f 636f 6e63 6570 7473 2f65 7865 6375  w/concepts/execu
+00003a20: 746f 722f 6465 706c 6f79 6d65 6e74 2d79  tor/deployment-y
+00003a30: 616d 6c2d 7370 6563 2f23 6465 706c 6f79  aml-spec/#deploy
+00003a40: 6d65 6e74 2d79 616d 6c2d 7370 6563 2920  ment-yaml-spec) 
+00003a50: 616e 6420 5b46 6c6f 7720 5941 4d4c 5d28  and [Flow YAML](
+00003a60: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00003a70: 6e2e 7077 2f63 6f6e 6365 7074 732f 666c  n.pw/concepts/fl
+00003a80: 6f77 2f79 616d 6c2d 7370 6563 2f29 2e20  ow/yaml-spec/). 
+00003a90: 5468 616e 6b73 2074 6f20 7468 6520 5941  Thanks to the YA
+00003aa0: 4d4c 2073 796e 7461 782c 2079 6f75 2063  ML syntax, you c
+00003ab0: 616e 2069 6e6a 6563 7420 6465 706c 6f79  an inject deploy
+00003ac0: 6d65 6e74 2063 6f6e 6669 6775 7261 7469  ment configurati
+00003ad0: 6f6e 7320 7265 6761 7264 6c65 7373 206f  ons regardless o
+00003ae0: 6620 4578 6563 7574 6f72 2063 6f64 652e  f Executor code.
+00003af0: 0d0a 0d0a 2323 2320 4765 7420 6f6e 2074  ....### Get on t
+00003b00: 6865 2066 6173 7420 6c61 6e65 2074 6f20  he fast lane to 
+00003b10: 636c 6f75 642d 6e61 7469 7665 0d0a 0d0a  cloud-native....
+00003b20: 5573 696e 6720 4b75 6265 726e 6574 6573  Using Kubernetes
+00003b30: 2077 6974 6820 436d 6f6e 2069 7320 6561   with Cmon is ea
+00003b40: 7379 3a0d 0a0d 0a60 6060 6261 7368 0d0a  sy:....```bash..
+00003b50: 636d 6f6e 2065 7870 6f72 7420 6b75 6265  cmon export kube
+00003b60: 726e 6574 6573 2066 6c6f 772e 796d 6c20  rnetes flow.yml 
+00003b70: 2e2f 6d79 2d6b 3873 0d0a 6b75 6265 6374  ./my-k8s..kubect
+00003b80: 6c20 6170 706c 7920 2d52 202d 6620 6d79  l apply -R -f my
+00003b90: 2d6b 3873 0d0a 6060 600d 0a0d 0a41 6e64  -k8s..```....And
+00003ba0: 2073 6f20 6973 2044 6f63 6b65 7220 436f   so is Docker Co
+00003bb0: 6d70 6f73 653a 0d0a 0d0a 6060 6062 6173  mpose:....```bas
+00003bc0: 680d 0a63 6d6f 6e20 6578 706f 7274 2064  h..cmon export d
+00003bd0: 6f63 6b65 722d 636f 6d70 6f73 6520 666c  ocker-compose fl
+00003be0: 6f77 2e79 6d6c 2064 6f63 6b65 722d 636f  ow.yml docker-co
+00003bf0: 6d70 6f73 652e 796d 6c0d 0a64 6f63 6b65  mpose.yml..docke
+00003c00: 722d 636f 6d70 6f73 6520 7570 0d0a 6060  r-compose up..``
+00003c10: 600d 0a0d 0a3e 202a 2a4e 6f74 652a 2a0d  `....> **Note**.
+00003c20: 0a3e 2059 6f75 2063 616e 2061 6c73 6f20  .> You can also 
+00003c30: 6578 706f 7274 2044 6570 6c6f 796d 656e  export Deploymen
+00003c40: 7420 5941 4d4c 2074 6f20 5b4b 7562 6572  t YAML to [Kuber
+00003c50: 6e65 7465 735d 2868 7474 7073 3a2f 2f64  netes](https://d
+00003c60: 6f63 732e 636d 6f6e 2e70 772f 636f 6e63  ocs.cmon.pw/conc
+00003c70: 6570 7473 2f65 7865 6375 746f 722f 7365  epts/executor/se
+00003c80: 7276 652f 2373 6572 7665 2d76 6961 2d6b  rve/#serve-via-k
+00003c90: 7562 6572 6e65 7465 7329 2061 6e64 205b  ubernetes) and [
+00003ca0: 446f 636b 6572 2043 6f6d 706f 7365 5d28  Docker Compose](
+00003cb0: 6874 7470 733a 2f2f 646f 6373 2e63 6d6f  https://docs.cmo
+00003cc0: 6e2e 7077 2f63 6f6e 6365 7074 732f 6578  n.pw/concepts/ex
+00003cd0: 6563 7574 6f72 2f73 6572 7665 2f23 7365  ecutor/serve/#se
+00003ce0: 7276 652d 7669 612d 646f 636b 6572 2d63  rve-via-docker-c
+00003cf0: 6f6d 706f 7365 292e 0d0a 0d0a 5468 6174  ompose).....That
+00003d00: 2773 206e 6f74 2061 6c6c 2e20 5765 2061  's not all. We a
+00003d10: 6c73 6f20 7375 7070 6f72 7420 5b4f 7065  lso support [Ope
+00003d20: 6e54 656c 656d 6574 7279 2c20 5072 6f6d  nTelemetry, Prom
+00003d30: 6574 6865 7573 2c20 616e 6420 4a61 6567  etheus, and Jaeg
+00003d40: 6572 5d28 6874 7470 733a 2f2f 646f 6373  er](https://docs
+00003d50: 2e63 6d6f 6e2e 7077 2f63 6c6f 7564 2d6e  .cmon.pw/cloud-n
+00003d60: 6174 6976 656e 6573 732f 6f70 656e 7465  ativeness/opente
+00003d70: 6c65 6d65 7472 792f 292e 0d0a 0d0a 5768  lemetry/).....Wh
+00003d80: 6174 2063 6c6f 7564 2d6e 6174 6976 6520  at cloud-native 
+00003d90: 7465 6368 6e6f 6c6f 6779 2069 7320 7374  technology is st
+00003da0: 696c 6c20 6368 616c 6c65 6e67 696e 6720  ill challenging 
+00003db0: 746f 2079 6f75 3f20 5b54 656c 6c20 7573  to you? [Tell us
+00003dc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003dd0: 2e63 6f6d 2f63 6d6f 6e2e 7077 2f63 6d6f  .com/cmon.pw/cmo
+00003de0: 6e2f 6973 7375 6573 2920 616e 6420 7765  n/issues) and we
+00003df0: 276c 6c20 6861 6e64 6c65 2074 6865 2063  'll handle the c
+00003e00: 6f6d 706c 6578 6974 7920 616e 6420 6d61  omplexity and ma
+00003e10: 6b65 2069 7420 6561 7379 2066 6f72 2079  ke it easy for y
+00003e20: 6f75 2e0d 0a0d 0a3c 212d 2d20 7374 6172  ou.....<!-- star
+00003e30: 7420 7375 7070 6f72 742d 7069 7463 6820  t support-pitch 
+00003e40: 2d2d 3e0d 0a0d 0a23 2320 5375 7070 6f72  -->....## Suppor
+00003e50: 740d 0a0d 0a2d 204a 6f69 6e20 6f75 7220  t....- Join our 
+00003e60: 5b44 6973 636f 7264 2063 6f6d 6d75 6e69  [Discord communi
+00003e70: 7479 5d28 6874 7470 733a 2f2f 6469 7363  ty](https://disc
+00003e80: 6f72 642e 636d 6f6e 2e70 7729 2061 6e64  ord.cmon.pw) and
+00003e90: 2063 6861 7420 7769 7468 206f 7468 6572   chat with other
+00003ea0: 2063 6f6d 6d75 6e69 7479 206d 656d 6265   community membe
+00003eb0: 7273 2061 626f 7574 2069 6465 6173 2e0d  rs about ideas..
+00003ec0: 0a2d 2053 7562 7363 7269 6265 2074 6f20  .- Subscribe to 
+00003ed0: 7468 6520 6c61 7465 7374 2076 6964 656f  the latest video
+00003ee0: 2074 7574 6f72 6961 6c73 206f 6e20 6f75   tutorials on ou
+00003ef0: 7220 5b59 6f75 5475 6265 2063 6861 6e6e  r [YouTube chann
+00003f00: 656c 5d28 6874 7470 733a 2f2f 796f 7574  el](https://yout
+00003f10: 7562 652e 636f 6d2f 632f 636d 6f6e 2e70  ube.com/c/cmon.p
+00003f20: 7729 0d0a 0d0a 2323 204a 6f69 6e20 5573  w)....## Join Us
+00003f30: 0d0a 0d0a 436d 6f6e 2069 7320 6261 636b  ....Cmon is back
+00003f40: 6564 2062 7920 5b43 6d6f 6e20 4149 5d28  ed by [Cmon AI](
+00003f50: 6874 7470 733a 2f2f 636d 6f6e 2e70 7729  https://cmon.pw)
+00003f60: 2061 6e64 206c 6963 656e 7365 6420 756e   and licensed un
+00003f70: 6465 7220 5b41 7061 6368 652d 322e 305d  der [Apache-2.0]
+00003f80: 282e 2f4c 4943 454e 5345 292e 0d0a 0d0a  (./LICENSE).....
+00003f90: 3c21 2d2d 2065 6e64 2073 7570 706f 7274  <!-- end support
+00003fa0: 2d70 6974 6368 202d 2d3e 0d0a            -pitch -->..
```

### Comparing `cmon-ai-0.38.5/cmon_cli/__init__.py` & `cmon-ai-0.42.6/cmon_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon_cli/api.py` & `cmon-ai-0.42.6/cmon_cli/api.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon_cli/autocomplete.py` & `cmon-ai-0.42.6/cmon_cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/cmon_cli/export.py` & `cmon-ai-0.42.6/cmon_cli/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     from cmon.parsers import get_main_parser
 
     all_d = {
         'name': 'Cmon',
         'description': 'Build multimodal AI services via cloud native technologies',
         'license': 'Apache 2.0',
         'vendor': 'Cmon AI Limited',
-        'source': 'https://github.com/cmon-ai/cmon/tree/'
+        'source': 'https://github.com/cmon.pw/cmon/tree/'
         + os.environ.get('CMON_VCS_VERSION', 'master'),
-        'url': 'https://cmon.ai',
-        'docs': 'https://docs.cmon.ai',
-        'authors': 'dev-team@cmon.ai',
+        'url': 'https://cmon.pw',
+        'docs': 'https://docs.cmon.pw',
+        'authors': 'dev-team@cmon.pw',
         'version': __version__,
         'methods': [],
         'revision': os.environ.get('CMON_VCS_VERSION'),
     }
 
     def get_p(p, parent_d):
         parsers = p()._actions[-1].choices
```

### Comparing `cmon-ai-0.38.5/cmon_cli/lookup.py` & `cmon-ai-0.42.6/cmon_cli/lookup.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/extra-requirements.txt` & `cmon-ai-0.42.6/extra-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 protobuf>=3.19.0           
 grpcio>=1.46.0<1.48.1     
 grpcio-reflection>=1.46.0<1.48.1  
 grpcio-health-checking>=1.46.0<1.48.1  
 pyyaml>=5.3.1              
 packaging>=20.0            
 docarray>=0.16.4<0.30.0  
-cmon-hubble-sdk>=0.30.4    
+# cmon-hubble-sdk>=0.30.4    
 jcloud>=0.0.35             
 opentelemetry-api>=1.12.0  
 opentelemetry-instrumentation-grpc>=0.35b0   
-uvloop                    
+#uvloop==0.15.0                    
 prometheus_client>=0.12.0          
 opentelemetry-sdk>=1.14.0   
 #opentelemetry-exporter-otlp>=1.12.0  
 #opentelemetry-exporter-prometheus>=1.12.0rc1  
 #opentelemetry-instrumentation-aiohttp-client>=0.33b0    
 #opentelemetry-instrumentation-fastapi>=0.33b0 
 #opentelemetry-exporter-otlp-proto-grpc>=1.13.0 
@@ -82,7 +82,8 @@
 jsonschema                 
 portforward>=0.2.4<0.4.3         
 tensorflow>=2.0            
 #opentelemetry-utils>=0.33b0  
 prometheus-api-client>=0.5.1  
 watchfiles>=0.18.0         
 urllib3<2.0.0              
+git+https://github.com/openai-ae/docarray.git
```

### Comparing `cmon-ai-0.38.5/fastentrypoints.py` & `cmon-ai-0.42.6/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `cmon-ai-0.38.5/setup.py` & `cmon-ai-0.42.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     libinfo_py = path.join(pkg_name, '__init__.py')
     libinfo_content = open(libinfo_py, 'r', encoding='utf-8').readlines()
     version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][
         0
     ]
     exec(version_line)  # gives __version__
 except FileNotFoundError:
-    __version__ = '0.38.5'
+    __version__ = '0.42.6'
 
 try:
     with open('README.md', encoding='utf-8') as fp:
         _long_description = fp.read()
 except FileNotFoundError:
     _long_description = ''
 
@@ -191,18 +191,18 @@
 setup(
     name=pkg_name,
     packages=find_packages(),
     version=__version__,
     include_package_data=True,
     description='Build multimodal AI services via cloud native technologies · Neural Search · Generative AI · MLOps',
     author='Cmon AI',
-    author_email='hello@cmon.ai',
+    author_email='hello@cmon.pw',
     license='Apache 2.0',
-    url='https://github.com/alinooriyan/Cmon-AI',
-    download_url='https://github.com/alinooriyan/Cmon-AI/archive/refs/tags/AI.zip',
+    url='https://github.com/openai-ae/Cmon-AI-Library',
+    download_url='https://github.com/openai-ae/Cmon-AI-Library/archive/refs/tags/AI.zip',
     long_description=_long_description,
     long_description_content_type='text/markdown',
     zip_safe=False,
     install_requires=list(final_deps),
     entry_points={
         'console_scripts': [
             'cmon=cmon_cli:main',
@@ -236,14 +236,14 @@
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     project_urls={
         'Documentation': 'https://docs.cmon.pw',
-        'Source': 'https://github.com/alinooriyan/cmon-ai/',
-        'Tracker': 'https://github.com/alinooriyan/cmon-ai/issues',
+        'Source': 'https://github.com/openai-ae/cmon-ai/',
+        'Tracker': 'https://github.com/openai-ae/cmon-ai/issues',
     },
     keywords='cmon cloud-native cross-modal multimodal neural-search query search index elastic neural-network encoding '
     'embedding serving docker container image video audio deep-learning mlops',
     **extra_golang_kw,
 )
```

