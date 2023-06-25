# Comparing `tmp/Authlib-1.2.0.tar.gz` & `tmp/Authlib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Authlib-1.2.0.tar", last modified: Tue Dec  6 08:39:40 2022, max compression
+gzip compressed data, was "Authlib-1.2.1.tar", last modified: Sun Jun 25 13:03:12 2023, max compression
```

## Comparing `Authlib-1.2.0.tar` & `Authlib-1.2.1.tar`

### file list

```diff
@@ -1,240 +1,241 @@
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/Authlib.egg-info/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3750 2022-12-06 08:39:40.000000 Authlib-1.2.0/Authlib.egg-info/PKG-INFO
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7197 2022-12-06 08:39:40.000000 Authlib-1.2.0/Authlib.egg-info/SOURCES.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2022-12-06 08:39:40.000000 Authlib-1.2.0/Authlib.egg-info/dependency_links.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2022-12-06 08:39:21.000000 Authlib-1.2.0/Authlib.egg-info/not-zip-safe
--rw-r--r--   0 lepture   (1000) lepture   (1000)       18 2022-12-06 08:39:40.000000 Authlib-1.2.0/Authlib.egg-info/requires.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)        8 2022-12-06 08:39:40.000000 Authlib-1.2.0/Authlib.egg-info/top_level.txt
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1514 2022-04-06 09:01:20.000000 Authlib-1.2.0/LICENSE
--rw-r--r--   0 lepture   (1000) lepture   (1000)       48 2022-04-06 09:01:20.000000 Authlib-1.2.0/MANIFEST.in
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3750 2022-12-06 08:39:40.616931 Authlib-1.2.0/PKG-INFO
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2264 2022-12-06 07:30:31.000000 Authlib-1.2.0/README.rst
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      476 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/__init__.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/common/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/common/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1546 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/common/encoding.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1711 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/common/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      493 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/common/security.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4501 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/common/urls.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      312 2022-12-06 08:32:20.000000 Authlib-1.2.0/authlib/consts.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      499 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/deprecate.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/__init__.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/base_client/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      653 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/base_client/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5855 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/base_client/async_app.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2811 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/base_client/async_openid.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      632 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/base_client/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1879 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/base_client/framework_integration.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4281 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/base_client/registry.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    12448 2022-12-06 07:47:11.000000 Authlib-1.2.0/authlib/integrations/base_client/sync_app.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2729 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/base_client/sync_openid.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/django_client/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      458 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_client/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3342 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_client/apps.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      650 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_client/integration.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      466 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_helpers.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/django_oauth1/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      221 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/django_oauth1/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4446 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/django_oauth1/authorization_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      420 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/django_oauth1/nonce.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2343 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_oauth1/resource_protector.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/django_oauth2/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      278 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/django_oauth2/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4526 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_oauth2/authorization_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1853 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_oauth2/endpoints.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2510 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/django_oauth2/resource_protector.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      236 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/django_oauth2/signals.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/flask_client/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1699 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/flask_client/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3631 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/flask_client/apps.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      815 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/flask_client/integration.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      758 2022-12-06 07:30:37.000000 Authlib-1.2.0/authlib/integrations/flask_helpers.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/flask_oauth1/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      260 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/flask_oauth1/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6320 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/flask_oauth1/authorization_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3020 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/flask_oauth1/cache.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3805 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/flask_oauth1/resource_protector.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/flask_oauth2/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      243 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/flask_oauth2/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5907 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/flask_oauth2/authorization_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1094 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/flask_oauth2/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3890 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/flask_oauth2/resource_protector.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      341 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/flask_oauth2/signals.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.596931 Authlib-1.2.0/authlib/integrations/httpx_client/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      804 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/httpx_client/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3210 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/httpx_client/assertion_client.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4068 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/httpx_client/oauth1_client.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     8513 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/httpx_client/oauth2_client.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      888 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/httpx_client/utils.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/integrations/requests_client/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      652 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/requests_client/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1854 2022-12-06 07:38:40.000000 Authlib-1.2.0/authlib/integrations/requests_client/assertion_session.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2233 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/requests_client/oauth1_session.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4525 2022-12-06 07:38:40.000000 Authlib-1.2.0/authlib/integrations/requests_client/oauth2_session.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      274 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/requests_client/utils.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/integrations/sqla_oauth2/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      548 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/integrations/sqla_oauth2/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4190 2022-12-06 07:30:37.000000 Authlib-1.2.0/authlib/integrations/sqla_oauth2/client_mixin.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3339 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/sqla_oauth2/functions.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2008 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/sqla_oauth2/tokens_mixins.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/integrations/starlette_client/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      677 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/starlette_client/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3328 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/starlette_client/apps.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1974 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/integrations/starlette_client/integration.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1399 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/__init__.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/drafts/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      518 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/drafts/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6925 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/drafts/_jwe_algorithms.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1860 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/drafts/_jwe_enc_cryptodome.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1743 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/drafts/_jwe_enc_cryptography.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3224 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      490 2022-12-06 08:30:04.000000 Authlib-1.2.0/authlib/jose/jwk.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/rfc7515/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      360 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/jose/rfc7515/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    11282 2022-12-06 08:19:55.000000 Authlib-1.2.0/authlib/jose/rfc7515/jws.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2483 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/jose/rfc7515/models.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/rfc7516/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      465 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7516/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    29722 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7516/jwe.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4401 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7516/models.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/rfc7517/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      424 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7517/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1257 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/jose/rfc7517/_cryptography_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6256 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7517/asymmetric_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3293 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7517/base_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2050 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7517/jwk.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      891 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7517/key_set.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/rfc7518/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      879 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3519 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/ec_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    11367 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/jwe_algs.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5081 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/jwe_encs.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      561 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/jwe_zips.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6589 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/jws_algs.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2387 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/oct_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4192 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7518/rsa_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      265 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/jose/rfc7518/util.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/rfc7519/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      333 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/jose/rfc7519/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     8423 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7519/claims.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5735 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc7519/jwt.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/jose/rfc8037/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      119 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc8037/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      716 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc8037/jws_eddsa.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3568 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/rfc8037/okp_key.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1097 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/jose/util.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/oauth1/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      752 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6574 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth1/client.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)       46 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/errors.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/oauth1/rfc5849/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1036 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    13869 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/authorization_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3857 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/base_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6950 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/client_auth.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2355 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3435 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3508 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/parameters.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1258 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/resource_protector.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      896 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/rsa.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    14159 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/signature.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      136 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/util.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3953 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth1/rfc5849/wrapper.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.606931 Authlib-1.2.0/authlib/oauth2/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      423 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3473 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/auth.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1009 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/base.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    17581 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/client.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc6749/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2322 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3756 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/authenticate_client.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    11425 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/authorization_server.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7540 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/errors.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1314 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    15352 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/authorization_code.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5054 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/base.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3924 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/client_credentials.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     9297 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/implicit.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6459 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/refresh_token.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5763 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/grants/resource_owner_password_credentials.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7526 2022-12-06 07:30:37.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     8296 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/parameters.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5305 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/resource_protector.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1111 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/token_endpoint.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1122 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/util.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2864 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6749/wrappers.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc6750/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      659 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6750/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2873 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6750/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1212 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc6750/parameters.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3358 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6750/token.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1377 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc6750/validator.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7009/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      377 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7009/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      854 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7009/parameters.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3942 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7009/revocation.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7521/
--rw-r--r--   0 lepture   (1000) lepture   (1000)       67 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7521/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2691 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7521/client.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7523/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      876 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2024 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/assertion.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3322 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/auth.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4396 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/client.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     6532 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/jwt_bearer.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3329 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/token.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1631 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7523/validator.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7591/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      667 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7591/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     9809 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7591/claims.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7704 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7591/endpoint.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1098 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7591/errors.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7592/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      315 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7592/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     9888 2022-12-06 07:30:37.000000 Authlib-1.2.0/authlib/oauth2/rfc7592/endpoint.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7636/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      364 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7636/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5126 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7636/challenge.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc7662/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      447 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7662/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5118 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7662/introspection.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      868 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc7662/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1339 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc7662/token_validator.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc8414/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      385 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc8414/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    17490 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc8414/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      745 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc8414/well_known.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc8628/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      702 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc8628/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7727 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc8628/device_code.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     7115 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc8628/endpoint.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      919 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc8628/errors.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      835 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oauth2/rfc8628/models.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oauth2/rfc8693/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      206 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oauth2/rfc8693/__init__.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oidc/
--rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/__init__.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oidc/core/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      650 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    10227 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/claims.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     2883 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/core/errors.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oidc/core/grants/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      226 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/grants/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4752 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/grants/code.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     3362 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/grants/hybrid.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     5313 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/grants/implicit.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)     4122 2022-12-06 07:30:31.000000 Authlib-1.2.0/authlib/oidc/core/grants/util.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      413 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/core/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      390 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/core/util.py
-drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2022-12-06 08:39:40.616931 Authlib-1.2.0/authlib/oidc/discovery/
--rw-r--r--   0 lepture   (1000) lepture   (1000)      321 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/discovery/__init__.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)    12611 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/discovery/models.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)      574 2022-12-06 07:30:11.000000 Authlib-1.2.0/authlib/oidc/discovery/well_known.py
--rw-r--r--   0 lepture   (1000) lepture   (1000)       90 2022-12-06 07:30:31.000000 Authlib-1.2.0/pyproject.toml
--rw-r--r--   0 lepture   (1000) lepture   (1000)     1754 2022-12-06 08:39:40.616931 Authlib-1.2.0/setup.cfg
--rw-r--r--   0 lepture   (1000) lepture   (1000)      195 2022-12-06 07:30:31.000000 Authlib-1.2.0/setup.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.826488 Authlib-1.2.1/
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/Authlib.egg-info/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3750 2023-06-25 13:03:12.000000 Authlib-1.2.1/Authlib.egg-info/PKG-INFO
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     7248 2023-06-25 13:03:12.000000 Authlib-1.2.1/Authlib.egg-info/SOURCES.txt
+-rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2023-06-25 13:03:12.000000 Authlib-1.2.1/Authlib.egg-info/dependency_links.txt
+-rw-r--r--   0 lepture   (1000) lepture   (1000)        1 2023-06-25 13:03:12.000000 Authlib-1.2.1/Authlib.egg-info/not-zip-safe
+-rw-r--r--   0 lepture   (1000) lepture   (1000)       18 2023-06-25 13:03:12.000000 Authlib-1.2.1/Authlib.egg-info/requires.txt
+-rw-r--r--   0 lepture   (1000) lepture   (1000)        8 2023-06-25 13:03:12.000000 Authlib-1.2.1/Authlib.egg-info/top_level.txt
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1514 2022-04-06 09:01:20.000000 Authlib-1.2.1/LICENSE
+-rw-r--r--   0 lepture   (1000) lepture   (1000)       48 2022-04-06 09:01:20.000000 Authlib-1.2.1/MANIFEST.in
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3750 2023-06-25 13:03:12.826488 Authlib-1.2.1/PKG-INFO
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2264 2022-12-06 07:30:31.000000 Authlib-1.2.1/README.rst
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/authlib/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      476 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/__init__.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/authlib/common/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/common/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1546 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/common/encoding.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1711 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/common/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      493 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/common/security.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4501 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/common/urls.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      312 2023-06-25 13:00:39.000000 Authlib-1.2.1/authlib/consts.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      499 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/deprecate.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/authlib/integrations/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/__init__.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/authlib/integrations/base_client/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      653 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/base_client/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5855 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/base_client/async_app.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2811 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/base_client/async_openid.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      632 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/base_client/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1879 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/base_client/framework_integration.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4281 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/base_client/registry.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    12448 2022-12-06 07:47:11.000000 Authlib-1.2.1/authlib/integrations/base_client/sync_app.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2729 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/base_client/sync_openid.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/authlib/integrations/django_client/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      458 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/django_client/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3342 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/django_client/apps.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      650 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/django_client/integration.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.766488 Authlib-1.2.1/authlib/integrations/django_oauth1/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      221 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/django_oauth1/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4566 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/integrations/django_oauth1/authorization_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      420 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/django_oauth1/nonce.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2343 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/django_oauth1/resource_protector.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/django_oauth2/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      278 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/django_oauth2/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4413 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/integrations/django_oauth2/authorization_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1853 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/django_oauth2/endpoints.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1023 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/integrations/django_oauth2/requests.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2373 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/django_oauth2/resource_protector.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      236 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/django_oauth2/signals.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/flask_client/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1699 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/flask_client/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3631 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/flask_client/apps.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      815 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/flask_client/integration.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/flask_oauth1/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      260 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/flask_oauth1/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6349 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/integrations/flask_oauth1/authorization_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3020 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/flask_oauth1/cache.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3805 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/flask_oauth1/resource_protector.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/flask_oauth2/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      243 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/flask_oauth2/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5884 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/integrations/flask_oauth2/authorization_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1094 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/flask_oauth2/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      765 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/integrations/flask_oauth2/requests.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3637 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/flask_oauth2/resource_protector.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      341 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/flask_oauth2/signals.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/httpx_client/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      804 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/httpx_client/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3226 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/httpx_client/assertion_client.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4084 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/httpx_client/oauth1_client.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     8529 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/httpx_client/oauth2_client.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      888 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/httpx_client/utils.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/requests_client/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      652 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/requests_client/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1854 2022-12-06 07:38:40.000000 Authlib-1.2.1/authlib/integrations/requests_client/assertion_session.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2233 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/requests_client/oauth1_session.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4525 2022-12-06 07:38:40.000000 Authlib-1.2.1/authlib/integrations/requests_client/oauth2_session.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      274 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/requests_client/utils.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.776488 Authlib-1.2.1/authlib/integrations/sqla_oauth2/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      548 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/integrations/sqla_oauth2/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4116 2022-12-22 06:24:27.000000 Authlib-1.2.1/authlib/integrations/sqla_oauth2/client_mixin.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3195 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/sqla_oauth2/functions.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2008 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/sqla_oauth2/tokens_mixins.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.786488 Authlib-1.2.1/authlib/integrations/starlette_client/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      677 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/starlette_client/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3564 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/integrations/starlette_client/apps.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1974 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/integrations/starlette_client/integration.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.786488 Authlib-1.2.1/authlib/jose/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1399 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/__init__.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.786488 Authlib-1.2.1/authlib/jose/drafts/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      518 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/drafts/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6925 2023-06-20 13:22:58.000000 Authlib-1.2.1/authlib/jose/drafts/_jwe_algorithms.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1860 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/drafts/_jwe_enc_cryptodome.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1743 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/drafts/_jwe_enc_cryptography.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3224 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      490 2022-12-06 08:30:04.000000 Authlib-1.2.1/authlib/jose/jwk.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.786488 Authlib-1.2.1/authlib/jose/rfc7515/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      360 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/jose/rfc7515/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    11286 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/jose/rfc7515/jws.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2483 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/jose/rfc7515/models.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.786488 Authlib-1.2.1/authlib/jose/rfc7516/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      465 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7516/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    29722 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7516/jwe.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4401 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7516/models.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.786488 Authlib-1.2.1/authlib/jose/rfc7517/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      424 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7517/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1257 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/jose/rfc7517/_cryptography_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6256 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7517/asymmetric_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3293 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7517/base_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2050 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7517/jwk.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      891 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7517/key_set.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.796488 Authlib-1.2.1/authlib/jose/rfc7518/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      879 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3519 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/ec_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    11367 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/jwe_algs.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5081 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/jwe_encs.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      561 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/jwe_zips.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6589 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/jws_algs.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2387 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/oct_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4192 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7518/rsa_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      265 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/jose/rfc7518/util.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.796488 Authlib-1.2.1/authlib/jose/rfc7519/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      333 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/jose/rfc7519/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     8423 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc7519/claims.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5735 2023-06-25 10:00:00.000000 Authlib-1.2.1/authlib/jose/rfc7519/jwt.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.796488 Authlib-1.2.1/authlib/jose/rfc8037/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      119 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc8037/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      716 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc8037/jws_eddsa.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3568 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/rfc8037/okp_key.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1097 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/jose/util.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.796488 Authlib-1.2.1/authlib/oauth1/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      752 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6574 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth1/client.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)       46 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/errors.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.796488 Authlib-1.2.1/authlib/oauth1/rfc5849/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1036 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    13869 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/authorization_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3857 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/base_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6950 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/client_auth.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2355 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3435 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/models.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3508 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/parameters.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1258 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/resource_protector.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      896 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/rsa.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    14159 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/signature.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      136 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/util.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3953 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth1/rfc5849/wrapper.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.806488 Authlib-1.2.1/authlib/oauth2/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      423 2022-12-27 07:21:16.000000 Authlib-1.2.1/authlib/oauth2/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3473 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/auth.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1009 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/base.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    17581 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/client.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.806488 Authlib-1.2.1/authlib/oauth2/rfc6749/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2347 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3756 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/authenticate_client.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    11506 2023-06-25 09:58:56.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/authorization_server.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     7540 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/errors.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.806488 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1314 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    15373 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/authorization_code.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5156 2023-06-25 09:58:56.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/base.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3892 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/client_credentials.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     9297 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/implicit.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6438 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/refresh_token.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5755 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/grants/resource_owner_password_credentials.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     7526 2022-12-06 07:30:37.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/models.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     8308 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/parameters.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2164 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/requests.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5305 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/resource_protector.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1111 2023-01-09 07:53:27.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/token_endpoint.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1122 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/util.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      705 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc6749/wrappers.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.806488 Authlib-1.2.1/authlib/oauth2/rfc6750/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      659 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6750/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2873 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6750/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1212 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc6750/parameters.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3358 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6750/token.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1377 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc6750/validator.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.806488 Authlib-1.2.1/authlib/oauth2/rfc7009/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      377 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7009/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      854 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7009/parameters.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3942 2023-01-09 07:53:27.000000 Authlib-1.2.1/authlib/oauth2/rfc7009/revocation.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc7521/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)       67 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7521/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2691 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7521/client.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc7523/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      876 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2024 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/assertion.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3354 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/auth.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4396 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/client.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     6532 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/jwt_bearer.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3329 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/token.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1631 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7523/validator.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc7591/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      667 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7591/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     9809 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7591/claims.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     8112 2023-06-25 09:59:18.000000 Authlib-1.2.1/authlib/oauth2/rfc7591/endpoint.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1098 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7591/errors.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc7592/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      315 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7592/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     9888 2022-12-06 07:30:37.000000 Authlib-1.2.1/authlib/oauth2/rfc7592/endpoint.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc7636/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      364 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7636/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5189 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oauth2/rfc7636/challenge.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc7662/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      447 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7662/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5118 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7662/introspection.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      868 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc7662/models.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1339 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc7662/token_validator.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc8414/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      385 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc8414/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    17490 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc8414/models.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      745 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc8414/well_known.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc8628/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      702 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc8628/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     7727 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc8628/device_code.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     7115 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc8628/endpoint.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      919 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc8628/errors.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      835 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oauth2/rfc8628/models.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oauth2/rfc8693/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      206 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oauth2/rfc8693/__init__.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oidc/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)        0 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/__init__.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.816488 Authlib-1.2.1/authlib/oidc/core/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      650 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oidc/core/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    10227 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oidc/core/claims.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     2883 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/core/errors.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.826488 Authlib-1.2.1/authlib/oidc/core/grants/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      226 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oidc/core/grants/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4856 2022-12-27 07:13:12.000000 Authlib-1.2.1/authlib/oidc/core/grants/code.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     3362 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oidc/core/grants/hybrid.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     5313 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oidc/core/grants/implicit.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     4122 2022-12-06 07:30:31.000000 Authlib-1.2.1/authlib/oidc/core/grants/util.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      413 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/core/models.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      390 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/core/util.py
+drwxr-xr-x   0 lepture   (1000) lepture   (1000)        0 2023-06-25 13:03:12.826488 Authlib-1.2.1/authlib/oidc/discovery/
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      321 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/discovery/__init__.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)    12611 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/discovery/models.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      574 2022-12-06 07:30:11.000000 Authlib-1.2.1/authlib/oidc/discovery/well_known.py
+-rw-r--r--   0 lepture   (1000) lepture   (1000)       90 2022-12-06 07:30:31.000000 Authlib-1.2.1/pyproject.toml
+-rw-r--r--   0 lepture   (1000) lepture   (1000)     1754 2023-06-25 13:03:12.826488 Authlib-1.2.1/setup.cfg
+-rw-r--r--   0 lepture   (1000) lepture   (1000)      195 2022-12-06 07:30:31.000000 Authlib-1.2.1/setup.py
```

### Comparing `Authlib-1.2.0/Authlib.egg-info/PKG-INFO` & `Authlib-1.2.1/Authlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Authlib
-Version: 1.2.0
+Version: 1.2.1
 Summary: The ultimate Python library in building OAuth and OpenID Connect servers and clients.
 Home-page: https://authlib.org/
 Author: Hsiaoming Yang
 Author-email: me@lepture.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://docs.authlib.org/
 Project-URL: Commercial License, https://authlib.org/plans
