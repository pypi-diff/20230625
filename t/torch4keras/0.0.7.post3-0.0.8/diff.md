# Comparing `tmp/torch4keras-0.0.7.post3.tar.gz` & `tmp/torch4keras-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.0.7.post3.tar", last modified: Thu May 18 14:52:57 2023, max compression
+gzip compressed data, was "torch4keras-0.0.8.tar", last modified: Sun Jun 25 15:00:44 2023, max compression
```

## Comparing `torch4keras-0.0.7.post3.tar` & `torch4keras-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 14:52:57.063193 torch4keras-0.0.7.post3/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.7.post3/LICENSE
--rw-rw-rw-   0        0        0     6839 2023-05-18 14:52:57.060190 torch4keras-0.0.7.post3/PKG-INFO
--rw-rw-rw-   0        0        0     6579 2023-05-18 14:49:58.000000 torch4keras-0.0.7.post3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 14:52:57.063193 torch4keras-0.0.7.post3/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-05-18 14:50:18.000000 torch4keras-0.0.7.post3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:52:57.054190 torch4keras-0.0.7.post3/torch4keras/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:52:53.000000 torch4keras-0.0.7.post3/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    43413 2023-05-17 13:36:22.000000 torch4keras-0.0.7.post3/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0    23549 2023-05-17 13:39:27.000000 torch4keras-0.0.7.post3/torch4keras/model.py
--rw-rw-rw-   0        0        0     8167 2023-04-24 15:56:30.000000 torch4keras-0.0.7.post3/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:52:57.060190 torch4keras-0.0.7.post3/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     6839 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-18 14:52:56.000000 torch4keras-0.0.7.post3/torch4keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 15:00:44.504998 torch4keras-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     7252 2023-06-25 15:00:44.502000 torch4keras-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6998 2023-06-25 14:58:24.000000 torch4keras-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 15:00:44.504998 torch4keras-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-05-21 14:39:27.000000 torch4keras-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:00:44.492006 torch4keras-0.0.8/torch4keras/
+-rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.0.8/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    51485 2023-06-10 11:46:06.000000 torch4keras-0.0.8/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    28907 2023-06-10 16:08:50.000000 torch4keras-0.0.8/torch4keras/model.py
+-rw-rw-rw-   0        0        0    13928 2023-06-10 03:46:15.000000 torch4keras-0.0.8/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:00:44.500993 torch4keras-0.0.8/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     7252 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.0.7.post3/LICENSE` & `torch4keras-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.0.7.post3/PKG-INFO` & `torch4keras-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.0.7.post3
+Version: 0.0.8
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,14 +16,15 @@
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
 
 [Documentation](https://torch4keras.readthedocs.io) |
+[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
 [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
 [Source code](https://github.com/Tongjilibo/torch4keras)
 
 ## 1. 下载安装
 安装稳定版
 ```shell
 pip install torch4keras
@@ -70,26 +71,28 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
 - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
```

### Comparing `torch4keras-0.0.7.post3/README.md` & `torch4keras-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
 
 [Documentation](https://torch4keras.readthedocs.io) |
+[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
 [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
 [Source code](https://github.com/Tongjilibo/torch4keras)
 
 ## 1. 下载安装
 安装稳定版
 ```shell
 pip install torch4keras
@@ -60,26 +61,28 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
 - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
```

### Comparing `torch4keras-0.0.7.post3/setup.py` & `torch4keras-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='torch4keras',
-    version='v0.0.7.post3',
+    version='v0.0.8',
     description='Use torch like keras',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License',
     url='https://github.com/Tongjilibo/torch4keras',
     author='Tongjilibo',
     install_requires=[],
```

### Comparing `torch4keras-0.0.7.post3/torch4keras/callbacks.py` & `torch4keras-0.0.8/torch4keras/callbacks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+from contextlib import redirect_stderr
 import sys
 import collections
 import time
 import numpy as np
 from datetime import datetime
-from tqdm import tqdm
 import warnings
 from collections import deque
 import json
 import copy
 import os
+from torch import nn
+from torch4keras.snippets import send_email, info_level_prefix
 
-try:
-    import requests
-except ImportError:
-    requests = None
 
 class Progbar(object):
-    """进度条，直接从keras引入
-    """
+    """进度条，直接从keras引入"""
     def __init__(self, target, width=30, verbose=1, interval=0.05, stateful_metrics=None):
         self.target = target
         self.width = width
         self.verbose = verbose
         self.interval = interval
         if stateful_metrics:
             self.stateful_metrics = set(stateful_metrics)
@@ -32,16 +29,15 @@
         self._total_width = 0
         self._seen_so_far = 0
         self._values = collections.OrderedDict()
         self._start = time.time()
         self._last_update = 0
 
     def update(self, current, values=None):
-        """Updates the progress bar.
-        """
+        """Updates the progress bar."""
         values = values or []
         for k, v in values:
             if k not in self.stateful_metrics:
                 if k not in self._values:
                     self._values[k] = [v * (current - self._seen_so_far),
                                        current - self._seen_so_far]
                 else:
@@ -119,15 +115,15 @@
                         self._values[k][0] / max(1, self._values[k][1]))
                     if abs(avg) > 1e-3:
                         info += ' %.4f' % avg
                     else:
                         info += ' %.4e' % avg
                 else:
                     info += ' %s' % self._values[k]
-
+            info += ' '  # 最后加个空格，防止中途有别的打印
             self._total_width += len(info)
             if prev_total_width > self._total_width:
                 info += (' ' * (prev_total_width - self._total_width))
 
             if self.target is not None and current >= self.target:
                 info += '\n'
 
@@ -270,16 +266,15 @@
             callback.on_train_step_end(logs)
 
     def __iter__(self):
         return iter(self.callbacks)
 
 
 class Callback(object):
-    '''Callback基类
-    '''
+    '''Callback基类'''
     def __init__(self, run_callback=True, **kwargs):
         self.trainer = None  # trainer
         self.model = None  # nn.Module模型，或者包含Trainer的nn.Module
         self.optimizer = None  # 优化器
         self.run_callback = run_callback  # 是否运行该callback
     def set_params(self, params):
         self.params = params
@@ -349,30 +344,28 @@
                     if k in self.stateful_metrics:
                         logs[k] = self.totals[k]
                     else:
                         logs[k] = self.totals[k] / self.seen
 
 
 class TerminateOnNaN(Callback):
-    """Loss出现NAN停止训练
-    """
+    """Loss出现NAN停止训练"""
     def on_batch_end(self, global_step, local_step, logs=None):
         logs = logs or {}
         loss = logs.get('loss')
         if loss is not None:
             if np.isnan(loss) or np.isinf(loss):
-                print('Step %d: Invalid loss, terminating training' % global_step)
+                info_level_prefix('Step %d: Invalid loss, terminating training' % global_step, 2)
                 self.trainer.stop_training = True
 
 
-class ProgbarLogger(Callback):
-    """ keras进度条
-    """
+class KerasProgbar(Callback):
+    """ keras进度条 """
     def __init__(self, stateful_metrics=None, **kwargs):
-        super(ProgbarLogger, self).__init__(**kwargs)
+        super(KerasProgbar, self).__init__(**kwargs)
         if stateful_metrics:
             self.stateful_metrics = set(stateful_metrics)
         else:
             self.stateful_metrics = set()
 
     def add_metrics(self, metrics, stateful_metrics=None, add_position=None):
         '''在指定位置插入metrics指标
@@ -432,19 +425,19 @@
     
     def on_train_end(self, logs=None):
         if self.verbose:
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Finish Training' % (time_start))
 
 
-class TqdmProgressBar(ProgbarLogger):
-    """ Tqdm进度条
-    """
+class TqdmProgbar(KerasProgbar):
+    """ Tqdm进度条 """
     def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
         if self.verbose:
+            from tqdm import tqdm
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
             self.target = self.params['steps']
             self.progbar = tqdm(total=self.params['steps'], desc='Training', dynamic_ncols=False, file=sys.stdout, smoothing=0)
         self.seen = 0
         self._values = collections.OrderedDict()
         self._seen_so_far = 0
@@ -475,16 +468,15 @@
         if self.verbose:
             self.progbar.n = self.seen
             self.progbar.refresh()
             self.progbar.set_postfix(self.log_values)
             self.progbar.close()
     
     def smooth_values(self, current, values=None):
-        '''从Progbar迁移过来
-        '''
+        '''从Progbar迁移过来'''
         values = values or []
         for k, v in values.items():
             if k not in self.stateful_metrics:
                 if k not in self._values:
                     self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
                 else:
                     self._values[k][0] += v * (current - self._seen_so_far)
@@ -504,17 +496,58 @@
                     logs[k] = ' %.4e' % avg
             else:
                 logs[k] = ' %s' % self._values[k]
 
         return logs
 
 
+class ProgressBar2Progbar(TqdmProgbar):
+    """ progressbar2进度条 """
+    def on_epoch_begin(self, global_step=None, epoch=None, logs=None):
+        if self.verbose:
+            import progressbar
+            time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            print('%s - Epoch: %d/%d' % (time_start, epoch+1, self.epochs))
+            self.target = self.params['steps']
+            widgets = [progressbar.SimpleProgress(format='%(value_s)s/%(max_value_s)s'), progressbar.Bar(marker='=', left='[', right=']'), ' ', 
+                       progressbar.AdaptiveETA(format='ETA: %(eta)s', format_finished='Time: %(elapsed)s'), ' - ']
+            for i, param in enumerate(self.params['metrics']):
+                widgets.append(progressbar.Variable(param, precision=7))
+                if i < len(self.params['metrics'])-1:
+                    widgets.append(' - ')
+            self.progbar = progressbar.bar.ProgressBar(min_value=0, max_value=self.params['steps'], widgets=widgets, 
+                                                       redirect_stdout=True, redirect_stderr=True)
+        self.seen = 0
+        self._values = collections.OrderedDict()
+        self._seen_so_far = 0
+
+    def on_batch_begin(self, global_step=None, local_step=None, logs=None):
+        if self.seen < self.target:
+            self.log_values = []
+
+    def on_batch_end(self, global_step=None, local_step=None, logs=None):
+        self.seen += 1
+        logs = self.smooth_values(self.seen, logs or {})
+        logs_new = {k:logs[k].strip() for k in self.params['metrics'] if k in logs}
+
+        # Skip progbar update for the last batch;
+        # will be handled by on_epoch_end.
+        if self.verbose and self.seen < self.target:
+            self.progbar.update(self.seen, **logs_new)
+
+    def on_epoch_end(self, global_step=None, epoch=None, logs=None):
+        logs = self.smooth_values(self.seen, logs or {})
+        logs_new = {k:logs[k].strip() for k in self.params['metrics'] if k in logs}
+        if self.verbose:
+            self.progbar.update(self.seen, **logs_new)
+            self.progbar.finish()
+    
+
 class History(Callback):
-    """指标历史，默认是fit的返回项, 这里仅记录epoch_end的指标
-    """
+    """指标历史，默认是fit的返回项, 这里仅记录epoch_end的指标"""
     def on_train_begin(self, logs=None):
         self.epoch = []
         self.history = {}
 
     def on_epoch_end(self, global_step, epoch, logs=None):
         logs = logs or {}
         self.epoch.append(epoch+1)  # 这里和keras相比+1了
@@ -731,29 +764,29 @@
                  headers=None, send_as_json=False, **kwargs):
         super(RemoteMonitor, self).__init__(**kwargs)
         self.root = root
         self.path = path
         self.field = field
         self.headers = headers
         self.send_as_json = send_as_json
+        import requests
+        self.requests = requests
 
     def on_epoch_end(self, global_step, epoch, logs=None):
-        if requests is None:
-            raise ImportError('RemoteMonitor requires the `requests` library.')
         logs = logs or {}
         send = {}
         send['epoch'] = epoch
         for k, v in logs.items():
             send[k] = v.item() if isinstance(v, (np.ndarray, np.generic)) else k
         try:
             if self.send_as_json:
-                requests.post(self.root + self.path, json=send, headers=self.headers)
+                self.requests.post(self.root + self.path, json=send, headers=self.headers)
             else:
-                requests.post(self.root + self.path, {self.field: json.dumps(send)}, headers=self.headers)
-        except requests.exceptions.RequestException:
+                self.requests.post(self.root + self.path, {self.field: json.dumps(send)}, headers=self.headers)
+        except self.requests.exceptions.RequestException:
             warnings.warn('Warning: could not reach RemoteMonitor root server at ' + str(self.root))
 
 
 class Checkpoint(Callback):
     '''保存Checkpoint, 可以每个epoch或者每隔一定的steps保存
 
     :param model_path: str, 模型保存路径(含文件名)，可以使用{epoch}和{step}占位符
@@ -850,29 +883,33 @@
     :param mode: str, log保存的模式, 默认为'a'表示追加
     :param separator: str, 指标间分隔符
     :param verbosity: int, 可选[0,1,2]，指定log的level
     :param name: str, 默认为None
     '''
     def __init__(self, log_path, interval=10, mode='a', separator='\t', verbosity=1, name=None, **kwargs):
         super(Logger, self).__init__(**kwargs)
-        import logging
-
+        self.log_path = log_path
         self.interval = interval
+        self.mode = mode
         self.sep = separator
+        self.name = name
+        self.verbosity = verbosity
+
+    def on_train_begin(self, logs=None):
+        import logging
         level_dict = {0: logging.DEBUG, 1: logging.INFO, 2: logging.WARNING}
         formatter = logging.Formatter("[%(asctime)s][%(filename)s][line:%(lineno)d][%(levelname)s] %(message)s")
-        self.logger = logging.getLogger(name)
-        self.logger.setLevel(level_dict[verbosity])
-        save_dir = os.path.dirname(log_path)
+        self.logger = logging.getLogger(self.name)
+        self.logger.setLevel(level_dict[self.verbosity])
+        save_dir = os.path.dirname(self.log_path)
+
         os.makedirs(save_dir, exist_ok=True)
-        fh = logging.FileHandler(log_path, mode)
+        fh = logging.FileHandler(self.log_path, self.mode)
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
-
-    def on_train_begin(self, logs=None):
         self.logger.info('Start Training'.center(40, '='))
 
     def on_train_end(self, logs=None):
         self.logger.info('Finish Training'.center(40, '='))
 
     def on_epoch_begin(self, global_step, epoch, logs=None):
         self.logger.info(f'Epoch {epoch+1}'.center(40, '='))
@@ -980,25 +1017,152 @@
     def on_train_begin(self, logs=None):
         from torchinfo import summary
         print()
         summary(self.model, input_data=next(iter(self.trainer.train_dataloader))[0])
         print()
 
 
-class AccelerateCallback(Callback):
-    """Accelerate的Callback
+class EmailCallback(Callback):
+    '''发送Email
+
+    :param receivers: str/list, 收件人邮箱
+    :param method: str, 控制是按照epoch还是step来发送邮件，默认为'epoch', 可选{'step', 'epoch'}
+    :param interval: int, 发送邮件的的step间隔
+    :param mail_host: str, 发件服务器host
+    :param mail_user: str, 发件人
+    :param mail_pwd: str, smtp的第三方密码
+    :param sender: str, 发件人邮箱
+    '''
+    def __init__(self, receivers, subject='', method='epoch', interval=10, mail_host=None, mail_user=None, mail_pwd=None, sender=None, **kwargs):
+        super(EmailCallback, self).__init__(**kwargs)
+        self.method = method
+        self.interval = interval
+        self.receivers = receivers
+        self.subject = subject
+        self.mail_host = mail_host
+        self.mail_user = mail_user
+        self.mail_pwd = mail_pwd
+        self.sender = sender
+
+    def on_epoch_end(self, global_step, epoch, logs=None):
+        if self.method == 'epoch':
+            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k!='size'}, indent=2, ensure_ascii=False)
+            subject = f'[INFO] Epoch {epoch+1} performance'
+            if self.subject != '':
+                subject = self.subject + ' | ' + subject
+            self._email(subject, msg)
+
+    def on_batch_end(self, global_step, local_step, logs=None):
+        if (self.method == 'step') and ((global_step+1) % self.interval == 0):
+            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k!='size'}, indent=2, ensure_ascii=False)
+            subject = f'[INFO] Step {global_step} performance'
+            if self.subject != '':
+                subject = self.subject + ' | ' + subject
+            self._email(subject, msg)
+
+    def on_train_end(self, logs=None):
+        msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k!='size'}, indent=2, ensure_ascii=False)
+        subject = f'[INFO] Finish training'
+        if self.subject != '':
+            subject = self.subject + ' | ' + subject
+        self._email(subject, msg)
+
+    def _email(self, subject, msg):
+        send_email(self.receivers, subject=subject, msg=msg, mail_host=self.mail_host,
+                   mail_user=self.mail_user, mail_pwd=self.mail_pwd, sender=self.sender)
+
+
+class WandbCallback(Callback):
+    """从transformers迁移过来
+    A :class:`~transformers.TrainerCallback` that sends the logs to `Weight and Biases <https://www.wandb.com/>`__.
+
+    :param method: str, 控制是按照epoch还是step来log，默认为'epoch', 可选{'step', 'epoch'}
+    :param interval: int, log的的step间隔
+    :param watch (:obj:`str`, `optional` defaults to :obj:`"gradients"`):
+        Can be :obj:`"gradients"`, :obj:`"all"` or :obj:`"false"`. Set to :obj:`"false"` to disable gradient
+        logging or :obj:`"all"` to log gradients and parameters.
+    :param project: str，wandb的project name, 默认为bert4torch
+    :param 
     """
-    def __init__(self, accelerator):
-        self.accelerator = accelerator
+    def __init__(self, method='epoch', project='bert4torch', trial_name=None, run_name=None, watch='gradients', 
+                 interval=100, save_code=False, config=None):
+        try:
+            import wandb
+            self._wandb = wandb
+        except:
+            print("[WARNING] WandbCallback requires wandb to be installed. Run `pip install wandb`.")
+            self._wandb = None
 
-    def get_module(self):
-        '''返回nn.Module模块
-        '''
-        unwrap_model = self.accelerator.unwrap_model(self.model)
-        return unwrap_model.module if hasattr(unwrap_model, 'module') else unwrap_model
+        self.method = method
+        self._initialized = False
+        # log outputs
+        self.project = project
+        if trial_name is None:
+            self.trial_name = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+        if run_name is None:
+            self.run_name = self.trial_name
+        self.watch = watch
+        self.interval = interval
+        self.save_code = save_code
+        self.config = config or {}
+        self.run_id = None
+        self.metrics = set()
+        self.hidden_metrics = {'size'}
+
+    def define_metric(self, logs=None):
+        if getattr(self._wandb, "define_metric", None):
+            for m in logs.keys():
+                if m not in self.metrics:
+                    self._wandb.define_metric(name=m, step_metric=self.method, hidden=True if m in self.hidden_metrics else False)
+                    self.metrics.add(m)
+    def adjust_logs(self, logs, **kwargs):
+        logs_new = {**logs, **kwargs}
+        return {k:v for k,v in logs_new.items() if k not in self.hidden_metrics}
+
+    def on_epoch_end(self, global_step, epoch, logs=None):
+        if self._wandb is None:
+            return
+        if self.method == 'epoch':
+            self.define_metric(logs)
+            self._wandb.log(self.adjust_logs(logs, epoch=epoch+1))
 
+    def on_batch_end(self, global_step, local_step, logs=None):
+        if self._wandb is None:
+            return
+        if (self.method == 'step') and ((global_step+1) % self.interval == 0):
+            self.define_metric(logs)
+            self._wandb.log(self.adjust_logs(logs, step=global_step))
+        
     def on_train_begin(self, logs=None):
-        self.trainer.loss_backward = False
-        self.trainer.get_module = self.get_module
+        if self._wandb is None:
+            return
 
-    def on_train_step_end(self, logs=None):
-        self.accelerator.backward(self.trainer.loss)
+        self._initialized = True
+        combined_dict = {**self.trainer.__dict__, **self.config}
+
+        if hasattr(self.model, "config") and self.model.config is not None:
+            combined_dict = {**self.model.config, **combined_dict}
+        init_args = {}
+        if self.trial_name is not None:
+            run_name = self.trial_name
+            init_args["group"] = self.run_name
+        else:
+            run_name = self.run_name
+
+        if self._wandb.run is None:
+            run = self._wandb.init(project=self.project, name=run_name, save_code=self.save_code, **init_args)
+            self.run_id = run.id
+
+        # add config parameters (run may have been created manually)
+        self._wandb.config.update(combined_dict, allow_val_change=True)
+
+        # keep track of model topology and gradients, unsupported on TPU
+        if self.watch != "false":
+            self._wandb.watch(self.model, log=self.watch, log_freq=max(100, self.interval))
+ 
+    def on_train_end(self, logs=None):
+        if self._wandb is None:
+            return
+
+        # transformer中的on_log
+        self._wandb.finish()
+        self._initialized = False
```

### Comparing `torch4keras-0.0.7.post3/torch4keras/model.py` & `torch4keras-0.0.8/torch4keras/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from torch import nn
 import torch
-from torch4keras.snippets import metric_mapping
-from torch4keras.callbacks import ProgbarLogger, Callback, CallbackList, BaseLogger, History, TqdmProgressBar
+from torch4keras.snippets import DottableDict, metric_mapping, get_parameter_device, info_level_prefix, print_trainable_parameters
+from torch4keras.callbacks import KerasProgbar, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, BaseLogger, History
 from collections import OrderedDict
 from inspect import isfunction
 import os
+import json
+import math
 
 
 class Trainer:
     """Trainer, 传入Module实例
 
     :param module: None/nn.Module，nn.Module()的模型实例
     """
@@ -24,30 +26,28 @@
         self.callbacks = []
         # 传入Module实例方式
         if module is not None:
             assert isinstance(module, nn.Module), 'Args `module` only support nn.Module format'
             self.module = module
         # 是否运行Callbacks，目前主要是在DDP模式下运用
         self.run_callbacks = True
-        # loss是否立即backward
-        self.loss_backward = True
 
     def compile(self, loss, optimizer, scheduler=None, clip_grad_norm=None, mixed_precision=False, metrics=None, 
                 stateful_metrics=None, grad_accumulation_steps=1, **kwargs):
         '''complile: 定义loss, optimizer, metrics等参数
         
         :param loss: loss
         :param optimizer: 优化器
         :param scheduler: scheduler
         :param clip_grad_norm: bool, 是否使用梯度裁剪, 默认为False
         :param mixed_precision: bool, 是否使用混合精度，默认为False
         :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric，形式为{key: func}
         :param stateful_metrics: List[str], 不滑动平均仅进行状态记录的metric，指标抖动会更加明显
         :param grad_accumulation_steps: int, 梯度累积步数，默认为1
-        :param tqdmbar: bool, 是否使用tqdm进度条，从kwargs中解析，默认为False
+        :param bar: str, 使用进度条的种类，从kwargs中解析，默认为keras, 可选keras, tqdm, progressbar2
         :return: None
         '''
         self.criterion = loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.clip_grad_norm = clip_grad_norm
         assert mixed_precision in {True, False, 'fp16', 'bf16'}
@@ -77,35 +77,44 @@
                 raise ValueError('Args metrics only support `String, Dict, Callback, List[String, Dict, Callback]` format')
         self.stateful_metrics = stateful_metrics
 
         # 梯度累积
         self.grad_accumulation_steps = grad_accumulation_steps
 
         # 进度条参数
-        self.tqdmbar = kwargs.get('tqdmbar', False)
+        self.bar = kwargs.get('bar', 'keras')
+        assert self.bar in {'keras', 'tqdm', 'progressbar2'}, f'Args `bar`={self.bar} illegal, only support `keras, tqdm, progressbar2`'
     
+    def print_trainable_parameters(self):
+        """打印可训练的参数量"""
+        print_trainable_parameters(self.unwrap_model())
+
+    @property
+    def device(self) -> torch.device:
+        """获取model所在的device"""
+        return get_parameter_device(self.unwrap_model())
+        
+    def to_model_device(self, *inputs, **input_kwargs):
+        '''遍历并转移到model.device上'''
+        # TODO
+        pass
+
     def _forward(self, *inputs, **input_kwargs):
         # 如果传入了网络结构module，则调用module的forward
         # 如果是继承方式，则调用自身的forward
         if (len(inputs)==1) and isinstance(inputs[0], (tuple,list)):
             inputs = inputs[0]
         if isinstance(inputs, torch.Tensor):  # tensor不展开
-            return self.get_module().forward(inputs, **input_kwargs)
+            return self.unwrap_model().forward(inputs, **input_kwargs)
         elif isinstance(inputs, (tuple, list)):
-            return self.get_module().forward(*inputs, **input_kwargs)
+            return self.unwrap_model().forward(*inputs, **input_kwargs)
         else:
-            return self.get_module().forward(inputs, **input_kwargs)
+            return self.unwrap_model().forward(inputs, **input_kwargs)
 
     def train_step(self, train_X, train_y):
-        '''forward并返回loss
-
-        :param train_X: List[torch.Tensor], 训练数据
-        :param train_y: torch.Tensor/List[torch.Tensor], 标签信息
-        :return: [output, loss, loss_detail] output: torch.Tensor/List[torch.Tensor], 模型输出; loss: nn.Tensor, 计算得到的loss; loss_detail: dict[nn.Tensor], 具体的各个loss
-        '''
         # 计算loss
         if self.mixed_precision:
             with self.autocast(dtype=torch.float16 if self.mixed_precision=='fp16' else torch.bfloat16):
                 output = self._forward(train_X)
                 loss_detail = self.criterion(output, train_y)
         else:
             output = self._forward(train_X)
@@ -123,149 +132,181 @@
             loss_detail = {f'loss{i}':v for i, v in enumerate(loss_detail[1:], start=1)}
         else:
             raise ValueError('Return loss only support `Tensor/dict/tuple/list` format')
 
         # 梯度累积
         loss = loss / self.grad_accumulation_steps if self.grad_accumulation_steps > 1 else loss
 
-        # loss.backward
-        if self.loss_backward:
-            self.scale_before_step = 0
-            if self.mixed_precision:  # 混合精度
-                self.scale_before_step = self.scaler.get_scale()
-                self.scaler.scale(loss).backward(retain_graph=self.retain_graph)
-            else:
-                loss.backward(retain_graph=self.retain_graph)
-                
+        # loss backward
+        loss = self.loss_backward(loss)
+        loss_detail = {k: (v.item() if isinstance(v, torch.Tensor) else v) / self.grad_accumulation_steps for k, v in loss_detail.items()}
         return output, loss, loss_detail
 
-    def fit(self, train_dataloader, steps_per_epoch=None, epochs=1, callbacks=None, verbose=1):
-        '''模型训练
-        
-        :param train_dataloader: Dataloader, 训练数据集
-        :param steps_per_epoch: int, 每个epoch训练的steps，默认为None表示自行计算 
-        :param epochs: int, 训练的轮次, 默认为1
-        :param callbacks: Callback/List[Callback], 回调函数，可调用预制的Callback或者自定义，默认为None 
-        :param verbose: int, 是否打印，默认为1表示打印
-        :return: None
-        '''
+    def loss_backward(self, loss):
+        '''loss.backward'''
+        self.scale_before_step = 0
+        if self.mixed_precision:  # 混合精度
+            self.scale_before_step = self.scaler.get_scale()
+            self.scaler.scale(loss).backward(retain_graph=self.retain_graph)
+        else:
+            loss.backward(retain_graph=self.retain_graph)
+        return loss
+    
+    def step(self):
+        '''参数更新'''
+        skip_scheduler = False
+        # 混合精度
+        if self.mixed_precision:
+            self.scaler.unscale_(self.optimizer)
+            if self.clip_grad_norm is not None:  # 梯度裁剪
+                torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
+            self.scaler.step(self.optimizer)
+            self.scaler.update()
+            skip_scheduler = self.scaler.get_scale() != self.scale_before_step
+        else:
+            if self.clip_grad_norm is not None:  # 梯度裁剪
+                torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
+            self.optimizer.step()
+
+        self.optimizer.zero_grad()  # 清梯度
+        if (self.scheduler is not None) and not skip_scheduler:
+            if isinstance(self.scheduler, (tuple, list)):
+                for scheduler in self.scheduler:
+                    scheduler.step()
+            else:
+                self.scheduler.step()
+
+    def _prepare_inputs(self, train_dataloader, steps_per_epoch, epochs, verbose):
+        '''对fit的输入进行类型检查并置为成员变量'''
         if not hasattr(train_dataloader, '__len__'):
             assert steps_per_epoch is not None, 'Either train_dataloader has attr `__len__` or steps_per_epoch is not None'
-
-        self.steps_per_epoch = len(train_dataloader) if steps_per_epoch is None else steps_per_epoch
+        if steps_per_epoch is None:
+            self.steps_per_epoch = math.ceil(len(train_dataloader) // self.grad_accumulation_steps)
+        else:
+            self.steps_per_epoch = steps_per_epoch
+        self.batch_size = train_dataloader.batch_size
+        self.epochs = epochs
         self.total_steps = self.steps_per_epoch * epochs
         self.train_dataloader = train_dataloader  # 设置为成员变量，可由外部的callbacks进行修改
-        train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
-        verbose = self.verbose if hasattr(self, 'verbose') else verbose
+        self.train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
+        self.verbose = self.verbose if hasattr(self, 'verbose') else verbose
 
-        # callbacks设置
+    def _prepare_callbacks(self, callbacks):
+        '''callbacks设置'''
         if callbacks is None:
             callbacks = []
         elif isinstance(callbacks, Callback):
             callbacks = [callbacks]
         for callback in callbacks:
             assert isinstance(callback, Callback), "Args `callbacks` only support Callback() inputs"
 
         history = History()
         callbacks_ = [BaseLogger(self.stateful_metrics)]
 
         # 进度条
-        if verbose:
-            if self.tqdmbar:
-                progbarlogger = TqdmProgressBar(stateful_metrics=self.stateful_metrics)
+        progbarlogger = None
+        if self.verbose:
+            if self.bar == 'keras':
+                progbarlogger = KerasProgbar(stateful_metrics=self.stateful_metrics)
+            elif self.bar == 'tqdm':
+                progbarlogger = TqdmProgbar(stateful_metrics=self.stateful_metrics)
+            elif self.bar == 'progressbar2':
+                progbarlogger = ProgressBar2Progbar(stateful_metrics=self.stateful_metrics)
             else:
-                progbarlogger = ProgbarLogger(stateful_metrics=self.stateful_metrics)
+                progbarlogger = KerasProgbar(stateful_metrics=self.stateful_metrics)
             callbacks_.append(progbarlogger)
         callbacks_  += callbacks + [history]
         self.callbacks = CallbackList(callbacks_, run_callbacks=self.run_callbacks)
         callback_trainer = self
-        callback_model = self.get_module()
+        callback_model = self.unwrap_model()
         params = {
-            'epochs': epochs,
+            'epochs': self.epochs,
             'steps': self.steps_per_epoch,
-            'verbose': verbose,
+            'verbose': self.verbose,
             'metrics': [i for i in self.metrics.keys() if isinstance(i, str)],
         }
         self.callbacks.set_all(trainer=callback_trainer, model=callback_model, optimizer=self.optimizer, scheduler=self.scheduler, params=params)
         logs = {}
         self.callbacks.on_train_begin(logs)
         callback_trainer.stop_training = False  # 在EarlyStopping中会重新设置
+        return history, callback_trainer, progbarlogger
+
+    def _prepare_nextbatch(self):
+        '''准备下一个batch数据'''
+        # 循环dataloader, 不要试用itertools的cycle，遇到过变量不释放的问题
+        try:
+            batch = next(self.train_dataloader_iter)
+        except StopIteration:
+            self.callbacks.on_dataloader_end()  # 适用于数据量较大时，动态读取文件并重新生成self.train_dataloader的情况，如预训练
+            self.train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候，其实顺序也重新生成了
+            self.bti = 0
+            batch = next(self.train_dataloader_iter)
+        return batch
+
+    def fit(self, train_dataloader, steps_per_epoch=None, epochs=1, callbacks=None, verbose=1):
+        '''模型训练
+        
+        :param train_dataloader: Dataloader, 训练数据集
+        :param steps_per_epoch: int, 每个epoch训练的steps，默认为None表示自行计算 
+        :param epochs: int, 训练的轮次, 默认为1
+        :param callbacks: Callback/List[Callback], 回调函数，可调用预制的Callback或者自定义，默认为None 
+        :param verbose: int, 是否打印，默认为1表示打印
+        :return: None
+        '''
+        # 输入处理
+        self._prepare_inputs(train_dataloader, steps_per_epoch, epochs, verbose)
+
+        # 准备callbacks
+        history, callback_trainer, progbarlogger  = self._prepare_callbacks(callbacks)
 
         # epoch：当前epoch
         # global_step：当前全局训练步数
         # local_step: 当前epoch内的训练步数，不同epoch中相同local_step对应的batch数据不一定相同，在steps_per_epoch=None时相同
         # bti：在dataloader中的index，不同epoch中相同的bti对应的batch数据一般相同，除非重新生成dataloader
         self.bti = 0
         for epoch in range(self.resume_epoch, epochs):
             self.epoch = epoch
             # resume_step：判断local_step的起点，以及进度条的起始位置
             resume_step = self.resume_step if epoch==self.resume_epoch else 0
             self.callbacks.on_epoch_begin(self.global_step, self.epoch)
-            if verbose:
+            if self.verbose:
                 progbarlogger.seen = resume_step  # 这里设置进度条的seen，在callbacks中也会修改
             
             for local_step in range(resume_step, self.steps_per_epoch):
                 self.local_step = local_step
                 self.global_step = self.epoch * self.steps_per_epoch + self.local_step
-                # 循环dataloader, 不要试用itertools的cycle，遇到过变量不释放的问题
-                try:
-                    batch = next(train_dataloader_iter)
-                except StopIteration:
-                    self.callbacks.on_dataloader_end()  # 适用于数据量较大时，动态读取文件并重新生成self.train_dataloader的情况，如预训练
-                    train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候，其实顺序也重新生成了
-                    self.bti = 0
-                    batch = next(train_dataloader_iter)
-                self.train_X, self.train_y = batch
-
-                logs = self.log_init()
+                logs = self._log_init()
                 self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
 
-                self.get_module().train()  # 设置为train模式
-
-                # 入参个数判断，如果入参>=3表示是多个入参，如果=2则表示是一个入参
-                self.output, self.loss, self.loss_detail = self.train_step(self.train_X, self.train_y)
-                self.callbacks.on_train_step_end()
-                                
-                # 参数更新, 真实的参数更新次数要除以grad_accumulation_steps，注意调整总的训练步数
-                if (self.global_step+1) % self.grad_accumulation_steps == 0:
-                    skip_scheduler = False
-                    # 混合精度
-                    if self.mixed_precision:
-                        self.scaler.unscale_(self.optimizer)
-                        if self.clip_grad_norm is not None:  # 梯度裁剪
-                            torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
-                        self.scaler.step(self.optimizer)
-                        self.scaler.update()
-                        skip_scheduler = self.scaler.get_scale() != self.scale_before_step
-                    else:
-                        if self.clip_grad_norm is not None:  # 梯度裁剪
-                            torch.nn.utils.clip_grad_norm_(self.parameters(), self.clip_grad_norm)
-                        self.optimizer.step()
-
-                    self.optimizer.zero_grad()  # 清梯度
-                    if (self.scheduler is not None) and not skip_scheduler:
-                        if isinstance(self.scheduler, (tuple, list)):
-                            for scheduler in self.scheduler:
-                                scheduler.step()
-                        else:
-                            self.scheduler.step()
+                # forward和backward
+                self.unwrap_model().train()  # 设置为train模式
+                tr_loss, tr_loss_detail = 0, {}
+                for _ in range(self.grad_accumulation_steps):
+                    self.train_X, self.train_y = self._prepare_nextbatch()  # 获取下一个batch的训练数据
+                    self.output, self.loss, self.loss_detail = self.train_step(self.train_X, self.train_y)
+                    self.callbacks.on_train_step_end()
+                    tr_loss += self.loss.item()
+                    for k, v in self.loss_detail.items():
+                        tr_loss_detail[k] = tr_loss_detail.get(k, 0) + v
+                # TODO: 理论上梯度累积时需对output和train_y进行合并，主要是为了metric_mapping计算的准确
+                
+                # 参数更新
+                self.step()
 
                 # 添加loss至log打印
-                logs.update({'loss': self.loss.item()})
-                logs_loss_detail = {k: v.item() if isinstance(v, torch.Tensor) else v for k, v in self.loss_detail.items()}
-                logs.update(logs_loss_detail)
-                if verbose and (self.global_step == resume_step):
-                    progbarlogger.add_metrics(list(logs_loss_detail.keys()), add_position=1)
+                logs.update(dict({'loss': tr_loss}, **tr_loss_detail))
+                if self.verbose and (self.global_step == resume_step):
+                    progbarlogger.add_metrics(list(tr_loss_detail.keys()), add_position=1)
                     
                 # 添加metrics至log打印
                 for metric, func in self.metrics.items():
                     perf = metric_mapping(metric, func, self.output, self.train_y)  # 内置的一些accuracy指标
                     if perf is not None:
                         if isfunction(metric):  # 直接传入回调函数(无key)
-                            if verbose and (self.global_step == resume_step):
+                            if self.verbose and (self.global_step == resume_step):
                                 progbarlogger.add_metrics(list(perf.keys()))
                             logs.update(perf)
                         elif isinstance(metric, str):  # 直接传入回调函数(有key)
                             logs[metric] = perf
 
                 self.callbacks.on_batch_end(self.global_step, self.local_step, logs)
 
@@ -273,43 +314,30 @@
             self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
             # TerminateOnNaN、EarlyStopping等停止训练策略
             if callback_trainer.stop_training:
                 break
         self.callbacks.on_train_end(logs)
         return history
 
-    def log_init(self):
+    def _log_init(self):
         '''获取batch_size，主要是用于callback中的BaseLogger和Callback
         '''
-        # 从train_X中取batch_size，最多允许嵌套两层，即encoder和decoder的((token_ids1, mask1), (token_ids2, mask2))
-        if isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], (list, tuple)):
-            btz = self.train_X[0][0].size(0)
-        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], torch.Tensor):
-            btz = self.train_X[0].size(0)
-        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], dict):
-            btz = self.train_X[0].get('batch_size', 0)
-        elif isinstance(self.train_X, dict):
-            btz = self.train_X.get('batch_size', 0)
-        elif isinstance(self.train_X, torch.Tensor):
-            btz = self.train_X.size(0)
-        else:
-            raise ValueError('Input only support `[list, tuple, tensor]`')
-        logs ={'size': btz}
+        logs = {'size': self.batch_size * self.grad_accumulation_steps}
 
         # 添加lr
         try:
             logs['lr'] = self.optimizer.param_groups[0]["lr"]
         except:
             pass
         return logs
 
     @torch.no_grad()
     def predict(self, *inputs, **input_kwargs):
         '''模型预测，调用forward()'''
-        self.get_module().eval()
+        self.unwrap_model().eval()
         return self._forward(*inputs, **input_kwargs)
         
     def load_steps_params(self, save_path):
         '''导入训练过程参数
         
         :param save_path: str, 训练过程参数保存路径
         '''
@@ -345,39 +373,39 @@
             raise ValueError('Args `load_path` only support str/tuple/list format')
         
         for load_path_i in load_path:
             state_dict = torch.load(load_path_i, map_location='cpu')
             for k, v in state_dict.items():
                 k = mapping.get(k, k)
                 state_dict_raw[k] = v
-            self.get_module().load_state_dict(state_dict_raw, strict=strict)
+            self.unwrap_model().load_state_dict(state_dict_raw, strict=strict)
 
     def save_weights(self, save_path, mapping={}, trainable_only=False, verbose=1):
         '''保存模型权重
 
         :param save_path: str, 权重保存路径
         :param mapping: dict, 指定key的映射
         :param trainable_only: bool, 指定仅保存可训练参数
         '''
         state_dict_raw = {}
-        state_dict = self.get_module().state_dict()
-        trainable_parameters = set(p for p,v in self.get_module().named_parameters() if v.requires_grad)
+        state_dict = self.unwrap_model().state_dict()
+        trainable_parameters = set(p for p,v in self.unwrap_model().named_parameters() if v.requires_grad)
         for k, v in state_dict.items():
             # 只保存可训练的模型部分
             if trainable_only and (k not in trainable_parameters):
                 continue
             k = mapping.get(k, k)
             state_dict_raw[k] = v
         
         save_dir = os.path.dirname(save_path)
         os.makedirs(save_dir, exist_ok=True)
         torch.save(state_dict_raw, save_path)
         if trainable_only and (verbose > 0):
-            params_all = sum(p.numel() for p in self.get_module().parameters())
-            params_trainable = sum(p.numel() for p in self.get_module().parameters() if p.requires_grad)
+            params_all = sum(p.numel() for p in self.unwrap_model().parameters())
+            params_trainable = sum(p.numel() for p in self.unwrap_model().parameters() if p.requires_grad)
             print(f"[INFO] Only trainable parameters saved and occupy {params_trainable}/{params_all} {params_trainable/params_all:.2f}%")
 
     def resume_from_checkpoint(self, model_path=None, optimizer_path=None, scheduler_path=None, step_params_path=None):
         '''同时加载模型、优化器、训练过程参数
 
         :param model_path: str, 模型文件路径
         :param optimizer_path: str, 优化器文件路径
@@ -422,15 +450,15 @@
             verbose_str += f'Scheduler successfuly saved to {scheduler_path}.\n'
         if step_params_path:
             self.save_steps_params(step_params_path)
             verbose_str += f'Steps_params successfuly saved to {step_params_path}.\n'
         if verbose != 0:
             print(verbose_str)
 
-    def get_module(self):
+    def unwrap_model(self):
         '''返回nn.Module模块
         '''
         if isinstance(self, nn.Module): return self
         return self.module if hasattr(self, 'module') else self
 
 
 class BaseModel(Trainer, nn.Module):
@@ -468,24 +496,137 @@
 
 
 def add_trainer(obj, include=None, exclude=None):
     '''为对象添加Triner对应的方法
     '''
     include = include or []
     exclude = exclude or []
+    if isinstance(include, str):
+        include = [include]
+    if isinstance(exclude, str):
+        exclude = [exclude]
+    
     if isinstance(obj, (Trainer, TrainerDP, TrainerDDP, BaseModel, BaseModelDP, BaseModelDDP)):
         return obj
     
     if isinstance(obj, nn.Module):
         import types
         for k in dir(Trainer):
             if k in include:  # 必须包含的
                 pass
             elif k in exclude:  # 必须屏蔽的
                 continue
             elif k.startswith('__') and k.endswith('__'):
                 continue
             elif hasattr(obj, k):  # 如果下游重新定义，则不继承
                 continue
-            exec(f'obj.{k} = types.MethodType(Trainer.{k}, obj)')
+           
+            if eval(f'isfunction(Trainer.{k})'):
+                 # 方法
+                exec(f'obj.{k} = types.MethodType(Trainer.{k}, obj)')
+            else:
+                # TODO 属性等其他
+                pass
         obj.initialize()
-    return obj
+    return obj
+
+
+class AccelerateTrainer(Trainer):
+    '''accelerate来训练'''
+    def __init__(self, module: nn.Module, **configs):
+        super().__init__(module)
+        from accelerate import Accelerator
+        accelerator = Accelerator(**configs)
+        self.model = accelerator.prepare(module)
+        self.accelerator = accelerator
+        self.device = accelerator.device
+        self.verbose = 1 if accelerator.is_local_main_process else 0
+        print(info_level_prefix('AcclerateTrainer may not be compatible with several callbacks, you may use custom callbacks instead.', 1))
+    
+    def compile(self, *args, **kwargs):
+        super().compile(*args, **kwargs)
+        self.optimizer, self.scheduler, self.criterion = self.accelerator.prepare(self.optimizer, self.scheduler, self.criterion)
+
+    def _prepare_inputs(self, *args):
+        super()._prepare_inputs(*args)
+        self.train_dataloader = self.accelerator.prepare(self.train_dataloader)
+        self.train_dataloader_iter = iter(self.train_dataloader)
+
+    def prepare(self, *args, **kwargs):
+        '''调用acclerate的prepare，如在外面评估时候需要对dev_dataloader使用'''
+        return self.accelerator.prepare(*args, **kwargs)
+
+    def unwrap_model(self):
+        '''返回nn.Module模块'''
+        unwrap_model = self.accelerator.unwrap_model(self.model)
+        if isinstance(unwrap_model, nn.Module): return unwrap_model
+        return unwrap_model.module if hasattr(unwrap_model, 'module') else unwrap_model
+
+    def loss_backward(self, loss):
+        self.accelerator.backward(loss)
+        return loss
+
+
+class DeepSpeedTrainer(Trainer):
+    '''deepspeed来训练'''
+    def __init__(self, module, config_path):
+        super().__init__(module)
+        self.model = add_trainer(module)
+        self.config = DottableDict(json.load(open(config_path)))
+        self.config['steps_per_print'] = self.config.get('steps_per_print', 1e9)  # 默认不打印，防止进度条打印问题
+
+    def compile(self, *args, log_level='warning', inference=False, master_rank=0, **kwargs):
+        super().compile(*args, **kwargs)
+        import deepspeed
+        from deepspeed.utils import logger as ds_logger
+        import logging
+        log_levels = {
+            "debug": logging.DEBUG,
+            "info": logging.INFO,
+            "warning": logging.WARNING,
+            "error": logging.ERROR,
+            "critical": logging.CRITICAL,
+        }
+
+        ds_logger.setLevel(log_levels.get(log_level, logging.WARNING))
+
+        if inference:
+            # only Z3 makes sense for the inference
+            info_level_prefix("ZeRO inference only makes sense with ZeRO Stage 3", 1)
+            self.optimizer, self.scheduler = None, None
+            model_parameters = None
+        else:
+            model_parameters = list(filter(lambda p: p.requires_grad, self.model.parameters()))
+        
+        kwargs = {
+            "model": self.model,  # deepspeed的forward默认是计算到loss输出的
+            "model_parameters": model_parameters,
+            "config_params": self.config,
+            "optimizer": self.optimizer,
+            "lr_scheduler": self.scheduler,
+        }
+        if self.config.get('zero_optimization', {}).get('offload_optimizer', {}).get('device') == 'cpu':
+            kwargs.pop('optimizer')
+            print(info_level_prefix('You may not use custom optimizer when offload_optimizer=`cpu`', 1))
+        self.deepspeed_engine, self.optimizer, _, self.scheduler = deepspeed.initialize(**kwargs)
+        self.verbose = 1 if self.deepspeed_engine.local_rank == master_rank else 0
+
+    def unwrap_model(self):
+        # 执行deepspeed_engine的forward
+        return self.deepspeed_engine
+
+    def loss_backward(self, loss):
+        self.deepspeed_engine.backward(loss)
+        return loss
+    
+    def step(self):
+        self.deepspeed_engine.step()
+
+    @torch.inference_mode()
+    def predict(self, *inputs, **input_kwargs):
+        return self.deepspeed_engine.module.predict(*inputs, **input_kwargs)
+
+    def resume_from_checkpoint(self, *args, **kwargs):
+        return self.deepspeed_engine.load_checkpoint(*args, **kwargs)
+
+    def save_to_checkpoint(self, *args, **kwargs):
+        return self.deepspeed_engine.save_checkpoint(*args, **kwargs)
```

### Comparing `torch4keras-0.0.7.post3/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.0.8/torch4keras.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.0.7.post3
+Version: 0.0.8
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,14 +16,15 @@
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/torch4keras?style=social)](https://github.com/Tongjilibo/torch4keras)
 [![GitHub Issues](https://img.shields.io/github/issues/Tongjilibo/torch4keras.svg)](https://github.com/Tongjilibo/torch4keras/issues)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Tongjilibo/torch4keras/issues)
 
 [Documentation](https://torch4keras.readthedocs.io) |
+[Bert4torch](https://github.com/Tongjilibo/bert4torch) |
 [Examples](https://github.com/Tongjilibo/torch4keras/blob/master/examples) |
 [Source code](https://github.com/Tongjilibo/torch4keras)
 
 ## 1. 下载安装
 安装稳定版
 ```shell
 pip install torch4keras
@@ -70,26 +71,28 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
+- **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
 - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
```

