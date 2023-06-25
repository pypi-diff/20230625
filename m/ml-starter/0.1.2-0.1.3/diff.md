# Comparing `tmp/ml-starter-0.1.2.tar.gz` & `tmp/ml-starter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.2.tar", last modified: Sun Jun 25 01:32:29 2023, max compression
+gzip compressed data, was "ml-starter-0.1.3.tar", last modified: Sun Jun 25 06:46:44 2023, max compression
```

## Comparing `ml-starter-0.1.2.tar` & `ml-starter-0.1.3.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 01:32:14.000000 ml-starter-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-25 01:32:14.000000 ml-starter-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 01:32:29.025124 ml-starter-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-25 01:32:14.000000 ml-starter-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.009124 ml-starter-0.1.2/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.009124 ml-starter-0.1.2/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.013124 ml-starter-0.1.2/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.017124 ml-starter-0.1.2/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.021124 ml-starter-0.1.2/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-25 01:32:14.000000 ml-starter-0.1.2/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:32:29.025124 ml-starter-0.1.2/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-25 01:32:29.000000 ml-starter-0.1.2/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-25 01:32:28.000000 ml-starter-0.1.2/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 01:32:14.000000 ml-starter-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-25 01:32:14.000000 ml-starter-0.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 01:32:14.000000 ml-starter-0.1.2/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 01:32:14.000000 ml-starter-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-25 01:32:29.025124 ml-starter-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 01:32:14.000000 ml-starter-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.610906 ml-starter-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 06:46:26.000000 ml-starter-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-25 06:46:26.000000 ml-starter-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 06:46:44.610906 ml-starter-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-25 06:46:26.000000 ml-starter-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.582906 ml-starter-0.1.3/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.582906 ml-starter-0.1.3/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.582906 ml-starter-0.1.3/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.586906 ml-starter-0.1.3/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.586906 ml-starter-0.1.3/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.586906 ml-starter-0.1.3/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.586906 ml-starter-0.1.3/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49884 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.590906 ml-starter-0.1.3/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.590906 ml-starter-0.1.3/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.590906 ml-starter-0.1.3/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.594906 ml-starter-0.1.3/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.594906 ml-starter-0.1.3/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.594906 ml-starter-0.1.3/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.594906 ml-starter-0.1.3/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.594906 ml-starter-0.1.3/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.598906 ml-starter-0.1.3/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.598906 ml-starter-0.1.3/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.606906 ml-starter-0.1.3/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.606906 ml-starter-0.1.3/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.606906 ml-starter-0.1.3/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-06-25 06:46:26.000000 ml-starter-0.1.3/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:46:44.610906 ml-starter-0.1.3/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 06:46:44.000000 ml-starter-0.1.3/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-25 06:46:44.000000 ml-starter-0.1.3/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:46:44.000000 ml-starter-0.1.3/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-25 06:46:44.000000 ml-starter-0.1.3/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-25 06:46:44.000000 ml-starter-0.1.3/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 06:46:26.000000 ml-starter-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-25 06:46:26.000000 ml-starter-0.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 06:46:26.000000 ml-starter-0.1.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 06:46:26.000000 ml-starter-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-25 06:46:44.610906 ml-starter-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-25 06:46:26.000000 ml-starter-0.1.3/setup.py
```

### Comparing `ml-starter-0.1.2/LICENSE` & `ml-starter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/PKG-INFO` & `ml-starter-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.2
+Version: 0.1.3
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.2/README.md` & `ml-starter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/api.py` & `ml-starter-0.1.3/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/core/common_types.py` & `ml-starter-0.1.3/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/core/config.py` & `ml-starter-0.1.3/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/core/env.py` & `ml-starter-0.1.3/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/core/registry.py` & `ml-starter-0.1.3/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/core/state.py` & `ml-starter-0.1.3/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/launchers/base.py` & `ml-starter-0.1.3/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/launchers/mp.py` & `ml-starter-0.1.3/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/launchers/slurm.py` & `ml-starter-0.1.3/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/launchers/torchrun.py` & `ml-starter-0.1.3/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/loggers/base.py` & `ml-starter-0.1.3/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/loggers/meter.py` & `ml-starter-0.1.3/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/loggers/multi.py` & `ml-starter-0.1.3/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/loggers/stdout.py` & `ml-starter-0.1.3/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/loggers/tensorboard.py` & `ml-starter-0.1.3/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/base.py` & `ml-starter-0.1.3/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/constant.py` & `ml-starter-0.1.3/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.3/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.3/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/linear.py` & `ml-starter-0.1.3/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.3/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.3/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/activations.py` & `ml-starter-0.1.3/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/base.py` & `ml-starter-0.1.3/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/embeddings.py` & `ml-starter-0.1.3/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/init.py` & `ml-starter-0.1.3/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/kmeans.py` & `ml-starter-0.1.3/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/lora.py` & `ml-starter-0.1.3/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/norms.py` & `ml-starter-0.1.3/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/models/parallel.py` & `ml-starter-0.1.3/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/adam.py` & `ml-starter-0.1.3/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/adamw.py` & `ml-starter-0.1.3/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/adan.py` & `ml-starter-0.1.3/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/base.py` & `ml-starter-0.1.3/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/common.py` & `ml-starter-0.1.3/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/lion.py` & `ml-starter-0.1.3/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/sgd.py` & `ml-starter-0.1.3/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/optimizers/shampoo.py` & `ml-starter-0.1.3/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/scripts/cli.py` & `ml-starter-0.1.3/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/scripts/stage.py` & `ml-starter-0.1.3/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/scripts/train.py` & `ml-starter-0.1.3/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/base.py` & `ml-starter-0.1.3/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.3/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.3/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/collate.py` & `ml-starter-0.1.3/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.3/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.3/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.3/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.3/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.3/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/utils.py` & `ml-starter-0.1.3/ml/tasks/datasets/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,29 +21,34 @@
 from torch.utils.data.dataset import Dataset, IterableDataset
 
 from ml.utils.logging import configure_logging
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def test_dataset(ds: Dataset | IterableDataset | DataLoader, max_samples: int = 3) -> None:
+def test_dataset(
+    ds: Dataset | IterableDataset | DataLoader,
+    max_samples: int = 3,
+    log_interval: int = 10,
+) -> None:
     """Iterates through a dataset.
 
     Args:
         ds: The dataset to iterate through
         max_samples: Maximum number of samples to loop through
+        log_interval: How often to log the time it takes to load a sample
     """
     configure_logging(use_tqdm=True)
     start_time = time.time()
 
     if isinstance(ds, (IterableDataset, DataLoader)):
         logger.info("Iterating samples in %s", "dataloader" if isinstance(ds, DataLoader) else "dataset")
         for i, _ in enumerate(itertools.islice(ds, max_samples)):