```

### Comparing `Authlib-1.2.0/Authlib.egg-info/SOURCES.txt` & `Authlib-1.2.1/Authlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 authlib/deprecate.py
 authlib/common/__init__.py
 authlib/common/encoding.py
 authlib/common/errors.py
 authlib/common/security.py
 authlib/common/urls.py
 authlib/integrations/__init__.py
-authlib/integrations/django_helpers.py
-authlib/integrations/flask_helpers.py
 authlib/integrations/base_client/__init__.py
 authlib/integrations/base_client/async_app.py
 authlib/integrations/base_client/async_openid.py
 authlib/integrations/base_client/errors.py
 authlib/integrations/base_client/framework_integration.py
 authlib/integrations/base_client/registry.py
 authlib/integrations/base_client/sync_app.py
@@ -35,26 +33,28 @@
 authlib/integrations/django_oauth1/__init__.py
 authlib/integrations/django_oauth1/authorization_server.py
 authlib/integrations/django_oauth1/nonce.py
 authlib/integrations/django_oauth1/resource_protector.py
 authlib/integrations/django_oauth2/__init__.py
 authlib/integrations/django_oauth2/authorization_server.py
 authlib/integrations/django_oauth2/endpoints.py
+authlib/integrations/django_oauth2/requests.py
 authlib/integrations/django_oauth2/resource_protector.py
 authlib/integrations/django_oauth2/signals.py
 authlib/integrations/flask_client/__init__.py
 authlib/integrations/flask_client/apps.py
 authlib/integrations/flask_client/integration.py
 authlib/integrations/flask_oauth1/__init__.py
 authlib/integrations/flask_oauth1/authorization_server.py
 authlib/integrations/flask_oauth1/cache.py
 authlib/integrations/flask_oauth1/resource_protector.py
 authlib/integrations/flask_oauth2/__init__.py
 authlib/integrations/flask_oauth2/authorization_server.py
 authlib/integrations/flask_oauth2/errors.py
