# Comparing `tmp/anytree-2.8.0.tar.gz` & `tmp/anytree-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anytree-2.8.0.tar", last modified: Wed Jan 15 01:21:44 2020, max compression
+gzip compressed data, was "anytree-2.9.0.tar", max compression
```

## Comparing `anytree-2.8.0.tar` & `anytree-2.9.0.tar`

### file list

```diff
@@ -1,118 +1,34 @@
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)    11357 2019-05-29 09:13:42.000000 anytree-2.8.0/LICENSE
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      198 2020-01-15 01:01:03.000000 anytree-2.8.0/MANIFEST.in
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     8898 2020-01-15 01:21:44.000000 anytree-2.8.0/PKG-INFO
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     6332 2020-01-15 01:07:02.000000 anytree-2.8.0/README.rst
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree/
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1539 2020-01-15 01:07:02.000000 anytree-2.8.0/anytree/__init__.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1572 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/cachedsearch.py
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      457 2019-05-29 09:13:42.000000 anytree-2.8.0/anytree/dotexport.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree/exporter/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      207 2019-09-24 22:40:32.000000 anytree-2.8.0/anytree/exporter/__init__.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     3923 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/exporter/dictexporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)    14594 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/exporter/dotexporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2372 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/exporter/jsonexporter.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree/importer/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      111 2019-05-29 09:13:42.000000 anytree-2.8.0/anytree/importer/__init__.py
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)     1540 2019-05-29 09:13:42.000000 anytree-2.8.0/anytree/importer/dictimporter.py
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)     1946 2019-05-29 09:13:42.000000 anytree-2.8.0/anytree/importer/jsonimporter.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree/iterators/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      806 2019-05-29 09:13:42.000000 anytree-2.8.0/anytree/iterators/__init__.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1704 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/iterators/abstractiter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2206 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/iterators/levelordergroupiter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1614 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/iterators/levelorderiter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1746 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/iterators/postorderiter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1738 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/iterators/preorderiter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2049 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/iterators/zigzaggroupiter.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree/node/
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      718 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/__init__.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     3469 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/anynode.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      142 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/exceptions.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2995 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/node.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)    15733 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/nodemixin.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1719 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/symlinknode.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1979 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/node/symlinknodemixin.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      472 2020-01-10 00:13:38.000000 anytree-2.8.0/anytree/node/util.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)    10991 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/render.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     7789 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/resolver.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     7341 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/search.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree/util/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)     2162 2019-09-29 20:43:25.000000 anytree-2.8.0/anytree/util/__init__.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2733 2020-01-15 01:01:03.000000 anytree-2.8.0/anytree/walker.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree.egg-info/
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     8898 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree.egg-info/PKG-INFO
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2520 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree.egg-info/SOURCES.txt
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)        1 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree.egg-info/dependency_links.txt
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)       50 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree.egg-info/requires.txt
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)        8 2020-01-15 01:21:44.000000 anytree-2.8.0/anytree.egg-info/top_level.txt
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/docs/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)     7596 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/Makefile
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/docs/api/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       72 2019-09-29 20:50:03.000000 anytree-2.8.0/docs/api/anytree.cachedsearch.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      318 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/api/anytree.iterators.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      299 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/api/anytree.node.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       62 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/api/anytree.render.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       66 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/api/anytree.resolver.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       52 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/api/anytree.search.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       50 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/api/anytree.util.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       58 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/api/anytree.walker.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      213 2019-09-29 20:50:03.000000 anytree-2.8.0/docs/api.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     9680 2020-01-15 01:07:02.000000 anytree-2.8.0/docs/conf.py
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      773 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/dotexport.rst
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/docs/exporter/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       87 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/exporter/dictexporter.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      165 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/exporter/dotexporter.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       75 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/exporter/jsonexporter.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      395 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/exporter.rst
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/docs/importer/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       87 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/importer/dictimporter.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)       75 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/importer/jsonimporter.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      370 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/importer.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     5907 2020-01-15 01:07:02.000000 anytree-2.8.0/docs/index.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      257 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/installation.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     4938 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/intro.rst
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/docs/static/
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     8640 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/static/buymeacoffee.png
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     8135 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/static/dan.png
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)    24801 2019-09-24 22:40:32.000000 anytree-2.8.0/docs/static/dotexporter0.png
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)    22607 2019-09-24 22:40:32.000000 anytree-2.8.0/docs/static/dotexporter1.png
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)    30760 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/static/tree.png
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)    18114 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/static/udo.png
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)    20092 2019-09-24 22:40:32.000000 anytree-2.8.0/docs/static/uniquedotexporter2.png
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)    12715 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/static/weight.png
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/docs/tricks/
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2147 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/tricks/multidim.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)     2876 2019-10-10 05:57:08.000000 anytree-2.8.0/docs/tricks/readonly.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1363 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/tricks/weightededges.rst
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)     2494 2019-05-29 09:13:42.000000 anytree-2.8.0/docs/tricks/yaml.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      109 2020-01-15 01:01:03.000000 anytree-2.8.0/docs/tricks.rst
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      418 2020-01-15 01:21:44.000000 anytree-2.8.0/setup.cfg
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2140 2020-01-15 01:01:03.000000 anytree-2.8.0/setup.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/tests/
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      694 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/helper.py
-drwxrwxr-x   0 djakschik (853001117) djakschik (853001296)        0 2020-01-15 01:21:44.000000 anytree-2.8.0/tests/refdata/
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      308 2019-09-24 22:40:32.000000 anytree-2.8.0/tests/refdata/tree1.dot
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      658 2019-09-23 19:32:05.000000 anytree-2.8.0/tests/refdata/tree2.dot
--rw-r--r--   0 djakschik (853001117) djakschik (853001296)      697 2019-09-23 19:32:05.000000 anytree-2.8.0/tests/refdata/tree3.dot
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)       97 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/refdata/tree4.dot
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2512 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_cachedsearch.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     3917 2020-01-09 23:12:08.000000 anytree-2.8.0/tests/test_dictexporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2567 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_dictimporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2317 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_dotexport.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     3968 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_dotexporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      847 2020-01-09 23:12:08.000000 anytree-2.8.0/tests/test_examples.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     5181 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_iterators.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2539 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_jsonexporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1801 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_jsonimporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)    15593 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_node.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2062 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_node_integrity.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2553 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_node_sep.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1726 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_node_symlink.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     4723 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_render.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     3167 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_resolver.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     2848 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_search.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     9717 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_special_methods_access.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1009 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_uniquedotexporter.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)     1261 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_util.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      811 2020-01-15 01:01:03.000000 anytree-2.8.0/tests/test_walker.py
--rw-rw-r--   0 djakschik (853001117) djakschik (853001296)      410 2020-01-15 01:01:03.000000 anytree-2.8.0/tox.ini
+-rw-r--r--   0        0        0    11357 2023-01-05 13:25:27.810703 anytree-2.9.0/LICENSE
+-rw-r--r--   0        0        0     6684 2023-06-25 19:19:27.462699 anytree-2.9.0/README.rst
+-rw-r--r--   0        0        0     1586 2023-06-25 19:19:27.462699 anytree-2.9.0/anytree/__init__.py
+-rw-r--r--   0        0        0     1606 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/cachedsearch.py
+-rw-r--r--   0        0        0      428 2023-06-25 20:19:09.395226 anytree-2.9.0/anytree/dotexport.py
+-rw-r--r--   0        0        0      207 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/exporter/__init__.py
+-rw-r--r--   0        0        0     3979 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/exporter/dictexporter.py
+-rw-r--r--   0        0        0    14985 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/exporter/dotexporter.py
+-rw-r--r--   0        0        0     2363 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/exporter/jsonexporter.py
+-rw-r--r--   0        0        0      111 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/importer/__init__.py
+-rw-r--r--   0        0        0     1530 2023-06-25 19:09:05.818704 anytree-2.9.0/anytree/importer/dictimporter.py
+-rw-r--r--   0        0        0     1936 2023-06-25 19:09:05.818704 anytree-2.9.0/anytree/importer/jsonimporter.py
+-rw-r--r--   0        0        0      806 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/__init__.py
+-rw-r--r--   0        0        0     1796 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/abstractiter.py
+-rw-r--r--   0        0        0     2204 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/levelordergroupiter.py
+-rw-r--r--   0        0        0     1614 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/levelorderiter.py
+-rw-r--r--   0        0        0     1746 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/postorderiter.py
+-rw-r--r--   0        0        0     1738 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/preorderiter.py
+-rw-r--r--   0        0        0     2049 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/iterators/zigzaggroupiter.py
+-rw-r--r--   0        0        0      711 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/node/__init__.py
+-rw-r--r--   0        0        0     3573 2023-06-25 19:19:27.462699 anytree-2.9.0/anytree/node/anynode.py
+-rw-r--r--   0        0        0      122 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/node/exceptions.py
+-rw-r--r--   0        0        0     2985 2023-06-25 19:09:05.818704 anytree-2.9.0/anytree/node/node.py
+-rw-r--r--   0        0        0    16390 2023-06-25 19:19:27.462699 anytree-2.9.0/anytree/node/nodemixin.py
+-rw-r--r--   0        0        0     1716 2023-06-25 19:09:05.818704 anytree-2.9.0/anytree/node/symlinknode.py
+-rw-r--r--   0        0        0     1953 2023-06-25 19:09:05.818704 anytree-2.9.0/anytree/node/symlinknodemixin.py
+-rw-r--r--   0        0        0      430 2023-01-05 13:25:27.810703 anytree-2.9.0/anytree/node/util.py
+-rw-r--r--   0        0        0    10624 2023-06-25 19:09:05.818704 anytree-2.9.0/anytree/render.py
+-rw-r--r--   0        0        0     9917 2023-01-05 13:25:27.814704 anytree-2.9.0/anytree/resolver.py
+-rw-r--r--   0        0        0     7330 2023-01-05 13:25:27.814704 anytree-2.9.0/anytree/search.py
+-rw-r--r--   0        0        0     2108 2023-01-05 13:25:27.814704 anytree-2.9.0/anytree/util/__init__.py
+-rw-r--r--   0        0        0     2786 2023-01-05 13:25:27.814704 anytree-2.9.0/anytree/walker.py
+-rw-r--r--   0        0        0     2187 2023-06-25 20:19:09.395226 anytree-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7612 1970-01-01 00:00:00.000000 anytree-2.9.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anytree-2.8.0/LICENSE` & `anytree-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anytree-2.8.0/README.rst` & `anytree-2.9.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 .. image:: https://badge.fury.io/py/anytree.svg
     :target: https://badge.fury.io/py/anytree
 
 .. image:: https://img.shields.io/pypi/dm/anytree.svg?label=pypi%20downloads
    :target: https://pypi.python.org/pypi/anytree
 
