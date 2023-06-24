# Comparing `tmp/Jug-2.2.3.tar.gz` & `tmp/Jug-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jug-2.2.3.tar", last modified: Fri May 26 11:38:17 2023, max compression
+gzip compressed data, was "Jug-2.3.0.tar", last modified: Sat Jun 24 22:21:27 2023, max compression
```

## Comparing `Jug-2.2.3.tar` & `Jug-2.3.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.338914 Jug-2.2.3/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1087 2020-10-10 13:38:46.000000 Jug-2.2.3/COPYING.MIT
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.326914 Jug-2.2.3/Jug.egg-info/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7550 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/PKG-INFO
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2788 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/SOURCES.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        1 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/dependency_links.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)       37 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/entry_points.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        4 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/top_level.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2021-03-18 04:18:20.000000 Jug-2.2.3/MANIFEST.in
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     7550 2023-05-26 11:38:17.338914 Jug-2.2.3/PKG-INFO
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6496 2023-05-26 11:36:42.000000 Jug-2.2.3/README.rst
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.326914 Jug-2.2.3/bin/
--rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)      182 2022-04-28 11:10:27.000000 Jug-2.2.3/bin/jug-execute
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.326914 Jug-2.2.3/jug/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2178 2017-01-12 09:06:55.000000 Jug-2.2.3/jug/__init__.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/backends/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1279 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/backends/__init__.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6760 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/backends/base.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6857 2022-05-19 20:42:40.000000 Jug-2.2.3/jug/backends/dict_store.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6225 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/backends/encode.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2508 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/backends/file_keepalive_monitor.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    18350 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/backends/file_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4863 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/backends/memoize_store.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6093 2022-05-19 20:42:40.000000 Jug-2.2.3/jug/backends/redis_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2140 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/backends/select.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5153 2020-06-11 19:25:43.000000 Jug-2.2.3/jug/barrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3204 2017-05-21 08:34:10.000000 Jug-2.2.3/jug/compound.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3493 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/hash.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/hooks/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2016-03-05 23:58:02.000000 Jug-2.2.3/jug/hooks/__init__.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1156 2020-10-28 22:12:26.000000 Jug-2.2.3/jug/hooks/execution.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3950 2020-09-25 14:40:43.000000 Jug-2.2.3/jug/hooks/exit_checks.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2374 2016-10-16 21:10:32.000000 Jug-2.2.3/jug/hooks/register.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/internal/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2020-06-11 19:25:43.000000 Jug-2.2.3/jug/internal/__init__.py
--rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     2748 2020-06-11 19:25:43.000000 Jug-2.2.3/jug/internal/debugger.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7483 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/io.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10352 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/jug.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)      218 2023-05-26 11:36:16.000000 Jug-2.2.3/jug/jug_version.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7881 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/mapreduce.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    10469 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/options.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/subcommands/
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    11604 2021-05-31 13:02:23.000000 Jug-2.2.3/jug/subcommands/__init__.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2974 2020-01-31 13:24:44.000000 Jug-2.2.3/jug/subcommands/check.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3309 2020-12-16 03:43:22.000000 Jug-2.2.3/jug/subcommands/cleanup.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1864 2017-05-19 19:02:51.000000 Jug-2.2.3/jug/subcommands/count.py
--rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     3057 2017-07-14 23:30:06.000000 Jug-2.2.3/jug/subcommands/demo.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6180 2020-10-28 22:12:46.000000 Jug-2.2.3/jug/subcommands/execute.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5451 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/subcommands/graph.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2072 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/subcommands/internal_validation.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3285 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/subcommands/invalidate.py
--rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     2014 2022-01-06 01:22:59.000000 Jug-2.2.3/jug/subcommands/pack.py
--rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     6099 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/subcommands/shell.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10506 2022-05-02 20:30:18.000000 Jug-2.2.3/jug/subcommands/status.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4839 2022-05-02 20:33:19.000000 Jug-2.2.3/jug/subcommands/webstatus.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    19139 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/task.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.334914 Jug-2.2.3/jug/tests/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      158 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/__init__.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.338914 Jug-2.2.3/jug/tests/jugfiles/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/__init__.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      471 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/barrier_mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      192 2018-04-13 18:55:39.000000 Jug-2.2.3/jug/tests/jugfiles/barrier_recurse.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      341 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/jugfiles/block_access.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      108 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/builtin_function.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      134 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/bvalue.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      337 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/compound.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      380 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/compound_nonsimple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      280 2019-08-11 14:57:49.000000 Jug-2.2.3/jug/tests/jugfiles/compound_wbarrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      277 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/custom_hash_function.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      141 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/empty_mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)       65 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/tests/jugfiles/exceptions.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      498 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/tests/jugfiles/failing.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      226 2020-01-31 13:24:44.000000 Jug-2.2.3/jug/tests/jugfiles/iteratetask.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      244 2018-04-13 19:35:09.000000 Jug-2.2.3/jug/tests/jugfiles/mapgenerator.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2018-04-07 13:03:52.000000 Jug-2.2.3/jug/tests/jugfiles/mapreduce_generator.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      394 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/jugfiles/no_load.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      327 2020-06-11 19:49:14.000000 Jug-2.2.3/jug/tests/jugfiles/run-simple-create-file.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      329 2017-08-29 16:56:39.000000 Jug-2.2.3/jug/tests/jugfiles/simple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      312 2017-05-19 19:02:51.000000 Jug-2.2.3/jug/tests/jugfiles/simple_multiple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/sleep_until_tasklet.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      348 2016-12-29 09:23:55.000000 Jug-2.2.3/jug/tests/jugfiles/slice_task.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      117 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/tasklet_simple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      268 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/tasklets.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      372 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/wbarrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      331 2016-03-04 01:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/write_with_meta.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      482 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/task_reset.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2010 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_barrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2376 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_compound.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1557 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_encode.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     2245 2022-07-18 23:06:59.000000 Jug-2.2.3/jug/tests/test_file_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      809 2016-12-29 00:15:41.000000 Jug-2.2.3/jug/tests/test_hash.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1558 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_hooks.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1125 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_io.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1666 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_jug_check.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4784 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_jug_execute.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3482 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_jug_invalidate.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3139 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_lock.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2835 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      382 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_no_load.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2059 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_options.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1886 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_status.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     4622 2022-05-19 20:42:40.000000 Jug-2.2.3/jug/tests/test_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3503 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_subcommand_api.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1158 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_sys_argv.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1341 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_tasklet.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6747 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_tasks.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      476 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_utils_customhash.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      154 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_utils_identity.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      742 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_utils_timed_path.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      464 2022-05-02 20:33:48.000000 Jug-2.2.3/jug/tests/test_webstatus.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      649 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/utils.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7531 2020-10-28 22:12:52.000000 Jug-2.2.3/jug/utils.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2021-03-21 03:34:18.000000 Jug-2.2.3/requirements.txt
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)       38 2023-05-26 11:38:17.338914 Jug-2.2.3/setup.cfg
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3000 2022-04-28 11:10:43.000000 Jug-2.2.3/setup.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)       19 2021-03-18 04:18:20.000000 Jug-2.2.3/test-requirements.txt
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.352942 Jug-2.3.0/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1087 2020-10-10 13:38:46.000000 Jug-2.3.0/COPYING.MIT
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.340942 Jug-2.3.0/Jug.egg-info/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     8170 2023-06-24 22:21:27.000000 Jug-2.3.0/Jug.egg-info/PKG-INFO
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2788 2023-06-24 22:21:27.000000 Jug-2.3.0/Jug.egg-info/SOURCES.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        1 2023-06-24 22:21:27.000000 Jug-2.3.0/Jug.egg-info/dependency_links.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)       37 2023-06-24 22:21:27.000000 Jug-2.3.0/Jug.egg-info/entry_points.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        4 2023-06-24 22:21:27.000000 Jug-2.3.0/Jug.egg-info/top_level.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2021-03-18 04:18:20.000000 Jug-2.3.0/MANIFEST.in
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     8170 2023-06-24 22:21:27.352942 Jug-2.3.0/PKG-INFO
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     7116 2023-06-24 22:18:42.000000 Jug-2.3.0/README.rst
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.340942 Jug-2.3.0/bin/
+-rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)      182 2022-04-28 11:10:27.000000 Jug-2.3.0/bin/jug-execute
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.340942 Jug-2.3.0/jug/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2178 2017-01-12 09:06:55.000000 Jug-2.3.0/jug/__init__.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.344942 Jug-2.3.0/jug/backends/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1279 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/backends/__init__.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     7424 2023-05-29 22:02:18.000000 Jug-2.3.0/jug/backends/base.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6857 2022-05-19 20:42:40.000000 Jug-2.3.0/jug/backends/dict_store.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6225 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/backends/encode.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2508 2019-08-11 14:59:21.000000 Jug-2.3.0/jug/backends/file_keepalive_monitor.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    18680 2023-05-29 22:02:18.000000 Jug-2.3.0/jug/backends/file_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4863 2019-08-11 14:59:21.000000 Jug-2.3.0/jug/backends/memoize_store.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6093 2022-05-19 20:42:40.000000 Jug-2.3.0/jug/backends/redis_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2140 2019-08-11 14:59:21.000000 Jug-2.3.0/jug/backends/select.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     4997 2023-06-24 22:18:42.000000 Jug-2.3.0/jug/barrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3204 2017-05-21 08:34:10.000000 Jug-2.3.0/jug/compound.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3493 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/hash.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.344942 Jug-2.3.0/jug/hooks/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2016-03-05 23:58:02.000000 Jug-2.3.0/jug/hooks/__init__.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1156 2020-10-28 22:12:26.000000 Jug-2.3.0/jug/hooks/execution.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3950 2020-09-25 14:40:43.000000 Jug-2.3.0/jug/hooks/exit_checks.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2374 2016-10-16 21:10:32.000000 Jug-2.3.0/jug/hooks/register.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.344942 Jug-2.3.0/jug/internal/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2020-06-11 19:25:43.000000 Jug-2.3.0/jug/internal/__init__.py
+-rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     2748 2020-06-11 19:25:43.000000 Jug-2.3.0/jug/internal/debugger.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7483 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/io.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10352 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/jug.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)      218 2023-06-24 22:18:42.000000 Jug-2.3.0/jug/jug_version.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7881 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/mapreduce.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    10479 2023-05-29 22:02:18.000000 Jug-2.3.0/jug/options.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.344942 Jug-2.3.0/jug/subcommands/
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    11604 2021-05-31 13:02:23.000000 Jug-2.3.0/jug/subcommands/__init__.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2974 2020-01-31 13:24:44.000000 Jug-2.3.0/jug/subcommands/check.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3309 2020-12-16 03:43:22.000000 Jug-2.3.0/jug/subcommands/cleanup.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1864 2017-05-19 19:02:51.000000 Jug-2.3.0/jug/subcommands/count.py
+-rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     3057 2017-07-14 23:30:06.000000 Jug-2.3.0/jug/subcommands/demo.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6180 2020-10-28 22:12:46.000000 Jug-2.3.0/jug/subcommands/execute.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5451 2019-08-11 14:59:21.000000 Jug-2.3.0/jug/subcommands/graph.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2072 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/subcommands/internal_validation.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3345 2023-05-29 22:02:18.000000 Jug-2.3.0/jug/subcommands/invalidate.py
+-rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     2014 2022-01-06 01:22:59.000000 Jug-2.3.0/jug/subcommands/pack.py
+-rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     6700 2023-05-29 22:02:18.000000 Jug-2.3.0/jug/subcommands/shell.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10506 2022-05-02 20:30:18.000000 Jug-2.3.0/jug/subcommands/status.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4839 2022-05-02 20:33:19.000000 Jug-2.3.0/jug/subcommands/webstatus.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)    19139 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/task.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.348942 Jug-2.3.0/jug/tests/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      158 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/__init__.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-06-24 22:21:27.352942 Jug-2.3.0/jug/tests/jugfiles/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2014-01-24 15:42:10.000000 Jug-2.3.0/jug/tests/jugfiles/__init__.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      471 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/barrier_mapreduce.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      192 2018-04-13 18:55:39.000000 Jug-2.3.0/jug/tests/jugfiles/barrier_recurse.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      341 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/jugfiles/block_access.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      108 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/builtin_function.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      134 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/bvalue.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      337 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/compound.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      380 2014-01-24 15:42:10.000000 Jug-2.3.0/jug/tests/jugfiles/compound_nonsimple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      280 2019-08-11 14:57:49.000000 Jug-2.3.0/jug/tests/jugfiles/compound_wbarrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      277 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/custom_hash_function.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      141 2014-01-24 15:42:10.000000 Jug-2.3.0/jug/tests/jugfiles/empty_mapreduce.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)       65 2019-08-11 14:59:21.000000 Jug-2.3.0/jug/tests/jugfiles/exceptions.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      498 2019-08-11 14:59:21.000000 Jug-2.3.0/jug/tests/jugfiles/failing.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      226 2020-01-31 13:24:44.000000 Jug-2.3.0/jug/tests/jugfiles/iteratetask.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      244 2018-04-13 19:35:09.000000 Jug-2.3.0/jug/tests/jugfiles/mapgenerator.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2018-04-07 13:03:52.000000 Jug-2.3.0/jug/tests/jugfiles/mapreduce_generator.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      394 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/jugfiles/no_load.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      327 2020-06-11 19:49:14.000000 Jug-2.3.0/jug/tests/jugfiles/run-simple-create-file.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      329 2017-08-29 16:56:39.000000 Jug-2.3.0/jug/tests/jugfiles/simple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      312 2017-05-19 19:02:51.000000 Jug-2.3.0/jug/tests/jugfiles/simple_multiple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/sleep_until_tasklet.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      348 2016-12-29 09:23:55.000000 Jug-2.3.0/jug/tests/jugfiles/slice_task.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      117 2016-03-04 01:41:49.000000 Jug-2.3.0/jug/tests/jugfiles/tasklet_simple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      268 2014-01-24 15:42:10.000000 Jug-2.3.0/jug/tests/jugfiles/tasklets.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      372 2014-01-24 15:42:10.000000 Jug-2.3.0/jug/tests/jugfiles/wbarrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      331 2016-03-04 01:42:10.000000 Jug-2.3.0/jug/tests/jugfiles/write_with_meta.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      482 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/task_reset.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2010 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_barrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2376 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_compound.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1557 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/tests/test_encode.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     2245 2022-07-18 23:06:59.000000 Jug-2.3.0/jug/tests/test_file_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      809 2016-12-29 00:15:41.000000 Jug-2.3.0/jug/tests/test_hash.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1558 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_hooks.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1125 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_io.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1666 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_jug_check.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4784 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_jug_execute.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3482 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_jug_invalidate.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3139 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_lock.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2835 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_mapreduce.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      382 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_no_load.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2059 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/tests/test_options.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1886 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_status.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     4622 2022-05-19 20:42:40.000000 Jug-2.3.0/jug/tests/test_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3503 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/tests/test_subcommand_api.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1158 2021-03-21 03:34:18.000000 Jug-2.3.0/jug/tests/test_sys_argv.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1341 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_tasklet.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6747 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_tasks.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      476 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_utils_customhash.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      154 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_utils_identity.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      742 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/test_utils_timed_path.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      464 2022-05-02 20:33:48.000000 Jug-2.3.0/jug/tests/test_webstatus.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      649 2020-10-10 13:38:46.000000 Jug-2.3.0/jug/tests/utils.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7531 2020-10-28 22:12:52.000000 Jug-2.3.0/jug/utils.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2021-03-21 03:34:18.000000 Jug-2.3.0/requirements.txt
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)       38 2023-06-24 22:21:27.352942 Jug-2.3.0/setup.cfg
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3000 2022-04-28 11:10:43.000000 Jug-2.3.0/setup.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)       19 2021-03-18 04:18:20.000000 Jug-2.3.0/test-requirements.txt
```

### Comparing `Jug-2.2.3/COPYING.MIT` & `Jug-2.3.0/COPYING.MIT`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/Jug.egg-info/PKG-INFO` & `Jug-2.3.0/Jug.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jug
-Version: 2.2.3
+Version: 2.3.0
 Summary: A Task Based Parallelization Framework
 Home-page: https://jug.readthedocs.io
 Author: Luis Pedro Coelho
 Author-email: luis@luispedro.org
 License: MIT
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,14 +38,17 @@
 
 .. image:: https://zenodo.org/badge/205237.svg
    :target: https://zenodo.org/badge/latestdoi/205237
 
 .. image:: https://anaconda.org/conda-forge/jug/badges/installer/conda.svg
     :target: https://anaconda.org/conda-forge/jug
 
+.. image:: https://static.pepy.tech/personalized-badge/jug?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+   :target: https://pepy.tech/project/jug
+
 .. image:: https://img.shields.io/badge/CITATION-doi.org%2F10.5334%2Fjors.161-green.svg
    :target: https://doi.org/10.5334/jors.161
 
 
 It uses the filesystem to communicate between processes and
 works correctly over NFS, so you can coordinate processes on
 different machines.
@@ -154,14 +157,22 @@
 
     In [2]: primes100[:10]
     Out[2]: [True, True, False, True, False, True, False, False, False, True]
 
 What's New
 ----------
 
+Version 2.3.0 (*25 June 2023*)
+
+- jug shell: Add ``get_filtered_tasks()``
+- jug: Fix ``jug --version`` (which had been broken in the refactoring to use subcommands)
+- jug shell: Fix message in jug shell when there are no dependencies (it would repeatedly print the message stating *this will only be run once*)
+- jug pack: Make it much faster to invalidate elements
+- file_store: ensure that the temporary directory exists
+
 Version 2.2.3 (*26 May 2023*)
 - Fix ``jug shell`` for newer versions of IPython
 
 Version 2.2.2 (*19 July 2022*)
 - Fix ``jug cleanup`` when packs are used (``jug pack``)
 
 Version 2.2.1 (*19 May 2022*)
```