+authlib/integrations/flask_oauth2/requests.py
 authlib/integrations/flask_oauth2/resource_protector.py
 authlib/integrations/flask_oauth2/signals.py
 authlib/integrations/httpx_client/__init__.py
 authlib/integrations/httpx_client/assertion_client.py
 authlib/integrations/httpx_client/oauth1_client.py
 authlib/integrations/httpx_client/oauth2_client.py
 authlib/integrations/httpx_client/utils.py
@@ -126,14 +126,15 @@
 authlib/oauth2/client.py
 authlib/oauth2/rfc6749/__init__.py
 authlib/oauth2/rfc6749/authenticate_client.py
 authlib/oauth2/rfc6749/authorization_server.py
 authlib/oauth2/rfc6749/errors.py
 authlib/oauth2/rfc6749/models.py
 authlib/oauth2/rfc6749/parameters.py
+authlib/oauth2/rfc6749/requests.py
 authlib/oauth2/rfc6749/resource_protector.py
 authlib/oauth2/rfc6749/token_endpoint.py
 authlib/oauth2/rfc6749/util.py
 authlib/oauth2/rfc6749/wrappers.py
 authlib/oauth2/rfc6749/grants/__init__.py
 authlib/oauth2/rfc6749/grants/authorization_code.py
 authlib/oauth2/rfc6749/grants/base.py
```

### Comparing `Authlib-1.2.0/LICENSE` & `Authlib-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/PKG-INFO` & `Authlib-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Authlib
-Version: 1.2.0
+Version: 1.2.1
 Summary: The ultimate Python library in building OAuth and OpenID Connect servers and clients.
 Home-page: https://authlib.org/
 Author: Hsiaoming Yang
 Author-email: me@lepture.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://docs.authlib.org/
 Project-URL: Commercial License, https://authlib.org/plans
```

### Comparing `Authlib-1.2.0/README.rst` & `Authlib-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/common/encoding.py` & `Authlib-1.2.1/authlib/common/encoding.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/common/errors.py` & `Authlib-1.2.1/authlib/common/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/common/urls.py` & `Authlib-1.2.1/authlib/common/urls.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/__init__.py` & `Authlib-1.2.1/authlib/integrations/base_client/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/async_app.py` & `Authlib-1.2.1/authlib/integrations/base_client/async_app.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/async_openid.py` & `Authlib-1.2.1/authlib/integrations/base_client/async_openid.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/errors.py` & `Authlib-1.2.1/authlib/integrations/base_client/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/framework_integration.py` & `Authlib-1.2.1/authlib/integrations/base_client/framework_integration.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/registry.py` & `Authlib-1.2.1/authlib/integrations/base_client/registry.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/sync_app.py` & `Authlib-1.2.1/authlib/integrations/base_client/sync_app.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/base_client/sync_openid.py` & `Authlib-1.2.1/authlib/integrations/base_client/sync_openid.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/django_client/apps.py` & `Authlib-1.2.1/authlib/integrations/django_client/apps.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/django_client/integration.py` & `Authlib-1.2.1/authlib/integrations/django_client/integration.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/django_oauth1/authorization_server.py` & `Authlib-1.2.1/authlib/integrations/django_oauth1/authorization_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from authlib.oauth1 import TemporaryCredential
 from authlib.common.security import generate_token
 from authlib.common.urls import url_encode
 from django.core.cache import cache
 from django.conf import settings
 from django.http import HttpResponse
 from .nonce import exists_nonce_in_cache
-from ..django_helpers import create_oauth_request
 
 log = logging.getLogger(__name__)
 
 
 class BaseServer(_AuthorizationServer):
     def __init__(self, client_model, token_model, token_generator=None):
         self.client_model = client_model
@@ -57,15 +56,20 @@
 
     def check_authorization_request(self, request):
         req = self.create_oauth1_request(request)
         self.validate_authorization_request(req)
         return req
 
     def create_oauth1_request(self, request):
-        return create_oauth_request(request, OAuth1Request)
+        if request.method == 'POST':
+            body = request.POST.dict()
+        else:
+            body = None
+        url = request.build_absolute_uri()
+        return OAuth1Request(request.method, url, body, request.headers)
 
     def handle_response(self, status_code, payload, headers):
         resp = HttpResponse(url_encode(payload), status=status_code)
         for k, v in headers:
             resp[k] = v
         return resp
```

### Comparing `Authlib-1.2.0/authlib/integrations/django_oauth1/resource_protector.py` & `Authlib-1.2.1/authlib/integrations/django_oauth1/resource_protector.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/django_oauth2/authorization_server.py` & `Authlib-1.2.1/authlib/integrations/django_oauth2/authorization_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from django.http import HttpResponse
 from django.utils.module_loading import import_string
 from django.conf import settings
 from authlib.oauth2 import (
-    OAuth2Request,
-    HttpRequest,
     AuthorizationServer as _AuthorizationServer,
 )
 from authlib.oauth2.rfc6750 import BearerTokenGenerator
 from authlib.common.security import generate_token as _generate_token
 from authlib.common.encoding import json_dumps
+from .requests import DjangoOAuth2Request, DjangoJsonRequest
 from .signals import client_authenticated, token_revoked