-.. image:: https://travis-ci.org/c0fec0de/anytree.svg?branch=master
-    :target: https://travis-ci.org/c0fec0de/anytree
+.. image:: https://readthedocs.org/projects/anytree/badge/?version=latest
+    :target: https://anytree.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://coveralls.io/repos/github/c0fec0de/anytree/badge.svg
     :target: https://coveralls.io/github/c0fec0de/anytree
 
-.. image:: https://readthedocs.org/projects/anytree/badge/?version=2.8.0
-    :target: http://anytree.readthedocs.io/en/2.8.0/?badge=2.8.0
+.. image:: https://readthedocs.org/projects/anytree/badge/?version=2.9.0
+    :target: http://anytree.readthedocs.io/en/2.9.0/?badge=2.9.0
 
-.. image:: https://codeclimate.com/github/c0fec0de/anytree.png
-    :target: https://codeclimate.com/github/c0fec0de/anytree
+.. image:: https://api.codeclimate.com/v1/badges/e6d325d6fd23a93aab20/maintainability
+   :target: https://codeclimate.com/github/c0fec0de/anytree/maintainability
+   :alt: Maintainability
 
 .. image:: https://img.shields.io/pypi/pyversions/anytree.svg
    :target: https://pypi.python.org/pypi/anytree
 
 .. image:: https://img.shields.io/badge/code%20style-pep8-brightgreen.svg
    :target: https://www.python.org/dev/peps/pep-0008/
 
 .. image:: https://img.shields.io/badge/code%20style-pep257-brightgreen.svg
    :target: https://www.python.org/dev/peps/pep-0257/
 
+.. image:: https://img.shields.io/badge/linter-pylint-%231674b1?style=flat
+   :target: https://www.pylint.org/
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
 Links
 =====
 
 * Documentation_
 * PyPI_
 * GitHub_
 * Changelog_
 * Issues_
 * Contributors_
 * If you enjoy anytree_
 
 .. image:: https://github.com/c0fec0de/anytree/raw/devel/docs/static/buymeacoffee.png
    :target: https://www.buymeacoffee.com/1oYX0sw
 
-.. _anytree: http://anytree.readthedocs.io/en/2.8.0/
-.. _Documentation: http://anytree.readthedocs.io/en/2.8.0/
-.. _PyPI: https://pypi.org/project/anytree/2.8.0/
+.. _anytree: http://anytree.readthedocs.io/en/2.9.0/
+.. _Documentation: http://anytree.readthedocs.io/en/2.9.0/
+.. _PyPI: https://pypi.org/project/anytree/2.9.0/
 .. _GitHub: https://github.com/c0fec0de/anytree
 .. _Changelog: https://github.com/c0fec0de/anytree/releases
 .. _Issues: https://github.com/c0fec0de/anytree/issues
 .. _Contributors: https://github.com/c0fec0de/anytree/graphs/contributors
 
-.. _Node: https://anytree.readthedocs.io/en/2.8.0/api/anytree.node.html#anytree.node.node.Node
-.. _RenderTree: https://anytree.readthedocs.io/en/2.8.0/api/anytree.render.html#anytree.render.RenderTree
-.. _DotExporter: https://anytree.readthedocs.io/en/2.8.0/exporter/dotexporter.html#anytree.exporter.dotexporter.DotExporter
-.. _NodeMixin: https://anytree.readthedocs.io/en/2.8.0/api/anytree.node.html#anytree.node.nodemixin.NodeMixin
-.. _Importers: https://anytree.readthedocs.io/en/2.8.0/importer.html
-.. _Exporters: https://anytree.readthedocs.io/en/2.8.0/exporter.html
+.. _Node: https://anytree.readthedocs.io/en/2.9.0/api/anytree.node.html#anytree.node.node.Node
+.. _RenderTree: https://anytree.readthedocs.io/en/2.9.0/api/anytree.render.html#anytree.render.RenderTree
+.. _UniqueDotExporter: https://anytree.readthedocs.io/en/2.9.0/exporter/dotexporter.html#anytree.exporter.dotexporter.UniqueDotExporter
+.. _NodeMixin: https://anytree.readthedocs.io/en/2.9.0/api/anytree.node.html#anytree.node.nodemixin.NodeMixin
+.. _Importers: https://anytree.readthedocs.io/en/2.9.0/importer.html
+.. _Exporters: https://anytree.readthedocs.io/en/2.9.0/exporter.html
 
 Getting started
 ---------------
 
 .. _getting_started:
 
 Usage is simple.
@@ -91,28 +98,28 @@
     ├── Jan
     └── Joe
 
 For details see Node_ and RenderTree_.
 
 **Visualization**
 
->>> from anytree.exporter import DotExporter
+>>> from anytree.exporter import UniqueDotExporter
 >>> # graphviz needs to be installed for the next line!
->>> DotExporter(udo).to_picture("udo.png")
+>>> UniqueDotExporter(udo).to_picture("udo.png")
 
-.. image:: http://anytree.readthedocs.io/en/latest/_images/udo.png
+.. image:: https://anytree.readthedocs.io/en/latest/_images/udo.png
 
-The DotExporter_ can be started at any node and has various formatting hookups:
+The UniqueDotExporter_ can be started at any node and has various formatting hookups:
 