-            if i % 10 == 0:
+            if i % log_interval == 0:
                 logger.info("Sample %d in %.2g seconds", i, time.time() - start_time)
     else:
         samples = len(ds)  # type: ignore[arg-type]
         logger.info("Dataset has %d items", samples)
         for i in tqdm.trange(min(samples, max_samples)):
             _ = ds[i]
-            if i % 10 == 0:
+            if i % log_interval == 0:
                 logger.info("Sample %d in %.2g seconds", i, time.time() - start_time)
```

### Comparing `ml-starter-0.1.2/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.3/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/environments/base.py` & `ml-starter-0.1.3/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/environments/utils.py` & `ml-starter-0.1.3/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/environments/worker.py` & `ml-starter-0.1.3/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/losses/reduce.py` & `ml-starter-0.1.3/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/rl/base.py` & `ml-starter-0.1.3/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/rl/replay.py` & `ml-starter-0.1.3/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/tasks/sl/base.py` & `ml-starter-0.1.3/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/base.py` & `ml-starter-0.1.3/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/learning.py` & `ml-starter-0.1.3/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/compile.py` & `ml-starter-0.1.3/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.3/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.3/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.3/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.1.3/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.3/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.3/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.3/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.3/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.3/ml/trainers/mixins/step_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,19 +40,14 @@
 
     def __init__(self, step: StepType) -> None:
         self.step = step
 
     def __enter__(self) -> None:
         StepContext.CURRENT_STEP = self.step
 