-from ..django_helpers import create_oauth_request
 
 
 class AuthorizationServer(_AuthorizationServer):
     """Django implementation of :class:`authlib.oauth2.rfc6749.AuthorizationServer`.
     Initialize it with client model and token model::
 
         from authlib.integrations.django_oauth2 import AuthorizationServer
@@ -55,20 +53,18 @@
             user_id=user_id,
             **token
         )
         item.save()
         return item
 
     def create_oauth2_request(self, request):
-        return create_oauth_request(request, OAuth2Request)
+        return DjangoOAuth2Request(request)
 
     def create_json_request(self, request):
-        req = create_oauth_request(request, HttpRequest, True)
-        req.user = request.user
-        return req
+        return DjangoJsonRequest(request)
 
     def handle_response(self, status_code, payload, headers):
         if isinstance(payload, dict):
             payload = json_dumps(payload)
         resp = HttpResponse(payload, status=status_code)
         for k, v in headers:
             resp[k] = v
```

### Comparing `Authlib-1.2.0/authlib/integrations/django_oauth2/endpoints.py` & `Authlib-1.2.1/authlib/integrations/django_oauth2/endpoints.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/django_oauth2/resource_protector.py` & `Authlib-1.2.1/authlib/integrations/django_oauth2/resource_protector.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 from django.http import JsonResponse
 from authlib.oauth2 import (
     OAuth2Error,
     ResourceProtector as _ResourceProtector,
 )
 from authlib.oauth2.rfc6749 import (
     MissingAuthorizationError,
-    HttpRequest,
 )
 from authlib.oauth2.rfc6750 import (
     BearerTokenValidator as _BearerTokenValidator
 )
+from .requests import DjangoJsonRequest
 from .signals import token_authenticated
 
 
 class ResourceProtector(_ResourceProtector):
     def acquire_token(self, request, scopes=None):
         """A method to acquire current valid token with the given scope.
 
         :param request: Django HTTP request instance
         :param scopes: a list of scope values
         :return: token object
         """
-        url = request.build_absolute_uri()
-        req = HttpRequest(request.method, url, None, request.headers)
-        req.req = request
+        req = DjangoJsonRequest(request)
         if isinstance(scopes, str):
             scopes = [scopes]
         token = self.validate_request(scopes, req)
         token_authenticated.send(sender=self.__class__, token=token)
         return token
 
     def __call__(self, scopes=None, optional=False):
@@ -57,17 +55,14 @@
 
     def authenticate_token(self, token_string):
         try:
             return self.token_model.objects.get(access_token=token_string)
         except self.token_model.DoesNotExist:
             return None
 
-    def request_invalid(self, request):
-        return False
-
 
 def return_error_response(error):
     body = dict(error.get_body())
     resp = JsonResponse(body, status=error.status_code)
     headers = error.get_headers()
     for k, v in headers:
         resp[k] = v
```

### Comparing `Authlib-1.2.0/authlib/integrations/flask_client/__init__.py` & `Authlib-1.2.1/authlib/integrations/flask_client/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/flask_client/apps.py` & `Authlib-1.2.1/authlib/integrations/flask_client/apps.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/flask_client/integration.py` & `Authlib-1.2.1/authlib/integrations/flask_client/integration.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/flask_oauth1/authorization_server.py` & `Authlib-1.2.1/authlib/integrations/flask_oauth1/authorization_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from werkzeug.utils import import_string
 from flask import Response
+from flask import request as flask_req
 from authlib.oauth1 import (
     OAuth1Request,
     AuthorizationServer as _AuthorizationServer,
 )
 from authlib.common.security import generate_token
 from authlib.common.urls import url_encode
-from ..flask_helpers import create_oauth_request
 
 log = logging.getLogger(__name__)
 
 
 class AuthorizationServer(_AuthorizationServer):
     """Flask implementation of :class:`authlib.rfc5849.AuthorizationServer`.
     Initialize it with Flask app instance, client model class and cache::
@@ -149,32 +149,34 @@
             token = self.token_generator()
             return func(token, temporary_credential)
 
         raise RuntimeError(
             '"create_token_credential" hook is required.'
         )
 
-    def create_temporary_credentials_response(self, request=None):
-        return super(AuthorizationServer, self)\
-            .create_temporary_credentials_response(request)
-
     def check_authorization_request(self):
         req = self.create_oauth1_request(None)
         self.validate_authorization_request(req)
         return req
 
     def create_authorization_response(self, request=None, grant_user=None):
         return super(AuthorizationServer, self)\
             .create_authorization_response(request, grant_user)
 
     def create_token_response(self, request=None):
         return super(AuthorizationServer, self).create_token_response(request)
 
     def create_oauth1_request(self, request):
-        return create_oauth_request(request, OAuth1Request)
+        if request is None:
+            request = flask_req
+        if request.method in ('POST', 'PUT'):
+            body = request.form.to_dict(flat=True)
+        else:
+            body = None
+        return OAuth1Request(request.method, request.url, body, request.headers)
 
     def handle_response(self, status_code, payload, headers):
         return Response(
             url_encode(payload),
             status=status_code,
             headers=headers
         )
```

### Comparing `Authlib-1.2.0/authlib/integrations/flask_oauth1/cache.py` & `Authlib-1.2.1/authlib/integrations/flask_oauth1/cache.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/flask_oauth1/resource_protector.py` & `Authlib-1.2.1/authlib/integrations/flask_oauth1/resource_protector.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/flask_oauth2/authorization_server.py` & `Authlib-1.2.1/authlib/integrations/flask_oauth2/authorization_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from werkzeug.utils import import_string
 from flask import Response, json
+from flask import request as flask_req
 from authlib.oauth2 import (
-    OAuth2Request,
-    HttpRequest,
     AuthorizationServer as _AuthorizationServer,
 )
 from authlib.oauth2.rfc6750 import BearerTokenGenerator
 from authlib.common.security import generate_token
+from .requests import FlaskOAuth2Request, FlaskJsonRequest
 from .signals import client_authenticated, token_revoked
-from ..flask_helpers import create_oauth_request
 
 
 class AuthorizationServer(_AuthorizationServer):
     """Flask implementation of :class:`authlib.oauth2.rfc6749.AuthorizationServer`.
     Initialize it with ``query_client``, ``save_token`` methods and Flask
     app instance::
 
@@ -66,18 +65,18 @@
 
     def get_error_uri(self, request, error):
         if self._error_uris:
             uris = dict(self._error_uris)
             return uris.get(error.error)
 
     def create_oauth2_request(self, request):
-        return create_oauth_request(request, OAuth2Request)
+        return FlaskOAuth2Request(flask_req)
 
     def create_json_request(self, request):
-        return create_oauth_request(request, HttpRequest, True)
+        return FlaskJsonRequest(flask_req)
 
     def handle_response(self, status_code, payload, headers):
         if isinstance(payload, dict):
             payload = json.dumps(payload)
         return Response(payload, status=status_code, headers=headers)
 
     def send_signal(self, name, *args, **kwargs):
```

### Comparing `Authlib-1.2.0/authlib/integrations/flask_oauth2/errors.py` & `Authlib-1.2.1/authlib/integrations/flask_oauth2/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/flask_oauth2/resource_protector.py` & `Authlib-1.2.1/authlib/integrations/flask_oauth2/resource_protector.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from werkzeug.local import LocalProxy
 from authlib.oauth2 import (
     OAuth2Error,
     ResourceProtector as _ResourceProtector
 )
 from authlib.oauth2.rfc6749 import (
     MissingAuthorizationError,
-    HttpRequest,
 )
+from .requests import FlaskJsonRequest
 from .signals import token_authenticated
 from .errors import raise_http_exception
 
 
 class ResourceProtector(_ResourceProtector):
     """A protecting method for resource servers. Creating a ``require_oauth``
     decorator easily with ResourceProtector::
@@ -27,20 +27,14 @@
         from authlib.oauth2.rfc6750 import BearerTokenValidator
         from project.models import Token
 
         class MyBearerTokenValidator(BearerTokenValidator):
             def authenticate_token(self, token_string):
                 return Token.query.filter_by(access_token=token_string).first()
 
-            def request_invalid(self, request):
-                return False
-
-            def token_revoked(self, token):
-                return False
-
         require_oauth.register_token_validator(MyBearerTokenValidator())
 
         # protect resource with require_oauth
 
         @app.route('/user')
         @require_oauth(['profile'])
         def user_profile():
@@ -62,21 +56,15 @@
 
     def acquire_token(self, scopes=None):
         """A method to acquire current valid token with the given scope.
 
         :param scopes: a list of scope values
         :return: token object
         """
-        request = HttpRequest(
-            _req.method,
-            _req.full_path,
-            None,
-            _req.headers
-        )
-        request.req = _req
+        request = FlaskJsonRequest(_req)
         # backward compatible
         if isinstance(scopes, str):
             scopes = [scopes]
         token = self.validate_request(scopes, request)
         token_authenticated.send(self, token=token)
         g.authlib_server_oauth2_token = token
         return token
```

### Comparing `Authlib-1.2.0/authlib/integrations/httpx_client/__init__.py` & `Authlib-1.2.1/authlib/integrations/httpx_client/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/httpx_client/assertion_client.py` & `Authlib-1.2.1/authlib/integrations/httpx_client/assertion_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-from httpx import AsyncClient, Client, Response, USE_CLIENT_DEFAULT
+import httpx
+from httpx import Response, USE_CLIENT_DEFAULT
 from authlib.oauth2.rfc7521 import AssertionClient as _AssertionClient
 from authlib.oauth2.rfc7523 import JWTBearerGrant
 from .utils import extract_client_kwargs
 from .oauth2_client import OAuth2Auth
 from ..base_client import OAuthError
 
 __all__ = ['AsyncAssertionClient']
 
 
-class AsyncAssertionClient(_AssertionClient, AsyncClient):
+class AsyncAssertionClient(_AssertionClient, httpx.AsyncClient):
     token_auth_class = OAuth2Auth
     oauth_error_class = OAuthError
     JWT_BEARER_GRANT_TYPE = JWTBearerGrant.GRANT_TYPE
     ASSERTION_METHODS = {
         JWT_BEARER_GRANT_TYPE: JWTBearerGrant.sign,
     }
     DEFAULT_GRANT_TYPE = JWT_BEARER_GRANT_TYPE
 
     def __init__(self, token_endpoint, issuer, subject, audience=None, grant_type=None,
                  claims=None, token_placement='header', scope=None, **kwargs):
 
         client_kwargs = extract_client_kwargs(kwargs)
-        AsyncClient.__init__(self, **client_kwargs)
+        httpx.AsyncClient.__init__(self, **client_kwargs)
 
         _AssertionClient.__init__(
             self, session=None,
             token_endpoint=token_endpoint, issuer=issuer, subject=subject,
             audience=audience, grant_type=grant_type, claims=claims,
             token_placement=token_placement, scope=scope, **kwargs
         )
@@ -43,28 +44,28 @@
     async def _refresh_token(self, data):
         resp = await self.request(
             'POST', self.token_endpoint, data=data, withhold_token=True)
 
         return self.parse_response_token(resp)
 
 
-class AssertionClient(_AssertionClient, Client):
+class AssertionClient(_AssertionClient, httpx.Client):
     token_auth_class = OAuth2Auth
     oauth_error_class = OAuthError
     JWT_BEARER_GRANT_TYPE = JWTBearerGrant.GRANT_TYPE
     ASSERTION_METHODS = {
         JWT_BEARER_GRANT_TYPE: JWTBearerGrant.sign,
     }
     DEFAULT_GRANT_TYPE = JWT_BEARER_GRANT_TYPE
 
     def __init__(self, token_endpoint, issuer, subject, audience=None, grant_type=None,
                  claims=None, token_placement='header', scope=None, **kwargs):
 
         client_kwargs = extract_client_kwargs(kwargs)