### Comparing `Jug-2.2.3/Jug.egg-info/SOURCES.txt` & `Jug-2.3.0/Jug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/PKG-INFO` & `Jug-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jug
-Version: 2.2.3
+Version: 2.3.0
 Summary: A Task Based Parallelization Framework
 Home-page: https://jug.readthedocs.io
 Author: Luis Pedro Coelho
 Author-email: luis@luispedro.org
 License: MIT
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,14 +38,17 @@
 
 .. image:: https://zenodo.org/badge/205237.svg
    :target: https://zenodo.org/badge/latestdoi/205237
 
 .. image:: https://anaconda.org/conda-forge/jug/badges/installer/conda.svg
     :target: https://anaconda.org/conda-forge/jug
 
+.. image:: https://static.pepy.tech/personalized-badge/jug?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+   :target: https://pepy.tech/project/jug
+
 .. image:: https://img.shields.io/badge/CITATION-doi.org%2F10.5334%2Fjors.161-green.svg
    :target: https://doi.org/10.5334/jors.161
 
 
 It uses the filesystem to communicate between processes and
 works correctly over NFS, so you can coordinate processes on
 different machines.
@@ -154,14 +157,22 @@
 
     In [2]: primes100[:10]
     Out[2]: [True, True, False, True, False, True, False, False, False, True]
 
 What's New
 ----------
 