-    def __exit__(
-        self,
-        exc_type: type[BaseException] | None,
-        exc: BaseException | None,
-        traceback: TracebackType | None,
-    ) -> None:
+    def __exit__(self, _t: type[BaseException] | None, _e: BaseException | None, _tr: TracebackType | None) -> None:
         StepContext.CURRENT_STEP = None
 
 
 class StepContextMixin(BaseTrainer[BaseTrainerConfigT, ModelT, TaskT], ABC):
     def step_context(self, step: StepType) -> ContextManager:
         return StepContext(step)
```

### Comparing `ml-starter-0.1.2/ml/trainers/rl.py` & `ml-starter-0.1.3/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/trainers/sl.py` & `ml-starter-0.1.3/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/argparse.py` & `ml-starter-0.1.3/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/atomic.py` & `ml-starter-0.1.3/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/audio.py` & `ml-starter-0.1.3/ml/utils/audio.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 """
 
 import fractions
 import shutil
 import warnings
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterator, Literal
+from typing import Iterator, Literal, TypeVar
 
 import av
 import numpy as np
 import soundfile as sf
 import torch
 import torchaudio.functional as A
 from torch import Tensor
 
+from ml.utils.io import prefetch_samples
 from ml.utils.numpy import as_numpy_array
 
+T = TypeVar("T")
+
+DEFAULT_BLOCKSIZE = 16_000
+
 
 @dataclass
 class AudioProps:
     sample_rate: int
     channels: int
     num_frames: int
 
@@ -75,15 +80,15 @@
 
 def _cleanup_wav_chunk(wav: np.ndarray, channels: int | None = None) -> np.ndarray:
     if wav.ndim == 1:
         wav = wav.reshape(-1, 1 if channels is None else channels).T
     return wav
 
 
-def read_audio_sf(in_file: str | Path, *, blocksize: int = 16_000) -> Iterator[np.ndarray]:
+def read_audio_sf(in_file: str | Path, *, blocksize: int = DEFAULT_BLOCKSIZE) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using SoundFile.
 
     Args:
         in_file: Path to the input file.
         blocksize: Number of samples to read at a time.
 
     Yields:
@@ -111,15 +116,15 @@
         for frame in container.decode(stream):
             frame_np = frame.to_ndarray().reshape(-1, props.channels).T
             if frame_np.dtype == np.int16:
                 frame_np = frame_np.astype(np.float32) / 2**15
             yield frame_np
 
 
-def read_audio_ffmpeg(in_file: str | Path, *, chunk_size: int = 16_000) -> Iterator[np.ndarray]:
+def read_audio_ffmpeg(in_file: str | Path, *, chunk_size: int = DEFAULT_BLOCKSIZE) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using FFMPEG.
 
     Args:
         in_file: Path to the input file.
         chunk_size: Size of the chunks to read.
 
     Yields:
@@ -263,25 +268,26 @@
 
     raise ValueError(f"Unknown reader {reader}")
 
 
 def _resample_audio(
     audio_chunks: Iterator[np.ndarray],
     *,
+    prefetch_n: int = 1,
     chunk_length: int | None = None,
     sampling_rate: tuple[int, int] | None = None,
 ) -> Iterator[np.ndarray]:
     if chunk_length is None:
-        yield from audio_chunks
+        yield from prefetch_samples(audio_chunks, prefetch_n)
         return
 
     audio_chunk_list: list[np.ndarray] = []
     total_length: int = 0
-    for chunk in audio_chunks:
-        if sampling_rate is not None:
+    for chunk in prefetch_samples(audio_chunks, prefetch_n):
+        if sampling_rate is not None and sampling_rate[0] != sampling_rate[1]:
             chunk = A.resample(torch.from_numpy(chunk), sampling_rate[0], sampling_rate[1]).numpy()
         cur_chunk_length = chunk.shape[-1]
         while total_length + cur_chunk_length >= chunk_length:
             yield np.concatenate(audio_chunk_list + [chunk[..., : chunk_length - total_length]], axis=-1)
             chunk = chunk[..., chunk_length - total_length :]
             audio_chunk_list = []
             total_length = 0
@@ -293,24 +299,28 @@
     if audio_chunk_list:
         yield np.concatenate(audio_chunk_list, axis=-1)
 
 
 def read_audio(
     in_file: str | Path,
     *,
+    blocksize: int = DEFAULT_BLOCKSIZE,
+    prefetch_n: int = 1,
     chunk_length: int | None = None,
     sampling_rate: int | None = None,
     reader: Reader = "sf",
 ) -> Iterator[np.ndarray]:
     """Function that reads a stream of audio from a file.
 
     The output audio is in ``float32`` format.
 
     Args:
         in_file: Path to the input file.
