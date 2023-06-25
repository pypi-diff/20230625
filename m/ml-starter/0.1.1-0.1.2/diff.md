# Comparing `tmp/ml-starter-0.1.1.tar.gz` & `tmp/ml-starter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.1.tar", last modified: Sat Jun 24 21:21:30 2023, max compression
+gzip compressed data, was "ml-starter-0.1.2.tar", last modified: Sun Jun 25 01:32:29 2023, max compression
```

## Comparing `ml-starter-0.1.1.tar` & `ml-starter-0.1.2.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.458876 ml-starter-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 21:21:17.000000 ml-starter-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-24 21:21:17.000000 ml-starter-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-24 21:21:30.458876 ml-starter-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-24 21:21:17.000000 ml-starter-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.426875 ml-starter-0.1.1/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.430875 ml-starter-0.1.1/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.430875 ml-starter-0.1.1/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.434875 ml-starter-0.1.1/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.434875 ml-starter-0.1.1/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.438875 ml-starter-0.1.1/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.438875 ml-starter-0.1.1/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47649 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.438875 ml-starter-0.1.1/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.442875 ml-starter-0.1.1/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.442875 ml-starter-0.1.1/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.442875 ml-starter-0.1.1/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.442875 ml-starter-0.1.1/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.446875 ml-starter-0.1.1/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.446875 ml-starter-0.1.1/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.446875 ml-starter-0.1.1/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.446875 ml-starter-0.1.1/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.446875 ml-starter-0.1.1/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.454876 ml-starter-0.1.1/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.454876 ml-starter-0.1.1/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.454876 ml-starter-0.1.1/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-24 21:21:17.000000 ml-starter-0.1.1/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 21:21:30.458876 ml-starter-0.1.1/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-24 21:21:30.000000 ml-starter-0.1.1/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-24 21:21:30.000000 ml-starter-0.1.1/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 21:21:30.000000 ml-starter-0.1.1/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-24 21:21:30.000000 ml-starter-0.1.1/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-24 21:21:30.000000 ml-starter-0.1.1/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-24 21:21:17.000000 ml-starter-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 21:21:17.000000 ml-starter-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-24 21:21:17.000000 ml-starter-0.1.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 21:21:17.000000 ml-starter-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-24 21:21:30.458876 ml-starter-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-24 21:21:17.000000 ml-starter-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 01:32:14.000000 ml-starter-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-25 01:32:14.000000 ml-starter-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 01:32:29.025124 ml-starter-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-25 01:32:14.000000 ml-starter-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.009124 ml-starter-0.1.2/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.009124 ml-starter-0.1.2/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-25 01:32:29.000000 ml-starter-0.1.2/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 01:32:14.000000 ml-starter-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-25 01:32:14.000000 ml-starter-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 01:32:14.000000 ml-starter-0.1.2/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 01:32:14.000000 ml-starter-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-25 01:32:29.025124 ml-starter-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 01:32:14.000000 ml-starter-0.1.2/setup.py
```

### Comparing `ml-starter-0.1.1/LICENSE` & `ml-starter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/PKG-INFO` & `ml-starter-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.1
+Version: 0.1.2
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.1/README.md` & `ml-starter-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/api.py` & `ml-starter-0.1.2/ml/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     "register_optimizer",
     "register_task",
     "register_trainer",
     "ReinforcementLearningTask",
     "ReinforcementLearningTaskConfig",
     "ReinforcementLearningTrainer",
     "ReinforcementLearningTrainerConfig",
+    "reset_lora_weights_",
     "reset_parallelism",
     "RotaryEmbeddings",
     "RowParallelLinear",
     "set_distributed_backend",
     "set_random_seed",
     "set_slurm_master_addr",
     "set_slurm_rank_and_world_size",
@@ -220,14 +221,15 @@
     LoraConvTranspose2d,
     LoraEmbedding,
     LoraGRU,
     LoraLinear,
     LoraLSTM,
     lora,
     maybe_lora,