+Version 2.3.0 (*25 June 2023*)
+
+- jug shell: Add ``get_filtered_tasks()``
+- jug: Fix ``jug --version`` (which had been broken in the refactoring to use subcommands)
+- jug shell: Fix message in jug shell when there are no dependencies (it would repeatedly print the message stating *this will only be run once*)
+- jug pack: Make it much faster to invalidate elements
+- file_store: ensure that the temporary directory exists
+
 Version 2.2.3 (*26 May 2023*)
 - Fix ``jug shell`` for newer versions of IPython
 
 Version 2.2.2 (*19 July 2022*)
 - Fix ``jug cleanup`` when packs are used (``jug pack``)
 
 Version 2.2.1 (*19 May 2022*)
```

### Comparing `Jug-2.2.3/README.rst` & `Jug-2.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 .. image:: https://zenodo.org/badge/205237.svg
    :target: https://zenodo.org/badge/latestdoi/205237
 
 .. image:: https://anaconda.org/conda-forge/jug/badges/installer/conda.svg
     :target: https://anaconda.org/conda-forge/jug
 
+.. image:: https://static.pepy.tech/personalized-badge/jug?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads
+   :target: https://pepy.tech/project/jug
+
 .. image:: https://img.shields.io/badge/CITATION-doi.org%2F10.5334%2Fjors.161-green.svg
    :target: https://doi.org/10.5334/jors.161
 
 
 It uses the filesystem to communicate between processes and
 works correctly over NFS, so you can coordinate processes on
 different machines.