+        blocksize: Number of samples to read at a time.
+        prefetch_n: Number of chunks to prefetch.
         chunk_length: Size of the chunks to read. If ``None``, will iterate
             whatever chunk size the underlying reader uses. Otherwise, samples
             will be rechunked to the desired size.
         sampling_rate: Sampling rate to resample the audio to. If ``None``,
             will use the sampling rate of the input audio.
         reader: Reader to use. Can be either ``sf``, ``ffmpeg`` or ``av``.
 
@@ -319,23 +329,38 @@
     """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             reader = "av"
         else:
             sr = None if sampling_rate is None else (AudioProps.from_file_ffmpeg(in_file).sample_rate, sampling_rate)
-            return _resample_audio(read_audio_ffmpeg(in_file), chunk_length=chunk_length, sampling_rate=sr)
+            return _resample_audio(
+                read_audio_ffmpeg(in_file, chunk_size=blocksize),
+                prefetch_n=prefetch_n,
+                chunk_length=chunk_length,
+                sampling_rate=sr,
+            )
 
     if reader == "sf":
         sr = None if sampling_rate is None else (AudioProps.from_file_sf(in_file).sample_rate, sampling_rate)
-        return _resample_audio(read_audio_sf(in_file), chunk_length=chunk_length, sampling_rate=sr)
+        return _resample_audio(
+            read_audio_sf(in_file, blocksize=blocksize),
+            prefetch_n=prefetch_n,
+            chunk_length=chunk_length,
+            sampling_rate=sr,
+        )
 
     if reader == "av":
         sr = None if sampling_rate is None else (AudioProps.from_file_av(in_file).sample_rate, sampling_rate)
-        return _resample_audio(read_audio_av(in_file), chunk_length=chunk_length, sampling_rate=sr)
+        return _resample_audio(
+            read_audio_av(in_file),
+            prefetch_n=prefetch_n,
+            chunk_length=chunk_length,
+            sampling_rate=sr,
+        )
 
     raise ValueError(f"Unknown reader {reader}")
 
 
 def write_audio(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
```

### Comparing `ml-starter-0.1.2/ml/utils/augmentation.py` & `ml-starter-0.1.3/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/caching.py` & `ml-starter-0.1.3/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/checkpoint.py` & `ml-starter-0.1.3/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/cli.py` & `ml-starter-0.1.3/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/colors.py` & `ml-starter-0.1.3/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/data.py` & `ml-starter-0.1.3/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/datetime.py` & `ml-starter-0.1.3/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/device/auto.py` & `ml-starter-0.1.3/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/device/base.py` & `ml-starter-0.1.3/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/device/cpu.py` & `ml-starter-0.1.3/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/device/gpu.py` & `ml-starter-0.1.3/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/device/metal.py` & `ml-starter-0.1.3/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/distributed.py` & `ml-starter-0.1.3/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/image.py` & `ml-starter-0.1.3/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/large_models.py` & `ml-starter-0.1.3/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/logging.py` & `ml-starter-0.1.3/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/meter.py` & `ml-starter-0.1.3/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/parallel.py` & `ml-starter-0.1.3/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/staging.py` & `ml-starter-0.1.3/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/timer.py` & `ml-starter-0.1.3/ml/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import os
 import signal
 import sys
 import threading
 import time
 import warnings
 from threading import Thread
-from typing import Any, Callable, TypeVar
+from types import TracebackType
+from typing import Any, Callable, ContextManager, TypeVar
 
 from ml.utils.colors import colorize
 from ml.utils.distributed import is_master
 
 timer_logger: logging.Logger = logging.getLogger(__name__)
 
 TimeoutFunc = TypeVar("TimeoutFunc", bound=Callable[..., Any])
@@ -93,15 +94,15 @@
 
 
 @functools.lru_cache
 def spinner() -> Spinner:
     return Spinner()
 
 
-class Timer:
+class Timer(ContextManager):
     """Defines a simple timer for logging an event."""
 
     def __init__(
         self,
         description: str,
         min_seconds_to_print: float = 5.0,
         logger: logging.Logger | None = None,
@@ -121,15 +122,15 @@
 
     def __enter__(self) -> "Timer":
         self._start_time = time.time()
         if self._use_spinner:
             spinner().set_text(self.description).start()
         return self
 
-    def __exit__(self, *args: Any, **kwargs: Any) -> None:  # noqa: ANN401
+    def __exit__(self, _t: type[BaseException] | None, _e: BaseException | None, _tr: TracebackType | None) -> None:
         assert self._start_time is not None
         self._elapsed_time = time.time() - self._start_time
         if self._elapsed_time > self.min_seconds_to_print:
             self._logger.warning("Finished %s in %.3g seconds", self.description, self._elapsed_time)
         spinner().stop()
```

### Comparing `ml-starter-0.1.2/ml/utils/tokens.py` & `ml-starter-0.1.3/ml/utils/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 
 import functools
 import gzip
 import logging
 import math
 import struct
 from pathlib import Path
-from typing import BinaryIO, Literal, Sequence
+from types import TracebackType
+from typing import BinaryIO, ContextManager, Literal, Sequence
 
 logger = logging.getLogger(__name__)
 
 NumberFormat = Literal["Q", "I", "H", "B"]
 
 MAGIC = b"MLTK"  # Magic number for the token file format.
 OFFSET_MAGIC = b"MLTO"  # Magic number for the offsets file format.
@@ -91,15 +92,15 @@
             arr.append(int(cur_token[:num_bits], 2))
             if len(arr) == seq_len:
                 return arr
             cur_token = cur_token[num_bits:]
     raise ValueError("Not enough bytes to fill sequence")
 
 
-class TokenWriter:
+class TokenWriter(ContextManager):
     """Helper class for writing a dataset of tokens to a file.
 
     This class can be used in conjunction with :class:`TokenReader` to write
     and read datasets of tokens. The default numerical formats are chosen to
     work well with typical ranges of token datasets. At the upper end, this
     supports ``2 ^ 32`` tokens, ``2 ^ 32`` tokens per line, and ``2 ^ 64``
     tokens per file.
