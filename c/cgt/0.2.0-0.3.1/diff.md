# Comparing `tmp/cgt-0.2.0.tar.gz` & `tmp/cgt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgt-0.2.0.tar", last modified: Thu Jun 22 02:11:52 2023, max compression
+gzip compressed data, was "cgt-0.3.1.tar", last modified: Sun Jun 25 12:21:18 2023, max compression
```

## Comparing `cgt-0.2.0.tar` & `cgt-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.067998 cgt-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-22 02:11:40.000000 cgt-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-22 02:11:40.000000 cgt-0.2.0/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 02:11:40.000000 cgt-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 02:11:40.000000 cgt-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 02:11:52.067998 cgt-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-22 02:11:40.000000 cgt-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 02:11:40.000000 cgt-0.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.063998 cgt-0.2.0/cgt/
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/# Representation theory of the Hyperocta.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/genome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20386 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/position_paradigm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/rearrangements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.067998 cgt-0.2.0/cgt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-22 02:11:40.000000 cgt-0.2.0/cgt/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:11:52.067998 cgt-0.2.0/cgt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 02:11:52.000000 cgt-0.2.0/cgt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-22 02:11:41.000000 cgt-0.2.0/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-22 02:11:41.000000 cgt-0.2.0/playground_2.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:11:52.067998 cgt-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 02:11:41.000000 cgt-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-25 12:20:58.000000 cgt-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-25 12:20:58.000000 cgt-0.3.1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 12:20:58.000000 cgt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-25 12:20:58.000000 cgt-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 12:21:18.023588 cgt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 12:20:58.000000 cgt-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 12:20:58.000000 cgt-0.3.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/cgt/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/hyperoctahedral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/position_paradigm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/rearrangements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/cgt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/cgt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 12:21:17.000000 cgt-0.3.1/cgt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 12:21:18.000000 cgt-0.3.1/cgt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 12:21:17.000000 cgt-0.3.1/cgt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-25 12:21:17.000000 cgt-0.3.1/cgt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-25 12:20:58.000000 cgt-0.3.1/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-25 12:20:58.000000 cgt-0.3.1/playground_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 12:21:18.023588 cgt-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-25 12:20:58.000000 cgt-0.3.1/setup.py
```

### Comparing `cgt-0.2.0/CONTRIBUTING.md` & `cgt-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/INSTALL.md` & `cgt-0.3.1/INSTALL.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,11 @@
 
 - [Download binaries](https://www.sagemath.org/download-linux.html). You will most likely need the 64bit version. Choose the latest one for your operating system, making sure the OS version is the same.
 - Make a directory on your machine called `Sage` or similar, where you will place the sage installation. Move the file you downloaded into this folder.
 - Extract the files using `tar`. For example: `tar -xjf sage-9.3-Ubuntu_20.04-x86_64.tar.bz2` After extracting, you can delete the `.bz2` file.
 - `cd` into SageMath and run sage for the first time by executing the `sage` file. Wait for it to finish loading, to the point where you get the sage prompt and can type commands. Exit sage.
 - Run the command `sudo ln -s /path/to/SageMath/sage /usr/local/bin/sage` You can now start SageMath from any directory by typing `sage`.
 
-## Installing repsn
-
-Some functions of Circular-genome-tools require the GAP package repsn to be installed within SageMath. To install repsn inside Sage,
-
-- [Download repsn from this link](https://www.gap-system.org/Packages/repsn.html)
-- Extract the files as explained above.
-- move the directory `repsn-3.1.0` into the directory `SageMath/local/share/gap/pkg`
-
 ## Installing Circular Genome Tools
 
 After completing the above steps, execute the command `sage -pip install cgt`. When you import the package, it will warn you of any missing python packages you might need to install, inclding `scipy`, `matplotlib` and `networkx`.
```

### Comparing `cgt-0.2.0/LICENSE` & `cgt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/PKG-INFO` & `cgt-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.2.0
+Version: 0.3.1
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,8 +23,8 @@
 
 and use `import cgt` in a sage script or environment.
 
 If you would like to contribute to `cgt`, please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to get set up.
 
 If you use this software in your work, please cite it use the citation function on the github page or see [`CITATION.cff`](CITATION.cff)
 
-**Note:** you will need to at least have Sage version 9.0 installed, and have the GAP package `repsn` installed for the copy of GAP that sits inside Sage. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
+**Note:** you will need to at least have Sage version 9.0 installed. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
```

### Comparing `cgt-0.2.0/README.md` & `cgt-0.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 and use `import cgt` in a sage script or environment.
 
 If you would like to contribute to `cgt`, please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to get set up.
 
 If you use this software in your work, please cite it use the citation function on the github page or see [`CITATION.cff`](CITATION.cff)
 
-**Note:** you will need to at least have Sage version 9.0 installed, and have the GAP package `repsn` installed for the copy of GAP that sits inside Sage. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
+**Note:** you will need to at least have Sage version 9.0 installed. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
```

### Comparing `cgt-0.2.0/cgt/distances.py` & `cgt-0.3.1/cgt/distances.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,161 @@
 """
 Implements a number of distance measures for genomes under the position paradigm.
+
+The primary function of this module is the distance_matrix function, which returns a distance matrix for a given set of genomes and distance measure.
+
+The distance measures implemented are:
+    - min: the minimum number of rearrangements required to transform one genome into another
+    - min_weighted: the minimum number of rearrangements required to transform one genome into another, weighted by the inverse of the probability of the rearrangement
+    - MFPT: the mean first passage time from the identity to a given genome, where the target is an absorbing state
+    - MLE: the maximum likelihood estimate of the time elapsed between the identity and a given genome
+
+Individual likelihood functions for the time elapsed between the identity and a given genome can also be obtained
 """
 
 from cgt.enums import ALGEBRA, DISTANCE
 import numpy as np
 import networkx as nx
 from sage.all import ComplexDoubleField, UniversalCyclotomicField, matrix, Matrix, real, exp, round, CC, log
 from scipy.optimize import minimize_scalar
 
 def mles(framework, model, genome_instances=None, verbose=False):
-    """Return maximum likelihood estimates for a set of genome instances under the given model and framework"""
+    """
+    Returns a dictionary of maximum likelihood estimates for each genome instance under the given model and framework.
+
+    Args:
+        framework (PositionParadigmFramework): the framework
+        model (Model): the model
+        genome_instances (list): a list of genome instances to compute MLEs for. If None, all genomes in the framework are used.
+        verbose (bool): whether to print progress
+    
+    Returns:
+        dict: a dictionary of maximum likelihood estimates, indexed by genome instance
+    """
     mles = {}
     if genome_instances is None:
         genome_instances = [framework.canonical_instance(g) for g in framework.genomes()]
     for instance in genome_instances:
         if verbose: print(f"Computing MLE for {instance}")
         mles[instance] = mle(framework, model, instance)
-    return mles
+        return mles
 
 def mle(framework, model, genome_instance):
-    """Return maximum likelihood estimates for a genome instance under the given model and framework"""
-    return maximise(framework, likelihood_function(framework, model, genome_instance, attempt_exact=False))
+    """
+    Returns the maximum likelihood estimate for a given genome instance under the given model and framework.
+
+    Args:
+        framework (PositionParadigmFramework): the framework
+        model (Model): the model
+        genome_instance (group element): the genome instance to compute the MLE for
+
+    Returns:
+        float: the maximum likelihood estimate
+    """
+    return maximise(framework, likelihood_function(framework, model, genome_instance))
 
 def maximise(framework, L, max_time=100):
-    """Return the time that maximises likelihood function L, using additional information from the framework"""
+    """
+    Return the time that maximises likelihood function L, using additional information from the framework
+    
+    Args:
+        framework (PositionParadigmFramework): the framework
+        L (function): the likelihood function to maximise
+        max_time (float): the maximum time to consider (default: 100)
+    
+    Returns:
+        float: the time that maximises the likelihood function
+    """
     limit = 1/framework.num_genomes()
     t_max = minimize_scalar(lambda t: -1*L(t), method='bounded', bounds=(0, max_time))['x']
     mle = t_max if L(t_max)>limit else np.nan
     return mle
 
 def _projection_operators(mat, eigs):
-    """Return projection operators for given matrix and its eigenvalues"""
+    """
+    Return projection operators for given matrix and its eigenvalues
+    
+    Args:
+        mat (matrix): a representation of zs
+        eigs (list): a list of eigenvalues of mat
+
+    Returns:
+        list: a list of projection operators
+    """
     dim = mat.nrows()
     projections = [matrix.identity(dim) for _ in eigs]
     for e1, eig1 in enumerate(eigs):
         for eig2 in eigs:
             if eig1 != eig2:
                 projections[e1] *= (mat-(eig2*matrix.identity(dim)))*(1/(eig1-eig2))
     return projections
 
-def _irreps_of_zs(framework, model, attempt_exact=False, force_recompute=False):
-    """Return a set of matrices---images of zs under each irrep"""
+def _irreps_of_zs(framework, model, force_recompute=False):
+    """
+    Return a set of matrices---images of zs under each irrep
+    
+    Args:
+        framework (PositionParadigmFramework): the framework
+        model (Model): the model 
+        force_recompute (bool): whether to force recomputation and invalidate cache (default: False)
+
+    Returns:
+        list: a list of irredicuble representations of the group applied to zs
+    """
     key = "irreps_of_zs"
     if key in model.data_bundle and not force_recompute:
         irreps_of_zs =  model.data_bundle[key]
     else:
         CDF, UCF = ComplexDoubleField(), UniversalCyclotomicField()
         z = framework.symmetry_element()
         s = model.s_element(in_algebra=ALGEBRA.genome)
         irreps_of_z, irreps_of_s = framework.irreps(z), framework.irreps(s)
         irreps_of_zs = (matrix(UCF, irrep_z*irrep_s) for irrep_z, irrep_s in zip(irreps_of_z, irreps_of_s))
-        irreps_of_zs = [Matrix(UCF if attempt_exact else CDF, irrep_zs) for irrep_zs in irreps_of_zs]
+        irreps_of_zs = [Matrix(CDF, irrep_zs) for irrep_zs in irreps_of_zs]
         for irrep in irreps_of_zs:
             irrep.set_immutable()
         model.data_bundle[key] = irreps_of_zs
     return irreps_of_zs
 
+def _irreps_of_z(framework, model, force_recompute=False):
+    """
+    Return a set of matrices---images of z (the symmetry element) under each irrep
+    
+    Args:
+        framework (PositionParadigmFramework): the framework
+        model (Model): the model
+        force_recompute (bool): whether to force recomputation and invalidate cache (default: False)
+
+    Returns:
+        list: a list of irredicuble representations of the group applied to z
+    """
+    key = "irreps_of_z"
+    if key in model.data_bundle and not force_recompute:
+        irreps_of_z =  model.data_bundle[key]
+    else:
+        CDF, UCF = ComplexDoubleField(), UniversalCyclotomicField()
+        z = framework.symmetry_element()
+        irreps_of_z = framework.irreps(z)
+        irreps_of_z = (matrix(UCF, irrep_z) for irrep_z in irreps_of_z)
+        irreps_of_z = [Matrix(CDF, irrep_z) for irrep_z in irreps_of_z]
+        for irrep in irreps_of_z:
+            irrep.set_immutable()
+        model.data_bundle[key] = irreps_of_z
+    return irreps_of_z
 
-def _eigenvalues(mat, round_to=7, make_real=True, inc_repeated=False, attempt_exact=False, use_numpy=True, bin_eigs=False, tol=10**(-8)):
+
+def _eigenvalues(mat, round_to=7, make_real=True, inc_repeated=False, use_numpy=True, bin_eigs=False, tol=10**(-8)):
     """Return all the eigenvalues for a given matrix mat"""
     col = list if inc_repeated else set
     if use_numpy:
         new_mat = np.array(matrix(CC, mat))
         all_eigs = np.linalg.eigvals(new_mat)
     else:
         all_eigs = (eig for eig in mat.eigenvalues())
-    if attempt_exact: 
-        return sorted(col(all_eigs))
-    elif bin_eigs:
+    if bin_eigs:
         return _bin(sorted(all_eigs), return_bin_size=False, tol=tol)
     else:
         return sorted(col(round(real(eig) if make_real else eig, round_to) for eig in all_eigs))
 
 def _bin(eigenvalues, tol=10**(-8), return_bin_size=False):
     binned_eigenvals = []
     num_eigs = len(eigenvalues) # ??
@@ -95,93 +179,48 @@
     for v in range(len(binned_eigenvals)):
         c=binned_eigenvals[v][1] 
         vec, _ = matrix([eigen_tuples[q+l][1][0].list() for l in range(c)]).gram_schmidt(orthonormal=True)
         eigenvectors.append(vec)
         q=q+c
     return binned_eigenvals, eigenvectors
 
-def _eigenvectors_reduce_error(mat, tol=10**(-8)):
-    eigen_tuples = sorted(mat.eigenvectors_right())
-    binned_eigenvals = _bin([et[0] for et in eigen_tuples], tol=tol, return_bin_size=True)
-    # Orthogonalise the eigenvectors                      
-    q = 0
-    eigenvectors = []
-    for v in range(len(binned_eigenvals)):
-        c = binned_eigenvals[v][1] 
-        A = matrix([eigen_tuples[q+l][1][0].list() for l in range(c)]).transpose()
-        print(A.ncols(), A.nrows())
-        # If the rounded eigenvalue is zero
-        if round(binned_eigenvals[v][0], 8) == 0:
-            Q = None
-        else:
-            Q, _ = A.QR()
-            print(Q.nrows(), Q.ncols())
-            Q = Q.delete_columns(list(range(A.ncols(),A.nrows())))
-            print(Q.nrows(), Q.ncols())
-        eigenvectors.append(Q)
-        q += c
-    return binned_eigenvals, eigenvectors
-
 def _partial_traces_for_genome(framework, instance, irreps, irreps_of_zs, projections, eig_lists, irreps_of_z=None):
     """Return dictionary of partial traces, indexed first by irrep index and then by eigenvalaue"""
     if irreps_of_z is None:
         irreps_of_z = [irrep(framework.symmetry_element()) for irrep in irreps]
-    CDF, UCF = ComplexDoubleField(), UniversalCyclotomicField()
     traces = {
         r: {
             eigenvalue: {} for eigenvalue in eig_lists[r]
         } for r in range(len(irreps_of_zs))
     }
     for r, irrep in enumerate(irreps): # Iterate over irreducible representations
-        sigd = irreps_of_z[r] * Matrix(CDF, matrix(UCF, irrep(framework.cycles(instance.inverse()))))
+        sigd = irreps_of_z[r] * irrep(instance.inverse())
         for e, eigenvalue in enumerate(eig_lists[r]):
-            traces[r][eigenvalue] = round(real((sigd*projections[r][e]).trace()), 6)
+            traces[r][eigenvalue] = real((sigd*projections[r][e]).trace())
     return traces
 
-def _partial_traces_for_genome_using_eigenvectors(framework, instance, irreps, irreps_of_zs):
-    """Return dictionary of partial traces, indexed first by irrep index and then by eigenvalaue"""
-    irreps_of_z = [irrep(framework.symmetry_element()) for irrep in irreps]
-    eigenvectors_list = [_eigenvectors(irrep_zs) for irrep_zs in irreps_of_zs]
-    CDF, UCF = ComplexDoubleField(), UniversalCyclotomicField()
-    traces = {
-        r: {
-            eigenvalue[0]: {} for eigenvalue in eigenvectors_list[r][0]
-        } for r in range(len(irreps_of_zs))
-    }
-    for r, irrep in enumerate(irreps): # Iterate over irreducible representations
-        sigd = irreps_of_z[r] * Matrix(CDF, matrix(UCF, irrep(framework.cycles(instance.inverse()))))
-        eigenvalues = eigenvectors_list[r][0]
-        eigenvector_list = eigenvectors_list[r][1]
-        for e, eigenvalue in enumerate(eigenvalues):
-            eigenvectors = eigenvector_list[e]
-            traces[r][eigenvalue[0]]=round(real((sum([(eigenvectors[m,:].H)*eigenvectors[m,:] for m in range(eigenvalue[1])])*sigd).trace()),6)
-    return traces
-
-def likelihood_function(framework, model, genome, attempt_exact=False, use_projections=True):
+def likelihood_function(framework, model, genome):
     """Return the likelihood function for a given genome"""
     instance = genome
     CDF, UCF = ComplexDoubleField(), UniversalCyclotomicField()
     G, Z = framework.genome_group(), framework.symmetry_group()
     irreps = framework.irreps()
-    irreps_of_zs = _irreps_of_zs(framework, model, attempt_exact=attempt_exact)
-    if use_projections:
-        if "eig_lists" in model.data_bundle:
-            eig_lists = model.data_bundle["eig_lists"]
-        else:
-            eig_lists = [_eigenvalues(irrep_zs, round_to=7, make_real=True, inc_repeated=False, attempt_exact=attempt_exact) for irrep_zs in irreps_of_zs]
-            model.data_bundle["eig_lists"] = eig_lists
-        if "projections" in model.data_bundle:
-            projections = model.data_bundle["projections"]
-        else:
-            projections = [_projection_operators(*vals) for vals in zip(irreps_of_zs, eig_lists)]
-            model.data_bundle["projections"] = projections
-        traces = _partial_traces_for_genome(framework, instance, irreps, irreps_of_zs, projections, eig_lists)
+    irreps_of_zs = _irreps_of_zs(framework, model)
+    irreps_of_z = _irreps_of_z(framework, model)
+    if "eig_lists" in model.data_bundle:
+        eig_lists = model.data_bundle["eig_lists"]
+    else:
+        eig_lists = [_eigenvalues(irrep_zs) for irrep_zs in irreps_of_zs]
+        model.data_bundle["eig_lists"] = eig_lists
+    if "projections" in model.data_bundle:
+        projections = model.data_bundle["projections"]
     else:
-        eig_lists = [[x[0] for x in _eigenvectors(irrep_zs)[0]] for irrep_zs in irreps_of_zs]
-        traces = _partial_traces_for_genome_using_eigenvectors(framework, instance, irreps, irreps_of_zs)
+        projections = [_projection_operators(*vals) for vals in zip(irreps_of_zs, eig_lists)]
+        model.data_bundle["projections"] = projections
+    traces = _partial_traces_for_genome(framework, instance, irreps, irreps_of_zs, projections, eig_lists, irreps_of_z)
     dims = [irrep_of_zs.nrows() for irrep_of_zs in irreps_of_zs]
     def likelihood(t):
         ans = 0
         for r, dim in enumerate(dims):
             ans += Z.order()*(exp(-t)/G.order())*dim*sum(exp(eigenvalue*CDF(t)) * traces[r][eigenvalue] for eigenvalue in eig_lists[r])
         return real(ans)
     return likelihood
@@ -230,14 +269,23 @@
     else:
         D = np.zeros((len(distances), len(distances)))
         for (i, j), distance in distances.items():
             D[i,j] = distance
     return D
 
 def distance_matrix(framework, model, genomes, distance):
+    """
+    Compute a distance matrix for a given set of genomes and distance measure.
+
+    Args:
+        framework (PositionParadigmFramework): the framework
+        model (Model): the model
+        genomes (list): a list of genomes to compute distances for
+        distance (DISTANCE): the distance measure to use
+    """
     instances = [framework.canonical_instance(g) for g in genomes]
     # Get the genomes g that we need dist(id -> g) for:
     need_distances = {}
     for i, _ in enumerate(genomes):
         for j, _ in enumerate(genomes):
             if i < j:
                 canonical_i, canonical_j = instances[i], instances[j]
```

### Comparing `cgt-0.2.0/cgt/enums.py` & `cgt-0.3.1/cgt/enums.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt/models.py` & `cgt-0.3.1/cgt/models.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt/parsers.py` & `cgt-0.3.1/cgt/parsers.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt/position_paradigm.py` & `cgt-0.3.1/cgt/position_paradigm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .enums import *
 import numpy as np
 import warnings
 from copy import deepcopy
 from .structures import HyperoctahedralGroup
 from scipy.sparse import dok_matrix as dok
 from random import choice
+from .hyperoctahedral import HyperoctahedralGroupRepresentations
 
 class PositionParadigmFramework:
     """Everything you need for working with genomes under the position paradigm"""
 
     def __init__(self, num_regions, oriented=True, symmetry=SYMMETRY.circular, genome_type=TYPE.reg_to_signed_pos):
         """Instantiate a system of position paradigm genomes with given set of symmetries and number of regions."""
         if genome_type != TYPE.reg_to_signed_pos:
@@ -366,24 +367,24 @@
         representations = []
         def irrep_function_factory(irrep, signed):
             def representation(sigma, _irrep=irrep, _signed=signed):
                     result = 0
                     if sigma in self.group_algebra(): # sigma is an algebra element
                         for term in sigma:
                             perm, coeff = term
-                            result += coeff * (gap.Image(_irrep, perm) if _signed else _irrep(perm))
+                            result += coeff * _irrep(perm)
                     else: # sigma is a group element
-                        result = (gap.Image(_irrep, sigma) if _signed else _irrep(sigma))
-                    mat = matrix(UniversalCyclotomicField(), result)
-                    return mat.transpose() if _signed else mat
+                        result = _irrep(sigma)
+                    mat = result
+                    return mat.transpose() if _signed else matrix(mat)
             return representation
         if not self.oriented:
             irreps = SymmetricGroupRepresentations(self.n)
         else:
-            irreps = (gap.IrreducibleAffordingRepresentation(character) for character in gap.Irr(self.genome_group()))
+            irreps = list(HyperoctahedralGroupRepresentations(self.n).values()) #(gap.IrreducibleAffordingRepresentation(character) for character in gap.Irr(self.genome_group()))
         for irrep in irreps:
             representations.append(irrep_function_factory(irrep, self.oriented))
         self.representations = representations
         return self.representations
 
     def regular_representation(self, g):
         """Return the regular representation of a single element"""
```

### Comparing `cgt-0.2.0/cgt/rearrangements.py` & `cgt-0.3.1/cgt/rearrangements.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt/simulations.py` & `cgt-0.3.1/cgt/simulations.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt/structures.py` & `cgt-0.3.1/cgt/structures.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt/visualisation.py` & `cgt-0.3.1/cgt/visualisation.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/cgt.egg-info/PKG-INFO` & `cgt-0.3.1/cgt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.2.0
+Version: 0.3.1
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,8 +23,8 @@
 
 and use `import cgt` in a sage script or environment.
 
 If you would like to contribute to `cgt`, please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to get set up.
 
 If you use this software in your work, please cite it use the citation function on the github page or see [`CITATION.cff`](CITATION.cff)
 
-**Note:** you will need to at least have Sage version 9.0 installed, and have the GAP package `repsn` installed for the copy of GAP that sits inside Sage. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
+**Note:** you will need to at least have Sage version 9.0 installed. If you aren't sure how to do this, see the installation instructions in [`INSTALL.md`](INSTALL.md).
```

### Comparing `cgt-0.2.0/playground.py` & `cgt-0.3.1/playground.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/playground_2.py` & `cgt-0.3.1/playground_2.py`

 * *Files identical despite different names*

### Comparing `cgt-0.2.0/setup.py` & `cgt-0.3.1/setup.py`

 * *Files identical despite different names*

