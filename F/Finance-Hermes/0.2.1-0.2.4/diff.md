# Comparing `tmp/Finance-Hermes-0.2.1.tar.gz` & `tmp/Finance-Hermes-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.2.1.tar", last modified: Mon Dec  5 09:10:18 2022, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.2.4.tar", last modified: Sat Jun 24 23:09:05 2023, max compression
```

## Comparing `Finance-Hermes-0.2.1.tar` & `Finance-Hermes-0.2.4.tar`

### file list

```diff
@@ -1,65 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      222 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1703 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      114 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      222 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/Izador/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/Izador/__init__.py
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/Izador/calculater.py
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-05 09:09:49.000000 Finance-Hermes-0.2.1/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7484 2022-12-03 08:36:51.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/alpha101.py
--rw-r--r--   0 root         (0) root         (0)    15211 2022-12-03 07:41:04.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/alpha191.py
--rw-r--r--   0 root         (0) root         (0)     7523 2022-12-03 08:19:08.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/factor_alpha101.py
--rw-r--r--   0 root         (0) root         (0)    13226 2022-12-03 07:37:08.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/factor_alpha191.py
--rw-r--r--   0 root         (0) root         (0)     1744 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/factors/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-10 07:28:19.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-13 12:40:33.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1673 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/core/basis.py
--rw-r--r--   0 root         (0) root         (0)     2241 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/factor_basis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/macroeconmic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-10 07:28:19.000000 Finance-Hermes-0.2.1/hermes/factors/macroeconmic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/technical/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-10 07:28:19.000000 Finance-Hermes-0.2.1/hermes/factors/technical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4925 2022-11-13 12:40:33.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/maturity.py
--rw-r--r--   0 root         (0) root         (0)    36381 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/momentum.py
--rw-r--r--   0 root         (0) root         (0)    14993 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/overlap.py
--rw-r--r--   0 root         (0) root         (0)     5954 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/statistics.py
--rw-r--r--   0 root         (0) root         (0)    16208 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/trend.py
--rw-r--r--   0 root         (0) root         (0)     5106 2022-11-06 15:36:30.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/utilities.py
--rw-r--r--   0 root         (0) root         (0)    16264 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/volatility.py
--rw-r--r--   0 root         (0) root         (0)    15946 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/volume.py
--rw-r--r--   0 root         (0) root         (0)     4608 2022-11-13 12:40:33.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_maturity.py
--rw-r--r--   0 root         (0) root         (0)    26641 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_momentum.py
--rw-r--r--   0 root         (0) root         (0)     9240 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_overlap.py
--rw-r--r--   0 root         (0) root         (0)     3907 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_statistics.py
--rw-r--r--   0 root         (0) root         (0)     6867 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_trend.py
--rw-r--r--   0 root         (0) root         (0)    11005 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_volatility.py
--rw-r--r--   0 root         (0) root         (0)    12352 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/kdutils/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/fixes.py
--rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/helper.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/kdutils/lazy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/requirements/
--rw-r--r--   0 root         (0) root         (0)       69 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1964 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-24 23:09:04.000000 Finance-Hermes-0.2.4/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      759 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 23:09:04.000000 Finance-Hermes-0.2.4/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-24 23:09:04.000000 Finance-Hermes-0.2.4/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-24 23:09:04.000000 Finance-Hermes-0.2.4/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-24 10:42:40.000000 Finance-Hermes-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-24 23:07:48.000000 Finance-Hermes-0.2.4/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.4/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   295777 2023-06-24 14:55:53.000000 Finance-Hermes-0.2.4/hermes/factors/base.c
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-06-24 14:38:59.000000 Finance-Hermes-0.2.4/hermes/factors/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.4/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271147 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.4/hermes/kdutils/base.c
+-rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.4/hermes/kdutils/base.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.4/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   678491 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.4/hermes/kdutils/core/fixes.c
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.4/hermes/kdutils/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)   392670 2023-06-24 10:39:53.000000 Finance-Hermes-0.2.4/hermes/kdutils/core/helper.c
+-rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.4/hermes/kdutils/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)   190192 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.4/hermes/kdutils/create_id.c
+-rw-r--r--   0 root         (0) root         (0)      870 2023-06-21 21:57:15.000000 Finance-Hermes-0.2.4/hermes/kdutils/create_id.pyx
+-rw-r--r--   0 root         (0) root         (0)   235985 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.4/hermes/kdutils/lazy.c
+-rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.4/hermes/kdutils/lazy.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.4/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161732 2023-06-24 10:51:00.000000 Finance-Hermes-0.2.4/hermes/lzador/calculater.c
+-rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.4/hermes/lzador/calculater.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/requirements/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-24 12:13:59.000000 Finance-Hermes-0.2.4/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 23:09:05.000000 Finance-Hermes-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-06-24 14:55:20.000000 Finance-Hermes-0.2.4/setup.py
```

### Comparing `Finance-Hermes-0.2.1/hermes/Izador/calculater.py` & `Finance-Hermes-0.2.4/hermes/lzador/calculater.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/factors/base.py` & `Finance-Hermes-0.2.4/hermes/factors/base.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- encoding:utf-8 -*-
+import copy, hashlib, json, pdb
 import six as six
 from abc import ABCMeta, abstractmethod
