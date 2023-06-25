# Comparing `tmp/simulated_bifurcation-1.0.2.tar.gz` & `tmp/simulated-bifurcation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "simulated-bifurcation-1.1.0.tar", last modified: Sun Jun 25 19:04:54 2023, max compression
```

## Comparing `simulated_bifurcation-1.0.2.tar` & `simulated-bifurcation-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,31 @@
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/CITATION.cff
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/requirements.txt
--rw-r--r--   0        0        0    24832 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/__init__.py
--rw-r--r--   0        0        0    13826 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/interface.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/markowitz.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/partitioning.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/src/simulated_bifurcation/qubo.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/.gitignore
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/LICENSE
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/README.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9425 2020-02-02 00:00:00.000000 simulated_bifurcation-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.474398 simulated-bifurcation-1.1.0/
+-rw-rw-rw-   0        0        0     1123 2023-04-30 10:03:26.000000 simulated-bifurcation-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-06-25 19:04:54.474398 simulated-bifurcation-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8949 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/README.md
+-rw-rw-rw-   0        0        0      215 2023-06-25 19:04:54.476396 simulated-bifurcation-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-06-25 19:04:46.000000 simulated-bifurcation-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.391415 simulated-bifurcation-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.419401 simulated-bifurcation-1.1.0/src/simulated_bifurcation/
+-rw-rw-rw-   0        0        0       97 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/__init__.py
+-rw-rw-rw-   0        0        0     5250 2023-06-25 18:59:06.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/interface.py
+-rw-rw-rw-   0        0        0    10533 2023-06-25 18:58:05.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/ising.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.439399 simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/__init__.py
+-rw-rw-rw-   0        0        0     1537 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/partitioning.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.453397 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/
+-rw-rw-rw-   0        0        0       88 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/__init__.py
+-rw-rw-rw-   0        0        0     4197 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/integer.py
+-rw-rw-rw-   0        0        0     1082 2023-06-24 13:09:23.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/markowitz.py
+-rw-rw-rw-   0        0        0     3705 2023-06-25 18:30:47.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/qubo.py
+-rw-rw-rw-   0        0        0    13605 2023-06-25 18:54:34.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.433402 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-25 19:04:54.000000 simulated-bifurcation-1.1.0/src/simulated_bifurcation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 19:04:54.469399 simulated-bifurcation-1.1.0/test/
+-rw-rw-rw-   0        0        0     2676 2023-06-25 08:57:26.000000 simulated-bifurcation-1.1.0/test/test_ising.py
+-rw-rw-rw-   0        0        0      217 2023-06-25 17:52:32.000000 simulated-bifurcation-1.1.0/test/test_ising_interface.py
+-rw-rw-rw-   0        0        0     1393 2023-06-25 17:48:34.000000 simulated-bifurcation-1.1.0/test/test_optimizer.py
+-rw-rw-rw-   0        0        0     4463 2023-06-25 10:08:24.000000 simulated-bifurcation-1.1.0/test/test_stop_window.py
+-rw-rw-rw-   0        0        0     3959 2023-06-25 17:41:12.000000 simulated-bifurcation-1.1.0/test/test_symplectic_integrator.py
```

### Comparing `simulated_bifurcation-1.0.2/src/simulated_bifurcation/markowitz.py` & `simulated-bifurcation-1.1.0/src/simulated_bifurcation/models/markowitz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from . interface import Integer
-from . import torch, Union
+from .integer import Integer
+import torch
+from typing import Union
 
 class Markowitz(Integer):
 
     """
     A representation of the Markowitz model for portolio optimization.
     Portfolio only takes integer stocks.
     """
```

### Comparing `simulated_bifurcation-1.0.2/src/simulated_bifurcation/partitioning.py` & `simulated-bifurcation-1.1.0/src/simulated_bifurcation/karp/partitioning.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from . import *
-from . interface import IsingInterface
+from ..ising import Ising
+from ..interface import IsingInterface
 from numpy import sum