+    reset_lora_weights_,
 )
 from ml.models.norms import NormType, cast_norm_type, get_norm_1d, get_norm_2d, get_norm_3d, get_norm_linear
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
```

### Comparing `ml-starter-0.1.1/ml/core/common_types.py` & `ml-starter-0.1.2/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/core/config.py` & `ml-starter-0.1.2/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/core/env.py` & `ml-starter-0.1.2/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/core/registry.py` & `ml-starter-0.1.2/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/core/state.py` & `ml-starter-0.1.2/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/launchers/base.py` & `ml-starter-0.1.2/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/launchers/mp.py` & `ml-starter-0.1.2/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/launchers/slurm.py` & `ml-starter-0.1.2/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/launchers/torchrun.py` & `ml-starter-0.1.2/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/loggers/base.py` & `ml-starter-0.1.2/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/loggers/meter.py` & `ml-starter-0.1.2/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/loggers/multi.py` & `ml-starter-0.1.2/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/loggers/stdout.py` & `ml-starter-0.1.2/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/loggers/tensorboard.py` & `ml-starter-0.1.2/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/base.py` & `ml-starter-0.1.2/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/constant.py` & `ml-starter-0.1.2/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.2/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.2/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/linear.py` & `ml-starter-0.1.2/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.2/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.2/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/activations.py` & `ml-starter-0.1.2/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/base.py` & `ml-starter-0.1.2/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/embeddings.py` & `ml-starter-0.1.2/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/init.py` & `ml-starter-0.1.2/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/kmeans.py` & `ml-starter-0.1.2/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/lora.py` & `ml-starter-0.1.2/ml/models/lora.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 ``r`` parameter. The ``lora_alpha`` parameter is typically set to 1.0, but
 can be tuned to improve performance.
 """
 
 import math
 import warnings
 import weakref
+from abc import abstractmethod
 from typing import Any, TypeVar, Union, cast, overload
 
 import torch.nn.functional as F
 from torch import Tensor, nn
 from torch.nn.modules.module import _IncompatibleKeys
 
 from ml.models.init import InitializationType
@@ -90,14 +91,18 @@
         super().__init__(*args, **kwargs)
 
         # This allows modules to use LoRA layers as drop-in replacements for
         # non-LoRA pretrained models without throwing annoying errors for
         # state dict incompatibility.
         self.register_load_state_dict_post_hook(_lora_post_hook)
 
+    @abstractmethod
+    def reset_lora_parameters(self) -> None:
+        """Resets LoRA parameters in-place."""
+
 
 class LoraEmbedding(nn.Embedding, _Lora):
     __constants__ = nn.Embedding.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
 
     def __init__(
         self,
         num_embeddings: int,
@@ -138,16 +143,19 @@
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.zeros_(self.lora_a)
-            nn.init.normal_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def train(self, mode: bool = True) -> "LoraEmbedding":
         super().train(mode)
 
         if mode:
             if self.merge and self.merged:
                 # Make sure that the weights are not merged
@@ -170,16 +178,15 @@
                 self.lora_a.transpose(0, 1),
                 self.padding_idx,
                 self.max_norm,
                 self.norm_type,
                 self.scale_grad_by_freq,
                 self.sparse,
             )
-            result += (after_a @ self.lora_b.transpose(0, 1)) * self.scaling
-            return result
+            return result + (after_a @ self.lora_b.transpose(0, 1)) * self.scaling
 
         return super().forward(x)
 
 
 class LoraLinear(nn.Linear, _Lora):
     __constants__ = nn.Linear.__constants__ + ["r", "lora_alpha", "scaling", "merge", "fan_in_fan_out", "merged"]
 
@@ -220,16 +227,19 @@
         if fan_in_fan_out:
             self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def _t(self, w: Tensor) -> Tensor:
         return w.transpose(0, 1) if self.fan_in_fan_out else w
 
     def train(self, mode: bool = True) -> "LoraLinear":
         super().train(mode)
 
@@ -248,16 +258,15 @@
 
         return self
 
     def forward(self, x: Tensor) -> Tensor:
         if self.lora_a is not None and self.lora_b is not None and not self.merged:
             result = F.linear(x, self._t(self.weight), bias=self.bias)
             mm = self.dropout(x) @ self.lora_a.transpose(0, 1) @ self.lora_b.transpose(0, 1)
-            result += mm * self.scaling
-            return result
+            return result + mm * self.scaling
 
         return F.linear(x, self._t(self.weight), bias=self.bias)
 
 
 class LoraConv1d(nn.Conv1d, _Lora):
     __constants__ = nn.Conv1d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
 
@@ -303,16 +312,19 @@
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def train(self, mode: bool = True) -> "LoraConv1d":
         super().train(mode)
 
         if mode:
             if self.merge and self.merged:
                 # Make sure that the weights are not merged
@@ -329,16 +341,15 @@
         return self
 
     def forward(self, x: Tensor) -> Tensor:
         if self.lora_a is not None and self.lora_b is not None and not self.merged:
             result = F.conv1d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
             mm_a = F.conv1d(self.dropout(x), self.lora_a, None, self.stride, self.padding, self.dilation, self.groups)
             mm = F.conv1d(mm_a, self.lora_b)
-            result += mm * self.scaling
-            return result
+            return result + mm * self.scaling
 
         return F.conv1d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 
 class LoraConvTranspose1d(nn.ConvTranspose1d, _Lora):
     __constants__ = nn.ConvTranspose1d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
 
@@ -386,16 +397,19 @@
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def train(self, mode: bool = True) -> "LoraConvTranspose1d":
         super().train(mode)
 
         if mode:
             if self.merge and self.merged:
                 # Make sure that the weights are not merged
@@ -432,16 +446,15 @@
                 self.stride,
                 self.padding,
                 self.output_padding,
                 self.groups,
                 self.dilation,
             )
             mm = F.conv_transpose1d(mm_a, self.lora_b)
-            result += mm * self.scaling
-            return result
+            return result + mm * self.scaling
 
         return F.conv_transpose1d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 
 class LoraConv2d(nn.Conv2d, _Lora):
     __constants__ = nn.Conv2d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
 
@@ -487,16 +500,19 @@
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def train(self, mode: bool = True) -> "LoraConv2d":
         super().train(mode)
 
         if mode:
             if self.merge and self.merged:
                 # Make sure that the weights are not merged
@@ -513,16 +529,15 @@
         return self
 
     def forward(self, x: Tensor) -> Tensor:
         if self.lora_a is not None and self.lora_b is not None and not self.merged:
             result = F.conv2d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
             mm_a = F.conv2d(self.dropout(x), self.lora_a, None, self.stride, self.padding, self.dilation, self.groups)
             mm = F.conv2d(mm_a, self.lora_b)
-            result += mm * self.scaling
-            return result
+            return result + mm * self.scaling
 
         return F.conv2d(x, self.weight, self.bias, self.stride, self.padding, self.dilation, self.groups)
 
 
 class LoraConvTranspose2d(nn.ConvTranspose2d, _Lora):
     __constants__ = nn.ConvTranspose2d.__constants__ + ["r", "lora_alpha", "scaling", "merge", "merged"]
 
@@ -570,16 +585,19 @@
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def train(self, mode: bool = True) -> "LoraConvTranspose2d":
         super().train(mode)
 
         if mode:
             if self.merge and self.merged:
                 # Make sure that the weights are not merged
@@ -616,16 +634,15 @@
                 self.stride,
                 self.padding,
                 self.output_padding,
                 self.groups,
                 self.dilation,
             )
             mm = F.conv_transpose2d(mm_a, self.lora_b)
-            result += mm * self.scaling
-            return result
+            return result + mm * self.scaling
 
         return F.conv_transpose2d(
             x,
             self.weight,
             self.bias,
             self.stride,
             self.padding,
@@ -724,19 +741,22 @@
         self._flat_weights = [self._get_weight(wn) if hasattr(self, wn) else None for wn in self._flat_weights_names]
         self._flat_weight_refs = [weakref.ref(w) if w is not None else None for w in self._flat_weights]
         self.flatten_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
+        self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
         for wn in self._flat_weights_names:
             lora_a_name, lora_b_name = self._lora_names(wn)
             if hasattr(self, lora_a_name) and hasattr(self, lora_b_name):
                 lora_a, lora_b = getattr(self, lora_a_name), getattr(self, lora_b_name)
-                nn.init.kaiming_uniform_(lora_a, a=math.sqrt(5))
+                nn.init.kaiming_normal_(lora_a, a=math.sqrt(5))
                 nn.init.zeros_(lora_b)
 
 
 class LoraLSTM(nn.LSTM, _LoraRNN):
     def __init__(
         self,
         input_size: int,
@@ -843,16 +863,19 @@
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.zeros_(self.lora_a)
-            nn.init.normal_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def train(self, mode: bool = True) -> "LoraParallelEmbedding":
         super().train(mode)
 
         if mode:
             if self.merge and self.merged:
                 # Make sure that the weights are not merged
@@ -887,17 +910,15 @@
                 self.padding_idx,
                 self.max_norm,
                 self.norm_type,
                 self.scale_grad_by_freq,
                 self.sparse,
             )
 
-            output_parallel += (after_a_parallel @ self.lora_b.transpose(0, 1)) * self.scaling
-
-            return mp_gather(output_parallel)
+            return mp_gather(output_parallel + (after_a_parallel @ self.lora_b.transpose(0, 1)) * self.scaling)
 
         return mp_gather(output_parallel)
 
 
 class LoraColumnParallelLinear(ColumnParallelLinear, _Lora):
     __constants__ = ColumnParallelLinear.__constants__ + [
         "r",
@@ -951,16 +972,19 @@
         if fan_in_fan_out:
             self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def _t(self, w: Tensor) -> Tensor:
         return w.transpose(0, 1) if self.fan_in_fan_out else w
 
     def train(self, mode: bool = True) -> "LoraColumnParallelLinear":
         super().train(mode)
 
@@ -981,15 +1005,15 @@
 
     def forward(self, x: Tensor) -> Tensor:
         input_parallel = mp_copy(x)
 
         if self.lora_a is not None and self.lora_b is not None and not self.merged:
             output_parallel = F.linear(input_parallel, self._t(self.weight), bias=self.bias)
             mm = self.dropout(input_parallel) @ self.lora_a.transpose(0, 1) @ self.lora_b.transpose(0, 1)
-            output_parallel += mm * self.scaling
+            output_parallel = output_parallel + mm * self.scaling
             return mp_gather(output_parallel) if self.gather_output else output_parallel
 
         output_parallel = F.linear(input_parallel, self.weight, self.bias)
         return mp_gather(output_parallel) if self.gather_output else output_parallel
 
 
 class LoraRowParallelLinear(RowParallelLinear, _Lora):
@@ -1043,16 +1067,19 @@
         if fan_in_fan_out:
             self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self) -> None:
         super().reset_parameters()
 
         if hasattr(self, "lora_a") and hasattr(self, "lora_b"):
-            nn.init.kaiming_uniform_(self.lora_a, a=math.sqrt(5))
-            nn.init.zeros_(self.lora_b)
+            self.reset_lora_parameters()
+
+    def reset_lora_parameters(self) -> None:
+        nn.init.kaiming_normal_(self.lora_a, a=math.sqrt(5))
+        nn.init.zeros_(self.lora_b)
 
     def _t(self, w: Tensor) -> Tensor:
         return w.transpose(0, 1) if self.fan_in_fan_out else w
 
     def train(self, mode: bool = True) -> "LoraRowParallelLinear":
         super().train(mode)
 
@@ -1073,15 +1100,15 @@
 
     def forward(self, x: Tensor) -> Tensor:
         input_parallel = x if self.input_is_parallel else mp_scatter(x)
 
         if self.lora_a is not None and self.lora_b is not None and not self.merged:
             output_parallel = F.linear(input_parallel, self._t(self.weight), bias=self.bias)
             mm = self.dropout(input_parallel) @ self.lora_a.transpose(0, 1) @ self.lora_b.transpose(0, 1)
-            output_parallel += mm * self.scaling
+            output_parallel = output_parallel + mm * self.scaling
             output = mp_reduce(output_parallel)
             return output if self.bias is None else output + self.bias
 
         output_parallel = F.linear(input_parallel, self.weight, self.bias)
         output = mp_reduce(output_parallel)
         return output if self.bias is None else output + self.bias
 
@@ -1413,10 +1440,44 @@
     module: T_module,
     r: int | None,
     alpha: float = 1.0,
     dropout: float = 0.0,
     merge: bool = False,
     freeze: bool = True,
 ) -> T_module:
-    if freeze:
+    """Apply LoRA to a supported module, if a LoRA rank is provided.
+
+    Args:
+        module: A supported module.
+        r: The LoRA rank.
+        alpha: The LoRA alpha parameter.
+        dropout: The LoRA dropout rate.
+        merge: Whether to merge the LoRA rank into the input dimension.
+        freeze: Whether to freeze the module's parameters if a LoRA rank is
+            not provided. This argument has no effect if a LoRA rank is
+            provided, since downstream users can always freeze just the module
+            themselves. Typically, when trying out LoRA fine-tuning, downstream
+            users will want to freeze most of the module parameters and apply
+            LoRA only to a subset of the module's layers, so this is the
+            default behavior.
+
+    Returns:
+        The module with LoRA applied, if a LoRA rank is provided.
+    """
+    if freeze and r is None:
         module = cast(T_module, module.requires_grad_(False))
     return module if r is None else lora(module, r, alpha, dropout, merge)
+
+
+def reset_lora_weights_(module: nn.Module) -> None:
+    """Resets any LoRA weights in the module.
+
+    All of the LoRA modules have a ``reset_lora_parameters`` method that will
+    reset the LoRA weights in-place. This function looks for any modules with
+    this method and calls it.
+
+    Args:
+        module: The module to reset, in-place.
+    """
+    for _, submodule in module.named_modules():
+        if isinstance(submodule, _Lora):
+            submodule.reset_lora_parameters()
```

### Comparing `ml-starter-0.1.1/ml/models/norms.py` & `ml-starter-0.1.2/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/models/parallel.py` & `ml-starter-0.1.2/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/adam.py` & `ml-starter-0.1.2/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/adamw.py` & `ml-starter-0.1.2/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/adan.py` & `ml-starter-0.1.2/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/base.py` & `ml-starter-0.1.2/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/common.py` & `ml-starter-0.1.2/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/lion.py` & `ml-starter-0.1.2/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/sgd.py` & `ml-starter-0.1.2/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/optimizers/shampoo.py` & `ml-starter-0.1.2/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/scripts/cli.py` & `ml-starter-0.1.2/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/scripts/stage.py` & `ml-starter-0.1.2/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/scripts/train.py` & `ml-starter-0.1.2/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/base.py` & `ml-starter-0.1.2/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.2/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.2/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/collate.py` & `ml-starter-0.1.2/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.2/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.2/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.2/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.2/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.2/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/utils.py` & `ml-starter-0.1.2/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.2/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/environments/base.py` & `ml-starter-0.1.2/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/environments/utils.py` & `ml-starter-0.1.2/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/environments/worker.py` & `ml-starter-0.1.2/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/losses/reduce.py` & `ml-starter-0.1.2/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/rl/base.py` & `ml-starter-0.1.2/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/rl/replay.py` & `ml-starter-0.1.2/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/tasks/sl/base.py` & `ml-starter-0.1.2/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/base.py` & `ml-starter-0.1.2/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/learning.py` & `ml-starter-0.1.2/ml/trainers/learning.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,32 +83,38 @@
         model: ModelT,
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> dict[str, Tensor]:
         with self.step_context("change_mode"):
             task_model, state.phase = set_phase(task_model, "train")
         total_bsz: int | None = None
-        first_batch = True
+        losses: dict[str, tuple[Tensor, int]] = {}
         for batch in batches:
             bsz = task.get_batch_size(batch)
             if bsz is not None:
                 total_bsz = bsz if total_bsz is None else total_bsz + bsz
             with self.step_context("forward"), self.autocast_context():
                 loss = task_model(batch, state)
             with self.step_context("get_single_loss"):
                 single_loss, loss_names = task.get_single_loss(loss)
             with self.step_context("backward"):
                 self.scale_mixed_precision(single_loss.sum()).backward()
-            if first_batch:
-                with self.step_context("log_losses"):
-                    self.log_mp_scale()
-                    single_loss_detached = single_loss.detach()
-                    loss_dict = {name: single_loss_detached[i] for i, name in enumerate(loss_names)}
-                    task.log_loss_dict(loss_dict, state)
-                first_batch = False
+            with self.step_context("log_losses"):
+                self.log_mp_scale()
+                single_loss_detached = single_loss.detach()
+                for i, name in enumerate(loss_names):
+                    new_loss = single_loss_detached[i]
+                    if name in losses:
+                        old_loss, count = losses[name]
+                        losses[name] = (old_loss + new_loss, count + 1)
+                    else:
+                        losses[name] = (new_loss, 1)
+        with self.step_context("log_losses"):
+            loss_dict = {k: value / count for k, (value, count) in losses.items()}
+            task.log_loss_dict(loss_dict, state)
         with self.step_context("clip_grads"):
             self.clip_grads(model=task_model, optim=optim)
         with self.step_context("step"):
             self.step_optimizer(optim=optim)
             lr_sched.step(state)
             self.logger.log_scalar("lr_scale", lr_sched.lr_scale, namespace="optim")
         with self.step_context("zero_grads"):
```

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/compile.py` & `ml-starter-0.1.2/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.2/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.2/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.2/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.1.2/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.2/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.2/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.2/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.2/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.2/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/rl.py` & `ml-starter-0.1.2/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/trainers/sl.py` & `ml-starter-0.1.2/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/argparse.py` & `ml-starter-0.1.2/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/atomic.py` & `ml-starter-0.1.2/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/audio.py` & `ml-starter-0.1.2/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/augmentation.py` & `ml-starter-0.1.2/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/caching.py` & `ml-starter-0.1.2/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/checkpoint.py` & `ml-starter-0.1.2/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/cli.py` & `ml-starter-0.1.2/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/colors.py` & `ml-starter-0.1.2/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/data.py` & `ml-starter-0.1.2/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/datetime.py` & `ml-starter-0.1.2/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/device/auto.py` & `ml-starter-0.1.2/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/device/base.py` & `ml-starter-0.1.2/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/device/cpu.py` & `ml-starter-0.1.2/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/device/gpu.py` & `ml-starter-0.1.2/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/device/metal.py` & `ml-starter-0.1.2/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/distributed.py` & `ml-starter-0.1.2/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/image.py` & `ml-starter-0.1.2/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/large_models.py` & `ml-starter-0.1.2/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/logging.py` & `ml-starter-0.1.2/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/meter.py` & `ml-starter-0.1.2/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/parallel.py` & `ml-starter-0.1.2/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/staging.py` & `ml-starter-0.1.2/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/timer.py` & `ml-starter-0.1.2/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/tokens.py` & `ml-starter-0.1.2/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/torch_distributed.py` & `ml-starter-0.1.2/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/triton/kmeans.py` & `ml-starter-0.1.2/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/triton/lion.py` & `ml-starter-0.1.2/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml/utils/video.py` & `ml-starter-0.1.2/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.2/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.1
+Version: 0.1.2
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.1/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.2/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/pyproject.toml` & `ml-starter-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.1/setup.py` & `ml-starter-0.1.2/setup.py`

 * *Files identical despite different names*