+from hermes.kdutils.create_id import create_id
 from hermes.kdutils.lazy import LazyFunc
 from hermes.kdutils.base import ParamBase, FreezeAttrMixin
 
 
 class LongCallMixin(FreezeAttrMixin):
     """
         混入类，混入代表多头，不完全是期权中buy call的概念，
@@ -35,29 +37,74 @@
 
     @LazyFunc
     def expect_direction(self):
         """期望收益方向，1.0即反向期望"""
         return -1.0
 
 
+
+class ShortMixin(FreezeAttrMixin):
+    """
+        混入类，混入代表空头，应用场景在于期权，期货策略中，
+        不完全是期权中buy put的概念，只代看跌反向操作，
+        即期望买入后交易目标价格下跌，下跌带来收益
+    """
+
+    @LazyFunc
+    def short_type_str(self):
+        """用来区别买入类型unique 值为put"""
+        return "short"
+
+    @LazyFunc
+    def expect_direction(self):
+        """期望收益方向，1.0即反向期望"""
+        return -1.0
+    
+
+class ShortCallMixin(FreezeAttrMixin):
+    """
+        混入类，混入代表空头，应用场景在于期权，期货策略中，
+        不完全是期权中buy put的概念，只代看跌反向操作，
+        即期望买入后交易目标价格下跌，下跌带来收益
+    """
+
+    @LazyFunc
+    def short_type_str(self):
+        """用来区别买入类型unique 值为put"""
+        return "short"
+
+    @LazyFunc
+    def expect_direction(self):
+        """期望收益方向，1.0即反向期望"""
+        return -1.0
+
+
 class FactorBase(six.with_metaclass(ABCMeta, ParamBase)):
 
     def __init__(self, **kwargs):
         # 子类继续完成自有的构造
         self._init_self(**kwargs)
 
     @abstractmethod
     def _init_self(self, **kwargs):
         """子类因子针对可扩展参数的初始化"""
         pass
 
-    def _format(self, data, name):
+    def _create_id(self, **kwargs):
+        feature = copy.deepcopy(kwargs)
+        feature['category'] = self.category
+        s = hashlib.md5(
+            json.dumps(feature).encode(encoding="utf-8")).hexdigest()
+        return "{0}".format(create_id(original=s, digit=10))
+
+    def _format(self, data, name, **kwargs):
         data = data.stack()
         data.name = name
         data.category = self.category
+        data.id = self._create_id(name=name, **kwargs)
         return data
 
     def factors_list(self):
         return list(
             filter(
                 lambda x: not x.startswith('_') and not x.islower() and
                 callable(getattr(self, x)), dir(self)))
```

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/base.py` & `Finance-Hermes-0.2.4/hermes/kdutils/base.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/core/fixes.py` & `Finance-Hermes-0.2.4/hermes/kdutils/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/core/helper.py` & `Finance-Hermes-0.2.4/hermes/kdutils/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/lazy.py` & `Finance-Hermes-0.2.4/hermes/kdutils/lazy.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/setup.py` & `Finance-Hermes-0.2.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from Cython.Build import cythonize
 from setuptools import setup
 from setuptools import find_packages
 from distutils.cmd import Command
 from distutils.extension import Extension
 import os, sys, io, subprocess, platform
 from hermes import __version__
 
@@ -18,14 +19,20 @@
 
 def git_version():
     from subprocess import Popen, PIPE
     gitproc = Popen(['git', 'rev-parse', 'HEAD'], stdout=PIPE)
     (stdout, _) = gitproc.communicate()
     return stdout.strip()
 
+if "--line_trace" in sys.argv:
+    line_trace = True
+    print("Build with line trace enabled ...")
+    sys.argv.remove("--line_trace")
+else:
+    line_trace = False
 
 class version_build(Command):
 
     description = "test the distribution prior to install"
 
     user_options = [
         ('test-dir=', None, "directory that contains the test definitions"),
@@ -59,18 +66,48 @@
 requirements = "requirements/py3.txt"
 
 if platform.system() != "Windows":
     import multiprocessing
     n_cpu = multiprocessing.cpu_count()
 else:
     n_cpu = 0
+    
+
+
+ext_modules = ['hermes/kdutils/core/fixes.pyx','hermes/kdutils/core/helper.pyx','hermes/kdutils/base.pyx','hermes/kdutils/create_id.pyx','hermes/kdutils/lazy.pyx',
+               'hermes/lzador/calculater.pyx','hermes/factors/base.pyx']
+
+def generate_extensions(ext_modules, line_trace=True):
+
+    extensions = []
+
+    if line_trace:
+        print("define cython trace to True ...")
+        define_macros = [('CYTHON_TRACE', 1), ('CYTHON_TRACE_NOGIL', 1)]
+    else:
+        define_macros = []
+
+    for pyxfile in ext_modules:
+        ext = Extension(name='.'.join(pyxfile.split('/'))[:-4],
+                        sources=[pyxfile],
+                        define_macros=define_macros)
+        extensions.append(ext)
+    return extensions
+
+ext_modules_settings = cythonize(generate_extensions(ext_modules, line_trace),
+                                 compiler_directives={
+                                     'embedsignature': True,
+                                     'linetrace': line_trace
+                                 },
+                                 nthreads=n_cpu)
 
 setup(name=NAME,
       version=VERSION,
       description=DESCRIPTION,
       author=AUTHOR,
       author_email=AUTHOR_EMAIL,
       url=URL,
+      ext_modules=ext_modules_settings,
       packages=find_packages(),
       include_package_data=False,
       install_requires=io.open(requirements, encoding='utf8').read(),
       classifiers=[])
```