@@ -126,14 +129,22 @@
 
     In [2]: primes100[:10]
     Out[2]: [True, True, False, True, False, True, False, False, False, True]
 
 What's New
 ----------
 
+Version 2.3.0 (*25 June 2023*)
+
+- jug shell: Add ``get_filtered_tasks()``
+- jug: Fix ``jug --version`` (which had been broken in the refactoring to use subcommands)
+- jug shell: Fix message in jug shell when there are no dependencies (it would repeatedly print the message stating *this will only be run once*)
+- jug pack: Make it much faster to invalidate elements
+- file_store: ensure that the temporary directory exists
+
 Version 2.2.3 (*26 May 2023*)
 - Fix ``jug shell`` for newer versions of IPython
 
 Version 2.2.2 (*19 July 2022*)
 - Fix ``jug cleanup`` when packs are used (``jug pack``)
 
 Version 2.2.1 (*19 May 2022*)
```

### Comparing `Jug-2.2.3/jug/__init__.py` & `Jug-2.3.0/jug/__init__.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/__init__.py` & `Jug-2.3.0/jug/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/base.py` & `Jug-2.3.0/jug/backends/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2011-2021, Luis Pedro Coelho <luis@luispedro.org>
+# Copyright (C) 2011-2023, Luis Pedro Coelho <luis@luispedro.org>
 # vim: set ts=4 sts=4 sw=4 expandtab smartindent:
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -103,14 +103,41 @@
 
         Returns
         -------
         obj : any
             The object that was saved under ``name``
         '''
 
+    def remove_many(self, names):
+        '''
+        removed = store.remove_many(names)
+
+        Remove the entry associated with ``names``.
+
+        Returns set of names that were actually removed.
+
+        Default implementation calls ``remove`` for each name, but this can be
+        overridden for efficiency.
+
+        Parameters
+        ----------
+        names : iterable of str
+            Keys
+
+        Returns
+        -------
+        removed : set of str
+            Keys that were actually removed
+        '''
+        removed = []
+        for name in names:
+            if self.remove(name):
+                removed.append(name)
+        return removed
+
     @abstractmethod
     def remove(self, name):
         '''
         was_removed = store.remove(name)
 
         Remove the entry associated with ``name``.
