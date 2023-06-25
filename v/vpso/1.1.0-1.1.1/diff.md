# Comparing `tmp/vpso-1.1.0.tar.gz` & `tmp/vpso-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vpso-1.1.0.tar", last modified: Sun Jun 18 08:23:23 2023, max compression
+gzip compressed data, was "vpso-1.1.1.tar", last modified: Sun Jun 25 09:13:07 2023, max compression
```

## Comparing `vpso-1.1.0.tar` & `vpso-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.932776 vpso-1.1.0/
--rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3575 2023-06-18 08:23:23.931776 vpso-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.1.0/README.md
--rw-rw-rw-   0        0        0      977 2023-06-18 07:38:18.000000 vpso-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 08:23:23.932776 vpso-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.893828 vpso-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.910774 vpso-1.1.0/src/vpso/
--rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.1.0/src/vpso/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-18 08:10:29.000000 vpso-1.1.0/src/vpso/adaptation.py
--rw-rw-rw-   0        0        0     6066 2023-06-18 08:08:37.000000 vpso-1.1.0/src/vpso/ask_and_tell.py
--rw-rw-rw-   0        0        0     5178 2023-06-18 08:09:33.000000 vpso-1.1.0/src/vpso/initialization.py
--rw-rw-rw-   0        0        0     7815 2023-06-18 07:14:19.000000 vpso-1.1.0/src/vpso/math.py
--rw-rw-rw-   0        0        0     4496 2023-06-18 08:12:30.000000 vpso-1.1.0/src/vpso/mutation.py
--rw-rw-rw-   0        0        0     3898 2023-06-18 08:08:51.000000 vpso-1.1.0/src/vpso/reparation.py
--rw-rw-rw-   0        0        0     6822 2023-06-18 08:22:24.000000 vpso-1.1.0/src/vpso/termination.py
--rw-rw-rw-   0        0        0      302 2023-06-18 08:09:11.000000 vpso-1.1.0/src/vpso/typing.py
--rw-rw-rw-   0        0        0     7396 2023-06-18 08:20:41.000000 vpso-1.1.0/src/vpso/vpso.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.917777 vpso-1.1.0/src/vpso.egg-info/
--rw-rw-rw-   0        0        0     3575 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-18 08:23:23.000000 vpso-1.1.0/src/vpso.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 08:23:23.930782 vpso-1.1.0/tests/
--rw-rw-rw-   0        0        0     4264 2023-06-18 07:52:24.000000 vpso-1.1.0/tests/test_adaptation.py
--rw-rw-rw-   0        0        0     1201 2023-06-10 15:53:49.000000 vpso-1.1.0/tests/test_initialization.py
--rw-rw-rw-   0        0        0     3467 2023-06-13 22:08:14.000000 vpso-1.1.0/tests/test_math.py
--rw-rw-rw-   0        0        0     3669 2023-06-10 15:56:14.000000 vpso-1.1.0/tests/test_mutation.py
--rw-rw-rw-   0        0        0     2119 2023-06-13 20:45:53.000000 vpso-1.1.0/tests/test_numerical.py
--rw-rw-rw-   0        0        0     3211 2023-06-10 15:56:23.000000 vpso-1.1.0/tests/test_reparation.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:13:06.998205 vpso-1.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-06 07:34:41.000000 vpso-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3575 2023-06-25 09:13:06.994287 vpso-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2872 2023-06-11 14:02:36.000000 vpso-1.1.1/README.md
+-rw-rw-rw-   0        0        0      977 2023-06-23 16:16:37.000000 vpso-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:13:06.998205 vpso-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 09:13:06.932579 vpso-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 09:13:06.964455 vpso-1.1.1/src/vpso/
+-rw-rw-rw-   0        0        0       50 2023-06-06 08:52:06.000000 vpso-1.1.1/src/vpso/__init__.py
+-rw-rw-rw-   0        0        0     4868 2023-06-24 19:57:21.000000 vpso-1.1.1/src/vpso/adaptation.py
+-rw-rw-rw-   0        0        0     6066 2023-06-24 19:57:21.000000 vpso-1.1.1/src/vpso/ask_and_tell.py
+-rw-rw-rw-   0        0        0     5178 2023-06-18 08:09:33.000000 vpso-1.1.1/src/vpso/initialization.py
+-rw-rw-rw-   0        0        0     7815 2023-06-24 19:57:21.000000 vpso-1.1.1/src/vpso/math.py
+-rw-rw-rw-   0        0        0     4494 2023-06-24 19:57:21.000000 vpso-1.1.1/src/vpso/mutation.py
+-rw-rw-rw-   0        0        0     3898 2023-06-24 19:57:21.000000 vpso-1.1.1/src/vpso/reparation.py
+-rw-rw-rw-   0        0        0     6822 2023-06-24 19:57:21.000000 vpso-1.1.1/src/vpso/termination.py
+-rw-rw-rw-   0        0        0      302 2023-06-18 08:09:11.000000 vpso-1.1.1/src/vpso/typing.py
+-rw-rw-rw-   0        0        0     7390 2023-06-21 12:22:03.000000 vpso-1.1.1/src/vpso/vpso.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:13:06.975087 vpso-1.1.1/src/vpso.egg-info/
+-rw-rw-rw-   0        0        0     3575 2023-06-25 09:13:06.000000 vpso-1.1.1/src/vpso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-06-25 09:13:06.000000 vpso-1.1.1/src/vpso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:13:06.000000 vpso-1.1.1/src/vpso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-25 09:13:06.000000 vpso-1.1.1/src/vpso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-25 09:13:06.000000 vpso-1.1.1/src/vpso.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 09:13:06.994287 vpso-1.1.1/tests/
+-rw-rw-rw-   0        0        0     4234 2023-06-20 15:11:09.000000 vpso-1.1.1/tests/test_adaptation.py
+-rw-rw-rw-   0        0        0     1186 2023-06-20 15:10:33.000000 vpso-1.1.1/tests/test_initialization.py
+-rw-rw-rw-   0        0        0     3437 2023-06-20 15:10:40.000000 vpso-1.1.1/tests/test_math.py
+-rw-rw-rw-   0        0        0     3594 2023-06-20 15:10:57.000000 vpso-1.1.1/tests/test_mutation.py
+-rw-rw-rw-   0        0        0     2119 2023-06-13 20:45:53.000000 vpso-1.1.1/tests/test_numerical.py
+-rw-rw-rw-   0        0        0     3181 2023-06-22 23:15:45.000000 vpso-1.1.1/tests/test_reparation.py
```

### Comparing `vpso-1.1.0/LICENSE` & `vpso-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/PKG-INFO` & `vpso-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vectorized Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vpso-1.1.0/README.md` & `vpso-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/pyproject.toml` & `vpso-1.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vpso"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Vectorized Particle Swarm Optimization"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
@@ -16,15 +16,15 @@
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics"
 ]
 dependencies = [
-    "numba >= 0.57.0",
+    "numba >= 0.57.1",
     "scipy >= 1.10.1",
     "typing_extensions >= 4.6.3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/FilippoAiraldi/vectorized-particle-swarm"
 "Bug Tracker" = "https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues"
```

### Comparing `vpso-1.1.0/src/vpso/adaptation.py` & `vpso-1.1.1/src/vpso/adaptation.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,28 +79,37 @@
     np_random: np.random.Generator,
 ) -> tuple[Array3d, Array3d, Array3d]:
     """Performs the adaptation of the parameters `w`, `c1` and `c2` based on the
     stage of the algorithm.
 
     Parameters
     ----------
+    px : 3d array
+        Best positions of the particles so far. An array of shape `(N, M, d)`, where `N`
+        is the number of vectorized problems to solve simultaneously, `M` the number of
+        particle, and `d` is the dimension of the search space.
+    sx : 3d array
+        Social best, i.e., the best particle so far. An array of shape `(N, 1, d)`.
     nvec : int
         Number of vectorized problems.
+    swarmsize : int
+        Number of particles in the swarm.
+    lb : 3d array
+        Lower bound of the search space. An array of shape `(N, 1, d)`.
+    ub : 3d array
+        Upper bound of the search space. An array of shape `(N, 1, d)`.
     w : 3d array
         Inertia weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
     c1 : 3d array
         Cognitive weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
     c2 : 3d array
         Social weight. An array of shape `(N, 1, 1)`, where each element is used for
         the corresponding problem.
-    stage : 1d array
-        Current stage of the algorithm. An array of shape `(N,)`, where each element
-        corresponds to a problem.
     np_random : np.random.Generator
         Random number generator.
 
     Returns
     -------
     tuple of 3d arrays
         The newly adapted parameters `w`, `c1` and `c2`.
```

### Comparing `vpso-1.1.0/src/vpso/ask_and_tell.py` & `vpso-1.1.1/src/vpso/ask_and_tell.py`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/src/vpso/initialization.py` & `vpso-1.1.1/src/vpso/initialization.py`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/src/vpso/math.py` & `vpso-1.1.1/src/vpso/math.py`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/src/vpso/mutation.py` & `vpso-1.1.1/src/vpso/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     mut_pow = 1.0 / eta
     xy1 = np.power((ub - x_best) / domain, eta)
     xy2 = np.power((x_best - lb) / domain, eta)
     R = np_random.random((nvec, dim))
     val1 = np.power(2.0 * R + (1.0 - 2.0 * R) * xy1, mut_pow)
     val2 = np.power(2.0 * (1.0 - R) + 2.0 * (R - 0.5) * xy2, mut_pow)
     deltaq = np.where(R <= 0.5, val1 - 1.0, 1.0 - val2)
-
     return np.where(mutation_mask, x_best + deltaq * domain, x_best).clip(lb, ub)
 
 
 @nb.njit(
     nb.types.void(
         nb.float64[:, :, :],  # x
         nb.float64[:, :, :],  # px
```

### Comparing `vpso-1.1.0/src/vpso/reparation.py` & `vpso-1.1.1/src/vpso/reparation.py`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/src/vpso/termination.py` & `vpso-1.1.1/src/vpso/termination.py`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/src/vpso/vpso.py` & `vpso-1.1.1/src/vpso/vpso.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Optional, Union
+from typing import Callable, Union
 
 import numpy as np
 from numpy.typing import ArrayLike
 from scipy.stats.qmc import LatinHypercube
 
 from vpso.adaptation import adapt
 from vpso.ask_and_tell import advance_population, generate_offsprings, get_best
@@ -24,20 +24,20 @@
     c2: Union[float, Array1d] = 2.0,
     #
     repair_iters: int = 20,
     perturb_best: bool = True,
     mutation_prob: float = 0.9,
     adaptive: bool = True,
     #
-    maxiter: int = 300,  # could be an array, but only the max would be then used
-    ftol: Union[float, Array1d] = 1e-8,
-    xtol: Union[float, Array1d] = 1e-8,
+    maxiter: int = 400,
+    ftol: Union[float, Array1d] = 1e-9,
+    xtol: Union[float, Array1d] = 1e-9,
     patience: Union[int, Array1i] = 30,
     #
-    seed: Optional[int] = None,
+    seed: Union[None, int, np.random.SeedSequence, np.random.Generator] = None,
 ) -> tuple[Array2d, Array1d, str]:
     """Vectorized Particle Swarm Optimization (VPSO). This implementation of PSO is able
     to solve multiple optimization problems simultaneously in a vectorized fashion.
 
     Parameters
     ----------
     func : callable