->>> DotExporter(dan,
-...             nodeattrfunc=lambda node: "fixedsize=true, width=1, height=1, shape=diamond",
-...             edgeattrfunc=lambda parent, child: "style=bold"
+>>> UniqueDotExporter(dan,
+...                   nodeattrfunc=lambda node: "fixedsize=true, width=1, height=1, shape=diamond",
+...                   edgeattrfunc=lambda parent, child: "style=bold"
 ... ).to_picture("dan.png")
 
-.. image:: http://anytree.readthedocs.io/en/latest/_images/static/dan.png
+.. image:: https://anytree.readthedocs.io/en/latest/_images/dan.png
 
 There are various other Importers_ and Exporters_.
 
 **Manipulation**
 
 A second tree:
 
@@ -155,15 +162,15 @@
 Node('/Dan')
 ├── Node('/Dan/Jet')
 ├── Node('/Dan/Jan')
 └── Node('/Dan/Joe')
 
 **Extending any python class to become a tree node**
 
-The enitre tree magic is encapsulated by NodeMixin_
+The entire tree magic is encapsulated by NodeMixin_
 add it as base class and the class becomes a tree node:
 
 >>> from anytree import NodeMixin, RenderTree
 >>> class MyBaseClass(object):  # Just an example of a base class
 ...     foo = 4
 >>> class MyClass(MyBaseClass, NodeMixin):  # Add Node feature
 ...     def __init__(self, name, length, width, parent=None, children=None):
```

### Comparing `anytree-2.8.0/anytree/__init__.py` & `anytree-2.9.0/anytree/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # -*- coding: utf-8 -*-
 
 """Powerful and Lightweight Python Tree Data Structure."""
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 __author__ = "c0fec0de"
 __author_email__ = "c0fec0de@gmail.com"
 __description__ = """Powerful and Lightweight Python Tree Data Structure.."""
 __url__ = "https://github.com/c0fec0de/anytree"
 
-from .search import CountError  # noqa
-from .search import find  # noqa
-from .search import find_by_attr  # noqa
-from .search import findall  # noqa
-from .search import findall_by_attr  # noqa
+from . import cachedsearch  # noqa
+from . import util  # noqa
 from .iterators import LevelOrderGroupIter  # noqa
 from .iterators import LevelOrderIter  # noqa
 from .iterators import PostOrderIter  # noqa
 from .iterators import PreOrderIter  # noqa
 from .iterators import ZigZagGroupIter  # noqa
 from .node import AnyNode  # noqa
 from .node import LoopError  # noqa
@@ -30,15 +27,18 @@
 from .render import ContRoundStyle  # noqa
 from .render import ContStyle  # noqa
 from .render import DoubleStyle  # noqa
 from .render import RenderTree  # noqa
 from .resolver import ChildResolverError  # noqa
 from .resolver import Resolver  # noqa
 from .resolver import ResolverError  # noqa
-from .walker import WalkError  # noqa
+from .resolver import RootResolverError  # noqa
+from .search import CountError  # noqa
+from .search import find  # noqa
+from .search import find_by_attr  # noqa
+from .search import findall  # noqa
+from .search import findall_by_attr  # noqa
 from .walker import Walker  # noqa
-from . import cachedsearch  # noqa
-from . import util  # noqa
-
+from .walker import WalkError  # noqa
 
 # legacy
 LevelGroupOrderIter = LevelOrderGroupIter
```

### Comparing `anytree-2.8.0/anytree/cachedsearch.py` & `anytree-2.9.0/anytree/cachedsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 try:
     from fastcache import clru_cache as _cache
 except ImportError:
     from functools import wraps
 
     # dummy decorator which does NOT cache
     def _cache(size):
+        # pylint: disable=W0613
         def decorator(func):
             @wraps(func)
             def wrapped(*args, **kwargs):
                 return func(*args, **kwargs)
+
             return wrapped
+
         return decorator
 
 
 CACHE_SIZE = 32
 
 
 @_cache(CACHE_SIZE)
```

### Comparing `anytree-2.8.0/anytree/exporter/dictexporter.py` & `anytree-2.9.0/anytree/exporter/dictexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-
-class DictExporter(object):
-
+class DictExporter:
     def __init__(self, dictcls=dict, attriter=None, childiter=list, maxlevel=None):
         """
         Tree to dictionary exporter.
 
         Every node is converted to a dictionary with all instance
         attributes as key-value pairs.
         Child nodes are exported to the children attribute.
@@ -75,18 +73,22 @@
         return self.__export(node, self.dictcls, attriter, self.childiter)
 
     def __export(self, node, dictcls, attriter, childiter, level=1):
         attr_values = attriter(self._iter_attr_values(node))
         data = dictcls(attr_values)
         maxlevel = self.maxlevel
         if maxlevel is None or level < maxlevel:
-            children = [self.__export(child, dictcls, attriter, childiter, level=level + 1)
-                        for child in childiter(node.children)]
+            children = [
+                self.__export(child, dictcls, attriter, childiter, level=level + 1)
+                for child in childiter(node.children)
+            ]
             if children:
-                data['children'] = children
+                data["children"] = children
         return data
 
-    def _iter_attr_values(self, node):
+    @staticmethod
+    def _iter_attr_values(node):
+        # pylint: disable=C0103
         for k, v in node.__dict__.items():
-            if k in ('_NodeMixin__children', '_NodeMixin__parent'):
+            if k in ("_NodeMixin__children", "_NodeMixin__parent"):
                 continue
             yield k, v
```

### Comparing `anytree-2.8.0/anytree/exporter/dotexporter.py` & `anytree-2.9.0/anytree/exporter/dotexporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import codecs
 import logging
 import re
-from os import path
-from os import remove
+from os import path, remove
 from subprocess import check_call
 from tempfile import NamedTemporaryFile
 
 import six
 
 from anytree import PreOrderIter
 
 _RE_ESC = re.compile(r'["\\]')
 
 
-class DotExporter(object):
-
-    def __init__(self, node, graph="digraph", name="tree", options=None,
-                 indent=4, nodenamefunc=None, nodeattrfunc=None,
-                 edgeattrfunc=None, edgetypefunc=None, maxlevel=None):
+class DotExporter:
+    def __init__(
+        self,
+        node,
+        graph="digraph",
+        name="tree",
+        options=None,
+        indent=4,
+        nodenamefunc=None,
+        nodeattrfunc=None,
+        edgeattrfunc=None,
+        edgetypefunc=None,
+        maxlevel=None,
+    ):
         """
         Dot Language Exporter.
 
         Args:
             node (Node): start node.
 
         Keyword Args:
@@ -169,31 +177,33 @@
     def __iter__(self):
         # prepare
         indent = " " * self.indent
         nodenamefunc = self.nodenamefunc or self._default_nodenamefunc
         nodeattrfunc = self.nodeattrfunc or self._default_nodeattrfunc
         edgeattrfunc = self.edgeattrfunc or self._default_edgeattrfunc
         edgetypefunc = self.edgetypefunc or self._default_edgetypefunc
-        return self.__iter(indent, nodenamefunc, nodeattrfunc, edgeattrfunc,
-                           edgetypefunc)
+        return self.__iter(indent, nodenamefunc, nodeattrfunc, edgeattrfunc, edgetypefunc)
 
     @staticmethod
     def _default_nodenamefunc(node):
         return node.name
 
     @staticmethod
     def _default_nodeattrfunc(node):
+        # pylint: disable=W0613
         return None
 
     @staticmethod
     def _default_edgeattrfunc(node, child):
+        # pylint: disable=W0613
         return None
 
     @staticmethod
     def _default_edgetypefunc(node, child):
+        # pylint: disable=W0613
         return "->"
 
     def __iter(self, indent, nodenamefunc, nodeattrfunc, edgeattrfunc, edgetypefunc):
         yield "{self.graph} {self.name} {{".format(self=self)
         for option in self.__iter_options(indent):
             yield option
         for node in self.__iter_nodes(indent, nodenamefunc, nodeattrfunc):
@@ -220,16 +230,21 @@
         for node in PreOrderIter(self.node, maxlevel=maxlevel):
             nodename = nodenamefunc(node)
             for child in node.children:
                 childname = nodenamefunc(child)
                 edgeattr = edgeattrfunc(node, child)
                 edgetype = edgetypefunc(node, child)
                 edgeattr = " [%s]" % edgeattr if edgeattr is not None else ""
-                yield '%s"%s" %s "%s"%s;' % (indent, DotExporter.esc(nodename), edgetype,
-                                             DotExporter.esc(childname), edgeattr)
+                yield '%s"%s" %s "%s"%s;' % (
+                    indent,
+                    DotExporter.esc(nodename),
+                    edgetype,
+                    DotExporter.esc(childname),
+                    edgeattr,
+                )
 
     def to_dotfile(self, filename):
         """
         Write graph to `filename`.
 
         >>> from anytree import Node
         >>> root = Node("root")
@@ -258,39 +273,48 @@
         """
         Write graph to a temporary file and invoke `dot`.
 
         The output file type is automatically detected from the file suffix.
 
         *`graphviz` needs to be installed, before usage of this method.*
         """
+        # pylint: disable=W0703
         fileformat = path.splitext(filename)[1][1:]
         with NamedTemporaryFile("wb", delete=False) as dotfile:
             dotfilename = dotfile.name
             for line in self:
                 dotfile.write(("%s\n" % line).encode("utf-8"))
             dotfile.flush()
             cmd = ["dot", dotfilename, "-T", fileformat, "-o", filename]
             check_call(cmd)
         try:
             remove(dotfilename)
         except Exception:  # pragma: no cover
-            msg = 'Could not remove temporary file %s' % dotfilename
-            logging.getLogger(__name__).warn(msg)
+            logging.getLogger(__name__).warning("Could not remove temporary file %s", dotfilename)
 
     @staticmethod
     def esc(value):
         """Escape Strings."""
         return _RE_ESC.sub(lambda m: r"\%s" % m.group(0), six.text_type(value))
 
 
 class UniqueDotExporter(DotExporter):
-
-    def __init__(self, node, graph="digraph", name="tree", options=None,
-                 indent=4, nodenamefunc=None, nodeattrfunc=None,
-                 edgeattrfunc=None, edgetypefunc=None):
+    def __init__(
+        self,
+        node,
+        graph="digraph",
+        name="tree",
+        options=None,
+        indent=4,
+        nodenamefunc=None,
+        nodeattrfunc=None,
+        edgeattrfunc=None,
+        edgetypefunc=None,
+        maxlevel=None,
+    ):
         """
         Unqiue Dot Language Exporter.
 
         Handle trees with random or conflicting node names gracefully.
 
         Args:
             node (Node): start node.
@@ -318,14 +342,16 @@
                           and return the attributes.
 
             edgetypefunc: Function to which gives the edge type.
                           The function shall accept two `node` objects as
                           argument. The first the node and the second the child
                           and return the edge (i.e. '->').
 
+            maxlevel (int): Limit export to this number of levels.
+
         >>> from anytree import Node
         >>> root = Node("root")
         >>> s0 = Node("sub0", parent=root)
         >>> s0b = Node("s0", parent=s0)
         >>> s0a = Node("s0", parent=s0)
         >>> s1 = Node("sub1", parent=root)
         >>> s1a = Node("s1", parent=s1)
@@ -377,18 +403,27 @@
             "0x7f5c70449c60" [label="s0"];
             "0x7f5c70449cf0" [label="s0"];
             "0x7f5c70449af8" -> "0x7f5c70449bd0";
             "0x7f5c70449bd0" -> "0x7f5c70449c60";
             "0x7f5c70449bd0" -> "0x7f5c70449cf0";
         }
         """
-        super(UniqueDotExporter, self).__init__(node, graph=graph, name=name, options=options, indent=indent,
-                                                nodenamefunc=nodenamefunc, nodeattrfunc=nodeattrfunc,
-                                                edgeattrfunc=edgeattrfunc, edgetypefunc=edgetypefunc)
+        super(UniqueDotExporter, self).__init__(
+            node,
+            graph=graph,
+            name=name,
+            options=options,
+            indent=indent,
+            nodenamefunc=nodenamefunc,
+            nodeattrfunc=nodeattrfunc,
+            edgeattrfunc=edgeattrfunc,
+            edgetypefunc=edgetypefunc,
+            maxlevel=maxlevel,
+        )
 
     @staticmethod
     def _default_nodenamefunc(node):
         return hex(id(node))
 
     @staticmethod
     def _default_nodeattrfunc(node):
-        return 'label="%s"' % (node.name)
+        return 'label="%s"' % (node.name,)
```

### Comparing `anytree-2.8.0/anytree/exporter/jsonexporter.py` & `anytree-2.9.0/anytree/exporter/jsonexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 
 from .dictexporter import DictExporter
 
 
-class JsonExporter(object):
-
+class JsonExporter:
     def __init__(self, dictexporter=None, maxlevel=None, **kwargs):
         """
         Tree to JSON exporter.
 
         The tree is converted to a dictionary via `dictexporter` and exported to JSON.
 
         Keyword Arguments:
```

### Comparing `anytree-2.8.0/anytree/importer/dictimporter.py` & `anytree-2.9.0/anytree/importer/dictimporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 from anytree import AnyNode
 
 
-class DictImporter(object):
-
+class DictImporter:
     def __init__(self, nodecls=AnyNode):
-        u"""
+        """
         Import Tree from dictionary.
 
         Every dictionary is converted to an instance of `nodecls`.
         The dictionaries listed in the children attribute are converted
         likewise and added as children.
 
         Keyword Args:
```

### Comparing `anytree-2.8.0/anytree/importer/jsonimporter.py` & `anytree-2.9.0/anytree/importer/jsonimporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 import json
 
 from .dictimporter import DictImporter
 
 
-class JsonImporter(object):
-
+class JsonImporter:
     def __init__(self, dictimporter=None, **kwargs):
-        u"""
+        """
         Import Tree from JSON.
 
         The JSON is read and converted to a dictionary via `dictimporter`.
 
         Keyword Arguments:
             dictimporter: Dictionary Importer used (see :any:`DictImporter`).
             kwargs: All other arguments are passed to
```

### Comparing `anytree-2.8.0/anytree/iterators/__init__.py` & `anytree-2.9.0/anytree/iterators/__init__.py`

 * *Files identical despite different names*

### Comparing `anytree-2.8.0/anytree/iterators/abstractiter.py` & `anytree-2.9.0/anytree/iterators/abstractiter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import six
 
 
 class AbstractIter(six.Iterator):
+    # pylint: disable=R0205
 
     def __init__(self, node, filter_=None, stop=None, maxlevel=None):
         """
         Iterate over tree starting at `node`.
 
         Base class for all iterators.
 
@@ -26,18 +27,20 @@
         filter_ = self.filter_ or AbstractIter.__default_filter
         stop = self.stop or AbstractIter.__default_stop
         children = [] if AbstractIter._abort_at_level(1, maxlevel) else AbstractIter._get_children([node], stop)
         return self._iter(children, filter_, stop, maxlevel)
 
     @staticmethod
     def __default_filter(node):
+        # pylint: disable=W0613
         return True
 
     @staticmethod
     def __default_stop(node):
+        # pylint: disable=W0613
         return False
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.__iter is None:
```

### Comparing `anytree-2.8.0/anytree/iterators/levelordergroupiter.py` & `anytree-2.9.0/anytree/iterators/levelordergroupiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     [['f'], ['b', 'g'], ['a', 'i'], ['h']]
     """
 
     @staticmethod
     def _iter(children, filter_, stop, maxlevel):
         level = 1
         while children:
-            yield tuple([child for child in children if filter_(child)])
+            yield tuple(child for child in children if filter_(child))
             level += 1
             if AbstractIter._abort_at_level(level, maxlevel):
                 break
             children = LevelOrderGroupIter._get_grandchildren(children, stop)
 
     @staticmethod
     def _get_grandchildren(children, stop):
```

### Comparing `anytree-2.8.0/anytree/iterators/levelorderiter.py` & `anytree-2.9.0/anytree/iterators/levelorderiter.py`

 * *Files identical despite different names*

### Comparing `anytree-2.8.0/anytree/iterators/postorderiter.py` & `anytree-2.9.0/anytree/iterators/postorderiter.py`

 * *Files identical despite different names*

### Comparing `anytree-2.8.0/anytree/iterators/preorderiter.py` & `anytree-2.9.0/anytree/iterators/preorderiter.py`

 * *Files identical despite different names*

### Comparing `anytree-2.8.0/anytree/iterators/zigzaggroupiter.py` & `anytree-2.9.0/anytree/iterators/zigzaggroupiter.py`

 * *Files identical despite different names*

### Comparing `anytree-2.8.0/anytree/node/__init__.py` & `anytree-2.9.0/anytree/node/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 * :any:`AnyNode`: a generic tree node with any number of attributes.
 * :any:`Node`: a simple tree node with at least a name attribute and any number of additional attributes.
 * :any:`NodeMixin`: extends any python class to a tree node.
 * :any:`SymlinkNode`: Tree node which references to another tree node.
 * :any:`SymlinkNodeMixin`: extends any Python class to a symbolic link to a tree node.
 """
 
-from .anynode import AnyNode   # noqa
-from .exceptions import LoopError   # noqa
-from .exceptions import TreeError   # noqa
-from .node import Node   # noqa
-from .nodemixin import NodeMixin   # noqa
-from .symlinknode import SymlinkNode   # noqa
-from .symlinknodemixin import SymlinkNodeMixin   # noqa
+from .anynode import AnyNode  # noqa
+from .exceptions import LoopError  # noqa
+from .exceptions import TreeError  # noqa
+from .node import Node  # noqa
+from .nodemixin import NodeMixin  # noqa
+from .symlinknode import SymlinkNode  # noqa
+from .symlinknodemixin import SymlinkNodeMixin  # noqa
```

### Comparing `anytree-2.8.0/anytree/node/anynode.py` & `anytree-2.9.0/anytree/node/anynode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
 from .nodemixin import NodeMixin
 from .util import _repr
 
 
-class AnyNode(NodeMixin, object):
-
+class AnyNode(NodeMixin):
     def __init__(self, parent=None, children=None, **kwargs):
-        u"""
+        """
         A generic tree node with any `kwargs`.
 
         Keyword Args:
             parent: Reference to parent node.
             children: Iterable with child nodes.
             *: Any other given attribute is just stored as object attribute.
 
-        Other than :any:`Node` this class has no default idenifier.
+        Other than :any:`Node` this class has no default identifier.
         It is up to the user to use other attributes for identification.
 
         The `parent` attribute refers the parent node:
 
         >>> from anytree import AnyNode, RenderTree
         >>> root = AnyNode(id="root")
         >>> s0 = AnyNode(id="sub0", parent=root)
@@ -42,56 +41,60 @@
         │   └── AnyNode(id='sub0A')
         └── AnyNode(id='sub1')
             ├── AnyNode(id='sub1A')
             ├── AnyNode(bar=8, id='sub1B')
             └── AnyNode(id='sub1C')
                 └── AnyNode(id='sub1Ca')
 
-        The same tree can be constructed by using the `children` attribute:
-
-        >>> root = AnyNode(id="root", children=[
-        ...     AnyNode(id="sub0", children=[
-        ...         AnyNode(id="sub0B", foo=4, bar=109),
-        ...         AnyNode(id="sub0A"),
-        ...     ]),
-        ...     AnyNode(id="sub1", children=[
-        ...         AnyNode(id="sub1A"),
-        ...         AnyNode(id="sub1B", bar=8),
-        ...         AnyNode(id="sub1C", children=[
-        ...             AnyNode(id="sub1Ca"),
-        ...         ]),
-        ...     ]),
-        ... ])
-
         >>> print(RenderTree(root))
         AnyNode(id='root')
         ├── AnyNode(id='sub0')
         │   ├── AnyNode(bar=109, foo=4, id='sub0B')
         │   └── AnyNode(id='sub0A')
         └── AnyNode(id='sub1')
             ├── AnyNode(id='sub1A')
             ├── AnyNode(bar=8, id='sub1B')
             └── AnyNode(id='sub1C')
                 └── AnyNode(id='sub1Ca')
 
         Node attributes can be added, modified and deleted the pythonic way:
 
         >>> root.new = 'a new attribute'
+        >>> s0b
+        AnyNode(bar=109, foo=4, id='sub0B')
         >>> s0b.bar = 110  # modified
+        >>> s0b
+        AnyNode(bar=110, foo=4, id='sub0B')
         >>> del s1b.bar
         >>> print(RenderTree(root))
         AnyNode(id='root', new='a new attribute')
         ├── AnyNode(id='sub0')
-        │   ├── AnyNode(bar=109, foo=4, id='sub0B')
+        │   ├── AnyNode(bar=110, foo=4, id='sub0B')
         │   └── AnyNode(id='sub0A')
         └── AnyNode(id='sub1')
             ├── AnyNode(id='sub1A')
-            ├── AnyNode(bar=8, id='sub1B')
+            ├── AnyNode(id='sub1B')
             └── AnyNode(id='sub1C')
                 └── AnyNode(id='sub1Ca')
+
+        The same tree can be constructed by using the `children` attribute:
+
+        >>> root = AnyNode(id="root", children=[
+        ...     AnyNode(id="sub0", children=[
+        ...         AnyNode(id="sub0B", foo=4, bar=109),
+        ...         AnyNode(id="sub0A"),
+        ...     ]),
+        ...     AnyNode(id="sub1", children=[
+        ...         AnyNode(id="sub1A"),
+        ...         AnyNode(id="sub1B", bar=8),
+        ...         AnyNode(id="sub1C", children=[
+        ...             AnyNode(id="sub1Ca"),
+        ...         ]),
+        ...     ]),
+        ... ])
         """
         self.__dict__.update(kwargs)
         self.parent = parent
         if children:
             self.children = children
 
     def __repr__(self):