-        Client.__init__(self, **client_kwargs)
+        httpx.Client.__init__(self, **client_kwargs)
 
         _AssertionClient.__init__(
             self, session=self,
             token_endpoint=token_endpoint, issuer=issuer, subject=subject,
             audience=audience, grant_type=grant_type, claims=claims,
             token_placement=token_placement, scope=scope, **kwargs
         )
```

### Comparing `Authlib-1.2.0/authlib/integrations/httpx_client/oauth1_client.py` & `Authlib-1.2.1/authlib/integrations/httpx_client/oauth1_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing
-from httpx import AsyncClient, Auth, Client, Request, Response
+import httpx
+from httpx import Auth, Request, Response
 from authlib.oauth1 import (
     SIGNATURE_HMAC_SHA1,
     SIGNATURE_TYPE_HEADER,
 )
 from authlib.common.encoding import to_unicode
 from authlib.oauth1 import ClientAuth
 from authlib.oauth1.client import OAuth1Client as _OAuth1Client
@@ -18,26 +19,26 @@
     def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
         url, headers, body = self.prepare(
             request.method, str(request.url), request.headers, request.content)
         headers['Content-Length'] = str(len(body))
         yield build_request(url=url, headers=headers, body=body, initial_request=request)
 
 
-class AsyncOAuth1Client(_OAuth1Client, AsyncClient):
+class AsyncOAuth1Client(_OAuth1Client, httpx.AsyncClient):
     auth_class = OAuth1Auth
 
     def __init__(self, client_id, client_secret=None,
                  token=None, token_secret=None,
                  redirect_uri=None, rsa_key=None, verifier=None,
                  signature_method=SIGNATURE_HMAC_SHA1,
                  signature_type=SIGNATURE_TYPE_HEADER,
                  force_include_body=False, **kwargs):
 
         _client_kwargs = extract_client_kwargs(kwargs)