@@ -89,16 +89,16 @@
         solver. Can also be an 1d array_like of shape `(N,)` to specify a different
         value for each of the `N` vectorized problems. By default, `1e-8`. Pass a
         negative value to disable this check.
     patience : int or 1d array_like of ints, optional
         Number of iterations to wait before terminating the solver if no improvement is
         witnessed. Can also be an 1d array_like of shape `(N,)` to specify a different
         value for each of the `N` vectorized problems. By default, `1`.
-    seed : int, optional
-        Seed for the random number generator. By default, `None`.
+    seed : int or generator, optional
+        Seed for the random number generator, or a generator. By default, `None`.
 
     Returns
     -------
     tuple of (2d array, 1d array, str)
         Returns a tuple containing
          - the best minimizer of each problem
          - the best minimum of each problem
@@ -106,15 +106,15 @@
     """
     # first, adjust some dimensions
     lb, ub, nvec, dim, max_velocity_rate, w, c1, c2, ftol, xtol, patience = adj_dim(
         lb, ub, max_velocity_rate, w, c1, c2, ftol, xtol, patience
     )
 
     # initialize particle positions and velocities
-    np_random = np.random.Generator(np.random.PCG64(seed))
+    np_random = np.random.default_rng(seed)
     lhs_sampler = LatinHypercube(d=nvec * dim, seed=np_random)
     x, v, v_max = initialize_particles(
         nvec, swarmsize, dim, lb, ub, max_velocity_rate, lhs_sampler, np_random
     )
 
     # initialize particle's best pos/value and global best
     px = x  # particle's best position
```

### Comparing `vpso-1.1.0/src/vpso.egg-info/PKG-INFO` & `vpso-1.1.1/src/vpso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpso
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vectorized Particle Swarm Optimization
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/vectorized-particle-swarm
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/vectorized-particle-swarm/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vpso-1.1.0/src/vpso.egg-info/SOURCES.txt` & `vpso-1.1.1/src/vpso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/tests/test_adaptation.py` & `vpso-1.1.1/tests/test_adaptation.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         )
         sx = np.random.uniform(lb, ub, (nvec, dim))
         seed = np.random.randint(0, 1000)
         w = np.random.rand(nvec)
         c1 = np.random.rand(nvec) + 2
         c2 = np.random.rand(nvec) + 2
 
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         deltas = 0.05 + np_random.random(size=nvec) * 0.05
         w_new, c1_new, c2_new = [], [], []
         for i in range(nvec):
             problem = FunctionalProblem(
                 dim,
                 lambda x: np.square(x).sum(),
                 xl=lb[i],
@@ -109,15 +109,15 @@
             o = original_implementation2(
                 problem, px[i], sx[i], w[i], c1[i], c2[i], deltas[i]
             )
             w_new.append(o[0])
             c1_new.append(o[1])
             c2_new.append(o[2])
 
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         w_new_, c1_new_, c2_new_ = adapt(
             px,
             sx[:, np.newaxis],
             nvec,
             swarmsize,
             lb[:, np.newaxis],
             ub[:, np.newaxis],
```

### Comparing `vpso-1.1.0/tests/test_initialization.py` & `vpso-1.1.1/tests/test_initialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def test_initialize_particles(self):
         nvec, dim = np.random.randint(3, 10, size=2)
         swarmsize = np.random.randint(1000, 2000)
         ub = np.abs(np.random.randn(nvec, 1, dim))
         lb = -np.abs(np.random.randn(nvec, 1, dim))
         max_velocity_rate = np.random.uniform(0.1, 0.5)
         lhs_sampler = LatinHypercube(d=nvec * dim, scramble=False)
-        np_random = np.random.Generator(np.random.PCG64())
+        np_random = np.random.default_rng()
 
         x, v, v_max = initialize_particles(
             nvec, swarmsize, dim, lb, ub, max_velocity_rate, lhs_sampler, np_random
         )
         self.assertTupleEqual(x.shape, (nvec, swarmsize, dim))
         self.assertTupleEqual(v.shape, (nvec, swarmsize, dim))
         self.assertTupleEqual(v_max.shape, (nvec, 1, dim))
```

### Comparing `vpso-1.1.0/tests/test_math.py` & `vpso-1.1.1/tests/test_math.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         np.testing.assert_allclose(actual_c, expected_c)
         np.testing.assert_allclose(actual_p, expected_p)
 
     def test_pso_equation(self):
         seed = np.random.randint(0, 1000)
         nvec, dim = np.random.randint(3, 10, size=2)
         swarmsize = np.random.randint(1000, 2000)
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         r1 = np_random.uniform(size=(nvec, swarmsize, dim))
         r2 = np_random.uniform(size=(nvec, swarmsize, dim))
         x = np_random.normal(size=(nvec, swarmsize, dim))
         px = np_random.normal(size=(nvec, swarmsize, dim))
         sx = np_random.normal(size=(nvec, 1, dim))
         v = np_random.normal(size=(nvec, swarmsize, dim))
         v_max = np_random.normal(size=(nvec, 1, dim))
@@ -66,15 +66,15 @@
             o = original_implementation(
                 x[i], px[i], sx[i], v[i], v_max[i], w[i], c1[i], c2[i], r1[i], r2[i]
             )
             x_new_.append(o[0])
             v_new_.append(o[1])
         x_new_, v_new_ = np.asarray(x_new_), np.asarray(v_new_)
 
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         x_new, v_new = pso_equation(x, px, sx, v, v_max, w, c1, c2, np_random)
 
         np.testing.assert_allclose(x_new, x_new_)
         np.testing.assert_allclose(v_new, v_new_)
 
 
 if __name__ == "__main__":
```

### Comparing `vpso-1.1.0/tests/test_mutation.py` & `vpso-1.1.1/tests/test_mutation.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import numpy as np
 
 from vpso.mutation import mutate, polynomial_mutation
 
 
 class TestMutation(unittest.TestCase):
     def test_mutate__if_mutation_prob_is_zero__returns_immediately(self):
-        np_random = np.random.Generator(np.random.PCG64())
+        np_random = np.random.default_rng()
         nvec, dim = np_random.integers(3, 10, size=2)
         swarmsize = np_random.integers(1000, 2000)
         ub = np.abs(np_random.normal(size=(nvec, 1, dim))) + 10
         lb = -np.abs(np_random.normal(size=(nvec, 1, dim))) - 10
         x_mutated = np_random.uniform(lb, ub, (nvec, swarmsize, dim))
         x_original = x_mutated.copy()
         px = np_random.uniform(lb, ub, (nvec, swarmsize, dim))
         pf = np_random.uniform(size=(nvec, swarmsize))
         mutation_prob = 0.0
 
         mutate(x_mutated, px, pf, lb, ub, nvec, dim, mutation_prob, np_random)
         np.testing.assert_array_equal(x_original, x_mutated)
 
     def test_mutate__performs_mutation(self):
-        np_random = np.random.Generator(np.random.PCG64(17))
+        np_random = np.random.default_rng(17)
         nvec, dim = np_random.integers(3, 10, size=2)
         swarmsize = np_random.integers(1000, 2000)
         ub = np.abs(np_random.normal(size=(nvec, 1, dim))) + 10
         lb = -np.abs(np_random.normal(size=(nvec, 1, dim))) - 10
         x_mutated = np_random.uniform(lb, ub, (nvec, swarmsize, dim))
         x_original = x_mutated.copy()
         px = np_random.uniform(lb, ub, (nvec, swarmsize, dim))
@@ -40,15 +40,15 @@
         bests = set(pf.argmin(1))
         for i, j in product(range(nvec), range(swarmsize)):
             if j not in bests:
                 np.testing.assert_array_equal(x_original[i, j], x_mutated[i, j])
 
     def test_polynomial_mutation(self):
         seed = np.random.randint(0, 1000)
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         nvec, dim = np_random.integers(3, 10, size=2)
         ub = np.abs(np_random.normal(size=(nvec, dim))) + 10
         lb = -np.abs(np_random.normal(size=(nvec, dim))) - 10
         x = np_random.uniform(lb, ub, (nvec, dim))
 
         def original_implementation(X, eta, lb, ub, rand):
             delta1 = (X - lb) / (ub - lb)
@@ -63,23 +63,23 @@
             deltaq[mask] = d[mask]
             xy = 1.0 - delta2
             val = 2.0 * (1.0 - rand) + 2.0 * (rand - 0.5) * (np.power(xy, (eta + 1.0)))
             d = 1.0 - (np.power(val, mut_pow))
             deltaq[mask_not] = d[mask_not]
             return (X + deltaq * (ub - lb)).clip(lb, ub)
 
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         eta = np_random.uniform(5, 30, size=nvec)
         rand = np_random.uniform(size=(nvec, dim))
         expected = [
             original_implementation(x[i], eta[i], lb[i], ub[i], rand[i])
             for i in range(nvec)
         ]
 
-        np_random = np.random.Generator(np.random.PCG64(seed))
+        np_random = np.random.default_rng(seed)
         actual = polynomial_mutation(
             x, np.full((nvec, dim), True), lb, ub, nvec, dim, np_random
         )
         np.testing.assert_allclose(actual, expected)
 
 
 if __name__ == "__main__":
```

### Comparing `vpso-1.1.0/tests/test_numerical.py` & `vpso-1.1.1/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `vpso-1.1.0/tests/test_reparation.py` & `vpso-1.1.1/tests/test_reparation.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from parameterized import parameterized
 
 from vpso.reparation import repair_out_of_bounds
 
 
 class TestReparation(unittest.TestCase):
     def test_repair_out_of_bounds__if_in_bounds__returns_immediately(self):
-        np_random = np.random.Generator(np.random.PCG64())
+        np_random = np.random.default_rng()
         nvec, dim = np_random.integers(3, 10, size=2)
         swarmsize = np_random.integers(1000, 2000)
         ub = np.abs(np_random.normal(size=(nvec, 1, dim))) + 10
         lb = -np.abs(np_random.normal(size=(nvec, 1, dim))) - 10
         x = np_random.uniform(lb, ub, (nvec, swarmsize, dim))
         x_new = np_random.uniform(lb + 0.1, ub - 0.1, (nvec, swarmsize, dim))
         v_new = np_random.uniform(size=(nvec, swarmsize, dim))
@@ -42,15 +42,15 @@
         )
 
         np.testing.assert_array_equal(x_new_, x_new)
         np.testing.assert_array_equal(v_new_, v_new)
 
     @parameterized.expand([(0,), (200,)])
     def test_repair_out_of_bounds__with_resamplimg_repair(self, iters: int):
-        np_random = np.random.Generator(np.random.PCG64())
+        np_random = np.random.default_rng()
         nvec, dim = np_random.integers(3, 10, size=2)
         swarmsize = np_random.integers(1000, 2000)
         ub = np.abs(np_random.normal(size=(nvec, 1, dim))) + 10
         lb = -np.abs(np_random.normal(size=(nvec, 1, dim))) - 10
         x = np_random.uniform(lb, ub, (nvec, swarmsize, dim))
         x_new = np_random.uniform(lb - 10, ub + 10, (nvec, swarmsize, dim))
         v_new = np_random.uniform(size=(nvec, swarmsize, dim))
```