```

### Comparing `anytree-2.8.0/anytree/node/node.py` & `anytree-2.9.0/anytree/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from .nodemixin import NodeMixin
 from .util import _repr
 
 
-class Node(NodeMixin, object):
-
+class Node(NodeMixin):
     def __init__(self, name, parent=None, children=None, **kwargs):
-        u"""
+        """
         A simple tree node with a `name` and any `kwargs`.
 
         Args:
-            name: A name or any other object this node can reference to as idendifier.
+            name: A name or any other object this node can reference to as identifier.
 
         Keyword Args:
             parent: Reference to parent node.
             children: Iterable with child nodes.
             *: Any other given attribute is just stored as object attribute.
 
         Other than :any:`AnyNode` this class has at least the `name` attribute,
```

### Comparing `anytree-2.8.0/anytree/node/nodemixin.py` & `anytree-2.9.0/anytree/node/nodemixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 
 import warnings
 
 from anytree.iterators import PreOrderIter
 
-from .exceptions import LoopError
-from .exceptions import TreeError
+from .exceptions import LoopError, TreeError
 
 
-class NodeMixin(object):
+class NodeMixin:
 
     separator = "/"
 
-    u"""
+    """
     The :any:`NodeMixin` class extends any Python class to a tree node.
 
     The only tree relevant information is the `parent` attribute.
     If `None` the :any:`NodeMixin` is root node.
     If set to another node, the :any:`NodeMixin` becomes the child of it.
 
     The `children` attribute can be used likewise.
@@ -77,15 +76,15 @@
     my0      0 0
     ├── my1  1 0
     └── my2  0 2
     """
 
     @property
     def parent(self):
-        u"""
+        """
         Parent Node.
 
         On set, the node is detached from any previous parent node and attached
         to the new node.
 
         >>> from anytree import Node, RenderTree
         >>> udo = Node("Udo")
@@ -111,71 +110,70 @@
 
         >>> marc.is_root
         False
         >>> marc.parent = None
         >>> marc.is_root
         True
         """
-        try:
+        if hasattr(self, "_NodeMixin__parent"):
             return self.__parent
-        except AttributeError:
-            return None
+        return None
 
     @parent.setter
     def parent(self, value):
         if value is not None and not isinstance(value, NodeMixin):
-            msg = "Parent node %r is not of type 'NodeMixin'." % value
+            msg = "Parent node %r is not of type 'NodeMixin'." % (value,)
             raise TreeError(msg)
-        try:
+        if hasattr(self, "_NodeMixin__parent"):
             parent = self.__parent
-        except AttributeError:
+        else:
             parent = None
         if parent is not value:
             self.__check_loop(value)
             self.__detach(parent)
             self.__attach(value)
 
     def __check_loop(self, node):
         if node is not None:
             if node is self:
                 msg = "Cannot set parent. %r cannot be parent of itself."
-                raise LoopError(msg % self)
+                raise LoopError(msg % (self,))
             if any(child is self for child in node.iter_path_reverse()):
                 msg = "Cannot set parent. %r is parent of %r."
                 raise LoopError(msg % (self, node))
 
     def __detach(self, parent):
+        # pylint: disable=W0212,W0238
         if parent is not None:
             self._pre_detach(parent)
             parentchildren = parent.__children_or_empty
             assert any(child is self for child in parentchildren), "Tree is corrupt."  # pragma: no cover
             # ATOMIC START
             parent.__children = [child for child in parentchildren if child is not self]
             self.__parent = None
             # ATOMIC END
             self._post_detach(parent)
 
     def __attach(self, parent):
+        # pylint: disable=W0212
         if parent is not None:
             self._pre_attach(parent)
             parentchildren = parent.__children_or_empty
             assert not any(child is self for child in parentchildren), "Tree is corrupt."  # pragma: no cover
             # ATOMIC START
             parentchildren.append(self)
             self.__parent = parent
             # ATOMIC END
             self._post_attach(parent)
 
     @property
     def __children_or_empty(self):
-        try:
-            return self.__children
-        except AttributeError:
+        if not hasattr(self, "_NodeMixin__children"):
             self.__children = []
-            return self.__children
+        return self.__children
 
     @property
     def children(self):
         """
         All child nodes.
 
         >>> from anytree import Node
@@ -225,21 +223,21 @@
         return tuple(self.__children_or_empty)
 
     @staticmethod
     def __check_children(children):
         seen = set()
         for child in children:
             if not isinstance(child, NodeMixin):
-                msg = "Cannot add non-node object %r. It is not a subclass of 'NodeMixin'." % child
+                msg = "Cannot add non-node object %r. It is not a subclass of 'NodeMixin'." % (child,)
                 raise TreeError(msg)
             childid = id(child)
             if childid not in seen:
                 seen.add(childid)
             else:
-                msg = "Cannot add node %r multiple times as child." % child
+                msg = "Cannot add node %r multiple times as child." % (child,)
                 raise TreeError(msg)
 
     @children.setter
     def children(self, children):
         # convert iterable to tuple
         children = tuple(children)
         NodeMixin.__check_children(children)
@@ -264,32 +262,28 @@
         for child in self.children:
             child.parent = None
         assert len(self.children) == 0
         self._post_detach_children(children)
 
     def _pre_detach_children(self, children):
         """Method call before detaching `children`."""
-        pass
 
     def _post_detach_children(self, children):
         """Method call after detaching `children`."""
-        pass
 
     def _pre_attach_children(self, children):
         """Method call before attaching `children`."""
-        pass
 
     def _post_attach_children(self, children):
         """Method call after attaching `children`."""
-        pass
 
     @property
     def path(self):
         """
-        Path of this `Node`.
+        Path from root node down to this `Node`.
 
         >>> from anytree import Node
         >>> udo = Node("Udo")
         >>> marc = Node("Marc", parent=udo)
         >>> lian = Node("Lian", parent=marc)
         >>> udo.path
         (Node('/Udo'),)
@@ -298,15 +292,15 @@
         >>> lian.path
         (Node('/Udo'), Node('/Udo/Marc'), Node('/Udo/Marc/Lian'))
         """
         return self._path
 
     def iter_path_reverse(self):
         """
-        Iterate up the tree from the current node.
+        Iterate up the tree from the current node to the root node.
 
         >>> from anytree import Node
         >>> udo = Node("Udo")
         >>> marc = Node("Marc", parent=udo)
         >>> lian = Node("Lian", parent=marc)
         >>> for node in udo.iter_path_reverse():
         ...     print(node)
