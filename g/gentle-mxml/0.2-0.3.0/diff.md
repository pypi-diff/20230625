# Comparing `tmp/gentle_mxml-0.2.tar.gz` & `tmp/gentle_mxml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentle_mxml-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gentle_mxml-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gentle_mxml-0.2.tar` & `gentle_mxml-0.3.0.tar`

### file list

```diff
@@ -1,81 +1,119 @@
--rw-r--r--   0        0        0      432 2023-06-09 12:39:00.288853 gentle_mxml-0.2/LICENSE
--rw-r--r--   0        0        0     1898 2023-06-14 11:55:07.237854 gentle_mxml-0.2/README.md
--rw-r--r--   0        0        0      160 2023-06-21 17:50:31.011919 gentle_mxml-0.2/gentle/__init__.py
--rw-r--r--   0        0        0     3493 2023-06-14 11:48:23.451489 gentle_mxml-0.2/gentle/__main__.py
--rw-r--r--   0        0        0      818 2023-06-07 14:39:09.326200 gentle_mxml-0.2/gentle/generators/__init__.py
--rw-r--r--   0        0        0     1628 2023-06-14 11:48:31.704149 gentle_mxml-0.2/gentle/generators/bower.py
--rw-r--r--   0        0        0     3045 2023-06-21 17:49:19.512874 gentle_mxml-0.2/gentle/generators/cargo.py
--rw-r--r--   0        0        0     2396 2023-06-11 14:01:29.545936 gentle_mxml-0.2/gentle/generators/composer.py
--rw-r--r--   0        0        0     2669 2023-06-08 00:17:25.827762 gentle_mxml-0.2/gentle/generators/npm.py
--rw-r--r--   0        0        0     2312 2023-06-11 14:04:52.074515 gentle_mxml-0.2/gentle/generators/pyproject.py
--rw-r--r--   0        0        0     1922 2023-06-11 14:05:23.291217 gentle_mxml-0.2/gentle/generators/shards.py
--rw-r--r--   0        0        0     7352 2023-06-07 19:23:58.799898 gentle_mxml-0.2/gentle/metadata/__init__.py
--rw-r--r--   0        0        0     3138 2023-06-06 10:17:51.869275 gentle_mxml-0.2/gentle/metadata/utils.py
--rw-r--r--   0        0        0     1177 2023-06-09 12:45:48.947477 gentle_mxml-0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:04:35.028663 gentle_mxml-0.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 11:52:07.066278 gentle_mxml-0.2/tests/bower/__init__.py
--rw-r--r--   0        0        0      905 2023-06-14 11:52:52.204418 gentle_mxml-0.2/tests/bower/aurelia/bower.json
--rw-r--r--   0        0        0       93 2023-06-14 11:53:17.309384 gentle_mxml-0.2/tests/bower/aurelia/bower.json.license
--rw-r--r--   0        0        0      151 2023-06-14 11:53:43.708296 gentle_mxml-0.2/tests/bower/aurelia/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-14 11:52:46.348659 gentle_mxml-0.2/tests/bower/aurelia/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.2/tests/bower/pkg_empty/bower.json
--rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.2/tests/bower/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1111 2023-06-14 11:54:26.724524 gentle_mxml-0.2/tests/bower/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.159951 gentle_mxml-0.2/tests/cargo/__init__.py
--rw-r--r--   0        0        0     4750 2023-06-21 17:39:19.188683 gentle_mxml-0.2/tests/cargo/lemmy/Cargo.toml
--rw-r--r--   0        0        0       83 2023-06-21 17:54:17.087576 gentle_mxml-0.2/tests/cargo/lemmy/Cargo.toml.license
--rw-r--r--   0        0        0      163 2023-06-21 17:42:36.044548 gentle_mxml-0.2/tests/cargo/lemmy/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-21 17:39:09.494084 gentle_mxml-0.2/tests/cargo/lemmy/metadata.xml.license
--rw-r--r--   0        0        0     2581 2023-06-07 19:44:08.872681 gentle_mxml-0.2/tests/cargo/orjson/Cargo.toml
--rw-r--r--   0        0        0       95 2023-06-07 19:44:24.198957 gentle_mxml-0.2/tests/cargo/orjson/Cargo.toml.license
--rw-r--r--   0        0        0      189 2023-06-07 19:42:12.112203 gentle_mxml-0.2/tests/cargo/orjson/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 19:41:23.961480 gentle_mxml-0.2/tests/cargo/orjson/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.2/tests/cargo/pkg_empty/Cargo.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.2/tests/cargo/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1119 2023-06-21 17:46:02.450018 gentle_mxml-0.2/tests/cargo/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.862715 gentle_mxml-0.2/tests/composer/__init__.py
--rw-r--r--   0        0        0     3329 2023-06-11 13:56:25.593575 gentle_mxml-0.2/tests/composer/composer/composer.json
--rw-r--r--   0        0        0      161 2023-06-11 13:58:46.476717 gentle_mxml-0.2/tests/composer/composer/composer.json.license
--rw-r--r--   0        0        0      318 2023-06-11 14:01:02.564058 gentle_mxml-0.2/tests/composer/composer/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-11 13:57:30.625871 gentle_mxml-0.2/tests/composer/composer/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.2/tests/composer/pkg_empty/composer.json
--rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.2/tests/composer/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1127 2023-06-11 13:57:14.003562 gentle_mxml-0.2/tests/composer/test_generator.py
--rw-r--r--   0        0        0      290 2023-06-07 15:18:39.595705 gentle_mxml-0.2/tests/conftest.py
--rw-r--r--   0        0        0      168 2023-06-07 14:51:10.813952 gentle_mxml-0.2/tests/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 15:22:49.997859 gentle_mxml-0.2/tests/metadata.xml.license
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.990442 gentle_mxml-0.2/tests/npm/__init__.py
--rw-r--r--   0        0        0      234 2023-06-08 00:13:02.172234 gentle_mxml-0.2/tests/npm/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-08 00:10:46.617642 gentle_mxml-0.2/tests/npm/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0     3382 2023-06-08 00:13:19.251427 gentle_mxml-0.2/tests/npm/mkdocs-material/package.json
--rw-r--r--   0        0        0      103 2023-06-08 00:10:46.616642 gentle_mxml-0.2/tests/npm/mkdocs-material/package.json.license
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.997442 gentle_mxml-0.2/tests/npm/pkg_empty/package.json
--rw-r--r--   0        0        0        0 2023-06-07 23:55:19.998442 gentle_mxml-0.2/tests/npm/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1109 2023-06-07 23:57:05.916436 gentle_mxml-0.2/tests/npm/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.372752 gentle_mxml-0.2/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      330 2023-06-07 19:13:56.979345 gentle_mxml-0.2/tests/pyproject/mkdocs-material/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 19:07:24.968873 gentle_mxml-0.2/tests/pyproject/mkdocs-material/metadata.xml.license
--rw-r--r--   0        0        0     2949 2023-06-07 19:07:42.936024 gentle_mxml-0.2/tests/pyproject/mkdocs-material/pyproject.toml
--rw-r--r--   0        0        0      103 2023-06-07 19:11:03.167560 gentle_mxml-0.2/tests/pyproject/mkdocs-material/pyproject.toml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.2/tests/pyproject/pkg_empty/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.2/tests/pyproject/pkg_none/.gitkeep
--rw-r--r--   0        0        0      214 2023-06-07 18:58:47.333338 gentle_mxml-0.2/tests/pyproject/pkgcraft/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 18:59:06.048453 gentle_mxml-0.2/tests/pyproject/pkgcraft/metadata.xml.license
--rw-r--r--   0        0        0     2549 2023-06-07 18:54:37.693136 gentle_mxml-0.2/tests/pyproject/pkgcraft/pyproject.toml
--rw-r--r--   0        0        0       92 2023-06-07 18:56:45.335103 gentle_mxml-0.2/tests/pyproject/pkgcraft/pyproject.toml.license
--rw-r--r--   0        0        0     1151 2023-06-07 19:38:35.578442 gentle_mxml-0.2/tests/pyproject/test_generator.py
--rw-r--r--   0        0        0        0 2023-06-07 15:05:22.876399 gentle_mxml-0.2/tests/shards/__init__.py
--rw-r--r--   0        0        0      262 2023-06-07 16:08:13.258065 gentle_mxml-0.2/tests/shards/athena-spec/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 16:19:57.337776 gentle_mxml-0.2/tests/shards/athena-spec/metadata.xml.license
--rw-r--r--   0        0        0      287 2023-06-07 15:44:23.136690 gentle_mxml-0.2/tests/shards/athena-spec/shard.yml
--rw-r--r--   0        0        0       97 2023-06-07 16:19:15.122771 gentle_mxml-0.2/tests/shards/athena-spec/shard.yml.license
--rw-r--r--   0        0        0      254 2023-06-07 18:34:22.044597 gentle_mxml-0.2/tests/shards/exception_page/metadata.xml
--rw-r--r--   0        0        0       85 2023-06-07 18:20:08.443939 gentle_mxml-0.2/tests/shards/exception_page/metadata.xml.license
--rw-r--r--   0        0        0      432 2023-06-07 18:17:35.813152 gentle_mxml-0.2/tests/shards/exception_page/shard.yml
--rw-r--r--   0        0        0      208 2023-06-07 18:19:13.172551 gentle_mxml-0.2/tests/shards/exception_page/shard.yml.license
--rw-r--r--   0        0        0        0 2023-06-07 15:12:58.225856 gentle_mxml-0.2/tests/shards/pkg_empty/shard.yml
--rw-r--r--   0        0        0        0 2023-06-07 14:55:14.309353 gentle_mxml-0.2/tests/shards/pkg_none/.gitkeep
--rw-r--r--   0        0        0     1137 2023-06-07 19:38:04.782898 gentle_mxml-0.2/tests/shards/test_generator.py
--rw-r--r--   0        0        0      979 2023-06-06 11:58:30.447349 gentle_mxml-0.2/tests/test_metadata.py
--rw-r--r--   0        0        0      361 2023-06-07 16:03:33.900274 gentle_mxml-0.2/tests/utils.py
--rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 gentle_mxml-0.2/PKG-INFO
+-rw-r--r--   0        0        0      432 2023-06-09 12:39:00.288853 gentle_mxml-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2244 2023-06-25 12:11:00.893469 gentle_mxml-0.3.0/README.md
+-rw-r--r--   0        0        0      162 2023-06-25 14:13:36.466085 gentle_mxml-0.3.0/gentle/__init__.py
+-rw-r--r--   0        0        0     3716 2023-06-25 12:27:13.516179 gentle_mxml-0.3.0/gentle/__main__.py
+-rw-r--r--   0        0        0      967 2023-06-24 19:59:23.234866 gentle_mxml-0.3.0/gentle/generators/__init__.py
+-rw-r--r--   0        0        0     1628 2023-06-14 11:48:31.704149 gentle_mxml-0.3.0/gentle/generators/bower.py
+-rw-r--r--   0        0        0     3061 2023-06-23 06:42:42.354791 gentle_mxml-0.3.0/gentle/generators/cargo.py
+-rw-r--r--   0        0        0     2396 2023-06-11 14:01:29.545936 gentle_mxml-0.3.0/gentle/generators/composer.py
+-rw-r--r--   0        0        0     2124 2023-06-25 12:08:57.131595 gentle_mxml-0.3.0/gentle/generators/doap.py
+-rw-r--r--   0        0        0     2495 2023-06-21 22:59:00.769937 gentle_mxml-0.3.0/gentle/generators/hpack.py
+-rw-r--r--   0        0        0     2672 2023-06-23 06:39:27.842866 gentle_mxml-0.3.0/gentle/generators/npm.py
+-rw-r--r--   0        0        0     2602 2023-06-24 19:10:52.669001 gentle_mxml-0.3.0/gentle/generators/pkg_info.py
+-rw-r--r--   0        0        0     2329 2023-06-23 06:42:35.538073 gentle_mxml-0.3.0/gentle/generators/pyproject.py
+-rw-r--r--   0        0        0     1922 2023-06-11 14:05:23.291217 gentle_mxml-0.3.0/gentle/generators/shards.py
+-rw-r--r--   0        0        0     7386 2023-06-23 06:37:52.366830 gentle_mxml-0.3.0/gentle/metadata/__init__.py
+-rw-r--r--   0        0        0     3138 2023-06-25 12:04:41.903135 gentle_mxml-0.3.0/gentle/metadata/utils.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:33:13.040427 gentle_mxml-0.3.0/gentle/py.typed
+-rw-r--r--   0        0        0     1701 2023-06-25 13:11:28.282190 gentle_mxml-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:04:35.028663 gentle_mxml-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 11:52:07.066278 gentle_mxml-0.3.0/tests/bower/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-14 11:52:52.204418 gentle_mxml-0.3.0/tests/bower/aurelia/bower.json
+-rw-r--r--   0        0        0       93 2023-06-14 11:53:17.309384 gentle_mxml-0.3.0/tests/bower/aurelia/bower.json.license
+-rw-r--r--   0        0        0      151 2023-06-14 11:53:43.708296 gentle_mxml-0.3.0/tests/bower/aurelia/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-14 11:52:46.348659 gentle_mxml-0.3.0/tests/bower/aurelia/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.0/tests/bower/pkg_empty/bower.json
+-rw-r--r--   0        0        0        0 2023-06-14 11:51:37.442498 gentle_mxml-0.3.0/tests/bower/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1111 2023-06-14 11:54:26.724524 gentle_mxml-0.3.0/tests/bower/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.159951 gentle_mxml-0.3.0/tests/cargo/__init__.py
+-rw-r--r--   0        0        0     4750 2023-06-21 17:39:19.188683 gentle_mxml-0.3.0/tests/cargo/lemmy/Cargo.toml
+-rw-r--r--   0        0        0       83 2023-06-21 17:54:17.087576 gentle_mxml-0.3.0/tests/cargo/lemmy/Cargo.toml.license
+-rw-r--r--   0        0        0      163 2023-06-21 17:42:36.044548 gentle_mxml-0.3.0/tests/cargo/lemmy/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 17:39:09.494084 gentle_mxml-0.3.0/tests/cargo/lemmy/metadata.xml.license
+-rw-r--r--   0        0        0     2581 2023-06-07 19:44:08.872681 gentle_mxml-0.3.0/tests/cargo/orjson/Cargo.toml
+-rw-r--r--   0        0        0       95 2023-06-07 19:44:24.198957 gentle_mxml-0.3.0/tests/cargo/orjson/Cargo.toml.license
+-rw-r--r--   0        0        0      189 2023-06-07 19:42:12.112203 gentle_mxml-0.3.0/tests/cargo/orjson/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 19:41:23.961480 gentle_mxml-0.3.0/tests/cargo/orjson/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.0/tests/cargo/pkg_empty/Cargo.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:22.160951 gentle_mxml-0.3.0/tests/cargo/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1119 2023-06-21 17:46:02.450018 gentle_mxml-0.3.0/tests/cargo/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.862715 gentle_mxml-0.3.0/tests/composer/__init__.py
+-rw-r--r--   0        0        0     3329 2023-06-11 13:56:25.593575 gentle_mxml-0.3.0/tests/composer/composer/composer.json
+-rw-r--r--   0        0        0      161 2023-06-11 13:58:46.476717 gentle_mxml-0.3.0/tests/composer/composer/composer.json.license
+-rw-r--r--   0        0        0      318 2023-06-11 14:01:02.564058 gentle_mxml-0.3.0/tests/composer/composer/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-11 13:57:30.625871 gentle_mxml-0.3.0/tests/composer/composer/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.0/tests/composer/pkg_empty/composer.json
+-rw-r--r--   0        0        0        0 2023-06-11 13:53:33.866715 gentle_mxml-0.3.0/tests/composer/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1127 2023-06-11 13:57:14.003562 gentle_mxml-0.3.0/tests/composer/test_generator.py
+-rw-r--r--   0        0        0      290 2023-06-07 15:18:39.595705 gentle_mxml-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.439617 gentle_mxml-0.3.0/tests/doap/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-25 11:59:51.296133 gentle_mxml-0.3.0/tests/doap/gnome-calls/calls.doap
+-rw-r--r--   0        0        0      193 2023-06-25 12:01:58.282890 gentle_mxml-0.3.0/tests/doap/gnome-calls/calls.doap.license
+-rw-r--r--   0        0        0      329 2023-06-25 12:03:47.156396 gentle_mxml-0.3.0/tests/doap/gnome-calls/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-25 12:00:30.912497 gentle_mxml-0.3.0/tests/doap/gnome-calls/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.441617 gentle_mxml-0.3.0/tests/doap/pkg_empty/null.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:21.257850 gentle_mxml-0.3.0/tests/doap/pkg_multiple/one.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:24.041735 gentle_mxml-0.3.0/tests/doap/pkg_multiple/two.doap
+-rw-r--r--   0        0        0        0 2023-06-25 11:57:38.444617 gentle_mxml-0.3.0/tests/doap/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1243 2023-06-25 11:59:31.351956 gentle_mxml-0.3.0/tests/doap/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.776769 gentle_mxml-0.3.0/tests/hpack/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-21 23:10:21.212904 gentle_mxml-0.3.0/tests/hpack/hpack/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 23:09:22.249333 gentle_mxml-0.3.0/tests/hpack/hpack/metadata.xml.license
+-rw-r--r--   0        0        0     1398 2023-06-21 23:08:08.575369 gentle_mxml-0.3.0/tests/hpack/hpack/package.yaml
+-rw-r--r--   0        0        0       90 2023-06-21 23:09:09.245869 gentle_mxml-0.3.0/tests/hpack/hpack/package.yaml.license
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.780768 gentle_mxml-0.3.0/tests/hpack/pkg_empty/package.yaml
+-rw-r--r--   0        0        0        0 2023-06-21 23:06:21.783768 gentle_mxml-0.3.0/tests/hpack/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      117 2023-06-21 23:11:51.765173 gentle_mxml-0.3.0/tests/hpack/stack/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-21 23:10:32.554437 gentle_mxml-0.3.0/tests/hpack/stack/metadata.xml.license
+-rw-r--r--   0        0        0    10727 2023-06-21 23:11:25.944237 gentle_mxml-0.3.0/tests/hpack/stack/package.yaml
+-rw-r--r--   0        0        0       91 2023-06-21 23:16:13.343396 gentle_mxml-0.3.0/tests/hpack/stack/package.yaml.license
+-rw-r--r--   0        0        0     1117 2023-06-21 23:07:37.239659 gentle_mxml-0.3.0/tests/hpack/test_generator.py
+-rw-r--r--   0        0        0      168 2023-06-07 14:51:10.813952 gentle_mxml-0.3.0/tests/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 15:22:49.997859 gentle_mxml-0.3.0/tests/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.990442 gentle_mxml-0.3.0/tests/npm/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-08 00:13:02.172234 gentle_mxml-0.3.0/tests/npm/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-08 00:10:46.617642 gentle_mxml-0.3.0/tests/npm/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0     3382 2023-06-08 00:13:19.251427 gentle_mxml-0.3.0/tests/npm/mkdocs-material/package.json
+-rw-r--r--   0        0        0      103 2023-06-08 00:10:46.616642 gentle_mxml-0.3.0/tests/npm/mkdocs-material/package.json.license
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.997442 gentle_mxml-0.3.0/tests/npm/pkg_empty/package.json
+-rw-r--r--   0        0        0        0 2023-06-07 23:55:19.998442 gentle_mxml-0.3.0/tests/npm/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1109 2023-06-07 23:57:05.916436 gentle_mxml-0.3.0/tests/npm/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.866553 gentle_mxml-0.3.0/tests/pkg_info/__init__.py
+-rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-06-24 18:59:44.869553 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/PKG-INFO.license
+-rw-r--r--   0        0        0      303 2023-06-24 19:09:17.624922 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-24 18:59:44.869553 gentle_mxml-0.3.0/tests/pkg_info/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.0/tests/pkg_info/pkg_empty/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-24 18:59:44.867553 gentle_mxml-0.3.0/tests/pkg_info/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1883 2023-02-18 15:55:47.929912 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/PKG-INFO
+-rw-r--r--   0        0        0       92 2023-06-24 18:59:44.868553 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/PKG-INFO.license
+-rw-r--r--   0        0        0      214 2023-06-24 18:59:44.868553 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-24 18:59:44.868553 gentle_mxml-0.3.0/tests/pkg_info/pkgcraft/metadata.xml.license
+-rw-r--r--   0        0        0     1142 2023-06-24 19:05:20.815692 gentle_mxml-0.3.0/tests/pkg_info/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.372752 gentle_mxml-0.3.0/tests/pyproject/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-07 19:13:56.979345 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 19:07:24.968873 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/metadata.xml.license
+-rw-r--r--   0        0        0     2949 2023-06-07 19:07:42.936024 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-06-07 19:11:03.167560 gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/pyproject.toml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.0/tests/pyproject/pkg_empty/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 15:33:26.373752 gentle_mxml-0.3.0/tests/pyproject/pkg_none/.gitkeep
+-rw-r--r--   0        0        0      214 2023-06-07 18:58:47.333338 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 18:59:06.048453 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/metadata.xml.license
+-rw-r--r--   0        0        0     2549 2023-06-07 18:54:37.693136 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-06-07 18:56:45.335103 gentle_mxml-0.3.0/tests/pyproject/pkgcraft/pyproject.toml.license
+-rw-r--r--   0        0        0     1151 2023-06-07 19:38:35.578442 gentle_mxml-0.3.0/tests/pyproject/test_generator.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:05:22.876399 gentle_mxml-0.3.0/tests/shards/__init__.py
+-rw-r--r--   0        0        0      262 2023-06-07 16:08:13.258065 gentle_mxml-0.3.0/tests/shards/athena-spec/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 16:19:57.337776 gentle_mxml-0.3.0/tests/shards/athena-spec/metadata.xml.license
+-rw-r--r--   0        0        0      287 2023-06-07 15:44:23.136690 gentle_mxml-0.3.0/tests/shards/athena-spec/shard.yml
+-rw-r--r--   0        0        0       97 2023-06-07 16:19:15.122771 gentle_mxml-0.3.0/tests/shards/athena-spec/shard.yml.license
+-rw-r--r--   0        0        0      254 2023-06-07 18:34:22.044597 gentle_mxml-0.3.0/tests/shards/exception_page/metadata.xml
+-rw-r--r--   0        0        0       85 2023-06-07 18:20:08.443939 gentle_mxml-0.3.0/tests/shards/exception_page/metadata.xml.license
+-rw-r--r--   0        0        0      432 2023-06-07 18:17:35.813152 gentle_mxml-0.3.0/tests/shards/exception_page/shard.yml
+-rw-r--r--   0        0        0      208 2023-06-07 18:19:13.172551 gentle_mxml-0.3.0/tests/shards/exception_page/shard.yml.license
+-rw-r--r--   0        0        0        0 2023-06-07 15:12:58.225856 gentle_mxml-0.3.0/tests/shards/pkg_empty/shard.yml
+-rw-r--r--   0        0        0        0 2023-06-07 14:55:14.309353 gentle_mxml-0.3.0/tests/shards/pkg_none/.gitkeep
+-rw-r--r--   0        0        0     1137 2023-06-07 19:38:04.782898 gentle_mxml-0.3.0/tests/shards/test_generator.py
+-rw-r--r--   0        0        0     1064 2023-06-23 06:29:53.471712 gentle_mxml-0.3.0/tests/test_metadata.py
+-rw-r--r--   0        0        0      361 2023-06-07 16:03:33.900274 gentle_mxml-0.3.0/tests/utils.py
+-rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 gentle_mxml-0.3.0/PKG-INFO
```