```

### Comparing `Jug-2.2.3/jug/backends/dict_store.py` & `Jug-2.3.0/jug/backends/dict_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/encode.py` & `Jug-2.3.0/jug/backends/encode.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/file_keepalive_monitor.py` & `Jug-2.3.0/jug/backends/file_keepalive_monitor.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/file_store.py` & `Jug-2.3.0/jug/backends/file_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,17 @@
 
         Internal. Use `self.keys()`
 
         '''
         if not exists(self.jugdir):
             return
 
-        for d in os.listdir(self.jugdir):
+        for d in sorted(os.listdir(self.jugdir)):
             if len(d) == 2:
-                for f in os.listdir(path.join(self.jugdir, d)):
+                for f in sorted(os.listdir(path.join(self.jugdir, d))):
                     yield (d+f).encode('ascii')
 
     def list(self):
         '''
         keys = store.list()
 
         Returns a list of all the keys in the store
@@ -202,14 +202,15 @@
             if lock.get():
                 break
             from time import sleep
             logging.warning("Waiting for lock file 'pack-save'")
             sleep(2**i)
         else:
             raise Exception('Could not obtain lock to save packed data')
+        self._maybe_create()
         fd, fname = tempfile.mkstemp('.jugtmp', 'jugtemp', self.tempdir())
         output = os.fdopen(fd, 'wb')
         encode_to(self.packed, output)
         output.flush()
         os.fsync(output.fileno())
         output.close()
 