@@ -146,15 +147,15 @@
         # Writes the file header.
         self._fp.write(MAGIC)
         self._fp.write((self._num_tokens_fmt + self._lengths_fmt + self._offset_fmt).encode("ascii"))
         self._fp.write(struct.pack(self._num_tokens_fmt, self._num_tokens))
 
         return self
 
-    def __exit__(self, _t: type[Exception] | None, _v: Exception | None, _tb: object | None) -> None:
+    def __exit__(self, _t: type[BaseException] | None, _e: BaseException | None, _tr: TracebackType | None) -> None:
         assert self._fp is not None
 
         self._fp.close()
 
     def write(self, tokens: Sequence[int]) -> None:
         assert self._fp is not None, "TokenWriter must be opened with a context manager"
```

### Comparing `ml-starter-0.1.2/ml/utils/torch_distributed.py` & `ml-starter-0.1.3/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/triton/kmeans.py` & `ml-starter-0.1.3/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/triton/lion.py` & `ml-starter-0.1.3/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/ml/utils/video.py` & `ml-starter-0.1.3/ml/utils/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 import av
 import numpy as np
 import torchvision.transforms.functional as F
 from torch import Tensor
 
 from ml.utils.image import as_uint8, standardize_image
+from ml.utils.io import prefetch_samples
 
 
 @functools.lru_cache()
 def ffmpeg_python_available() -> bool:
     try:
         import ffmpeg
 