@@ -421,16 +415,15 @@
         (Node('/Udo/Marc/Loui'), Node('/Udo/Marc/Lazy'))
         >>> loui.siblings
         (Node('/Udo/Marc/Lian'), Node('/Udo/Marc/Lazy'))
         """
         parent = self.parent
         if parent is None:
             return tuple()
-        else:
-            return tuple(node for node in parent.children if node is not self)
+        return tuple(node for node in parent.children if node is not self)
 
     @property
     def leaves(self):
         """
         Tuple of all leaf nodes.
 
         >>> from anytree import Node
@@ -497,16 +490,15 @@
         1
         >>> lian.height
         0
         """
         children = self.__children_or_empty
         if children:
             return max(child.height for child in children) + 1
-        else:
-            return 0
+        return 0
 
     @property
     def depth(self):
         """
         Number of edges to the root `Node`.
 
         >>> from anytree import Node
@@ -517,26 +509,49 @@
         0
         >>> marc.depth
         1
         >>> lian.depth
         2
         """
         # count without storing the entire path
-        for i, _ in enumerate(self.iter_path_reverse()):
+        # pylint: disable=W0631
+        for depth, _ in enumerate(self.iter_path_reverse()):
+            continue
+        return depth
+
+    @property
+    def size(self):
+        """
+        Tree size --- the number of nodes in tree starting at this node.
+
+        >>> from anytree import Node
+        >>> udo = Node("Udo")
+        >>> marc = Node("Marc", parent=udo)
+        >>> lian = Node("Lian", parent=marc)
+        >>> loui = Node("Loui", parent=marc)
+        >>> soe = Node("Soe", parent=lian)
+        >>> udo.size
+        5
+        >>> marc.size
+        4
+        >>> lian.size
+        2
+        >>> loui.size
+        1
+        """
+        # count without storing the entire path
+        # pylint: disable=W0631
+        for size, _ in enumerate(PreOrderIter(self), 1):
             continue
-        return i
+        return size
 
     def _pre_detach(self, parent):
         """Method call before detaching from `parent`."""
-        pass
 
     def _post_detach(self, parent):
         """Method call after detaching from `parent`."""
-        pass
 
     def _pre_attach(self, parent):
         """Method call before attaching to `parent`."""
-        pass
 
     def _post_attach(self, parent):
         """Method call after attaching to `parent`."""
-        pass
```

### Comparing `anytree-2.8.0/anytree/node/symlinknode.py` & `anytree-2.9.0/anytree/node/symlinknode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 from .symlinknodemixin import SymlinkNodeMixin
 from .util import _repr
 
 
 class SymlinkNode(SymlinkNodeMixin):
-
     def __init__(self, target, parent=None, children=None, **kwargs):
-        u"""
+        """
         Tree node which references to another tree node.
 
         Args:
             target: Symbolic Link Target. Another tree node, which is refered to.
 
         Keyword Args:
             parent: Reference to parent node.
@@ -47,8 +46,8 @@
         self.target = target
         self.target.__dict__.update(kwargs)
         self.parent = parent
         if children:
             self.children = children
 
     def __repr__(self):
-        return _repr(self, [repr(self.target)], nameblacklist=("target", ))
+        return _repr(self, [repr(self.target)], nameblacklist=("target",))
```

### Comparing `anytree-2.8.0/anytree/node/symlinknodemixin.py` & `anytree-2.9.0/anytree/node/symlinknodemixin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from .nodemixin import NodeMixin
 
 
 class SymlinkNodeMixin(NodeMixin):
-    u"""
+    """
     The :any:`SymlinkNodeMixin` class extends any Python class to a symbolic link to a tree node.
 
     The class **MUST** have a `target` attribute refering to another tree node.
     The :any:`SymlinkNodeMixin` class has its own parent and its own child nodes.
     All other attribute accesses are just forwarded to the target node.
     A minimal implementation looks like (see :any:`SymlinkNode` for a full implemenation):
 
@@ -42,17 +42,16 @@
     >>> s1.foo
     9
     >>> l.foo
     9
     """
 
     def __getattr__(self, name):
-        if name in ('_NodeMixin__parent', '_NodeMixin__children'):
+        if name in ("_NodeMixin__parent", "_NodeMixin__children"):
             return super(SymlinkNodeMixin, self).__getattr__(name)
-        else:
-            return getattr(self.target, name)
+        return getattr(self.target, name)
 
     def __setattr__(self, name, value):
-        if name in ('_NodeMixin__parent', '_NodeMixin__children', 'parent', 'children', 'target'):
+        if name in ("_NodeMixin__parent", "_NodeMixin__children", "parent", "children", "target"):
             super(SymlinkNodeMixin, self).__setattr__(name, value)
         else:
-            return setattr(self.target, name, value)
+            setattr(self.target, name, value)
```

### Comparing `anytree-2.8.0/anytree/render.py` & `anytree-2.9.0/anytree/render.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import collections
 
 import six
 
 Row = collections.namedtuple("Row", ("pre", "fill", "node"))
 
 
-class AbstractStyle(object):
-
+class AbstractStyle:
     def __init__(self, vertical, cont, end):
         """
         Tree Render Style.
 
         Args:
 
             vertical: Sign for vertical line.
@@ -39,23 +38,22 @@
             cont,
             end,
         )
 
     @property
     def empty(self):
         """Empty string as placeholder."""
-        return ' ' * len(self.end)
+        return " " * len(self.end)
 
     def __repr__(self):
         classname = self.__class__.__name__
         return "%s()" % classname
 
 
 class AsciiStyle(AbstractStyle):
-
     def __init__(self):
         """
         Ascii style.
 
         >>> from anytree import Node, RenderTree
         >>> root = Node("root")
         >>> s0 = Node("sub0", parent=root)
@@ -66,21 +64,20 @@
         >>> print(RenderTree(root, style=AsciiStyle()))
         Node('/root')
         |-- Node('/root/sub0')
         |   |-- Node('/root/sub0/sub0B')
         |   +-- Node('/root/sub0/sub0A')
         +-- Node('/root/sub1')
         """
-        super(AsciiStyle, self).__init__(u'|   ', u'|-- ', u'+-- ')
+        super(AsciiStyle, self).__init__("|   ", "|-- ", "+-- ")
 
 
 class ContStyle(AbstractStyle):
-
     def __init__(self):
-        u"""
+        """
         Continued style, without gaps.
 
         >>> from anytree import Node, RenderTree
         >>> root = Node("root")
         >>> s0 = Node("sub0", parent=root)
         >>> s0b = Node("sub0B", parent=s0)
         >>> s0a = Node("sub0A", parent=s0)
@@ -89,23 +86,20 @@
         >>> print(RenderTree(root, style=ContStyle()))
         Node('/root')
         ├── Node('/root/sub0')
         │   ├── Node('/root/sub0/sub0B')
         │   └── Node('/root/sub0/sub0A')
         └── Node('/root/sub1')
         """
-        super(ContStyle, self).__init__(u'\u2502   ',
-                                        u'\u251c\u2500\u2500 ',
-                                        u'\u2514\u2500\u2500 ')
+        super(ContStyle, self).__init__("\u2502   ", "\u251c\u2500\u2500 ", "\u2514\u2500\u2500 ")
 
 
 class ContRoundStyle(AbstractStyle):
-
     def __init__(self):
-        u"""
+        """
         Continued style, without gaps, round edges.
 
         >>> from anytree import Node, RenderTree
         >>> root = Node("root")
         >>> s0 = Node("sub0", parent=root)
         >>> s0b = Node("sub0B", parent=s0)
         >>> s0a = Node("sub0A", parent=s0)
@@ -114,23 +108,20 @@
         >>> print(RenderTree(root, style=ContRoundStyle()))
         Node('/root')
         ├── Node('/root/sub0')
         │   ├── Node('/root/sub0/sub0B')
         │   ╰── Node('/root/sub0/sub0A')
         ╰── Node('/root/sub1')
         """
-        super(ContRoundStyle, self).__init__(u'\u2502   ',
-                                             u'\u251c\u2500\u2500 ',
-                                             u'\u2570\u2500\u2500 ')
+        super(ContRoundStyle, self).__init__("\u2502   ", "\u251c\u2500\u2500 ", "\u2570\u2500\u2500 ")
 
 
 class DoubleStyle(AbstractStyle):
-
     def __init__(self):
-        u"""
+        """
         Double line style, without gaps.
 
         >>> from anytree import Node, RenderTree
         >>> root = Node("root")
         >>> s0 = Node("sub0", parent=root)
         >>> s0b = Node("sub0B", parent=s0)
         >>> s0a = Node("sub0A", parent=s0)
@@ -140,24 +131,21 @@
         Node('/root')
         ╠══ Node('/root/sub0')
         ║   ╠══ Node('/root/sub0/sub0B')
         ║   ╚══ Node('/root/sub0/sub0A')
         ╚══ Node('/root/sub1')
 
         """