@@ -272,33 +273,43 @@
             except ValueError:
                 ifile.seek(0)
             except ImportError:
                 pass
             return decode_from(ifile)
 
 
+    def remove_many(self, names):
+        '''
+        store.remove_many(names)
+
+        Removes the objects with the given names from the store.
+        '''
+        removed = set()
+        for name in names:
+            if name in self.packed:
+                del self.packed[name]
+                removed.add(name)
+            try:
+                fname = self._getfname(name)
+                os.unlink(fname)
+                removed.add(name)
+            except OSError:
+                pass
+        self.resave_pack()
+        return removed
+
     def remove(self, name):
         '''
         was_removed = store.remove(name)
 
         Remove the entry associated with name.
 
         Returns whether any entry was actually removed.
         '''
-        removed = False
-        if name in self.packed:
-            del self.packed[name]
-            self.resave_pack()
-            removed = True
-        try:
-            fname = self._getfname(name)
-            os.unlink(fname)
-            return True
-        except OSError:
-            return removed
+        return bool(self.remove_many([name]))
 
 
     def cleanup(self, active, keeplocks=False):
         '''
         nr_removed = store.cleanup(active, keeplocks)
 
         Implement 'cleanup' command
```

### Comparing `Jug-2.2.3/jug/backends/memoize_store.py` & `Jug-2.3.0/jug/backends/memoize_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/redis_store.py` & `Jug-2.3.0/jug/backends/redis_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/backends/select.py` & `Jug-2.3.0/jug/backends/select.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/barrier.py` & `Jug-2.3.0/jug/barrier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # vim: set ts=4 sts=4 sw=4 expandtab smartindent:
-# Copyright (C) 2010-2020, Luis Pedro Coelho <luis@luispedro.org>
+# Copyright (C) 2010-2023, Luis Pedro Coelho <luis@luispedro.org>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -40,18 +40,15 @@
     # list of dependencies with an explicit stack (`q`). Then, we iterate over
     # the list of dependencies and trigger hash computation for each of the
     # dependencies. This should ensures that the next call to `can_load()`
     # returns immediately.
 
     try:
         return tsk.can_load()
-    # RecursionError was introduced in Python 3.5, so we cannot use it
-    # until we stop supporting earlier versions of Python
-    except RuntimeError:
-    # except RecursionError:
+    except RecursionError:
         dependencies = set()
         q = [tsk]
         while q:
             top = q.pop()
             ndeps = top.dependencies()
             ndeps = [t for t in ndeps if id(t) not in dependencies]
             q.extend(ndeps)
```

### Comparing `Jug-2.2.3/jug/compound.py` & `Jug-2.3.0/jug/compound.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/hash.py` & `Jug-2.3.0/jug/hash.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/hooks/execution.py` & `Jug-2.3.0/jug/hooks/execution.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/hooks/exit_checks.py` & `Jug-2.3.0/jug/hooks/exit_checks.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/hooks/register.py` & `Jug-2.3.0/jug/hooks/register.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/internal/debugger.py` & `Jug-2.3.0/jug/internal/debugger.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/io.py` & `Jug-2.3.0/jug/io.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/jug.py` & `Jug-2.3.0/jug/jug.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/mapreduce.py` & `Jug-2.3.0/jug/mapreduce.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/options.py` & `Jug-2.3.0/jug/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2008-2021, Luis Pedro Coelho <luis@luispedro.org>
+# Copyright (C) 2008-2022, Luis Pedro Coelho <luis@luispedro.org>
 # vim: set ts=4 sts=4 sw=4 expandtab smartindent:
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -153,19 +153,18 @@
 
             logging.debug("Setting %s to %s", new_name, value)
             setattr(inifile, new_name, value)
 
     return inifile
 
 
-def define_options(parser):
+def add_common_options(parser):
     group = parser.add_argument_group("common")
     group.add_argument('jugfile', action='store', nargs='?',
                        help="Python script to use. (Default: %(default)s)" % {"default": default_options.jugfile})
-    group.add_argument('--version', action="version", version=__version__)
     group.add_argument('--aggressive-unload',
                        action='store_true',
                        dest='aggressive_unload',
                        help='''\
 Aggressively unload data from memory. This causes many more reloading of
 information, but is necessary if keeping too much in memory is leading to
 memory errors.''')
@@ -228,23 +227,25 @@
         cmdapi.usage()
 
     parser = argparse.ArgumentParser(
         description=cmdapi.usage(_print=False, exit=False),
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
+    parser.add_argument('--version', action="version", version=__version__)
+
     sub = parser.add_subparsers(dest="subcommand", help=argparse.SUPPRESS)
     sub.required = True
     subparsers = cmdapi.get_subcommand_parsers(sub)
 
     # NOTE The parents=[parent] feature of argparse is severely broken
     # causing dependency loops in required arguments.
     # To workaround we re-define all global options in all subparsers
     for sub in subparsers:
-        define_options(sub)
+        add_common_options(sub)
         sub.add_argument('user_args', nargs='*', default=[])
 
     argopts = parser.parse_args(args)
 
     inifile = read_configuration_file(optionsfile, default_options=default_options)
     # Priority is: user-supplied command line, config file, default options
     cmdline = Options(inifile)
```

### Comparing `Jug-2.2.3/jug/subcommands/__init__.py` & `Jug-2.3.0/jug/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/check.py` & `Jug-2.3.0/jug/subcommands/check.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/cleanup.py` & `Jug-2.3.0/jug/subcommands/cleanup.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/count.py` & `Jug-2.3.0/jug/subcommands/count.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/demo.py` & `Jug-2.3.0/jug/subcommands/demo.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/execute.py` & `Jug-2.3.0/jug/subcommands/execute.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/graph.py` & `Jug-2.3.0/jug/subcommands/graph.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/internal_validation.py` & `Jug-2.3.0/jug/subcommands/internal_validation.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/invalidate.py` & `Jug-2.3.0/jug/subcommands/invalidate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-# Copyright (C) 2008-2015, Luis Pedro Coelho <luis@luispedro.org>
+# Copyright (C) 2008-2023, Luis Pedro Coelho <luis@luispedro.org>
 # vim: set ts=4 sts=4 sw=4 expandtab smartindent:
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -73,16 +73,17 @@
             return False
 
         invalid = list(filter(isinvalid, tasks))
         if not invalid:
             options.print_out('No results invalidated.')
             return
         task_counts = defaultdict(int)
+        removed = store.remove_many(t.hash() for t in invalid)
         for t in invalid:
-            if store.remove(t.hash()):
+            if t.hash() in removed:
                 task_counts[t.name] += 1
         if sum(task_counts.values()) == 0:
             options.print_out('Tasks invalidated, but no results removed')
         else:
             print_task_summary_table(options, [("Invalidated", task_counts)])
 
     def parse(self, parser):
```

### Comparing `Jug-2.2.3/jug/subcommands/pack.py` & `Jug-2.3.0/jug/subcommands/pack.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/shell.py` & `Jug-2.3.0/jug/subcommands/shell.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         from jug.task import Tasklet
         print("Building task DAG... (only performed once)")
         for t in tasklist:
             for d in t.dependencies():
                 while isinstance(d, Tasklet):
                     d = d.base
                 reverse.setdefault(d.hash(), []).append(t)
+        if not reverse:
+            # This can happen if the script is very trivial
+            # Which can then lead to multiple "only performed once" messages
+            reverse['#'] = None
     queue = [task]
     seen = set()
     while queue:
         task = queue.pop()
         if task.hash() in seen:
             continue
         seen.add(task.hash())
@@ -143,19 +147,29 @@
                 If true (default), it will return a _copy_ of the internal list
             '''
             from ..task import alltasks
             if copy:
                 return alltasks[:]
             return alltasks
 