### Comparing `gentle_mxml-0.2/README.md` & `gentle_mxml-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 
 
 Supported generators
 --------------------
 
 * [Bower](https://github.com/bower/spec/blob/master/json.md)
 * Crystal ([Shards](https://github.com/crystal-lang/shards/blob/master/docs/shard.yml.adoc))
+* [DOAP](https://github.com/ewilderj/doap/wiki)
+* Haskell ([Hpack](https://github.com/sol/hpack/blob/main/README.md))
 * Node.js ([npm](https://docs.npmjs.com/files/package.json/))
-* Python ([PEP 621](https://peps.python.org/pep-0621/))
+* PHP ([Composer](https://getcomposer.org/doc/04-schema.md))
+* Python ([PEP 621](https://peps.python.org/pep-0621/) and [PEP 643](https://peps.python.org/pep-0643/))
 * Rust ([Cargo](https://doc.rust-lang.org/cargo/reference/manifest.html))
 
 
 Dependencies
 ------------
 
 * [Portage](https://pypi.org/project/portage/)
+* [pkginfo](https://pypi.org/project/pkginfo/) *(optional)*
 * [PyYAML](https://pyyaml.org/) *(optional)*
+* [rdflib](https://pypi.org/project/rdflib/) *(optional)*
 * [Tomli](https://pypi.org/project/tomli/) *(optional)*
 
 
 Installing
 ----------
 
 ### Gentoo
```

### Comparing `gentle_mxml-0.2/gentle/__main__.py` & `gentle_mxml-0.3.0/gentle/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 import logging
 import os
 import re
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import gentle
-from gentle.generators import AbstractGenerator
+from gentle.generators import AbstractGenerator, GeneratorClass
 from gentle.metadata import MetadataXML
 
 import gentle.generators.bower
 import gentle.generators.cargo
 import gentle.generators.composer
+import gentle.generators.doap
+import gentle.generators.hpack
 import gentle.generators.npm
+import gentle.generators.pkg_info
 import gentle.generators.pyproject
 import gentle.generators.shards
 
 try:
     import portage
     from portage.package.ebuild.doebuild import doebuild
 except ModuleNotFoundError:
@@ -42,15 +45,17 @@
     """
     ebuild = ebuild.resolve()
     portdir = str(ebuild.parents[2])
 
     # pylint: disable=protected-access
     if portdir not in portage.portdb.porttrees:
         portdir_overlay = portage.settings.get("PORTDIR_OVERLAY", "")
-        os.environ["PORTDIR_OVERLAY"] = portdir_overlay + " " + portage._shell_quote(portdir)
+        os.environ["PORTDIR_OVERLAY"] = (portdir_overlay
+                                         + " "
+                                         + portage._shell_quote(portdir))
 
         print(f"Appending {portdir} to PORTDIR_OVERLAY...")
         portage._reset_legacy_globals()
 
     tmpsettings: portage.config = portage.portdb.doebuild_settings
     tmpsettings["PORTAGE_USERNAME"] = os.getlogin()
     tmpsettings["PORTAGE_TMPDIR"] = tmpdir
@@ -95,14 +100,15 @@
     args = parser.parse_args()
 
     mxml_file = args.ebuild.parent / "metadata.xml"
     mxml = MetadataXML(mxml_file)
 
     with TemporaryDirectory(prefix="gentle-") as tmpdir:
         srcdir = portage_src_unpack(args.ebuild, tmpdir)
+        cls: GeneratorClass
         for cls in AbstractGenerator.get_generator_subclasses():
             generator = cls(srcdir)
             if generator.active:
                 logger.info("Starting %s", cls.__name__)
                 generator.update_metadata_xml(mxml)
     mxml.dump()
```

### Comparing `gentle_mxml-0.2/gentle/generators/__init__.py` & `gentle_mxml-0.3.0/gentle/generators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 # SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in>
 # No warranty
 
 """ Generic generator routines """
 
 from abc import ABC, abstractmethod
 from pathlib import Path
+from typing import Type
 
 from gentle.metadata import MetadataXML
 
 
 class AbstractGenerator(ABC):
     """ Generic class for metadata generators. """
-    _subclasses = []
+    _subclasses: "list[GeneratorClass]" = []
 
     @classmethod
-    def get_generator_subclasses(cls):
+    def get_generator_subclasses(cls) -> "list[GeneratorClass]":
         return cls._subclasses.copy()
 
     @abstractmethod
     def __init__(self, srcdir: Path):
         ...
 
-    def __init_subclass__(cls, **kwargs):
+    def __init_subclass__(cls: "GeneratorClass", **kwargs: dict) -> None:
         super().__init_subclass__(**kwargs)
         AbstractGenerator._subclasses.append(cls)
 
     @abstractmethod
     def update_metadata_xml(self, mxml: MetadataXML) -> None:
         ...
 
     @property
     @abstractmethod
     def active(self) -> bool:
         ...
+
+
+GeneratorClass = Type[AbstractGenerator]
```

### Comparing `gentle_mxml-0.2/gentle/generators/bower.py` & `gentle_mxml-0.3.0/gentle/generators/bower.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/gentle/generators/cargo.py` & `gentle_mxml-0.3.0/gentle/generators/cargo.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gentle.metadata import MetadataXML
 from gentle.metadata.utils import extract_name_email, extract_remote_id
 
 try:
     try:
         import tomllib
     except ModuleNotFoundError:
-        import tomli as tomllib
+        import tomli as tomllib  # type: ignore
     _HAS_TOMLLIB = True
 except ModuleNotFoundError:
     _HAS_TOMLLIB = False
 
 logger = logging.getLogger("cargo")
```

### Comparing `gentle_mxml-0.2/gentle/generators/composer.py` & `gentle_mxml-0.3.0/gentle/generators/composer.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/gentle/generators/npm.py` & `gentle_mxml-0.3.0/gentle/generators/npm.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if (repo := package.get("repository")) is not None:
             logger.info("Found repository: %s", repo)
             # TODO: process 'repository' objects
             if isinstance(repo, str):
                 *attr, value = repo.split(":")
                 match attr:
                     case ["bitbucket"] | ["github"] | ["gitlab"]:
-                        remote_id = RemoteID(attr=attr, value=value)
+                        remote_id = RemoteID(attr=attr[0], value=value)
                         mxml.add_upstream_remote_id(remote_id)
                     case []:
                         remote_id = RemoteID(attr="github", value=value)
                         mxml.add_upstream_remote_id(remote_id)
 
     @property
     def active(self) -> bool:
```

### Comparing `gentle_mxml-0.2/gentle/generators/pyproject.py` & `gentle_mxml-0.3.0/gentle/generators/pyproject.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from gentle.metadata import Person, MetadataXML
 from gentle.metadata.utils import extract_remote_id
 
 try:
     try:
         import tomllib
     except ModuleNotFoundError:
-        import tomli as tomllib
+        import tomli as tomllib  # type: ignore
     _HAS_TOMLLIB = True
 except ModuleNotFoundError:
     _HAS_TOMLLIB = False
 
 logger = logging.getLogger("pyproject")
 
 
@@ -63,10 +63,11 @@
                 case "changelog" | "changes":
                     mxml.set_upstream_changelog(value)
                 case "doc" | "docs" | "documentation":
                     mxml.set_upstream_doc(value)
                 case "source" | "repo" | "repository" | "home" | "homepage":
                     if (remote_id := extract_remote_id(value)) is not None:
                         mxml.add_upstream_remote_id(remote_id)
+
     @property
     def active(self) -> bool:
         return _HAS_TOMLLIB and self.pyproject_toml.is_file()
```

### Comparing `gentle_mxml-0.2/gentle/generators/shards.py` & `gentle_mxml-0.3.0/gentle/generators/shards.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/gentle/metadata/__init__.py` & `gentle_mxml-0.3.0/gentle/metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """ Parse and write :file:`metadata.xml` files. """
 
     def __init__(self, xmlfile: Path):
         """
         :param xmlfile: path to the :file:`metadata.xml` file
         """
         self.xmlfile: Path = xmlfile
-        self.xml: ET = ET.parse(self.xmlfile)
+        self.xml: ET.ElementTree = ET.parse(self.xmlfile)
 
         self._maintainers: list[Person] = []
         self._upstream = Upstream()
         self._parse_metadata_xml()
 
     @property
     def maintainers(self) -> list[Person]:
@@ -90,15 +90,15 @@
             file.write(textwrap.dedent("""\
                 <?xml version="1.0" encoding="UTF-8"?>
                 <!DOCTYPE pkgmetadata SYSTEM "https://www.gentoo.org/dtd/metadata.dtd">
             """))
             self.xml.write(file, encoding="unicode")
             file.write("\n")
 
-    def dumps(self) -> None:
+    def dumps(self) -> str:
         """ Convert the object to text """
         ET.indent(self.xml, space="\t", level=0)
         return ET.tostring(self.xml.getroot(), encoding="unicode")
 
     def add_upstream_maintainer(self, person: Person) -> None:
         """ Add a person to the list of upstream maintainers """
         if person in self._upstream.maintainers:
@@ -188,15 +188,15 @@
         if (name_tag := xml.find("name")) is not None:
             name = "".join(name_tag.itertext())
         elif name_optional:
             name = None
         else:
             return None
 
-        return Person(name, email)
+        return Person(name or "", email or "")
 
     def _parse_package_maintainer(self, xml: ET.Element) -> None:
         """
         :param xml: top-level ``<maintainer>`` XML tag
         """
         if (person := self._parse_person(xml, name_optional=True)) is not None:
             self._maintainers.append(person)
@@ -208,15 +208,15 @@
         assert xml.tag == "upstream"
 
         for maint in xml.findall("maintainer"):
             if (person := self._parse_person(maint, email_optional=True)) is not None:
                 self._upstream.maintainers.append(person)
 
         for remote in xml.findall("remote-id"):
-            attr = remote.get("type")
+            attr = remote.get("type", "unknown")
             value = "".join(remote.itertext())
             self._upstream.remote_ids.append(RemoteID(attr, value))
 
         if (changelog := xml.find("changelog")) is not None:
             self._upstream.changelog = "".join(changelog.itertext())
 
         if (doc := xml.find("doc")) is not None:
```

### Comparing `gentle_mxml-0.2/gentle/metadata/utils.py` & `gentle_mxml-0.3.0/gentle/metadata/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "gentoo":
         re.compile(r"https?://gitweb.gentoo.org/(?P<v>.+)[.]git"),
     "github":
         re.compile(r"https?://github.com/(?P<v>\S+/\S+)"),
     "gitlab":
         re.compile(r"https?://gitlab.com/(?P<v>.+?)/?"),
     "gnome-gitlab":
-        re.compile(r"https?://gitlab.gnome.org/(?P<v>.+?)/?"),
+        re.compile(r"https?://gitlab.gnome.org/(?P<v>\S+)/?"),
     "google-code":
         re.compile(r"https?://code.google.com/archive/p/(?P<v>\S+)"),
     "hackage":
         re.compile(r"https?://hackage.haskell.org/package/(?P<v>\S+)"),
     "heptapod":
         re.compile(r"https?://foss.heptapod.net/(?P<v>.+?)/?"),
     "launchpad":
```

### Comparing `gentle_mxml-0.2/pyproject.toml` & `gentle_mxml-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -22,19 +22,28 @@
     "License :: DFSG approved",
     "Operating System :: POSIX",
     "Topic :: System :: Software Distribution",
     "Topic :: Utilities"
 ]
 
 [project.optional-dependencies]
+# PKG-INFO
+pkginfo = ["pkginfo"]
+# DOAP
+rdf = ["rdflib"]
 # Cargo.toml, pyproject.toml, ...
 toml = ["tomli; python_version <= '3.11'"]
 # shard.yml
 yaml = ["PyYAML"]
 
+docs = [
+    "insipid-sphinx-theme",
+    "sphinx",
+    "sphinx-prompt"
+]
 test = [
     "pytest",
     "xmldiff"
 ]
 
 [project.scripts]
 gentle = "gentle.__main__:main"
@@ -47,7 +56,28 @@
 name = "gentle"
 
 [tool.flit.sdist]
 include = ["tests/"]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
+
+[tool.mypy]
+disallow_untyped_defs = true
+no_implicit_optional = true
+
+[[tool.mypy.overrides]]
+module = [
+    "tests.*",
+]
+# requiring explicit types for all test methods would be cumbersome
+disallow_untyped_defs = false
+check_untyped_defs = true
+
+[[tool.mypy.overrides]]
+module = [
+    "portage.*",
+    "tomllib.*",
+    "xml.sax._exceptions.*",
+    "xmldiff.*"
+]
+ignore_missing_imports = true
```

### Comparing `gentle_mxml-0.2/tests/bower/aurelia/bower.json` & `gentle_mxml-0.3.0/tests/bower/aurelia/bower.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/bower/test_generator.py` & `gentle_mxml-0.3.0/tests/bower/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/cargo/lemmy/Cargo.toml` & `gentle_mxml-0.3.0/tests/cargo/lemmy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/cargo/orjson/Cargo.toml` & `gentle_mxml-0.3.0/tests/cargo/orjson/Cargo.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/cargo/test_generator.py` & `gentle_mxml-0.3.0/tests/cargo/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/composer/composer/composer.json` & `gentle_mxml-0.3.0/tests/composer/composer/composer.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/composer/test_generator.py` & `gentle_mxml-0.3.0/tests/composer/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/npm/mkdocs-material/package.json` & `gentle_mxml-0.3.0/tests/npm/mkdocs-material/package.json`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/npm/test_generator.py` & `gentle_mxml-0.3.0/tests/npm/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/pyproject/mkdocs-material/pyproject.toml` & `gentle_mxml-0.3.0/tests/pyproject/mkdocs-material/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/pyproject/pkgcraft/pyproject.toml` & `gentle_mxml-0.3.0/tests/pyproject/pkgcraft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/pyproject/test_generator.py` & `gentle_mxml-0.3.0/tests/pyproject/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/shards/test_generator.py` & `gentle_mxml-0.3.0/tests/shards/test_generator.py`

 * *Files identical despite different names*

### Comparing `gentle_mxml-0.2/tests/test_metadata.py` & `gentle_mxml-0.3.0/tests/test_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 # SPDX-License-Identifier: WTFPL
 # SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in>
 # No warranty
 
 import xml.etree.ElementTree as ET
 
-from gentle.metadata import Person, RemoteID, MetadataXML
+from gentle.metadata import Person, RemoteID
+
 
 def test_person_to_xml():
     person = Person(name="Larry the Cow", email="larry@gentoo.org")
-    assert ET.tostring(person.to_xml(), encoding="unicode") == '<maintainer><name>Larry the Cow</name><email>larry@gentoo.org</email></maintainer>'
+    assert (
+        ET.tostring(person.to_xml(), encoding="unicode") ==
+        '<maintainer><name>Larry the Cow</name><email>larry@gentoo.org</email></maintainer>'
+    )
 
     person = Person(name="Larry the Cow")
-    assert ET.tostring(person.to_xml(), encoding="unicode") == '<maintainer><name>Larry the Cow</name></maintainer>'
+    assert (
+        ET.tostring(person.to_xml(), encoding="unicode") ==
+        '<maintainer><name>Larry the Cow</name></maintainer>'
+    )
 
     person = Person(email="larry@gentoo.org")
-    assert ET.tostring(person.to_xml(), encoding="unicode") == '<maintainer><email>larry@gentoo.org</email></maintainer>'
+    assert (
+        ET.tostring(person.to_xml(), encoding="unicode") ==
+        '<maintainer><email>larry@gentoo.org</email></maintainer>'
+    )
+
 
 def test_remote_id_to_xml():
     remote_id = RemoteID(attr="github", value="gentoo/gentoo")
-    assert ET.tostring(remote_id.to_xml(), encoding="unicode") == '<remote-id type="github">gentoo/gentoo</remote-id>'
+    assert (
+        ET.tostring(remote_id.to_xml(), encoding="unicode") ==
+        '<remote-id type="github">gentoo/gentoo</remote-id>'
+    )
```

### Comparing `gentle_mxml-0.2/PKG-INFO` & `gentle_mxml-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: gentle-mxml
-Version: 0.2
+Version: 0.3.0
 Summary: Gentoo Metadata XML generator 
 Author-email: Anna <cyber@sysrq.in>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: Operating System :: POSIX
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Dist: portage
+Requires-Dist: insipid-sphinx-theme ; extra == "docs"
+Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx-prompt ; extra == "docs"
+Requires-Dist: pkginfo ; extra == "pkginfo"
+Requires-Dist: rdflib ; extra == "rdf"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: xmldiff ; extra == "test"
 Requires-Dist: tomli ; extra == "toml" and ( python_version <= '3.11')
 Requires-Dist: PyYAML ; extra == "yaml"
 Project-URL: Issues, https://bugs.sysrq.in/enter_bug.cgi?product=Software&component=gentle
 Project-URL: Source, https://git.sysrq.in/gentle
+Provides-Extra: docs
+Provides-Extra: pkginfo
+Provides-Extra: rdf
 Provides-Extra: test
 Provides-Extra: toml
 Provides-Extra: yaml
 
 <!-- SPDX-FileCopyrightText: 2023 Anna <cyber@sysrq.in> -->
 <!-- SPDX-License-Identifier: CC0-1.0 -->
 
@@ -35,24 +43,29 @@
 
 
 Supported generators
 --------------------
 
 * [Bower](https://github.com/bower/spec/blob/master/json.md)
 * Crystal ([Shards](https://github.com/crystal-lang/shards/blob/master/docs/shard.yml.adoc))
+* [DOAP](https://github.com/ewilderj/doap/wiki)
+* Haskell ([Hpack](https://github.com/sol/hpack/blob/main/README.md))
 * Node.js ([npm](https://docs.npmjs.com/files/package.json/))
-* Python ([PEP 621](https://peps.python.org/pep-0621/))
+* PHP ([Composer](https://getcomposer.org/doc/04-schema.md))
+* Python ([PEP 621](https://peps.python.org/pep-0621/) and [PEP 643](https://peps.python.org/pep-0643/))
 * Rust ([Cargo](https://doc.rust-lang.org/cargo/reference/manifest.html))
 
 
 Dependencies
 ------------
 
 * [Portage](https://pypi.org/project/portage/)
+* [pkginfo](https://pypi.org/project/pkginfo/) *(optional)*
 * [PyYAML](https://pyyaml.org/) *(optional)*
+* [rdflib](https://pypi.org/project/rdflib/) *(optional)*
 * [Tomli](https://pypi.org/project/tomli/) *(optional)*
 
 
 Installing
 ----------
 
 ### Gentoo
```