@@ -124,14 +125,22 @@
                     frame_count=count,
                     fps=Fraction(int(fps_num), int(fps_denom)),
                 )
 
         raise ValueError(f"Could not parse video properties from video in {fpath}")
 
 
+def _resample_video(
+    video_chunks: Iterator[np.ndarray],
+    *,
+    prefetch_n: int = 1,
+) -> Iterator[np.ndarray]:
+    yield from prefetch_samples(video_chunks, prefetch_n)
+
+
 def read_video_av(
     in_file: str | Path,
     *,
     target_dims: tuple[int | None, int | None] | None = None,
 ) -> Iterator[np.ndarray]:
     """Function that reads a video file to a stream of numpy arrays using PyAV.
 
@@ -529,43 +538,58 @@
 
     if reader == "av":
         return VideoProps.from_file_av(in_file)
 
     raise ValueError(f"Unknown reader {reader}")
 
 
-def read_video(in_file: str | Path, *, reader: Reader = "av") -> Iterator[np.ndarray]:
+def read_video(
+    in_file: str | Path,
+    *,
+    prefetch_n: int = 1,
+    reader: Reader = "av",
+) -> Iterator[np.ndarray]:
     """Function that reads a video from a file to a stream of Numpy arrays.
 
     Args:
         in_file: The path to the input file.
+        prefetch_n: Number of chunks to prefetch.
         reader: The video reader to use.
 
     Yields:
         The video frames as Numpy arrays.
     """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in the system.")
             reader = "av"
         elif not ffmpeg_python_available():
             warnings.warn("FFMPEG Python is not installed; install with `pip install ffmpeg-python`")
             reader = "av"
         else:
-            return read_video_ffmpeg(in_file)
+            return _resample_video(
+                read_video_ffmpeg(in_file),
+                prefetch_n=prefetch_n,
+            )
 
     if reader == "opencv":
         if not cv2_available():
             warnings.warn("OpenCV is not installed; install with `pip install opencv-python`")
             reader = "av"
         else:
-            return read_video_opencv(in_file)
+            return _resample_video(
+                read_video_opencv(in_file),
+                prefetch_n=prefetch_n,
+            )
 
     if reader == "av":
-        return read_video_av(in_file)
+        return _resample_video(
+            read_video_av(in_file),
+            prefetch_n=prefetch_n,
+        )
 
     raise ValueError(f"Invalid reader: {reader}")
 
 
 def write_video(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
```

### Comparing `ml-starter-0.1.2/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.3/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.2
+Version: 0.1.3
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.2/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.3/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 ml/utils/checks.py
 ml/utils/cli.py
 ml/utils/colors.py
 ml/utils/data.py
 ml/utils/datetime.py
 ml/utils/distributed.py
 ml/utils/image.py
+ml/utils/io.py
 ml/utils/large_models.py
 ml/utils/logging.py
 ml/utils/meter.py
 ml/utils/networking.py
 ml/utils/numpy.py
 ml/utils/parallel.py
 ml/utils/random.py
```

### Comparing `ml-starter-0.1.2/pyproject.toml` & `ml-starter-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.2/setup.py` & `ml-starter-0.1.3/setup.py`

 * *Files identical despite different names*