+        def _get_filtered_tasks(loadable=False, failed=False, available=False):
+            return [t
+                    for t in _get_tasks()
+                    if (loadable and t.can_load()) or
+                        (failed and t.is_failed()) or
+                        (available and not t.can_load() and t.can_run())
+                        ]
+
+
         local_ns = {
             'load_all': _load_all,
             'value': value,
             'invalidate': _invalidate,
             'get_tasks': _get_tasks,
+            'get_filtered_tasks': _get_filtered_tasks,
         }
         # This is necessary for some versions of Ipython. See:
         # http://groups.google.com/group/pylons-discuss/browse_thread/thread/312e3ead5967468a
         try:
             del jugspace['__builtins__']
         except KeyError:
             pass
```

### Comparing `Jug-2.2.3/jug/subcommands/status.py` & `Jug-2.3.0/jug/subcommands/status.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/subcommands/webstatus.py` & `Jug-2.3.0/jug/subcommands/webstatus.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/task.py` & `Jug-2.3.0/jug/task.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_barrier.py` & `Jug-2.3.0/jug/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_compound.py` & `Jug-2.3.0/jug/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_encode.py` & `Jug-2.3.0/jug/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_file_store.py` & `Jug-2.3.0/jug/tests/test_file_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_hash.py` & `Jug-2.3.0/jug/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_hooks.py` & `Jug-2.3.0/jug/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_io.py` & `Jug-2.3.0/jug/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_jug_check.py` & `Jug-2.3.0/jug/tests/test_jug_check.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_jug_execute.py` & `Jug-2.3.0/jug/tests/test_jug_execute.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_jug_invalidate.py` & `Jug-2.3.0/jug/tests/test_jug_invalidate.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_lock.py` & `Jug-2.3.0/jug/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_mapreduce.py` & `Jug-2.3.0/jug/tests/test_mapreduce.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_options.py` & `Jug-2.3.0/jug/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_status.py` & `Jug-2.3.0/jug/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_store.py` & `Jug-2.3.0/jug/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_subcommand_api.py` & `Jug-2.3.0/jug/tests/test_subcommand_api.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_sys_argv.py` & `Jug-2.3.0/jug/tests/test_sys_argv.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_tasklet.py` & `Jug-2.3.0/jug/tests/test_tasklet.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_tasks.py` & `Jug-2.3.0/jug/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/test_utils_timed_path.py` & `Jug-2.3.0/jug/tests/test_utils_timed_path.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/tests/utils.py` & `Jug-2.3.0/jug/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/jug/utils.py` & `Jug-2.3.0/jug/utils.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.3/setup.py` & `Jug-2.3.0/setup.py`

 * *Files identical despite different names*