-        super(DoubleStyle, self).__init__(u'\u2551   ',
-                                          u'\u2560\u2550\u2550 ',
-                                          u'\u255a\u2550\u2550 ')
+        super(DoubleStyle, self).__init__("\u2551   ", "\u2560\u2550\u2550 ", "\u255a\u2550\u2550 ")
 
 
 @six.python_2_unicode_compatible
-class RenderTree(object):
-
+class RenderTree:
     def __init__(self, node, style=ContStyle(), childiter=list, maxlevel=None):
-        u"""
+        """
         Render tree starting at `node`.
 
         Keyword Args:
             style (AbstractStyle): Render Style.
             childiter: Child iterator.
             maxlevel: Limit rendering to this depth.
 
@@ -280,42 +268,39 @@
     def __next(self, node, continues, level=0):
         yield RenderTree.__item(node, continues, self.style)
         children = node.children
         level += 1
         if children and (self.maxlevel is None or level < self.maxlevel):
             children = self.childiter(children)
             for child, is_last in _is_last(children):
-                for grandchild in self.__next(child, continues + (not is_last, ), level=level):
+                for grandchild in self.__next(child, continues + (not is_last,), level=level):
                     yield grandchild
 
     @staticmethod
     def __item(node, continues, style):
         if not continues:
-            return Row(u'', u'', node)
-        else:
-            items = [style.vertical if cont else style.empty for cont in continues]
-            indent = ''.join(items[:-1])
-            branch = style.cont if continues[-1] else style.end
-            pre = indent + branch
-            fill = ''.join(items)
-            return Row(pre, fill, node)
+            return Row("", "", node)
+        items = [style.vertical if cont else style.empty for cont in continues]
+        indent = "".join(items[:-1])
+        branch = style.cont if continues[-1] else style.end
+        pre = indent + branch
+        fill = "".join(items)
+        return Row(pre, fill, node)
 
     def __str__(self):
         lines = ["%s%r" % (pre, node) for pre, _, node in self]
         return "\n".join(lines)
 
     def __repr__(self):
         classname = self.__class__.__name__
-        args = [repr(self.node),
-                "style=%s" % repr(self.style),
-                "childiter=%s" % repr(self.childiter)]
+        args = [repr(self.node), "style=%s" % repr(self.style), "childiter=%s" % repr(self.childiter)]
         return "%s(%s)" % (classname, ", ".join(args))
 
     def by_attr(self, attrname="name"):
-        u"""
+        """
         Return rendered tree with node attribute `attrname`.
 
         >>> from anytree import AnyNode, RenderTree
         >>> root = AnyNode(id="root")
         >>> s0 = AnyNode(id="sub0", parent=root)
         >>> s0b = AnyNode(id="sub0B", parent=s0, foo=4, bar=109)
         >>> s0a = AnyNode(id="sub0A", parent=s0)
@@ -332,24 +317,25 @@
         └── sub1
             ├── sub1A
             ├── sub1B
             └── sub1C
                 └── sub1Ca
 
         """
+
         def get():
             for pre, fill, node in self:
                 attr = attrname(node) if callable(attrname) else getattr(node, attrname, "")
                 if isinstance(attr, (list, tuple)):
                     lines = attr
                 else:
                     lines = str(attr).split("\n")
-                yield u"%s%s" % (pre, lines[0])
+                yield "%s%s" % (pre, lines[0])
                 for line in lines[1:]:
-                    yield u"%s%s" % (fill, line)
+                    yield "%s%s" % (fill, line)
 
         return "\n".join(get())
 
 
 def _is_last(iterable):
     iter_ = iter(iterable)
     try:
```

### Comparing `anytree-2.8.0/anytree/resolver.py` & `anytree-2.9.0/anytree/resolver.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 from __future__ import print_function
 
 import re
 
 _MAXCACHE = 20
 
 
-class Resolver(object):
+class Resolver:
 
     _match_cache = {}
 
-    def __init__(self, pathattr='name'):
-        """Resolve :any:`NodeMixin` paths using attribute `pathattr`."""
+    def __init__(self, pathattr="name", ignorecase=False):
+        """
+        Resolve :any:`NodeMixin` paths using attribute `pathattr`.
+
+        Keyword Args:
+            name (str): Name of the node attribute to be used for resolving
+            ignorecase (bool): Enable case insensisitve handling.
+        """
         super(Resolver, self).__init__()
         self.pathattr = pathattr
+        self.ignorecase = ignorecase
 
     def get(self, node, path):
         """
         Return instance at `path`.
 
         An example module tree:
 
@@ -61,28 +68,53 @@
         Traceback (most recent call last):
           ...
         anytree.resolver.ResolverError: root node missing. root is '/top'.
         >>> r.get(sub0sub0, "/bar")
         Traceback (most recent call last):
           ...
         anytree.resolver.ResolverError: unknown root node '/bar'. root is '/top'.
+
+        Going above the root node raises a :any:`RootResolverError`:
+
+        >>> r.get(top, "..")
+        Traceback (most recent call last):
+            ...
+        anytree.resolver.RootResolverError: Cannot go above root node Node('/top')
+
+        .. note:: Please not that :any:`get()` returned `None` in exactly that case above,
+                  which was a bug until version 1.8.1.
+
+        Case insensitive matching:
+
+        >>> r.get(top, '/TOP')
+        Traceback (most recent call last):
+            ...
+        anytree.resolver.ResolverError: unknown root node '/TOP'. root is '/top'.
+
+        >>> r = Resolver('name', ignorecase=True)
+        >>> r.get(top, '/TOp')
+        Node('/top')
         """
-        node, parts = self.__start(node, path)
+        node, parts = self.__start(node, path, self.__cmp)
         for part in parts:
             if part == "..":
-                node = node.parent
+                parent = node.parent
+                if parent is None:
+                    raise RootResolverError(node)
+                node = parent
             elif part in ("", "."):
                 pass
             else:
                 node = self.__get(node, part)
         return node
 
     def __get(self, node, name):
+        namestr = str(name)
         for child in node.children:
-            if str(_getattr(child, self.pathattr)) == name:
+            if self.__cmp(_getattr(child, self.pathattr), namestr):
                 return child
         raise ChildResolverError(node, name, self.pathattr)
 
     def glob(self, node, path):
         """
         Return instances at `path` supporting wildcards.
 
@@ -138,108 +170,135 @@
         Traceback (most recent call last):
           ...
         anytree.resolver.ResolverError: root node missing. root is '/top'.
         >>> r.glob(sub0sub0, "/bar")
         Traceback (most recent call last):
           ...
         anytree.resolver.ResolverError: unknown root node '/bar'. root is '/top'.
