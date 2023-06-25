# Comparing `tmp/openapi-pydantic-models-0.1.0.tar.gz` & `tmp/openapi-pydantic-models-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi-pydantic-models-0.1.0.tar", last modified: Sun Jun 25 16:17:32 2023, max compression
+gzip compressed data, was "openapi-pydantic-models-0.1.1.tar", last modified: Sun Jun 25 16:50:58 2023, max compression
```

## Comparing `openapi-pydantic-models-0.1.0.tar` & `openapi-pydantic-models-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-25 16:17:32.360415 openapi-pydantic-models-0.1.0/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      133 2023-06-25 16:13:38.000000 openapi-pydantic-models-0.1.0/.bumpversion.cfg
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-25 16:04:19.000000 openapi-pydantic-models-0.1.0/.gitignore
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-25 16:04:19.000000 openapi-pydantic-models-0.1.0/LICENSE
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      608 2023-06-25 16:04:35.000000 openapi-pydantic-models-0.1.0/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4104 2023-06-25 16:17:32.360415 openapi-pydantic-models-0.1.0/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3250 2023-06-25 16:13:38.000000 openapi-pydantic-models-0.1.0/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2630 2023-06-25 16:13:27.000000 openapi-pydantic-models-0.1.0/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-25 16:17:32.360415 openapi-pydantic-models-0.1.0/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-25 16:17:32.352415 openapi-pydantic-models-0.1.0/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-25 16:17:32.356415 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       50 2023-06-25 16:04:35.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/__init__.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-25 16:17:32.356415 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/commons/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      100 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/commons/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      507 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/commons/base_model.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1712 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/commons/utilities.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-25 16:17:32.360415 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1491 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3576 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1319 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/components_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      194 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/contact_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      528 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      295 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/example_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      186 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      864 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/header_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      473 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/info_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      199 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/license_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      396 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/link_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      129 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/locations.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      630 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      259 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      354 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1115 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1207 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      988 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      948 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3800 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      253 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/reference_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      283 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      503 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/response_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3869 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      377 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/schema_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       49 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      882 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      325 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/server_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      253 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3218 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      230 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/styles.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      300 2023-06-25 16:04:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/tag_object.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-25 16:17:32.356415 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4104 2023-06-25 16:17:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2470 2023-06-25 16:17:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-25 16:17:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-25 16:16:12.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      366 2023-06-25 16:17:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       24 2023-06-25 16:17:32.000000 openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.140567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/callback_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/components_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/contact_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/example_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/header_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/info_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/license_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/link_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/operation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/paths_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/reference_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/response_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/responses_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/schema_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/server_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-25 16:50:47.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/tag_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:50:58.136567 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:50:57.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-25 16:50:58.000000 openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/top_level.txt
```

### Comparing `openapi-pydantic-models-0.1.0/.gitignore` & `openapi-pydantic-models-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/LICENSE` & `openapi-pydantic-models-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/MANIFEST.in` & `openapi-pydantic-models-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/PKG-INFO` & `openapi-pydantic-models-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,18 @@
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 # openapi-pydantic-models
 
+[![PyPI Status](https://badge.fury.io/py/openapi-pydantic-models.svg)](https://badge.fury.io/py/openapi-pydantic-models)
+[![license](https://img.shields.io/pypi/l/openapi-pydantic-models.svg)](https://opensource.org/licenses/MIT)
+[![python_versions](https://img.shields.io/pypi/pyversions/openapi-pydantic-models.svg)](https://pypi.org/project/openapi-pydantic-models/)
+
 [OpenAPI Specification v3.1.0](https://spec.openapis.org/oas/v3.1.0) objects implemented
 as [pydantic](https://docs.pydantic.dev/) models.
 
 ## Install
 
 ```sh
 pip install openapi-pydantic-models
```

### Comparing `openapi-pydantic-models-0.1.0/README.md` & `openapi-pydantic-models-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # openapi-pydantic-models
 
+[![PyPI Status](https://badge.fury.io/py/openapi-pydantic-models.svg)](https://badge.fury.io/py/openapi-pydantic-models)
+[![license](https://img.shields.io/pypi/l/openapi-pydantic-models.svg)](https://opensource.org/licenses/MIT)
+[![python_versions](https://img.shields.io/pypi/pyversions/openapi-pydantic-models.svg)](https://pypi.org/project/openapi-pydantic-models/)
+
 [OpenAPI Specification v3.1.0](https://spec.openapis.org/oas/v3.1.0) objects implemented
 as [pydantic](https://docs.pydantic.dev/) models.
 
 ## Install
 
 ```sh
 pip install openapi-pydantic-models
```

### Comparing `openapi-pydantic-models-0.1.0/pyproject.toml` & `openapi-pydantic-models-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "openapi-pydantic-models"
-version = "0.1.0"
+version = "0.1.1"
 description = "pydantic models for OpeanAPI Specification 3.1.0 objects."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/commons/utilities.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/commons/utilities.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/__init__.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/callback_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/components_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/components_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/encoding_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/header_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/header_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/media_type_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/openapi_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/operation_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/parameter_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/path_item_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/paths_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/responses_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/PKG-INFO` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 0.1.0
+Version: 0.1.1
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,18 @@
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 # openapi-pydantic-models
 
+[![PyPI Status](https://badge.fury.io/py/openapi-pydantic-models.svg)](https://badge.fury.io/py/openapi-pydantic-models)
+[![license](https://img.shields.io/pypi/l/openapi-pydantic-models.svg)](https://opensource.org/licenses/MIT)
+[![python_versions](https://img.shields.io/pypi/pyversions/openapi-pydantic-models.svg)](https://pypi.org/project/openapi-pydantic-models/)
+
 [OpenAPI Specification v3.1.0](https://spec.openapis.org/oas/v3.1.0) objects implemented
 as [pydantic](https://docs.pydantic.dev/) models.
 
 ## Install
 
 ```sh
 pip install openapi-pydantic-models
```

### Comparing `openapi-pydantic-models-0.1.0/src/openapi_pydantic_models.egg-info/SOURCES.txt` & `openapi-pydantic-models-0.1.1/src/openapi_pydantic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