-        AsyncClient.__init__(self, **_client_kwargs)
+        httpx.AsyncClient.__init__(self, **_client_kwargs)
 
         _OAuth1Client.__init__(
             self, None,
             client_id=client_id, client_secret=client_secret,
             token=token, token_secret=token_secret,
             redirect_uri=redirect_uri, rsa_key=rsa_key, verifier=verifier,
             signature_method=signature_method, signature_type=signature_type,
@@ -71,26 +72,26 @@
         return token
 
     @staticmethod
     def handle_error(error_type, error_description):
         raise OAuthError(error_type, error_description)
 
 
-class OAuth1Client(_OAuth1Client, Client):
+class OAuth1Client(_OAuth1Client, httpx.Client):
     auth_class = OAuth1Auth
 
     def __init__(self, client_id, client_secret=None,
                  token=None, token_secret=None,
                  redirect_uri=None, rsa_key=None, verifier=None,
                  signature_method=SIGNATURE_HMAC_SHA1,
                  signature_type=SIGNATURE_TYPE_HEADER,
                  force_include_body=False, **kwargs):
 
         _client_kwargs = extract_client_kwargs(kwargs)
-        Client.__init__(self, **_client_kwargs)
+        httpx.Client.__init__(self, **_client_kwargs)
 
         _OAuth1Client.__init__(
             self, self,
             client_id=client_id, client_secret=client_secret,
             token=token, token_secret=token_secret,
             redirect_uri=redirect_uri, rsa_key=rsa_key, verifier=verifier,
             signature_method=signature_method, signature_type=signature_type,
```

### Comparing `Authlib-1.2.0/authlib/integrations/httpx_client/oauth2_client.py` & `Authlib-1.2.1/authlib/integrations/httpx_client/oauth2_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing
 from contextlib import asynccontextmanager
 
-from httpx import AsyncClient, Auth, Client, Request, Response, USE_CLIENT_DEFAULT
+import httpx
+from httpx import Auth, Request, Response, USE_CLIENT_DEFAULT
 from anyio import Lock  # Import after httpx so import errors refer to httpx
 from authlib.common.urls import url_decode
 from authlib.oauth2.client import OAuth2Client as _OAuth2Client
 from authlib.oauth2.auth import ClientAuth, TokenAuth
 from .utils import HTTPX_CLIENT_KWARGS, build_request
 from ..base_client import (
     OAuthError,
@@ -41,15 +42,15 @@
     def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
         url, headers, body = self.prepare(
             request.method, str(request.url), request.headers, request.content)
         headers['Content-Length'] = str(len(body))
         yield build_request(url=url, headers=headers, body=body, initial_request=request)
 
 
-class AsyncOAuth2Client(_OAuth2Client, AsyncClient):
+class AsyncOAuth2Client(_OAuth2Client, httpx.AsyncClient):
     SESSION_REQUEST_PARAMS = HTTPX_CLIENT_KWARGS
 
     client_auth_class = OAuth2ClientAuth
     token_auth_class = OAuth2Auth
     oauth_error_class = OAuthError
 
     def __init__(self, client_id=None, client_secret=None,
@@ -57,15 +58,15 @@
                  revocation_endpoint_auth_method=None,
                  scope=None, redirect_uri=None,
                  token=None, token_placement='header',
                  update_token=None, **kwargs):
 
         # extract httpx.Client kwargs
         client_kwargs = self._extract_session_request_params(kwargs)
-        AsyncClient.__init__(self, **client_kwargs)
+        httpx.AsyncClient.__init__(self, **client_kwargs)
 
         # We use a Lock to synchronize coroutines to prevent
         # multiple concurrent attempts to refresh the same token
         self._token_refresh_lock = Lock()
 
         _OAuth2Client.__init__(
             self, session=None,
@@ -156,15 +157,15 @@
 
     def _http_post(self, url, body=None, auth=USE_CLIENT_DEFAULT, headers=None, **kwargs):
         return self.post(
             url, data=dict(url_decode(body)),
             headers=headers, auth=auth, **kwargs)
 
 
-class OAuth2Client(_OAuth2Client, Client):
+class OAuth2Client(_OAuth2Client, httpx.Client):
     SESSION_REQUEST_PARAMS = HTTPX_CLIENT_KWARGS
 
     client_auth_class = OAuth2ClientAuth
     token_auth_class = OAuth2Auth
     oauth_error_class = OAuthError
 
     def __init__(self, client_id=None, client_secret=None,
@@ -172,15 +173,15 @@
                  revocation_endpoint_auth_method=None,
                  scope=None, redirect_uri=None,
                  token=None, token_placement='header',
                  update_token=None, **kwargs):
 
         # extract httpx.Client kwargs
         client_kwargs = self._extract_session_request_params(kwargs)
-        Client.__init__(self, **client_kwargs)
+        httpx.Client.__init__(self, **client_kwargs)
 
         _OAuth2Client.__init__(
             self, session=self,
             client_id=client_id, client_secret=client_secret,
             token_endpoint_auth_method=token_endpoint_auth_method,
             revocation_endpoint_auth_method=revocation_endpoint_auth_method,
             scope=scope, redirect_uri=redirect_uri,
```

### Comparing `Authlib-1.2.0/authlib/integrations/httpx_client/utils.py` & `Authlib-1.2.1/authlib/integrations/httpx_client/utils.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/requests_client/__init__.py` & `Authlib-1.2.1/authlib/integrations/requests_client/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/requests_client/assertion_session.py` & `Authlib-1.2.1/authlib/integrations/requests_client/assertion_session.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/requests_client/oauth1_session.py` & `Authlib-1.2.1/authlib/integrations/requests_client/oauth1_session.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/requests_client/oauth2_session.py` & `Authlib-1.2.1/authlib/integrations/requests_client/oauth2_session.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/sqla_oauth2/__init__.py` & `Authlib-1.2.1/authlib/integrations/sqla_oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/sqla_oauth2/client_mixin.py` & `Authlib-1.2.1/authlib/integrations/sqla_oauth2/client_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,17 +118,14 @@
         allowed = set(self.scope.split())
         scopes = scope_to_list(scope)
         return list_to_scope([s for s in scopes if s in allowed])
 
     def check_redirect_uri(self, redirect_uri):
         return redirect_uri in self.redirect_uris
 
-    def has_client_secret(self):
-        return bool(self.client_secret)
-
     def check_client_secret(self, client_secret):
         return secrets.compare_digest(self.client_secret, client_secret)
 
     def check_endpoint_auth_method(self, method, endpoint):
         if endpoint == 'token':
             return self.token_endpoint_auth_method == method
         # TODO
```

### Comparing `Authlib-1.2.0/authlib/integrations/sqla_oauth2/functions.py` & `Authlib-1.2.1/authlib/integrations/sqla_oauth2/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,8 @@
     from authlib.oauth2.rfc6750 import BearerTokenValidator
 
     class _BearerTokenValidator(BearerTokenValidator):
         def authenticate_token(self, token_string):
             q = session.query(token_model)
             return q.filter_by(access_token=token_string).first()
 
-        def request_invalid(self, request):
-            return False
-
-        def token_revoked(self, token):
-            return token.revoked
-
     return _BearerTokenValidator
```

### Comparing `Authlib-1.2.0/authlib/integrations/sqla_oauth2/tokens_mixins.py` & `Authlib-1.2.1/authlib/integrations/sqla_oauth2/tokens_mixins.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/starlette_client/__init__.py` & `Authlib-1.2.1/authlib/integrations/starlette_client/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/integrations/starlette_client/apps.py` & `Authlib-1.2.1/authlib/integrations/starlette_client/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from starlette.datastructures import URL
 from starlette.responses import RedirectResponse
 from ..base_client import OAuthError
 from ..base_client import BaseApp
 from ..base_client.async_app import AsyncOAuth1Mixin, AsyncOAuth2Mixin
 from ..base_client.async_openid import AsyncOpenIDMixin
 from ..httpx_client import AsyncOAuth1Client, AsyncOAuth2Client
 
@@ -22,14 +23,18 @@
         """Create a HTTP Redirect for Authorization Endpoint.
 
         :param request: HTTP request instance from Starlette view.
         :param redirect_uri: Callback or redirect URI for authorization.
         :param kwargs: Extra parameters to include.
         :return: A HTTP redirect response.
         """
+
+        # Handle Starlette >= 0.26.0 where redirect_uri may now be a URL and not a string
+        if redirect_uri and isinstance(redirect_uri, URL):
+            redirect_uri = str(redirect_uri)
         rv = await self.create_authorization_url(redirect_uri, **kwargs)
         await self.save_authorize_data(request, redirect_uri=redirect_uri, **rv)
         return RedirectResponse(rv['url'], status_code=302)
 
 
 class StarletteOAuth1App(StarletteAppMixin, AsyncOAuth1Mixin, BaseApp):
     client_cls = AsyncOAuth1Client
```

### Comparing `Authlib-1.2.0/authlib/integrations/starlette_client/integration.py` & `Authlib-1.2.1/authlib/integrations/starlette_client/integration.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/__init__.py` & `Authlib-1.2.1/authlib/jose/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/drafts/__init__.py` & `Authlib-1.2.1/authlib/jose/drafts/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/drafts/_jwe_algorithms.py` & `Authlib-1.2.1/authlib/jose/drafts/_jwe_algorithms.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/drafts/_jwe_enc_cryptodome.py` & `Authlib-1.2.1/authlib/jose/drafts/_jwe_enc_cryptodome.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/drafts/_jwe_enc_cryptography.py` & `Authlib-1.2.1/authlib/jose/drafts/_jwe_enc_cryptography.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/errors.py` & `Authlib-1.2.1/authlib/jose/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7515/jws.py` & `Authlib-1.2.1/authlib/jose/rfc7515/jws.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         :raise: BadSignatureError
 
         .. _`Section 7.2`: https://tools.ietf.org/html/rfc7515#section-7.2
         """
         obj = ensure_dict(obj, 'JWS')
 
         payload_segment = obj.get('payload')
-        if not payload_segment:
+        if payload_segment is None:
             raise DecodeError('Missing "payload" value')
 
         payload_segment = to_bytes(payload_segment)
         payload = _extract_payload(payload_segment)
         if decode:
             payload = decode(payload)
```

### Comparing `Authlib-1.2.0/authlib/jose/rfc7515/models.py` & `Authlib-1.2.1/authlib/jose/rfc7515/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7516/jwe.py` & `Authlib-1.2.1/authlib/jose/rfc7516/jwe.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7516/models.py` & `Authlib-1.2.1/authlib/jose/rfc7516/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7517/_cryptography_key.py` & `Authlib-1.2.1/authlib/jose/rfc7517/_cryptography_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7517/asymmetric_key.py` & `Authlib-1.2.1/authlib/jose/rfc7517/asymmetric_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7517/base_key.py` & `Authlib-1.2.1/authlib/jose/rfc7517/base_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7517/jwk.py` & `Authlib-1.2.1/authlib/jose/rfc7517/jwk.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7517/key_set.py` & `Authlib-1.2.1/authlib/jose/rfc7517/key_set.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/__init__.py` & `Authlib-1.2.1/authlib/jose/rfc7518/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/ec_key.py` & `Authlib-1.2.1/authlib/jose/rfc7518/ec_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/jwe_algs.py` & `Authlib-1.2.1/authlib/jose/rfc7518/jwe_algs.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/jwe_encs.py` & `Authlib-1.2.1/authlib/jose/rfc7518/jwe_encs.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/jwe_zips.py` & `Authlib-1.2.1/authlib/jose/rfc7518/jwe_zips.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/jws_algs.py` & `Authlib-1.2.1/authlib/jose/rfc7518/jws_algs.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/oct_key.py` & `Authlib-1.2.1/authlib/jose/rfc7518/oct_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7518/rsa_key.py` & `Authlib-1.2.1/authlib/jose/rfc7518/rsa_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7519/claims.py` & `Authlib-1.2.1/authlib/jose/rfc7519/claims.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc7519/jwt.py` & `Authlib-1.2.1/authlib/jose/rfc7519/jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if 'enc' in header:
             return self._jwe.serialize_compact(header, text, key)
         else:
             return self._jws.serialize_compact(header, text, key)
 
     def decode(self, s, key, claims_cls=None,
                claims_options=None, claims_params=None):
-        """Decode the JWS with the given key. This is similar with
+        """Decode the JWT with the given key. This is similar with
         :meth:`verify`, except that it will raise BadSignatureError when
         signature doesn't match.
 
         :param s: text of JWT
         :param key: key used to verify the signature
         :param claims_cls: class to be used for JWT claims
         :param claims_options: `options` parameters for claims_cls
```

### Comparing `Authlib-1.2.0/authlib/jose/rfc8037/jws_eddsa.py` & `Authlib-1.2.1/authlib/jose/rfc8037/jws_eddsa.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/rfc8037/okp_key.py` & `Authlib-1.2.1/authlib/jose/rfc8037/okp_key.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/jose/util.py` & `Authlib-1.2.1/authlib/jose/util.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/__init__.py` & `Authlib-1.2.1/authlib/oauth1/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/client.py` & `Authlib-1.2.1/authlib/oauth1/client.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/__init__.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/authorization_server.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/authorization_server.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/base_server.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/base_server.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/client_auth.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/client_auth.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/errors.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/models.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/parameters.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/parameters.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/resource_protector.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/resource_protector.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/rsa.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/rsa.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/signature.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/signature.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth1/rfc5849/wrapper.py` & `Authlib-1.2.1/authlib/oauth1/rfc5849/wrapper.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/auth.py` & `Authlib-1.2.1/authlib/oauth2/auth.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/base.py` & `Authlib-1.2.1/authlib/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/client.py` & `Authlib-1.2.1/authlib/oauth2/client.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/__init__.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
     This module represents a direct implementation of
     The OAuth 2.0 Authorization Framework.
 
     https://tools.ietf.org/html/rfc6749
 """
 
-from .wrappers import OAuth2Request, OAuth2Token, HttpRequest
+from .requests import OAuth2Request, JsonRequest
+from .wrappers import OAuth2Token
 from .errors import (
     OAuth2Error,
     AccessDeniedError,
     MissingAuthorizationError,
     InvalidGrantError,
     InvalidClientError,
     InvalidRequestError,
@@ -43,15 +44,16 @@
     ResourceOwnerPasswordCredentialsGrant,
     ClientCredentialsGrant,
     RefreshTokenGrant,
 )
 from .util import scope_to_list, list_to_scope
 
 __all__ = [
-    'OAuth2Request', 'OAuth2Token', 'HttpRequest',
+    'OAuth2Token',
+    'OAuth2Request', 'JsonRequest',
     'OAuth2Error',
     'AccessDeniedError',
     'MissingAuthorizationError',
     'InvalidGrantError',
     'InvalidClientError',
     'InvalidRequestError',
     'InvalidScopeError',
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/authenticate_client.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/authenticate_client.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/authorization_server.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/authorization_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .authenticate_client import ClientAuthentication
+from .requests import OAuth2Request, JsonRequest
 from .errors import (
     OAuth2Error,
     InvalidScopeError,
     UnsupportedResponseTypeError,
     UnsupportedGrantTypeError,
 )
 from .util import scope_to_list
@@ -123,24 +124,24 @@
 
     def send_signal(self, name, *args, **kwargs):
         """Framework integration can re-implement this method to support
         signal system.
         """
         raise NotImplementedError()
 
-    def create_oauth2_request(self, request):
+    def create_oauth2_request(self, request) -> OAuth2Request:
         """This method MUST be implemented in framework integrations. It is
         used to create an OAuth2Request instance.
 
         :param request: the "request" instance in framework
         :return: OAuth2Request instance
         """
         raise NotImplementedError()
 
-    def create_json_request(self, request):
+    def create_json_request(self, request) -> JsonRequest:
         """This method MUST be implemented in framework integrations. It is
         used to create an HttpRequest instance.
 
         :param request: the "request" instance in framework
         :return: HttpRequest instance
         """
         raise NotImplementedError()
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/errors.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/__init__.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/authorization_code.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/authorization_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         an authorization decision (by asking the resource owner or by
         establishing approval via other means).
 
         .. _`Section 4.1.1`: https://tools.ietf.org/html/rfc6749#section-4.1.1
         """
         return validate_code_authorization_request(self)
 
-    def create_authorization_response(self, redirect_uri, grant_user):
+    def create_authorization_response(self, redirect_uri: str, grant_user):
         """If the resource owner grants the access request, the authorization
         server issues an authorization code and delivers it to the client by
         adding the following parameters to the query component of the
         redirection URI using the "application/x-www-form-urlencoded" format.
         Per `Section 4.1.2`_.
 
         code
@@ -228,15 +228,15 @@
         redirect_uri = self.request.redirect_uri
         original_redirect_uri = authorization_code.get_redirect_uri()
         if original_redirect_uri and redirect_uri != original_redirect_uri:
             raise InvalidGrantError('Invalid "redirect_uri" in request.')
 
         # save for create_token_response
         self.request.client = client
-        self.request.credential = authorization_code
+        self.request.authorization_code = authorization_code
         self.execute_hook('after_validate_token_request')
 
     def create_token_response(self):
         """If the access token request is valid and authorized, the
         authorization server issues an access token and optional refresh
         token as described in Section 5.1.  If the request client
         authentication failed or is invalid, the authorization server returns
@@ -260,15 +260,15 @@
             }
 
         :returns: (status_code, body, headers)
 
         .. _`Section 4.1.4`: https://tools.ietf.org/html/rfc6749#section-4.1.4
         """
         client = self.request.client
-        authorization_code = self.request.credential
+        authorization_code = self.request.authorization_code
 
         user = self.authenticate_user(authorization_code)
         if not user:
             raise InvalidGrantError('There is no "user" for this code.')
         self.request.user = user
 
         scope = authorization_code.get_scope()
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/base.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from authlib.consts import default_json_headers
+from ..requests import OAuth2Request
 from ..errors import InvalidRequestError
 
 
 class BaseGrant(object):
     #: Allowed client auth methods for token endpoint
     TOKEN_ENDPOINT_AUTH_METHODS = ['client_secret_basic']
 
@@ -11,15 +12,15 @@
 
     # NOTE: there is no charset for application/json, since
     # application/json should always in UTF-8.
     # The example on RFC is incorrect.
     # https://tools.ietf.org/html/rfc4627
     TOKEN_RESPONSE_HEADER = default_json_headers
 
-    def __init__(self, request, server):
+    def __init__(self, request: OAuth2Request, server):
         self.prompt = None
         self.redirect_uri = None
         self.request = request
         self.server = server
         self._hooks = {
             'after_validate_authorization_request': set(),
             'after_validate_consent_request': set(),
@@ -96,15 +97,15 @@
     #: Allowed HTTP methods of this token endpoint
     TOKEN_ENDPOINT_HTTP_METHODS = ['POST']
 
     #: Designed for which "grant_type"
     GRANT_TYPE = None
 
     @classmethod
-    def check_token_endpoint(cls, request):
+    def check_token_endpoint(cls, request: OAuth2Request):
         return request.grant_type == cls.GRANT_TYPE and \
                request.method in cls.TOKEN_ENDPOINT_HTTP_METHODS
 
     def validate_token_request(self):
         raise NotImplementedError()
 
     def create_token_response(self):
@@ -112,19 +113,19 @@
 
 
 class AuthorizationEndpointMixin(object):
     RESPONSE_TYPES = set()
     ERROR_RESPONSE_FRAGMENT = False
 
     @classmethod
-    def check_authorization_endpoint(cls, request):
+    def check_authorization_endpoint(cls, request: OAuth2Request):
         return request.response_type in cls.RESPONSE_TYPES
 
     @staticmethod
-    def validate_authorization_redirect_uri(request, client):
+    def validate_authorization_redirect_uri(request: OAuth2Request, client):
         if request.redirect_uri:
             if not client.check_redirect_uri(request.redirect_uri):
                 raise InvalidRequestError(
                     f'Redirect URI {request.redirect_uri} is not supported by client.',
                     state=request.state)
             return request.redirect_uri
         else:
@@ -139,9 +140,9 @@
         redirect_uri = self.validate_authorization_request()
         self.execute_hook('after_validate_consent_request', redirect_uri)
         self.redirect_uri = redirect_uri
 
     def validate_authorization_request(self):
         raise NotImplementedError()
 
-    def create_authorization_response(self, redirect_uri, grant_user):
+    def create_authorization_response(self, redirect_uri: str, grant_user):
         raise NotImplementedError()
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/client_credentials.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/client_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,13 +91,12 @@
                 "token_type":"example",
                 "expires_in":3600,
                 "example_parameter":"example_value"
             }
 
         :returns: (status_code, body, headers)
         """
-        client = self.request.client
         token = self.generate_token(scope=self.request.scope, include_refresh_token=False)
-        log.debug('Issue token %r to %r', token, client)
+        log.debug('Issue token %r to %r', token, self.client)
         self.save_token(token)
         self.execute_hook('process_token', self, token=token)
         return 200, token, self.TOKEN_RESPONSE_HEADER
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/implicit.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/implicit.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/refresh_token.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/refresh_token.py`

 * *Files 13% similar despite different names*

```diff
@@ -98,48 +98,46 @@
             Authorization: Basic czZCaGRSa3F0MzpnWDFmQmF0M2JW
             Content-Type: application/x-www-form-urlencoded
 
             grant_type=refresh_token&refresh_token=tGzv3JOkF0XG5Qx2TlKWIA
         """
         client = self._validate_request_client()
         self.request.client = client
-        token = self._validate_request_token(client)
-        self._validate_token_scope(token)
-        self.request.credential = token
+        refresh_token = self._validate_request_token(client)
+        self._validate_token_scope(refresh_token)
+        self.request.refresh_token = refresh_token
 
     def create_token_response(self):
         """If valid and authorized, the authorization server issues an access
         token as described in Section 5.1.  If the request failed
         verification or is invalid, the authorization server returns an error
         response as described in Section 5.2.
         """
-        credential = self.request.credential
-        user = self.authenticate_user(credential)
+        refresh_token = self.request.refresh_token
+        user = self.authenticate_user(refresh_token)
         if not user:
             raise InvalidRequestError('There is no "user" for this token.')
 
         client = self.request.client
-        token = self.issue_token(user, credential)
+        token = self.issue_token(user, refresh_token)
         log.debug('Issue token %r to %r', token, client)
 
         self.request.user = user
         self.save_token(token)
         self.execute_hook('process_token', token=token)
-        self.revoke_old_credential(credential)
+        self.revoke_old_credential(refresh_token)
         return 200, token, self.TOKEN_RESPONSE_HEADER
 
-    def issue_token(self, user, credential):
-        expires_in = credential.get_expires_in()
+    def issue_token(self, user, refresh_token):
         scope = self.request.scope
         if not scope:
-            scope = credential.get_scope()
+            scope = refresh_token.get_scope()
 
         token = self.generate_token(
             user=user,
-            expires_in=expires_in,
             scope=scope,
             include_refresh_token=self.INCLUDE_NEW_REFRESH_TOKEN,
         )
         return token
 
     def authenticate_refresh_token(self, refresh_token):
         """Get token information with refresh_token string. Developers MUST
@@ -151,31 +149,31 @@
                     return token
 
         :param refresh_token: The refresh token issued to the client
         :return: token
         """
         raise NotImplementedError()
 
-    def authenticate_user(self, credential):
+    def authenticate_user(self, refresh_token):
         """Authenticate the user related to this credential. Developers MUST
         implement this method in subclass::
 
             def authenticate_user(self, credential):
                 return User.query.get(credential.user_id)
 
-        :param credential: Token object
+        :param refresh_token: Token object
         :return: user
         """
         raise NotImplementedError()
 
-    def revoke_old_credential(self, credential):
+    def revoke_old_credential(self, refresh_token):
         """The authorization server MAY revoke the old refresh token after
         issuing a new refresh token to the client. Developers MUST implement
         this method in subclass::
 
-            def revoke_old_credential(self, credential):
+            def revoke_old_credential(self, refresh_token):
                 credential.revoked = True
                 credential.save()
 
-        :param credential: Token object
+        :param refresh_token: Token object
         """
         raise NotImplementedError()
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/grants/resource_owner_password_credentials.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/grants/resource_owner_password_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             }
 
         :returns: (status_code, body, headers)
         """
         user = self.request.user
         scope = self.request.scope
         token = self.generate_token(user=user, scope=scope)
-        log.debug('Issue token %r to %r', token, self.request.client)
+        log.debug('Issue token %r to %r', token, self.client)
         self.save_token(token)
         self.execute_hook('process_token', token=token)
         return 200, token, self.TOKEN_RESPONSE_HEADER
 
     def authenticate_user(self, username, password):
         """validate the resource owner password credentials using its
         existing password validation algorithm::
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/models.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/parameters.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         params.append(('redirect_uri', redirect_uri))
     if scope:
         params.append(('scope', list_to_scope(scope)))
     if state:
         params.append(('state', state))
 
     for k in kwargs:
-        if kwargs[k]:
+        if kwargs[k] is not None:
             params.append((to_unicode(k), kwargs[k]))
 
     return add_params_to_uri(uri, params)
 
 
 def prepare_token_request(grant_type, body='', redirect_uri=None, **kwargs):
     """Prepare the access token request. Per `Section 4.1.3`_.
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/resource_protector.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/resource_protector.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/token_endpoint.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/token_endpoint.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/util.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/util.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6749/wrappers.py` & `Authlib-1.2.1/authlib/oauth2/rfc6749/requests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,84 @@
-import time
+from authlib.common.encoding import json_loads
 from authlib.common.urls import urlparse, url_decode
 from .errors import InsecureTransportError
 
 
-class OAuth2Token(dict):
-    def __init__(self, params):
-        if params.get('expires_at'):
-            params['expires_at'] = int(params['expires_at'])
-        elif params.get('expires_in'):
-            params['expires_at'] = int(time.time()) + \
-                                   int(params['expires_in'])
-        super(OAuth2Token, self).__init__(params)
-
-    def is_expired(self):
-        expires_at = self.get('expires_at')
-        if not expires_at:
-            return None
-        return expires_at < time.time()
-
-    @classmethod
-    def from_dict(cls, token):
-        if isinstance(token, dict) and not isinstance(token, cls):
-            token = cls(token)
-        return token
-
-
 class OAuth2Request(object):
-    def __init__(self, method, uri, body=None, headers=None):
+    def __init__(self, method: str, uri: str, body=None, headers=None):
         InsecureTransportError.check(uri)
         #: HTTP method
         self.method = method
         self.uri = uri
         self.body = body
         #: HTTP headers
         self.headers = headers or {}
 
-        self.query = urlparse.urlparse(uri).query
+        self.client = None
+        self.auth_method = None
+        self.user = None
+        self.authorization_code = None
+        self.refresh_token = None
+        self.credential = None
 
-        self.args = dict(url_decode(self.query))
-        self.form = self.body or {}
+    @property
+    def args(self):
+        query = urlparse.urlparse(self.uri).query
+        return dict(url_decode(query))
 
-        #: dict of query and body params
+    @property
+    def form(self):
+        return self.body or {}
+
+    @property
+    def data(self):
         data = {}
         data.update(self.args)
         data.update(self.form)
-        self.data = data
-
-        #: authenticate method
-        self.auth_method = None
-        #: authenticated user on this request
-        self.user = None
-        #: authorization_code or token model instance
-        self.credential = None
-        #: client which sending this request
-        self.client = None
+        return data
 
     @property
-    def client_id(self):
+    def client_id(self) -> str:
         """The authorization server issues the registered client a client
         identifier -- a unique string representing the registration
         information provided by the client. The value is extracted from
         request.
 
         :return: string
         """
         return self.data.get('client_id')
 
     @property
-    def response_type(self):
+    def response_type(self) -> str:
         rt = self.data.get('response_type')
         if rt and ' ' in rt:
             # sort multiple response types
             return ' '.join(sorted(rt.split()))
         return rt
 
     @property
-    def grant_type(self):
-        return self.data.get('grant_type')
+    def grant_type(self) -> str:
+        return self.form.get('grant_type')
 
     @property
     def redirect_uri(self):
         return self.data.get('redirect_uri')
 
     @property
-    def scope(self):
+    def scope(self) -> str:
         return self.data.get('scope')
 
     @property
     def state(self):
         return self.data.get('state')
 
 
-class HttpRequest(object):
-    def __init__(self, method, uri, data=None, headers=None):
+class JsonRequest(object):
+    def __init__(self, method, uri, body=None, headers=None):
         self.method = method
         self.uri = uri
-        self.data = data
+        self.body = body
         self.headers = headers or {}
-        self.user = None
-        # the framework request instance
-        self.req = None
+
+    @property
+    def data(self):
+        return json_loads(self.body)
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6750/__init__.py` & `Authlib-1.2.1/authlib/oauth2/rfc6750/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6750/errors.py` & `Authlib-1.2.1/authlib/oauth2/rfc6750/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6750/parameters.py` & `Authlib-1.2.1/authlib/oauth2/rfc6750/parameters.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6750/token.py` & `Authlib-1.2.1/authlib/oauth2/rfc6750/token.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc6750/validator.py` & `Authlib-1.2.1/authlib/oauth2/rfc6750/validator.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7009/parameters.py` & `Authlib-1.2.1/authlib/oauth2/rfc7009/parameters.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7009/revocation.py` & `Authlib-1.2.1/authlib/oauth2/rfc7009/revocation.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7521/client.py` & `Authlib-1.2.1/authlib/oauth2/rfc7521/client.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/__init__.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/assertion.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/assertion.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/auth.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def sign(self, auth, token_endpoint):
         return client_secret_jwt_sign(
             auth.client_secret,
             client_id=auth.client_id,
             token_endpoint=token_endpoint,
             claims=self.claims,
-            headers=self.headers,
+            header=self.headers,
             alg=self.alg,
         )
 
     def __call__(self, auth, method, uri, headers, body):
         token_endpoint = self.token_endpoint
         if not token_endpoint:
             token_endpoint = uri
@@ -85,9 +85,10 @@
 
     def sign(self, auth, token_endpoint):
         return private_key_jwt_sign(
             auth.client_secret,
             client_id=auth.client_id,
             token_endpoint=token_endpoint,
             claims=self.claims,
+            header=self.headers,
             alg=self.alg,
         )
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/client.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/client.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/jwt_bearer.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/jwt_bearer.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/token.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/token.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7523/validator.py` & `Authlib-1.2.1/authlib/oauth2/rfc7523/validator.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7591/__init__.py` & `Authlib-1.2.1/authlib/oauth2/rfc7591/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7591/claims.py` & `Authlib-1.2.1/authlib/oauth2/rfc7591/claims.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7591/endpoint.py` & `Authlib-1.2.1/authlib/oauth2/rfc7591/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,23 +104,29 @@
 
             options['scope'] = {'validate': _validate_scope}
 
         if response_types_supported is not None:
             response_types_supported = set(response_types_supported)
 
             def _validate_response_types(claims, value):
-                return response_types_supported.issuperset(set(value))
+                # If omitted, the default is that the client will use only the "code"
+                # response type.
+                response_types = set(value) if value else {"code"}
+                return response_types_supported.issuperset(response_types)
 
             options['response_types'] = {'validate': _validate_response_types}
 
         if grant_types_supported is not None:
             grant_types_supported = set(grant_types_supported)
 
             def _validate_grant_types(claims, value):
-                return grant_types_supported.issuperset(set(value))
+                # If omitted, the default behavior is that the client will use only
+                # the "authorization_code" Grant Type.
+                grant_types = set(value) if value else {"authorization_code"}
+                return grant_types_supported.issuperset(grant_types)
 
             options['grant_types'] = {'validate': _validate_grant_types}
 
         if auth_methods_supported is not None:
             options['token_endpoint_auth_method'] = {'values': auth_methods_supported}
 
         return options
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7591/errors.py` & `Authlib-1.2.1/authlib/oauth2/rfc7591/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7592/endpoint.py` & `Authlib-1.2.1/authlib/oauth2/rfc7592/endpoint.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7636/challenge.py` & `Authlib-1.2.1/authlib/oauth2/rfc7636/challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import re
 import hashlib
 from authlib.common.encoding import to_bytes, to_unicode, urlsafe_b64encode
-from ..rfc6749.errors import InvalidRequestError, InvalidGrantError
+from ..rfc6749 import (
+    InvalidRequestError,
+    InvalidGrantError,
+    OAuth2Request,
+)
 
 
 CODE_VERIFIER_PATTERN = re.compile(r'^[a-zA-Z0-9\-._~]{43,128}$')
 
 
 def create_s256_code_challenge(code_verifier):
     """Create S256 code_challenge with the given code_verifier."""
@@ -59,35 +63,35 @@
         )
         grant.register_hook(
             'after_validate_token_request',
             self.validate_code_verifier,
         )
 
     def validate_code_challenge(self, grant):
-        request = grant.request
+        request: OAuth2Request = grant.request
         challenge = request.data.get('code_challenge')
         method = request.data.get('code_challenge_method')
         if not challenge and not method:
             return
 
         if not challenge:
             raise InvalidRequestError('Missing "code_challenge"')
 
         if method and method not in self.SUPPORTED_CODE_CHALLENGE_METHOD:
             raise InvalidRequestError('Unsupported "code_challenge_method"')
 
     def validate_code_verifier(self, grant):
-        request = grant.request
+        request: OAuth2Request = grant.request
         verifier = request.form.get('code_verifier')
 
         # public client MUST verify code challenge
         if self.required and request.auth_method == 'none' and not verifier:
             raise InvalidRequestError('Missing "code_verifier"')
 
-        authorization_code = request.credential
+        authorization_code = request.authorization_code
         challenge = self.get_authorization_code_challenge(authorization_code)
 
         # ignore, it is the normal RFC6749 authorization_code request
         if not challenge and not verifier:
             return
 
         # challenge exists, code_verifier is required
```

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7662/introspection.py` & `Authlib-1.2.1/authlib/oauth2/rfc7662/introspection.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7662/models.py` & `Authlib-1.2.1/authlib/oauth2/rfc7662/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc7662/token_validator.py` & `Authlib-1.2.1/authlib/oauth2/rfc7662/token_validator.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8414/models.py` & `Authlib-1.2.1/authlib/oauth2/rfc8414/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8414/well_known.py` & `Authlib-1.2.1/authlib/oauth2/rfc8414/well_known.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8628/__init__.py` & `Authlib-1.2.1/authlib/oauth2/rfc8628/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8628/device_code.py` & `Authlib-1.2.1/authlib/oauth2/rfc8628/device_code.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8628/endpoint.py` & `Authlib-1.2.1/authlib/oauth2/rfc8628/endpoint.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8628/errors.py` & `Authlib-1.2.1/authlib/oauth2/rfc8628/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oauth2/rfc8628/models.py` & `Authlib-1.2.1/authlib/oauth2/rfc8628/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/core/__init__.py` & `Authlib-1.2.1/authlib/oidc/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/core/claims.py` & `Authlib-1.2.1/authlib/oidc/core/claims.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/core/errors.py` & `Authlib-1.2.1/authlib/oidc/core/errors.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/core/grants/code.py` & `Authlib-1.2.1/authlib/oidc/core/grants/code.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Implementation of Authentication using the Authorization Code Flow
     per `Section 3.1`_.
 
     .. _`Section 3.1`: http://openid.net/specs/openid-connect-core-1_0.html#CodeFlowAuth
 """
 
 import logging
+from authlib.oauth2.rfc6749 import OAuth2Request
 from .util import (
     is_openid_scope,
     validate_nonce,
     validate_request_prompt,
     generate_id_token,
 )
 
@@ -65,23 +66,23 @@
 
     def process_token(self, grant, token):
         scope = token.get('scope')
         if not scope or not is_openid_scope(scope):
             # standard authorization code flow
             return token
 
-        request = grant.request
-        credential = request.credential
+        request: OAuth2Request = grant.request
+        authorization_code = request.authorization_code
 
         config = self.get_jwt_config(grant)
         config['aud'] = self.get_audiences(request)
 
-        if credential:
-            config['nonce'] = credential.get_nonce()
-            config['auth_time'] = credential.get_auth_time()
+        if authorization_code:
+            config['nonce'] = authorization_code.get_nonce()
+            config['auth_time'] = authorization_code.get_auth_time()
 
         user_info = self.generate_user_info(request.user, token['scope'])
         id_token = generate_id_token(token, user_info, **config)
         token['id_token'] = id_token
         return token
 
     def __call__(self, grant):
```

### Comparing `Authlib-1.2.0/authlib/oidc/core/grants/hybrid.py` & `Authlib-1.2.1/authlib/oidc/core/grants/hybrid.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/core/grants/implicit.py` & `Authlib-1.2.1/authlib/oidc/core/grants/implicit.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/core/grants/util.py` & `Authlib-1.2.1/authlib/oidc/core/grants/util.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/discovery/models.py` & `Authlib-1.2.1/authlib/oidc/discovery/models.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/authlib/oidc/discovery/well_known.py` & `Authlib-1.2.1/authlib/oidc/discovery/well_known.py`

 * *Files identical despite different names*

### Comparing `Authlib-1.2.0/setup.cfg` & `Authlib-1.2.1/setup.cfg`

 * *Files identical despite different names*