+
+        Going above the root node raises a :any:`RootResolverError`:
+
+        >>> r.glob(top, "..")
+        Traceback (most recent call last):
+            ...
+        anytree.resolver.RootResolverError: Cannot go above root node Node('/top')
         """
-        node, parts = self.__start(node, path)
+        node, parts = self.__start(node, path, self.__match)
         return self.__glob(node, parts)
 
-    def __start(self, node, path):
+    def __start(self, node, path, cmp_):
         sep = node.separator
         parts = path.split(sep)
+        # resolve root
         if path.startswith(sep):
             node = node.root
-            rootpart = str(_getattr(node, self.pathattr))
+            rootpart = _getattr(node, self.pathattr)
             parts.pop(0)
             if not parts[0]:
                 msg = "root node missing. root is '%s%s'."
                 raise ResolverError(node, "", msg % (sep, str(rootpart)))
-            elif parts[0] != rootpart:
+            if not cmp_(rootpart, parts[0]):
                 msg = "unknown root node '%s%s'. root is '%s%s'."
                 raise ResolverError(node, "", msg % (sep, parts[0], sep, str(rootpart)))
             parts.pop(0)
         return node, parts
 
     def __glob(self, node, parts):
+        assert node is not None
         nodes = []
-        name = parts[0]
-        remainder = parts[1:]
-        # handle relative
-        if name == "..":
-            nodes += self.__glob(node.parent, remainder)
-        elif name in ("", "."):
-            nodes += self.__glob(node, remainder)
+        if parts:
+            name = parts[0]
+            remainder = parts[1:]
+            # handle relative
+            if name == "..":
+                parent = node.parent
+                if parent is None:
+                    raise RootResolverError(node)
+                nodes += self.__glob(parent, remainder)
+            elif name in ("", "."):
+                nodes += self.__glob(node, remainder)
+            else:
+                matches = self.__find(node, name, remainder)
+                if not matches and not Resolver.is_wildcard(name):
+                    raise ChildResolverError(node, name, self.pathattr)
+                nodes += matches
         else:
-            matches = self.__find(node, name, remainder)
-            if not matches and not Resolver.is_wildcard(name):
-                raise ChildResolverError(node, name, self.pathattr)
-            nodes += matches
+            nodes = [node]
         return nodes
 
     def __find(self, node, pat, remainder):
         matches = []
         for child in node.children:
-            name = str(_getattr(child, self.pathattr))
+            name = _getattr(child, self.pathattr)
             try:
-                if Resolver.__match(name, pat):
+                if self.__match(name, pat):
                     if remainder:
                         matches += self.__glob(child, remainder)
                     else:
                         matches.append(child)
             except ResolverError as exc:
                 if not Resolver.is_wildcard(pat):
                     raise exc
         return matches
 
     @staticmethod
     def is_wildcard(path):
         """Return `True` is a wildcard."""
         return "?" in path or "*" in path
 
-    @staticmethod
-    def __match(name, pat):
+    def __match(self, name, pat):
+        k = (pat, self.ignorecase)
         try:
-            re_pat = Resolver._match_cache[pat]
+            re_pat = Resolver._match_cache[k]
         except KeyError:
             res = Resolver.__translate(pat)
             if len(Resolver._match_cache) >= _MAXCACHE:
                 Resolver._match_cache.clear()
-            Resolver._match_cache[pat] = re_pat = re.compile(res)
+            flags = 0
+            if self.ignorecase:
+                flags |= re.IGNORECASE
+            Resolver._match_cache[k] = re_pat = re.compile(res, flags=flags)
         return re_pat.match(name) is not None
 
+    def __cmp(self, name, pat):
+        if self.ignorecase:
+            return name.upper() == pat.upper()
+        return name == pat
+
     @staticmethod
     def __translate(pat):
-        re_pat = ''
+        re_pat = ""
         for char in pat:
             if char == "*":
                 re_pat += ".*"
             elif char == "?":
                 re_pat += "."
             else:
                 re_pat += re.escape(char)
-        return r'(?ms)' + re_pat + r'\Z'
+        return r"(?ms)" + re_pat + r"\Z"
 
 
 class ResolverError(RuntimeError):
-
     def __init__(self, node, child, msg):
         """Resolve Error at `node` handling `child`."""
         super(ResolverError, self).__init__(msg)
         self.node = node
         self.child = child
 
 
-class ChildResolverError(ResolverError):
+class RootResolverError(ResolverError):
+    def __init__(self, root):
+        """Root Resolve Error, cannot go above root node."""
+        msg = "Cannot go above root node %r" % (root,)
+        super(RootResolverError, self).__init__(root, None, msg)
+
 
+class ChildResolverError(ResolverError):
     def __init__(self, node, child, pathattr):
         """Child Resolve Error at `node` handling `child`."""
         names = [repr(_getattr(c, pathattr)) for c in node.children]
-        msg = "%r has no child %s. Children are: %s."
-        msg = msg % (node, child, ", ".join(names))
+        msg = "%r has no child %s. Children are: %s." % (node, child, ", ".join(names))
         super(ChildResolverError, self).__init__(node, child, msg)
 
 
 def _getattr(node, name):
-    return getattr(node, name, None)
+    return str(getattr(node, name, None))
```

### Comparing `anytree-2.8.0/anytree/search.py` & `anytree-2.9.0/anytree/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,15 @@
       ...
     anytree.search.CountError: Expecting at least 4 elements, but found 3. ... Node('/f/b/d/e'))
     >>> findall(f, filter_=lambda node: d in node.path, maxcount=2)  # doctest: +ELLIPSIS
     Traceback (most recent call last):
       ...
     anytree.search.CountError: Expecting 2 elements at maximum, but found 3. ... Node('/f/b/d/e'))
     """
-    return _findall(node, filter_=filter_, stop=stop,
-                    maxlevel=maxlevel, mincount=mincount, maxcount=maxcount)
+    return _findall(node, filter_=filter_, stop=stop, maxlevel=maxlevel, mincount=mincount, maxcount=maxcount)
 
 
 def findall_by_attr(node, value, name="name", maxlevel=None, mincount=None, maxcount=None):
     """
     Search nodes with attribute `name` having `value` but stop at `maxlevel`.
 
     Return tuple with matching nodes.
@@ -105,16 +104,21 @@
     +-- g
         +-- i
             +-- h
 
     >>> findall_by_attr(f, "d")
     (Node('/f/b/d'),)
     """
-    return _findall(node, filter_=lambda n: _filter_by_name(n, name, value),
-                    maxlevel=maxlevel, mincount=mincount, maxcount=maxcount)
+    return _findall(
+        node,
+        filter_=lambda n: _filter_by_name(n, name, value),
+        maxlevel=maxlevel,
+        mincount=mincount,
+        maxcount=maxcount,
+    )
 
 
 def find(node, filter_=None, stop=None, maxlevel=None):
     """
     Search for *single* node matching `filter_` but stop at `maxlevel` or `stop`.
 
     Return matching node.
@@ -201,16 +205,15 @@
 
     >>> find_by_attr(f, "d")
     Node('/f/b/d')
     >>> find_by_attr(f, name="foo", value=4)
     Node('/f/b/d/c', foo=4)
     >>> find_by_attr(f, name="foo", value=8)
     """
-    return _find(node, filter_=lambda n: _filter_by_name(n, name, value),
-                 maxlevel=maxlevel)
+    return _find(node, filter_=lambda n: _filter_by_name(n, name, value), maxlevel=maxlevel)
 
 
 def _find(node, filter_, stop=None, maxlevel=None):
     items = _findall(node, filter_, stop=stop, maxlevel=maxlevel, maxcount=1)
     return items[0] if items else None
 
 
@@ -230,13 +233,12 @@
     try:
         return getattr(node, name) == value
     except AttributeError:
         return False
 
 
 class CountError(RuntimeError):
-
     def __init__(self, msg, result):
         """Error raised on `mincount` or `maxcount` mismatch."""
         if result:
             msg += " " + repr(result)
         super(CountError, self).__init__(msg)
```

### Comparing `anytree-2.8.0/anytree/util/__init__.py` & `anytree-2.9.0/anytree/util/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     >>> commonancestors()
     ()
     """
     ancestors = [node.ancestors for node in nodes]
     common = []
     for parentnodes in zip(*ancestors):
         parentnode = parentnodes[0]
-        if all([parentnode is p for p in parentnodes[1:]]):
+        if all(parentnode is p for p in parentnodes[1:]):
             common.append(parentnode)
         else:
             break
     return tuple(common)
 
 
 def leftsibling(node):
@@ -51,18 +51,15 @@
     Node('/Dan/Jan')
     """
     if node.parent:
         pchildren = node.parent.children
         idx = pchildren.index(node)
         if idx:
             return pchildren[idx - 1]
-        else:
-            return None
-    else:
-        return None
+    return None
 
 
 def rightsibling(node):
     """
     Return Right Sibling of `node`.
 
     >>> from anytree import Node
```

### Comparing `anytree-2.8.0/anytree/walker.py` & `anytree-2.9.0/anytree/walker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 
 
-class Walker(object):
+class Walker:
+    """Walk from one node to another."""
 
-    def __init__(self):
-        """Walk from one node to another."""
-        super(Walker, self).__init__()
-
-    def walk(self, start, end):
+    @staticmethod
+    def walk(start, end):
         """
         Walk from `start` node to `end` node.
 
         Returns:
             (upwards, common, downwards): `upwards` is a list of nodes to go upward to.
             `common` top node. `downwards` is a list of nodes to go downward to.
 
@@ -61,35 +59,35 @@
         For a proper walking the nodes need to be part of the same tree:
 
         >>> w.walk(Node("a"), Node("b"))
         Traceback (most recent call last):
           ...
         anytree.walker.WalkError: Node('/a') and Node('/b') are not part of the same tree.
         """
-        s = start.path
-        e = end.path
+        startpath = start.path
+        endpath = end.path
         if start.root is not end.root:
             msg = "%r and %r are not part of the same tree." % (start, end)
             raise WalkError(msg)
         # common
-        c = Walker.__calc_common(s, e)
-        assert c[0] is start.root
-        len_c = len(c)
-        # up
-        if start is c[-1]:
-            up = tuple()
+        common = Walker.__calc_common(startpath, endpath)
+        assert common[0] is start.root
+        len_common = len(common)
+        # upwards
+        if start is common[-1]:
+            upwards = tuple()
         else:
-            up = tuple(reversed(s[len_c:]))
+            upwards = tuple(reversed(startpath[len_common:]))
         # down
-        if end is c[-1]:
+        if end is common[-1]:
             down = tuple()
         else:
-            down = e[len_c:]
-        return up, c[-1], down
+            down = endpath[len_common:]
+        return upwards, common[-1], down
 
     @staticmethod
-    def __calc_common(s, e):
-        return tuple([si for si, ei in zip(s, e) if si is ei])
+    def __calc_common(start, end):
+        return tuple(si for si, ei in zip(start, end) if si is ei)
 
 
 class WalkError(RuntimeError):
     """Walk Error."""
```