+import torch
 
 
 class NumberPartioning(IsingInterface):
 
     """
     A solver that separates a set of numbers into two subsets whose 
     respective sums are as close as possible.
@@ -17,23 +18,23 @@
         self.partition = {
             'left': {'values': [], 'sum': None},
             'right': {'values': [], 'sum': None}
         }
 
     def __len__(self): return len(self.numbers)
 
-    def __to_Ising__(self) -> Ising:
+    def to_ising(self) -> Ising:
         
         tensor_numbers = torch.Tensor(self.numbers, device=self.device)
         J = -2 * tensor_numbers.reshape(-1, 1) @ tensor_numbers.reshape(1, -1)
         h = torch.zeros((len(self), 1))
 
         return Ising(J, h, self.dtype, self.device)
 
-    def __from_Ising__(self, ising: Ising) -> None:
+    def from_ising(self, ising: Ising) -> None:
         
         subset_left = []
         subset_right = []
 
         partition = ising.ground_state.reshape(-1,)
 
         for elt in range(len(self)):
```

### Comparing `simulated_bifurcation-1.0.2/LICENSE` & `simulated-bifurcation-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simulated_bifurcation-1.0.2/README.md` & `simulated-bifurcation-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,38 +116,38 @@
 Once created, such an object can be optimized using the same principle as an `Ising` object, using the `optimize` methods which uses the same parameters as the `Ising`'s one:
 
 ```python
 your_model = YourModel(...)
 your_model.optimize()
 ```
 
-Yet, to make it work, you will first have to overwrite two abstract methods of the `IsingInterface` class (`__to_Ising__` and `__from_Ising__`) that are called by the `optimize` method. Otherwise you will get a `NotImplementedError` error message.
+Yet, to make it work, you will first have to overwrite two abstract methods of the `IsingInterface` class (`to_ising` and `from_ising`) that are called by the `optimize` method. Otherwise you will get a `NotImplementedError` error message.
 
-When the `optimize` method is called, an equivalent Ising model will first be created using `__to_Ising__` and then optimized using the exact same parameters you provided as input for the `IsingInterface.optimize` method. Once it is optimized, information for your own model will be derived from the optimal features of this equivalent Ising model using `__from_Ising__`.
+When the `optimize` method is called, an equivalent Ising model will first be created using `to_ising` and then optimized using the exact same parameters you provided as input for the `IsingInterface.optimize` method. Once it is optimized, information for your own model will be derived from the optimal features of this equivalent Ising model using `from_ising`.
 
-### `__to_Ising__` method
+### `to_ising` method
 
-The `__to_Ising__` is meant to create an instance of an Ising model based on the data of your problem. It takes no argument and must only return an `Ising` object. The idea is to rely on the parameters of your problems to derive an Ising representation of it. At some point in the definition of the method, you will have to create the `J` matrix and the `h` vector and eventually return `Ising(J, h)`.
+The `to_ising` is meant to create an instance of an Ising model based on the data of your problem. It takes no argument and must only return an `Ising` object. The idea is to rely on the parameters of your problems to derive an Ising representation of it. At some point in the definition of the method, you will have to create the `J` matrix and the `h` vector and eventually return `Ising(J, h)`.
 
 ```python
-def __to_Ising__(self) -> sb.Ising:
+def to_ising(self) -> sb.Ising:
     # YOUR CODE HERE
     J = ...
     h = ...
     return sb.Ising(J, h, dtype=self.dtype, device=self.device)
 ```
 
 > Do not forget to set the `device` attribute when you instantiate the class if you are working on a GPU because all the tensors must be set on the same device.
 
-### `__from_Ising__` method
+### `from_ising` method
 
-The `__from_Ising__` is the reciprocal method. Once the equivalent Ising model of your problem has been optimized, you can retrieve information from its ground state and/or energy and adapt them to your own problem. It must only take an `Ising` object for input and return `None`.
+The `from_ising` is the reciprocal method. Once the equivalent Ising model of your problem has been optimized, you can retrieve information from its ground state and/or energy and adapt them to your own problem. It must only take an `Ising` object for input and return `None`.
 
 ```python
-def __from_Ising__(self, ising: sb.Ising) -> None:
+def from_ising(self, ising: sb.Ising) -> None:
     # YOUR CODE HERE
     return 
 ```
 
 ### Binary and integer formulations
 
 Note that many problems that can be represented as Ising models are not based on spin vectors but rather on binary or integer vectors. The `interface` submodule thus has two additional classes, `Binary` and `Integer`, both of which inherit from `IsingInterface` in order to generalize these cases more easily.
@@ -159,11 +159,11 @@
 If you are using this code for your own projects please cite our work:
 
 ```bibtex
 @software{Ageron_Simulated_Bifurcation_SB_2022,
     author = {Ageron, Romain and Bouquet, Thomas and Pugliese, Lorenzo},
     month = {4},
     title = {{Simulated Bifurcation (SB) algorithm for Python}},
-    version = {1.0.2},
+    version = {1.1.0},
     year = {2023}
 }
 ```
```

