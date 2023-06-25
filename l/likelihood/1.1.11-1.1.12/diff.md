# Comparing `tmp/likelihood-1.1.11.tar.gz` & `tmp/likelihood-1.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likelihood-1.1.11.tar", last modified: Fri Feb  3 04:07:58 2023, max compression
+gzip compressed data, was "likelihood-1.1.12.tar", last modified: Sun Jun 25 18:29:21 2023, max compression
```

## Comparing `likelihood-1.1.11.tar` & `likelihood-1.1.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 04:07:58.305735 likelihood-1.1.11/
--rw-rw-rw-   0        0        0     1087 2022-01-07 23:59:47.000000 likelihood-1.1.11/LICENSE
-drwxrwxrwx   0        0        0        0 2023-02-03 04:07:58.278331 likelihood-1.1.11/Likelihood.egg-info/
--rw-rw-rw-   0        0        0     1764 2023-02-03 04:07:53.000000 likelihood-1.1.11/Likelihood.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-02-03 04:07:57.000000 likelihood-1.1.11/Likelihood.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 04:07:54.000000 likelihood-1.1.11/Likelihood.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-02-03 04:07:56.000000 likelihood-1.1.11/Likelihood.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-03 04:07:56.000000 likelihood-1.1.11/Likelihood.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1764 2023-02-03 04:07:58.296136 likelihood-1.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2022-01-07 23:59:47.000000 likelihood-1.1.11/README.md
-drwxrwxrwx   0        0        0        0 2023-02-03 04:07:58.249952 likelihood-1.1.11/likelihood/
--rw-rw-rw-   0        0        0      350 2022-03-31 01:21:31.000000 likelihood-1.1.11/likelihood/__init__.py
--rw-rw-rw-   0        0        0     8324 2022-12-20 01:46:12.000000 likelihood-1.1.11/likelihood/main.py
--rw-rw-rw-   0        0        0     3698 2020-11-27 02:29:48.000000 likelihood-1.1.11/likelihood/numeric_tools.py
--rw-rw-rw-   0        0        0    15167 2022-12-20 01:46:12.000000 likelihood-1.1.11/likelihood/regression_models.py
--rw-rw-rw-   0        0        0    16368 2023-02-03 04:02:46.000000 likelihood-1.1.11/likelihood/tools.py
--rw-rw-rw-   0        0        0       42 2023-02-03 04:07:58.306760 likelihood-1.1.11/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-02-03 04:04:45.000000 likelihood-1.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:29:21.097117 likelihood-1.1.12/
+-rw-rw-rw-   0        0        0     1087 2023-05-16 17:47:36.000000 likelihood-1.1.12/LICENSE
+-rw-rw-rw-   0        0        0     1723 2023-06-25 18:29:21.084556 likelihood-1.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-05-16 17:47:36.000000 likelihood-1.1.12/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 18:29:20.925236 likelihood-1.1.12/likelihood/
+-rw-rw-rw-   0        0        0      350 2023-05-16 17:47:37.000000 likelihood-1.1.12/likelihood/__init__.py
+-rw-rw-rw-   0        0        0     8330 2023-06-25 17:44:00.000000 likelihood-1.1.12/likelihood/main.py
+-rw-rw-rw-   0        0        0     3601 2023-06-25 17:44:00.000000 likelihood-1.1.12/likelihood/numeric_tools.py
+-rw-rw-rw-   0        0        0    15348 2023-06-25 17:44:00.000000 likelihood-1.1.12/likelihood/regression_models.py
+-rw-rw-rw-   0        0        0    18905 2023-06-25 18:22:06.000000 likelihood-1.1.12/likelihood/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:29:21.071616 likelihood-1.1.12/likelihood.egg-info/
+-rw-rw-rw-   0        0        0     1723 2023-06-25 18:29:20.000000 likelihood-1.1.12/likelihood.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-25 18:29:20.000000 likelihood-1.1.12/likelihood.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:29:20.000000 likelihood-1.1.12/likelihood.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-25 18:29:20.000000 likelihood-1.1.12/likelihood.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 18:29:20.000000 likelihood-1.1.12/likelihood.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:29:21.097117 likelihood-1.1.12/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-06-25 18:28:44.000000 likelihood-1.1.12/setup.py
```

### Comparing `likelihood-1.1.11/LICENSE` & `likelihood-1.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `likelihood-1.1.11/Likelihood.egg-info/PKG-INFO` & `likelihood-1.1.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: likelihood
-Version: 1.1.11
+Version: 1.1.12
 Summary: A package that performs the maximum likelihood algorithm.
 Home-page: https://github.com/jzsmoreno/likelihood/
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,9 +36,7 @@
 ```
 
 ## Examples
 
 You can check the [examples](https://github.com/jzsmoreno/likelihood/tree/main/examples) folder.
 
 More examples will be added soon.
-
-
```

### Comparing `likelihood-1.1.11/PKG-INFO` & `likelihood-1.1.12/likelihood.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: likelihood
-Version: 1.1.11
+Version: 1.1.12
 Summary: A package that performs the maximum likelihood algorithm.
 Home-page: https://github.com/jzsmoreno/likelihood/
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,9 +36,7 @@
 ```
 
 ## Examples
 
 You can check the [examples](https://github.com/jzsmoreno/likelihood/tree/main/examples) folder.
 
 More examples will be added soon.
-
-
```

### Comparing `likelihood-1.1.11/README.md` & `likelihood-1.1.12/README.md`

 * *Files identical despite different names*

### Comparing `likelihood-1.1.11/likelihood/main.py` & `likelihood-1.1.12/likelihood/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
+import corner
 import matplotlib.pyplot as plt
 import numpy as np
-import corner
 
 
 def lnprior(theta, conditions):
     """Computes the prior probability.
 
     Parameters
     ----------
     theta : np.ndarray
         An array containing the parameters of the model.
     conditions : list
-        A list containing $2n$-conditions for the (min, max) range of the 
+        A list containing $2n$-conditions for the (min, max) range of the
         $n$ parameters.
-    
+
     Returns
     -------
     lp : float
         The a priori probability.
     """
 
-    try: 
+    try:
         if len(conditions) != 2 * len(theta):
-            error_type = 'IndexError'
-            msg = 'Length of conditions must be twice the length of theta.'
-            print(f'{error_type}: {msg}')
+            error_type = "IndexError"
+            msg = "Length of conditions must be twice the length of theta."
+            print(f"{error_type}: {msg}")
         else:
             cond = np.array(conditions).reshape((len(theta), 2))
             for i in range(len(theta)):
                 if cond[i, 0] < theta[i] < cond[i, 1]:
-                    lp =  0.0
+                    lp = 0.0
                 else:
                     return np.inf
             return lp
     except:
         return 0.0
-    
+
 
 def fun_like(x, y, model, theta, conditions=None, var2=1.0):
     """Computes the likelihood.
 
     Parameters
     ----------
     x : np.ndarray
@@ -48,15 +48,15 @@
         An $n$ dimensional array that will be compared with model's output.
     model : function
         A Python function defined by the user. This function should recieve
         two arguments $(x, theta)$.
     theta : np.ndarray
         The array containing the model's parameters.
     conditions : list
-        A list containing $2n$-conditions for the (min, max) range of the 
+        A list containing $2n$-conditions for the (min, max) range of the
         $n$ parameters.
     var2 : float
         Determines the step size of the walker. By default it is set to `1.0`.
 
     Returns
     -------
     lhood : float
@@ -75,18 +75,18 @@
     y_sum = np.sum((y - y_hat) ** 2 * inv_sigma2 - np.log(inv_sigma2))
     lhood = 0.5 * y_sum
 
     if not np.isfinite(lp):
         lhood = np.inf
     else:
         lhood += lp
-    
+
     return lhood
 
-    
+
 def update_theta(theta, d):
     """Updates the theta parameters.
 
     Parameters
     ----------
     theta : np.ndarray
         The ndarray containing the model's parameters.
@@ -98,50 +98,49 @@
     theta_new : np.array
         An ndarray with the updated theta values.
     """
 
     theta_new = []
 
     for k in range(len(theta)):
-        theta_new.append(np.random.normal(theta[k], d / 2.))
+        theta_new.append(np.random.normal(theta[k], d / 2.0))
 
     return theta_new
 
-    
-def walk(x, y, model, theta, conditions=None, var2=0.01, mov=100,
-         d=1, tol=1e-3, mode=True):
+
+def walk(x, y, model, theta, conditions=None, var2=0.01, mov=100, d=1, tol=1e-3, mode=True):
     """Executes the walker implementation.
-    
+
     Parameters
     ----------
     x : np.ndarray
         An $(m, n)$ dimensional array for (cols, rows).
     y : np.ndarray
         An $n$ dimensional array that will be compared with model's output.
     model : function
         A Python function defined by the user. This function should recieve
         two arguments $(x, theta)$.
     theta : np.ndarray
         The array containing the model's parameters.
     conditions : list
-        A list containing $2n$-conditions for the (min, max) range of the 
+        A list containing $2n$-conditions for the (min, max) range of the
         $n$ parameters.
     var2 : float
         Determines the step size of the walker. By default it is set to `1.0`.
     mov : int
         Number of movements that walker will perform. By default it is set
         to `100`.
     d : float
         Size of the Gaussian step for the walker.
     tol : float
         Convergence criteria for the log-likelihhod. By default it is set
         to `1e-3`.
     mode : bool
         By default it is set to `True`.
-    
+
     Returns
     -------
     theta : np.array
         An ndarray with the updated theta values.
     nwalk : np.array
         Updates of theta for each movement performed by the walker.
     y0 : float
@@ -154,23 +153,23 @@
     for i in range(mov):
         nwalk.append(theta)
         theta_new = update_theta(theta, d)
 
         if not greach:
             y0 = fun_like(x, y, model, theta, conditions, var2)
             y1 = fun_like(x, y, model, theta_new, conditions, var2)
-            
+
             if y0 <= tol and mode:
-                print('Goal reached!')
+                print("Goal reached!")
                 greach = True
-                
+
                 return theta, nwalk, y0
             else:
                 if y1 <= tol and mode:
-                    print('Goal reached!')
+                    print("Goal reached!")
                     greach = True
 
                     return theta_new, nwalk, y1
                 else:
                     ratio = y0 / y1
                     boltz = np.random.rand(1)
                     prob = np.exp(-ratio)
@@ -181,39 +180,51 @@
                     else:
                         if prob > boltz:
                             theta = theta_new
                             theta_new = update_theta(theta, d)
                         else:
                             theta_new = update_theta(theta, d)
     if mode:
-        print('Maximum number of iterations reached!')
-        print(f'The log-likelihood is: {y0}')
+        print("Maximum number of iterations reached!")
+        print(f"The log-likelihood is: {y0}")
 
     return theta, nwalk, y0
 
 
-def walkers(nwalkers, x, y, model, theta, conditions=None, var2=0.01,
-            mov=100, d=1, tol=1e-3, mode=False, figname='fig_out.png'):
+def walkers(
+    nwalkers,
+    x,
+    y,
+    model,
+    theta,
+    conditions=None,
+    var2=0.01,
+    mov=100,
+    d=1,
+    tol=1e-3,
+    mode=False,
+    figname="fig_out.png",
+):
     """Executes multiple walkers.
-    
+
     Parameters
     ----------
     nwalkers : int
         The number of walkers to be executed.
     x : np.ndarray
         An $(m, n)$ dimensional array for (cols, rows).
     y : np.ndarray
         An $n$ dimensional array that will be compared with model's output.
     model : function
         A Python function defined by the user. This function should recieve
         two arguments $(x, theta)$.
     theta : np.ndarray
         The array containing the model's parameters.
     conditions : list
-        A list containing $2n$-conditions for the (min, max) range of the 
+        A list containing $2n$-conditions for the (min, max) range of the
         $n$ parameters.
     var2 : float
         Determines the step size of the walker. By default it is set to `1.0`.
     mov : int
         Number of movements that walker will perform. By default it is set
         to `100`.
     d : float
@@ -223,47 +234,52 @@
         to `1e-3`.
     mode : bool
         Specifies that we will be working with more than one walker. By
         default it is set to `False`.
     figname : str
         The name of the output file for the figure. By default it is set
         to `fig_out.png`.
-    
+
     Returns
     -------
     par : np.array
         The theta found by each of the walkers.
     error : np.array
         The log-likelihood array.
     """
 
     error = []
     par = []
 
     for i in range(nwalkers):
-        theta, nwalk, y0 = walk(x, y, model, theta, conditions,
-                                var2, mov, d, tol, mode)
+        theta, nwalk, y0 = walk(x, y, model, theta, conditions, var2, mov, d, tol, mode)
         par.append(theta)
         nwalk = np.array(nwalk).reshape((len(nwalk), len(nwalk[i])))
         error.append(y0)
-    
+
         if figname != None:
             for k in range(nwalk.shape[1]):
-                sub = '$\\theta _{' + str(k) + '}$'
-                plt.plot(range(len(nwalk[:, k])), nwalk[:, k], '-', label=sub)
-                plt.ylabel('$\\theta$')
-                plt.xlabel('iterations')
-                plt.savefig('walkers_'+figname, dpi = 300, transparent = True)
+                sub = "$\\theta _{" + str(k) + "}$"
+                plt.plot(range(len(nwalk[:, k])), nwalk[:, k], "-", label=sub)
+                plt.ylabel("$\\theta$")
+                plt.xlabel("iterations")
+                plt.savefig("walkers_" + figname, dpi=300, transparent=True)
 
-    if figname != None: plt.show()
+    if figname != None:
+        plt.show()
 
     if nwalk.shape[1] == 2:
         if figname != None:
-            fig = corner.hist2d(nwalk[:, 0], nwalk[:, 1], range=None, bins=18, 
-                                smooth=True, plot_datapoints=True,
-                                plot_density=True)
-            plt.ylabel('$\\theta_{1}$')
-            plt.xlabel('$\\theta_{0}$')
-            plt.savefig('theta_'+figname, dpi = 300, transparent = True)
+            fig = corner.hist2d(
+                nwalk[:, 0],
+                nwalk[:, 1],
+                range=None,
+                bins=18,
+                smooth=True,
+                plot_datapoints=True,
+                plot_density=True,
+            )
+            plt.ylabel("$\\theta_{1}$")
+            plt.xlabel("$\\theta_{0}$")
+            plt.savefig("theta_" + figname, dpi=300, transparent=True)
 
     return par, error
-
```

### Comparing `likelihood-1.1.11/likelihood/numeric_tools.py` & `likelihood-1.1.12/likelihood/numeric_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+
 def subs(a, b):
     """Function that subtracts lists element by element.
 
     Parameters
     ----------
     a
     b
@@ -13,49 +14,49 @@
         val = val - b[i]
         a[i] = val
     return a
 
 
 def ecprint(A):
     """Function that prints the augmented matrix.
-    
+
     Parameters
     ----------
     A : np.array
         The augmented matrix.
-    
+
     """
 
     n = len(A)
     for i in range(0, n):
         line = ""
     for j in range(0, n + 1):
         line += str(format(round(A[i][j], 2))) + "\t"
-        if j == n-1:
+        if j == n - 1:
             line += "| "
         print(line)
     print()
-    
+
 
 def sor_elimination(A, b, n, nmax, w):
     """Computes the successive over-relaxation algorithm.
-    
+
     Parameters
     ----------
     A : np.array
         An array containing the parameters of the $n$ equations.
     b : np.array
         An array containing the equalities of the $n$ equations.
     n : int
         Is the dimension of the system of equations.
     nmax : int
         Is the maximum number of iterations.
     w : float
         Is a parameter of the SOR method
-        
+
     Returns
     -------
     xi : np.array
         The solution of the system of $n$ equations
     """
 
     xin = np.zeros(n)
@@ -63,81 +64,80 @@
         xi = np.zeros(n)
         for i in range(n):
             s1, s2 = 0, 0
             for j in range(i):
                 s1 = s1 + (A[i, j] * xin[j])
             for j in range(i + 1, n):
                 s2 = s2 + (A[i, j] * xin[j])
-            xi[i] = (w / A[i, i]) * (b[i] - s1 - s2) \
-                    + (1. / A[i, i]) * (b[i] - s1) * (1 - w)
-            
-        error = np.max(np.abs(xi - xin))  
+            xi[i] = (w / A[i, i]) * (b[i] - s1 - s2) + (1.0 / A[i, i]) * (b[i] - s1) * (1 - w)
+
+        error = np.max(np.abs(xi - xin))
         print(xi)
-        print(f'solution error : {error}')
+        print(f"solution error : {error}")
         if error <= 0.00001:
-            print(f'iterations : {k}')
+            print(f"iterations : {k}")
             return xi
         else:
             xin = np.copy(xi)
-    return 'number of iterations exceeded'
+    return "number of iterations exceeded"
 
 
 def gauss_elimination(A, pr=2):
     """Computes the Gauss elimination algorithm.
-    
+
     Parameters
     ----------
     A : np.array or list
         An array containing the parameters of the $n$ equations
         with the equalities.
-        
+
     pr : int
         significant numbers of decimals.
-        
+
     Returns
     -------
     X : np.array
         The solution of the system of $n$ equations
-    
+
     """
 
     n = len(A)
     M = [[0 for x in range(n + 1)] for x in range(n)]
     X = [0 for x in range(n)]
-    
+
     for i in range(n - 1):
         for p in range(i, n):
             if i <= p <= (n - 1) and A[p][i] != 0:
-                if p!= i:
+                if p != i:
                     A[p], A[i] = A[i], A[p]
                 break
             elif p == (n - 1):
-                print('there is no single solution')
+                print("there is no single solution")
                 return None
 
         for j in range(i + 1, n):
             if i <= j <= n and A[j][i] != 0:
                 if A[i][i] < A[j][i]:
                     A[j], A[i] = A[i], A[j]
                 break
 
         for j in range(i + 1, n):
             M[j][i] = A[j][i] / A[i][i]
             A[j] = subs(A[j], np.multiply(M[j][i], A[i]))
 
         if A[n - 1][n - 1] == 0:
-            print('there is no single solution')
+            print("there is no single solution")
             return None
         ecprint(A)
 
         X[n - 1] = A[n - 1][n] / A[n - 1][n - 1]
         for i in list(reversed(range(n - 1))):
             s = 0
             for j in range(i + 1, n):
                 s += A[i][j] * X[j]
             X[i] = (A[i][n] - s) / A[i][i]
-        print('the solution is:')
-        
+        print("the solution is:")
+
         for i in range(n):
-            print(f'X{i} = {round(X[i], pr)}')
-        
-        return X
+            print(f"X{i} = {round(X[i], pr)}")
+
+        return X
```

### Comparing `likelihood-1.1.11/likelihood/regression_models.py` & `likelihood-1.1.12/likelihood/regression_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,469 +1,498 @@
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
+
 from likelihood.main import *
 from likelihood.tools import *
 
-#-------------------------------------------------------------------------
+# -------------------------------------------------------------------------
+
 
 class fourier_regression:
     """A class that implements the arima model with FFT noise filtering
 
     Parameters
     ----------
-    
+
     datapoints : np.array
         A set of points to train the arima model.
-        
+
     n_steps : int
-        Is the number of points that in predict(n_steps) 
+        Is the number of points that in predict(n_steps)
         stage will estimate foward. By default it is set to `0`.
-        
+
     Returns
     -------
-    
+
     new_datapoints : np.array
-        It is the number of predicted points. It is necessary 
+        It is the number of predicted points. It is necessary
         to apply predict(n_steps) followed by fit()
 
     """
 
     def __init__(self, datapoints, n_steps=0):
         self.datapoints_ = datapoints
         self.n_steps = n_steps
 
-    def fit(self, sigma = 0, mov = 200, mode = False):
+    def fit(self, sigma=0, mov=200, mode=False):
         self.sigma = sigma
         self.mode = mode
         self.mov = mov
 
         datapoints = self.datapoints_
         self.datapoints_ = fft_denoise(datapoints, sigma, mode)
 
-    def predict(self, n_steps = 0, n_walkers = 1, name = 'fourier_model', save = True):
-
+    def predict(self, n_steps=0, n_walkers=1, name="fourier_model", save=True):
         self.n_steps = n_steps
         self.n_walkers = n_walkers
         self.name = name
         mov = self.mov
 
-        assert self.n_walkers <= mov, 'n_walkers must be less or equal than mov'
+        assert self.n_walkers <= mov, "n_walkers must be less or equal than mov"
 
         new_datapoints = []
         for i in range(self.datapoints_.shape[0]):
             model_ = regressive_arima(self.datapoints_[i, :])
             model_.train(n_walkers, mov)
             if save:
-                model_.save_model(str(i)+'_'+name)
+                model_.save_model(str(i) + "_" + name)
             y_pred_ = model_.predict(n_steps)
             new_datapoints.append(y_pred_)
-        
+
         new_datapoints = np.array(new_datapoints)
         new_datapoints = np.reshape(new_datapoints, (len(new_datapoints), -1))
-            
+
         return new_datapoints
 
-    def load_predict(self, name = 'fourier_model'):
+    def load_predict(self, name="fourier_model"):
         n_steps = self.n_steps
 
         new_datapoints = []
-    
+
         for i in range(self.datapoints_.shape[0]):
             model_ = regressive_arima(self.datapoints_[i, :])
-            model_.load_model(str(i)+'_'+name)
+            model_.load_model(str(i) + "_" + name)
             y_pred_ = model_.predict(n_steps)
             new_datapoints.append(y_pred_)
-        
+
         new_datapoints = np.array(new_datapoints)
         new_datapoints = np.reshape(new_datapoints, (len(new_datapoints), -1))
-            
+
         return new_datapoints
 
-    def plot_pred(self, y_real, y_pred, ci = 0.90, mode = True):
+    def plot_pred(self, y_real, y_pred, ci=0.90, mode=True):
         plt.figure()
         n = self.n_steps
         y_mean = np.mean(y_pred, axis=0)
         y_std = np.std(y_pred, axis=0)
         ci = ci - 0.68
         if ci < 0.95:
-            Z = (ci/0.90)*1.64
+            Z = (ci / 0.90) * 1.64
         else:
-            Z = (ci/0.95)*1.96
+            Z = (ci / 0.95) * 1.96
 
-        plt.plot(y_pred, label = 'Predicted')
-        plt.plot(y_real, '.--', label = 'Real', alpha = 0.5)
-        plt.fill_between((range(y_pred.shape[0]))[-n:]
-        , (y_pred - Z*y_std)[-n:]
-        , (y_pred + Z*y_std)[-n:], alpha=0.2)
-        plt.xlabel('Time steps')
-        plt.ylabel('y')
+        plt.plot(y_pred, label="Predicted")
+        plt.plot(y_real, ".--", label="Real", alpha=0.5)
+        plt.fill_between(
+            (range(y_pred.shape[0]))[-n:],
+            (y_pred - Z * y_std)[-n:],
+            (y_pred + Z * y_std)[-n:],
+            alpha=0.2,
+        )
+        plt.xlabel("Time steps")
+        plt.ylabel("y")
         plt.legend()
-        print('Confidence Interval: {:.4f}'.format(Z*y_std))
+        print("Confidence Interval: {:.4f}".format(Z * y_std))
         if mode:
-            plt.savefig('pred_'+str(n)+'.png', dpi=300)
+            plt.savefig("pred_" + str(n) + ".png", dpi=300)
         plt.show()
 
+
 class arima:
     """A class that implements the (p, d, q) arima model
-    
+
     Parameters
     ----------
-    
+
     datapoints : np.array
         A set of points to train the arima model.
-        
+
     p : int
         Is the number of auto-regressive terms (ratio). By default it is set to `1`
 
     d : int
         Is known as the degree of differencing. By default it is set to `0`
 
     q : int
         Is the number of forecast errors in the model (ratio). By default it is set to `1`
-        
+
     Returns
     -------
-    
+
     y_pred : np.array
-        It is the number of predicted points. It is necessary 
+        It is the number of predicted points. It is necessary
         to apply predict(n_steps) followed by train()
     """
-    def __init__(self, datapoints, p=1, d=0, q=1, n_steps=0, noise=0, alpha = 0.1):
+
+    def __init__(self, datapoints, p=1, d=0, q=1, n_steps=0, noise=0, alpha=0.1):
         self.datapoints = datapoints
         self.n_steps = n_steps
         self.noise = noise
         self.alpha = alpha
-        self.p = int(p*len(datapoints))
+        self.p = int(p * len(datapoints))
         self.d = d
-        self.q = int(q*len(datapoints))
+        self.q = int(q * len(datapoints))
 
     def forward(self, y_sum, theta, mode, noise):
         if mode:
             y_vec = []
 
             y_t = np.dot(theta, y_sum)
 
             n = y_sum.shape[0]
 
             for i in range(n):
                 try:
                     n_int = np.where(y_sum != y_sum[i])[0]
-                    y_i = (y_t - np.dot(theta[n_int], y_sum[n_int]))/theta[i]
-                    y_i += np.random.rand()*noise
+                    y_i = (y_t - np.dot(theta[n_int], y_sum[n_int])) / theta[i]
+                    y_i += np.random.rand() * noise
                 except:
-                    y_i = (y_t - np.dot(theta[0:i], y_sum[0:i]))/theta[i]
+                    y_i = (y_t - np.dot(theta[0:i], y_sum[0:i])) / theta[i]
                 y_vec.append(y_i)
         else:
             y_t = np.dot(theta, y_sum) + y_sum[0]
             n_int = np.where(y_sum != y_sum[0])[0]
-            y_i = (y_t - np.dot(theta[n_int], y_sum[n_int]))/theta[0]
-            y_i += np.random.rand()*noise
+            y_i = (y_t - np.dot(theta[n_int], y_sum[n_int])) / theta[0]
+            y_i += np.random.rand() * noise
             return y_i
 
         return np.array(y_vec)
 
     def integrated(self, datapoints):
         datapoints = self.datapoints
         n = datapoints.shape[0]
 
-        y_sum = [((1.0-datapoints[i-1]/datapoints[i])**self.d)*datapoints[i] for i in range(1, n)]
+        y_sum = [
+            ((1.0 - datapoints[i - 1] / datapoints[i]) ** self.d) * datapoints[i]
+            for i in range(1, n)
+        ]
         y_sum.insert(0, datapoints[0])
 
         return np.array(y_sum)
 
     def average(self, datapoints):
         y_sum_average = cal_average(datapoints, self.alpha)
-        y_sum_eps = datapoints-y_sum_average
+        y_sum_eps = datapoints - y_sum_average
 
         return y_sum_eps
 
     def abstract_model(self, datapoints, theta, mode=True):
         datapoints = self.datapoints
         noise = self.noise
         self.theta_trained = theta
 
-        phi = theta[0:self.p]
+        phi = theta[0 : self.p]
         if self.d != 0:
             y_sum = self.integrated(datapoints)
         else:
             y_sum = datapoints
 
-        y_sum_regr = y_sum[-self.p:]
+        y_sum_regr = y_sum[-self.p :]
         y_regr_vec = self.forward(y_sum_regr, phi, mode, noise)
         if self.q != 0:
-            y_sum_average = self.average(y_sum[-self.q:])
-            y_average_vec = self.forward(y_sum_average, theta[-self.q:], mode, noise)
+            y_sum_average = self.average(y_sum[-self.q :])
+            y_average_vec = self.forward(y_sum_average, theta[-self.q :], mode, noise)
             check = 0
         else:
             check = None
-        
+
         if check == 0:
             if mode:
                 y_vec = y_regr_vec
                 for i in reversed(range(y_average_vec.shape[0])):
                     y_vec[i] += y_average_vec[i]
             else:
-                y_vec = y_regr_vec+y_average_vec
+                y_vec = y_regr_vec + y_average_vec
         else:
             y_vec = y_regr_vec
-        
-        return y_vec
 
+        return y_vec
 
-    def xvec(self, datapoints, n_steps = 0):
+    def xvec(self, datapoints, n_steps=0):
         datapoints = self.datapoints
         self.n_steps = n_steps
 
         return datapoints[n_steps:]
 
-    def train(self, nwalkers = 1, mov = 200, weights = False):
-
+    def train(self, nwalkers=1, mov=200, weights=False):
         datapoints = self.datapoints
         xvec = self.xvec
-        
+
         self.nwalkers = nwalkers
         self.mov = mov
 
-        assert self.nwalkers <= self.mov, 'n_walkers must be less or equal than mov' 
+        assert self.nwalkers <= self.mov, "n_walkers must be less or equal than mov"
 
         arima_model = self.abstract_model
 
-        n = self.p+self.q
-        
+        n = self.p + self.q
+
         if n == 0:
             n = datapoints.shape[0]
 
         theta = np.random.rand(n)
- 
+
         x_vec = xvec(datapoints)
 
-        if weights: 
-            par, error = walkers(nwalkers, x_vec, datapoints, arima_model,
-                             theta = self.theta_trained, mov = mov, tol = 1e-4, figname = None)
+        if weights:
+            par, error = walkers(
+                nwalkers,
+                x_vec,
+                datapoints,
+                arima_model,
+                theta=self.theta_trained,
+                mov=mov,
+                tol=1e-4,
+                figname=None,
+            )
         else:
-            par, error = walkers(nwalkers, x_vec, datapoints, arima_model,
-                             theta, mov = mov, tol = 1e-4, figname = None)
+            par, error = walkers(
+                nwalkers, x_vec, datapoints, arima_model, theta, mov=mov, tol=1e-4, figname=None
+            )
 
         index = np.where(error == np.min(error))[0][0]
         trained = np.array(par[index])
 
         self.theta_trained = trained
 
-    def predict(self, n_steps = 0):
-
+    def predict(self, n_steps=0):
         self.n_steps = n_steps
 
         datapoints = self.datapoints
         arima_model = self.abstract_model
         theta_trained = self.theta_trained
-        
+
         y_pred = arima_model(datapoints, theta_trained)
-        
+
         for i in range(n_steps):
             self.datapoints = y_pred[i:]
-            y_new = arima_model(datapoints, theta_trained, mode = False)
+            y_new = arima_model(datapoints, theta_trained, mode=False)
             y_pred = y_pred.tolist()
             y_pred.append(y_new)
             y_pred = np.array(y_pred)
-        
+
         return y_pred
-    
-    def save_model(self, name = 'model'):
-        np.savetxt(name+'.txt', self.theta_trained)
-    
-    def load_model(self, name = 'model'):
-        self.theta_trained = np.loadtxt(name+'.txt')
+
+    def save_model(self, name="model"):
+        np.savetxt(name + ".txt", self.theta_trained)
+
+    def load_model(self, name="model"):
+        self.theta_trained = np.loadtxt(name + ".txt")
 
     def eval(self, y_val, y_pred):
-        rmse = np.sqrt(np.mean((y_pred - y_val)**2))
-        square_error = np.sqrt((y_pred - y_val)**2)
+        rmse = np.sqrt(np.mean((y_pred - y_val) ** 2))
+        square_error = np.sqrt((y_pred - y_val) ** 2)
         accuracy = np.sum(square_error[np.where(square_error < rmse)])
         accuracy /= np.sum(square_error)
         print("Accuracy: {:.4f}".format(accuracy))
         print("RMSE: {:.4f}".format(rmse))
 
-    def plot_pred(self, y_real, y_pred, ci = 0.90, mode = True):
+    def plot_pred(self, y_real, y_pred, ci=0.90, mode=True):
         plt.figure()
         n = self.n_steps
         y_mean = np.mean(y_pred, axis=0)
         y_std = np.std(y_pred, axis=0)
         if ci < 0.95:
-            Z = (ci/0.90)*1.64
+            Z = (ci / 0.90) * 1.64
         else:
-            Z = (ci/0.95)*1.96
-    
-        plt.plot(y_pred, label = 'Predicted')
-        plt.plot(y_real, '.--', label = 'Real', alpha = 0.5)
-        plt.fill_between((range(y_pred.shape[0]))[-n:]
-        , (y_pred - Z*y_std)[-n:]
-        , (y_pred + Z*y_std)[-n:], alpha=0.2)
-        plt.xlabel('Time steps')
-        plt.ylabel('y')
+            Z = (ci / 0.95) * 1.96
+
+        plt.plot(y_pred, label="Predicted")
+        plt.plot(y_real, ".--", label="Real", alpha=0.5)
+        plt.fill_between(
+            (range(y_pred.shape[0]))[-n:],
+            (y_pred - Z * y_std)[-n:],
+            (y_pred + Z * y_std)[-n:],
+            alpha=0.2,
+        )
+        plt.xlabel("Time steps")
+        plt.ylabel("y")
         plt.legend()
-        print('Confidence Interval: {:.4f}'.format(Z*y_std))
+        print("Confidence Interval: {:.4f}".format(Z * y_std))
         if mode:
-            plt.savefig('pred_'+str(n)+'.png', dpi=300)
+            plt.savefig("pred_" + str(n) + ".png", dpi=300)
         plt.show()
 
     def summary(self):
-        print('\nSummary:')
-        print('--------')
-        print('\nLenght of theta: {}'.format(len(self.theta_trained)))
-        print('\nMean of theta: {:.4f}'.format(np.mean(self.theta_trained)))
-        print('------------------------------------------------------------------')
+        print("\nSummary:")
+        print("--------")
+        print("\nLenght of theta: {}".format(len(self.theta_trained)))
+        print("\nMean of theta: {:.4f}".format(np.mean(self.theta_trained)))
+        print("------------------------------------------------------------------")
 
 
-class regressive_arima: 
+class regressive_arima:
     """A class that implements the auto-regressive arima (1, 0, 0) model
-    
+
     Parameters
     ----------
-    
+
     datapoints : np.array
         A set of points to train the arima model.
-        
+
     n_steps : int
-        Is the number of points that in predict(n_steps) 
+        Is the number of points that in predict(n_steps)
         stage will estimate foward. By default it is set to `0`.
-        
+
     Returns
     -------
-    
+
     y_pred : np.array
-        It is the number of predicted points. It is necessary 
+        It is the number of predicted points. It is necessary
         to apply predict(n_steps) followed by train()
     """
+
     def __init__(self, datapoints, n_steps=0, noise=0):
         self.datapoints = datapoints
         self.n_steps = n_steps
         self.noise = noise
 
     def arima_model(self, datapoints, theta, mode=True):
         datapoints = self.datapoints
         noise = self.noise
         self.theta_trained = theta
 
         if mode:
             y_vec = []
 
-            y_sum = datapoints 
+            y_sum = datapoints
             y_t = np.dot(theta, y_sum)
 
             n = y_sum.shape[0]
 
             for i in range(n):
                 try:
                     n_int = np.where(y_sum != y_sum[i])[0]
-                    y_i = (y_t - np.dot(theta[n_int], y_sum[n_int]))/theta[i]
-                    y_i += np.random.rand()*noise
+                    y_i = (y_t - np.dot(theta[n_int], y_sum[n_int])) / theta[i]
+                    y_i += np.random.rand() * noise
                 except:
-                    y_i = (y_t - np.dot(theta[0:i], y_sum[0:i]))/theta[i]
+                    y_i = (y_t - np.dot(theta[0:i], y_sum[0:i])) / theta[i]
                 y_vec.append(y_i)
         else:
             y_sum = datapoints
             y_t = np.dot(theta, y_sum) + y_sum[0]
             n_int = np.where(y_sum != y_sum[0])[0]
-            y_i = (y_t - np.dot(theta[n_int], y_sum[n_int]))/theta[0]
-            y_i += np.random.rand()*noise
+            y_i = (y_t - np.dot(theta[n_int], y_sum[n_int])) / theta[0]
+            y_i += np.random.rand() * noise
             return y_i
 
         return np.array(y_vec)
 
-    def xvec(self, datapoints, n_steps = 0):
+    def xvec(self, datapoints, n_steps=0):
         datapoints = self.datapoints
         self.n_steps = n_steps
 
         return datapoints[n_steps:]
 
-    def train(self, nwalkers = 1, mov = 200, weights = False):
-
+    def train(self, nwalkers=1, mov=200, weights=False):
         datapoints = self.datapoints
         xvec = self.xvec
-        
+
         self.nwalkers = nwalkers
         self.mov = mov
 
-        assert self.nwalkers <= self.mov, 'n_walkers must be less or equal than mov' 
+        assert self.nwalkers <= self.mov, "n_walkers must be less or equal than mov"
 
         arima_model = self.arima_model
 
         n = datapoints.shape[0]
 
         theta = np.random.rand(n)
-        
+
         x_vec = xvec(datapoints)
-        
-        if weights: 
-            par, error = walkers(nwalkers, x_vec, datapoints, arima_model,
-                             theta = self.theta_trained, mov = mov, tol = 1e-4, figname = None)
+
+        if weights:
+            par, error = walkers(
+                nwalkers,
+                x_vec,
+                datapoints,
+                arima_model,
+                theta=self.theta_trained,
+                mov=mov,
+                tol=1e-4,
+                figname=None,
+            )
         else:
-            par, error = walkers(nwalkers, x_vec, datapoints, arima_model,
-                             theta, mov = mov, tol = 1e-4, figname = None)
+            par, error = walkers(
+                nwalkers, x_vec, datapoints, arima_model, theta, mov=mov, tol=1e-4, figname=None
+            )
 
         index = np.where(error == np.min(error))[0][0]
         trained = np.array(par[index])
 
         self.theta_trained = trained
 
-    def predict(self, n_steps = 0):
-
+    def predict(self, n_steps=0):
         self.n_steps = n_steps
 
         datapoints = self.datapoints
         arima_model = self.arima_model
         theta_trained = self.theta_trained
 
         y_pred = arima_model(datapoints, theta_trained)
 
         for i in range(n_steps):
             self.datapoints = y_pred[i:]
 
-            y_new = arima_model(datapoints, theta_trained, mode = False)
+            y_new = arima_model(datapoints, theta_trained, mode=False)
             y_pred = y_pred.tolist()
             y_pred.append(y_new)
             y_pred = np.array(y_pred)
-            
+
         return np.array(y_pred)
-    
-    def save_model(self, name = 'model'):
-        np.savetxt(name+'.txt', self.theta_trained)
-    
-    def load_model(self, name = 'model'):
-        self.theta_trained = np.loadtxt(name+'.txt')
+
+    def save_model(self, name="model"):
+        np.savetxt(name + ".txt", self.theta_trained)
+
+    def load_model(self, name="model"):
+        self.theta_trained = np.loadtxt(name + ".txt")
 
     def eval(self, y_val, y_pred):
-        rmse = np.sqrt(np.mean((y_pred - y_val)**2))
-        square_error = np.sqrt((y_pred - y_val)**2)
+        rmse = np.sqrt(np.mean((y_pred - y_val) ** 2))
+        square_error = np.sqrt((y_pred - y_val) ** 2)
         accuracy = np.sum(square_error[np.where(square_error < rmse)])
         accuracy /= np.sum(square_error)
         print("Accuracy: {:.4f}".format(accuracy))
         print("RMSE: {:.4f}".format(rmse))
 
-    def plot_pred(self, y_real, y_pred, ci = 0.90, mode = True):
+    def plot_pred(self, y_real, y_pred, ci=0.90, mode=True):
         plt.figure()
         n = self.n_steps
         y_mean = np.mean(y_pred, axis=0)
         y_std = np.std(y_pred, axis=0)
         if ci < 0.95:
-            Z = (ci/0.90)*1.64
+            Z = (ci / 0.90) * 1.64
         else:
-            Z = (ci/0.95)*1.96
-    
-        plt.plot(y_pred, label = 'Predicted')
-        plt.plot(y_real, '.--', label = 'Real', alpha = 0.5)
-        plt.fill_between((range(y_pred.shape[0]))[-n:]
-        , (y_pred - Z*y_std)[-n:]
-        , (y_pred + Z*y_std)[-n:], alpha=0.2)
-        plt.xlabel('Time steps')
-        plt.ylabel('y')
+            Z = (ci / 0.95) * 1.96
+
+        plt.plot(y_pred, label="Predicted")
+        plt.plot(y_real, ".--", label="Real", alpha=0.5)
+        plt.fill_between(
+            (range(y_pred.shape[0]))[-n:],
+            (y_pred - Z * y_std)[-n:],
+            (y_pred + Z * y_std)[-n:],
+            alpha=0.2,
+        )
+        plt.xlabel("Time steps")
+        plt.ylabel("y")
         plt.legend()
-        print('Confidence Interval: {:.4f}'.format(Z*y_std))
+        print("Confidence Interval: {:.4f}".format(Z * y_std))
         if mode:
-            plt.savefig('pred_'+str(n)+'.png', dpi=300)
+            plt.savefig("pred_" + str(n) + ".png", dpi=300)
         plt.show()
 
     def summary(self):
-        print('\nSummary:')
-        print('--------')
-        print('\nLenght of theta: {}'.format(len(self.theta_trained)))
-        print('\nMean of theta: {:.4f}'.format(np.mean(self.theta_trained)))
-        print('------------------------------------------------------------------')
+        print("\nSummary:")
+        print("--------")
+        print("\nLenght of theta: {}".format(len(self.theta_trained)))
+        print("\nMean of theta: {:.4f}".format(np.mean(self.theta_trained)))
+        print("------------------------------------------------------------------")
```

### Comparing `likelihood-1.1.11/likelihood/tools.py` & `likelihood-1.1.12/likelihood/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,579 +1,644 @@
-import numpy as np
+from typing import List, Tuple
+
 import matplotlib.pyplot as plt
+import numpy as np
+from pandas.core.frame import DataFrame
 
-#-------------------------------------------------------------------------
+# -------------------------------------------------------------------------
 
 """
 Data Science from Scratch, Second Edition, by Joel Grus (O'Reilly).Copyright 2019 Joel Grus, 978-1-492-04113-9
 """
 
 
-def minibatches(dataset, batch_size, shuffle = True):
-
+def minibatches(dataset, batch_size, shuffle=True):
     """Generates 'batch_size'-sized minibatches from the dataset
-    
+
     Parameters
     ----------
     dataset : List
     batch_size : int
     shuffle : bool
-    
+
     """
-    
+
     # start indexes 0, batch_size, 2 * batch_size, ...
     batch_starts = [start for start in range(0, len(dataset), batch_size)]
-    
-    if shuffle: np.random.shuffle(batch_starts)  # shuffle the batches
-            
+
+    if shuffle:
+        np.random.shuffle(batch_starts)  # shuffle the batches
+
     for start in batch_starts:
         end = start + batch_size
         yield dataset[start:end]
-      
-        
+
+
 def difference_quotient(f, x, h):
-    
     """Calculates the difference quotient of 'f' evaluated at x and x + h
-    
+
     Parameters
     ----------
     f(x) : Callable function
     x : float
     h : float
-    
+
     Returns
     -------
     '(f(x + h) - f(x)) / h'
-    
+
     """
-    
+
     return (f(x + h) - f(x)) / h
 
 
 def partial_difference_quotient(f, v, i, h):
-    
     """Calculates the partial difference quotient of 'f'
-    
+
     Parameters
     ----------
     f(x0,...,xi-th) : Callable function
     v : Vector or np.array
     h : float
-    
+
     Returns
     -------
     the i-th partial difference quotient of f at v
-    
+
     """
-    
-    w = [v_j + (h if j == i else 0)  # add h to just the ith element of v
-         for j, v_j in enumerate(v)]
+
+    w = [
+        v_j + (h if j == i else 0) for j, v_j in enumerate(v)  # add h to just the ith element of v
+    ]
     return (f(w) - f(v)) / h
 
 
-def estimate_gradient(f, v, h = 0.0001):
+def estimate_gradient(f, v, h=0.0001):
     """Calculates the gradient of 'f' at v
-    
+
     Parameters
     ----------
     f(x0,...,xi-th) : Callable function
     v : Vector or np.array
     h : float. By default it is set to 0.0001
-    
+
     """
-    return [partial_difference_quotient(f, v, i, h)
-            for i in range(len(v))]
+    return [partial_difference_quotient(f, v, i, h) for i in range(len(v))]
+
+
+# -------------------------------------------------------------------------
 
-#-------------------------------------------------------------------------
 
 # a function that calculates the percentage of missing values per column is defined
 def cal_missing_values(df):
     col = df.columns
-    print('Total size : ', "{:,}".format(len(df)))
+    print("Total size : ", "{:,}".format(len(df)))
     for i in col:
-        print(str(i)+' : 'f"{(df.isnull().sum()[i]/(df.isnull().sum()[i]+df[i].count()))*100:.2f}%")
+        print(
+            str(i) + " : " f"{(df.isnull().sum()[i]/(df.isnull().sum()[i]+df[i].count()))*100:.2f}%"
+        )
 
-def calculate_probability(x, points = 1, cond = True):
+
+def calculate_probability(x, points=1, cond=True):
     """Calculates the probability of the data
-    
+
     Parameters
     ----------
     x : np.array
         An array containing the data.
     points : int
         An integer value. By default it is set to `1`.
     cond : bool
         A boolean value. By default it is set to `True`.
-    
+
     Returns
     -------
     p : np.array
         An array containing the probability of the data.
-    
+
     """
-    
+
     p = []
 
     f = cdf(x)[0]
     for i in range(len(x)):
         p.append(f(x[i]))
     p = np.array(p)
     if cond:
-        if(np.prod(p[-points]) > 1):
-            print('\nThe probability of the data cannot be calculated.\n')
+        if np.prod(p[-points]) > 1:
+            print("\nThe probability of the data cannot be calculated.\n")
         else:
-            if(np.prod(p[-points]) < 0):
-                print('\nThe probability of the data cannot be calculated.\n')
+            if np.prod(p[-points]) < 0:
+                print("\nThe probability of the data cannot be calculated.\n")
             else:
-                print('The model has a probability of {:.2f}% of being correct'.format(np.prod(p[-points])*100))
+                print(
+                    "The model has a probability of {:.2f}% of being correct".format(
+                        np.prod(p[-points]) * 100
+                    )
+                )
     else:
-        if(np.sum(p[-points]) < 0):
-            print('\nThe probability of the data cannot be calculated.\n')
+        if np.sum(p[-points]) < 0:
+            print("\nThe probability of the data cannot be calculated.\n")
         else:
-            if(np.sum(p[-points]) > 1):
-                print('\nThe probability of the data cannot be calculated.\n')
+            if np.sum(p[-points]) > 1:
+                print("\nThe probability of the data cannot be calculated.\n")
             else:
-                print('The model has a probability of {:.2f}% of being correct'.format(np.sum(p[-points])*100))
+                print(
+                    "The model has a probability of {:.2f}% of being correct".format(
+                        np.sum(p[-points]) * 100
+                    )
+                )
     return p
 
-def cdf(x, poly = 9, inv = False, plot = False, savename = None):
+
+def cdf(x, poly=9, inv=False, plot=False, savename=None):
     """Calculates the cumulative distribution function of the data
 
     Parameters
     ----------
     x : np.array
         An array containing the data.
     poly : int
         An integer value. By default it is set to `9`.
     inv : bool
         A boolean value. By default it is set to `False`.
-    
+
     Returns
     -------
     cdf_ : np.array
         An array containing the cumulative distribution function.
-    
+
     """
-    
+
     cdf_ = np.cumsum(x) / np.sum(x)
 
     ox = np.sort(x)
     I = np.ones(len(ox))
     M = np.triu(I)
     df = np.dot(ox, M)
-    df_ = df/np.max(df)
+    df_ = df / np.max(df)
 
     if inv:
         fit = np.polyfit(df_, ox, poly)
         f = np.poly1d(fit)
     else:
         fit = np.polyfit(ox, df_, poly)
         f = np.poly1d(fit)
-    
+
     if plot:
         if inv:
-            plt.plot(df_, ox, 'o', label = 'inv cdf')
-            plt.plot(df_, f(df_), 'r--', label = 'fit')
-            plt.title('Quantile Function')
+            plt.plot(df_, ox, "o", label="inv cdf")
+            plt.plot(df_, f(df_), "r--", label="fit")
+            plt.title("Quantile Function")
             plt.xlabel("Probability")
             plt.ylabel("Value")
             plt.legend()
             if savename != None:
-                plt.savefig(savename, dpi = 300)
+                plt.savefig(savename, dpi=300)
             plt.show()
         else:
-            plt.plot(ox, cdf_, 'o', label = 'cdf')
-            plt.plot(ox, f(ox), 'r--', label = 'fit')
-            plt.title('Cumulative Distribution Function')
+            plt.plot(ox, cdf_, "o", label="cdf")
+            plt.plot(ox, f(ox), "r--", label="fit")
+            plt.title("Cumulative Distribution Function")
             plt.xlabel("Value")
             plt.ylabel("Probability")
             plt.legend()
             if savename != None:
-                plt.savefig(savename, dpi = 300)
+                plt.savefig(savename, dpi=300)
             plt.show()
 
     return f, cdf_, ox
 
-class corr():
+
+class corr:
     """Calculates the correlation of the data
-    
+
     Parameters
     ----------
     x : np.array
         An array containing the data.
     y : np.array
         An array containing the data.
-    
+
     Returns
     -------
     z : np.array
         An array containing the correlation of x and y.
-    
+
     """
-    
+
     def __init__(self, x, y):
         self.x = x
         self.y = y
-        self.result = np.correlate(x, y, mode='full')
-        self.z = self.result[self.result.size//2:]
-        self.z = self.z/float(np.abs(self.z).max())
-    
+        self.result = np.correlate(x, y, mode="full")
+        self.z = self.result[self.result.size // 2 :]
+        self.z = self.z / float(np.abs(self.z).max())
+
     def plot(self):
-        plt.plot(range(len(self.z)), self.z, label = 'Correlation')
+        plt.plot(range(len(self.z)), self.z, label="Correlation")
         plt.legend()
         plt.show()
-    
+
     def __call__(self):
         return self.z
 
-class autocorr():
+
+class autocorr:
     """Calculates the autocorrelation of the data
-    
+
     Parameters
     ----------
     x : np.array
         An array containing the data.
-    
+
     Returns
     -------
     z : np.array
         An array containing the autocorrelation of the data.
-    
+
     """
-    
+
     def __init__(self, x):
         self.x = x
-        self.result = np.correlate(x, x, mode='full')
-        self.z = self.result[self.result.size//2:]
-        self.z = self.z/float(np.abs(self.z).max())
-    
+        self.result = np.correlate(x, x, mode="full")
+        self.z = self.result[self.result.size // 2 :]
+        self.z = self.z / float(np.abs(self.z).max())
+
     def plot(self):
-        plt.plot(range(len(self.z)), self.z, label = 'Autocorrelation')
+        plt.plot(range(len(self.z)), self.z, label="Autocorrelation")
         plt.legend()
         plt.show()
-    
+
     def __call__(self):
         return self.z
 
-def fft_denoise(dataset, sigma = 0, mode = True):
+
+def fft_denoise(dataset, sigma=0, mode=True):
     """Performs the noise removal using the Fast Fourier Transform
-    
+
     Parameters
     ----------
     dataset : np.array
         An array containing the noised data.
     sigma : float
         A float between 0 and 1. By default it is set to `0`.
     mode : bool
         A boolean value. By default it is set to `True`.
-    
+
     Returns
     -------
     dataset : np.array
         An array containing the denoised data.
-    
+
     """
     dataset_ = dataset.copy()
     for i in range(dataset.shape[0]):
         n = dataset.shape[1]
         fhat = np.fft.fft(dataset[i, :], n)
-        freq = (1/n) * np.arange(n)         
-        L = np.arange(1,np.floor(n/2),dtype='int')
+        freq = (1 / n) * np.arange(n)
+        L = np.arange(1, np.floor(n / 2), dtype="int")
         PSD = fhat * np.conj(fhat) / n
         indices = PSD > np.mean(PSD) + sigma * np.std(PSD)
         PSDclean = PSD * indices  # Zero out all others
-        fhat = indices * fhat   
-        ffilt = np.fft.ifft(fhat) # Inverse FFT for filtered time signal
+        fhat = indices * fhat
+        ffilt = np.fft.ifft(fhat)  # Inverse FFT for filtered time signal
         dataset_[i, :] = ffilt.real
         # Calculate the period of the signal
         period = 1 / freq[L][np.argmax(fhat[L])]
         if mode:
-            print(f'The {i+1}-th row of the dataset has been denoised.')
-            print(f'The period is {round(period, 4)}')
+            print(f"The {i+1}-th row of the dataset has been denoised.")
+            print(f"The period is {round(period, 4)}")
     return dataset_
 
 
-def feature_importance(dataset, values):
-    """Calculates the importance of each feature
-    
-    Parameters
-    ----------
-    dataset : np.array
-        An array containing the scaled data.
-    values : np.ndarray
-        A set of values returned by the linear function.
-    
-    Returns
-    -------
-    importance : np.array
-        An array containing the importance of each feature.
-    
-    """
-    
-    importance = []
-    print('\nFeature importance:')
-    U, S, VT = np.linalg.svd(dataset, full_matrices=False)
-    w = (VT.T@np.linalg.inv(np.diag(S))@U.T).T@values
+class linear_regression:
 
-    for i in range(dataset.shape[0]):
-        a = np.around(w[i], decimals=4)
-        importance.append(a)
-        print(f'The importance of the {i+1} feature is {a}')
-    return np.array(importance)
+    """class implementing multiple linear regression"""
+
+    def __init__(self) -> None:
+        """
+        The class initializer
+
+        """
+        self.importance = []
+
+    def fit(self, dataset: np.ndarray, values: np.ndarray) -> None:
+        """Performs linear multiple model training
+
+        Parameters
+        ----------
+        dataset : np.array
+            An array containing the scaled data.
+        values : np.ndarray
+            A set of values returned by the linear function.
+
+        Returns
+        -------
+        importance : np.array
+            An array containing the importance of each feature.
+
+        """
+
+        self.X = dataset
+        self.y = values
+
+        U, S, VT = np.linalg.svd(self.X, full_matrices=False)
+        w = (VT.T @ np.linalg.inv(np.diag(S)) @ U.T).T @ self.y
+
+        for i in range(self.X.shape[0]):
+            a = np.around(w[i], decimals=8)
+            self.importance.append(a)
+
+        print("\nSummary:")
+        print("--------")
+        print("\nParameters:", np.array(self.importance).shape)
+        print("RMSE: {:.4f}".format(mean_square_error(self.y, self.predict(self.X))))
+
+    def predict(self, datapoints) -> np.ndarray:
+        """
+        Performs predictions for a set of points
+
+        Parameters
+        ----------
+        datapoints : np.array
+            An array containing the values of the independent variable.
+
+        """
+        return np.array(self.importance) @ datapoints
+
+    def get_importances(self, print_important_features: bool = False) -> np.ndarray:
+        """
+        Returns the important features
 
-def cal_average(y, alpha = 1):
+        Parameters
+        ----------
+        print_important_features : bool
+            determines whether or not are printed on the screen. By default it is set to `False`.
+
+        Returns
+        -------
+        importance : np.array
+            An array containing the importance of each feature.
+
+
+        """
+        if print_important_features:
+            for i, a in enumerate(self.importance):
+                print(f"The importance of the {i+1} feature is {a}")
+        return np.array(self.importance)
+
+
+def cal_average(y, alpha=1):
     """Calculates the moving average of the data
-    
+
     Parameters
     ----------
     y : np.array
         An array containing the data.
     alpha : float
         A float between 0 and 1. By default it is set to `1`.
-    
+
     Returns
     -------
     average : float
         The average of the data.
-    
+
     """
-    
+
     n = int(alpha * len(y))
     w = np.ones(n) / n
-    average = np.convolve(y, w, mode='same') / np.convolve(np.ones_like(y), w, mode='same')
+    average = np.convolve(y, w, mode="same") / np.convolve(np.ones_like(y), w, mode="same")
     return average
 
-def rescale(dataset, n=1):
-    """Perform a standard rescaling of the data
-    
-    Parameters
-    ----------
-    dataset : np.array
-        An array containing the model data.
-    n : int
-        Is the degree of the polynomial to subtract 
-        the slope. By default it is set to `1`.
-        
-    Returns
-    -------
-    data_scaled : np.array
-        An array containing the scaled data.
-        
-    mu : np.array
-        An array containing the min of the 
-        original data.
-    sigma : np.array
-        An array containing the (max - min) 
-        of the original data.
-    """
-    
-    mu = []
-    sigma = []
-    fitting = []
-    dataset_ = dataset.copy()
-    try:
-        xaxis = range(dataset.shape[1])
-    except:
-        error_type = 'IndexError'
-        msg = 'Trying to access an item at an invalid index.'
-        print(f'{error_type}: {msg}')
-        return None
-    for i in range(dataset.shape[0]):
-        if n != None:
-            fit = np.polyfit(xaxis, dataset[i, :], n)
-            f = np.poly1d(fit)
-            poly = f(xaxis)
-            fitting.append(f)
-        else:
-            fitting.append(0.0)
-        dataset_[i, :] += -poly
-        mu.append(np.min(dataset_[i, :]))
-        if np.max(dataset_[i, :]) != 0: 
-            sigma.append(np.max(dataset_[i, :])-mu[i])
-        else:
-            sigma.append(1)
-            
-        dataset_[i, :] = 2*((dataset_[i, :] - mu[i]) / sigma[i])-1
-         
-    values = [mu, sigma, fitting]
-    
-    return dataset_, values
-
-def scale(dataset, values):
-    """Performs the inverse operation to the rescale function
-    
-    Parameters
-    ----------
-    dataset : np.array
-        An array containing the scaled data.
-    values : np.ndarray
-        A set of values returned by the rescale function.
-    
-    """
-    dataset_ = dataset.copy()
-    for i in range(dataset.shape[0]):
-        dataset_[i, :] += 1
-        dataset_[i, :] /= 2
-        dataset_[i, :] = dataset_[i, :]*values[1][i]
-        dataset_[i, :] += values[0][i]
-        dataset_[i, :] += values[2][i](range(dataset_.shape[1]))
-    
-    return dataset_
 
-def generate_series(n, n_steps, incline = True):
-    """Function that generates $n$ series of length $n_steps$
-    """
+class DataScaler:
+    """numpy array scaler and rescaler"""
+
+    def __init__(self, dataset: np.ndarray, n: int = 1) -> None:
+        """Initializes the parameters required for scaling the data"""
+        self.dataset_ = dataset.copy()
+        self._n = n
+
+    def rescale(self) -> np.ndarray:
+        """Perform a standard rescaling of the data
+
+        Returns
+        -------
+        data_scaled : np.array
+            An array containing the scaled data.
+        """
+
+        mu = []
+        sigma = []
+        fitting = []
+        self.data_scaled = np.copy(self.dataset_)
+        try:
+            xaxis = range(self.dataset_.shape[1])
+        except:
+            error_type = "IndexError"
+            msg = "Trying to access an item at an invalid index."
+            print(f"{error_type}: {msg}")
+            return None
+        for i in range(self.dataset_.shape[0]):
+            if self._n != None:
+                fit = np.polyfit(xaxis, self.dataset_[i, :], self._n)
+                f = np.poly1d(fit)
+                poly = f(xaxis)
+                fitting.append(f)
+            else:
+                fitting.append(0.0)
+            self.data_scaled[i, :] += -poly
+            mu.append(np.min(self.data_scaled[i, :]))
+            if np.max(self.data_scaled[i, :]) != 0:
+                sigma.append(np.max(self.data_scaled[i, :]) - mu[i])
+            else:
+                sigma.append(1)
+
+            self.data_scaled[i, :] = 2 * ((self.data_scaled[i, :] - mu[i]) / sigma[i]) - 1
+
+        self.values = [mu, sigma, fitting]
+
+        return self.data_scaled
+
+    def scale(self, dataset_) -> np.ndarray:
+        """Performs the inverse operation to the rescale function
+
+        Parameters
+        ----------
+        dataset_ : np.array
+            An array containing the scaled values.
+
+        Returns
+        -------
+        dataset_ : np.array
+            An array containing the rescaled data.
+        """
+        for i in range(dataset_.shape[0]):
+            dataset_[i, :] += 1
+            dataset_[i, :] /= 2
+            dataset_[i, :] = dataset_[i, :] * self.values[1][i]
+            dataset_[i, :] += self.values[0][i]
+            dataset_[i, :] += self.values[2][i](range(dataset_.shape[1]))
+
+        return dataset_
+
+
+def generate_series(n, n_steps, incline=True):
+    """Function that generates $n$ series of length $n_steps$"""
     freq1, freq2, offsets1, offsets2 = np.random.rand(4, n, 1)
-    
-    if incline :
+
+    if incline:
         slope = np.random.rand(n, 1)
-    else: 
+    else:
         slope = 0.0
         offsets2 = 1
-        
+
     time = np.linspace(0, 1, n_steps)
-    series = 0.5 * np.sin((time - offsets1) * (freq1 * 10 + 10)) # wave 1
-    series += 0.2 * np.sin((time - offsets2) * (freq2 * 20 + 20)) # + wave 2
-    series += 0.7 * (np.random.rand(n, n_steps) - 0.5) # + noise
-    series += 5 * slope * time + 2 * (offsets2-offsets1) * time ** (1-offsets2)
+    series = 0.5 * np.sin((time - offsets1) * (freq1 * 10 + 10))  # wave 1
+    series += 0.2 * np.sin((time - offsets2) * (freq2 * 20 + 20))  # + wave 2
+    series += 0.7 * (np.random.rand(n, n_steps) - 0.5)  # + noise
+    series += 5 * slope * time + 2 * (offsets2 - offsets1) * time ** (1 - offsets2)
     series = series
     return series.astype(np.float32)
 
-def RMSE(y_true, y_pred):
+
+def mean_square_error(y_true, y_pred, print_error=False):
     """Calculates the Root Mean Squared Error
-    
+
     Parameters
     ----------
     y_true : np.array
         An array containing the true values.
     y_pred : np.array
         An array containing the predicted values.
-    
+
     Returns
     -------
     RMSE : float
         The Root Mean Squared Error.
-    
-    """
 
-    print(f'The RMSE is {np.sqrt(np.mean((y_true - y_pred)**2))}')
-
-    return np.sqrt(np.mean((y_true - y_pred)**2))
-
-def to_codes_transformation(x, dict_type):
-    """Auxiliary function to perform data transformation using a dictionary
-
-    Parameters
-    ----------
-    x : str 
-        A character data type.
-    dict_type : dict
-        An object of dictionary type.
-
-    Returns
-    -------
-    dict_type[x] or np.nan if dict_type[x] doesn't exist.
     """
-    try:
-        return dict_type[x]
-    except:
-        return np.nan
+    if print_error:
+        print(f"The RMSE is {np.sqrt(np.mean((y_true - y_pred)**2))}")
 
-def data_codification(data):
-    """Function that allows us to perform the encoding and obtain the dictionaries.
+    return np.sqrt(np.mean((y_true - y_pred) ** 2))
 
-    Parameters
-    ----------
-    data : pd.DataFrame()
-        An object of type pandas dataframe.
 
-    Returns
-    -------
-    df : pd.DataFrame()
-        The encoded input dataframe.
+class DataFrameEncoder:
+    """Allows encoding and decoding Dataframes"""
 
-    decode_dicts : dict
-        An object of dictionary type to decodes.
+    def __init__(self, data: DataFrame) -> None:
+        """Sets the columns of the dataframe"""
+        self._df = data.copy()
+        self._names = data.columns
+        self.encoding_list = []
+
+    def encode(self) -> DataFrame:
+        """Encodes the object type columns of the dataframe"""
+        self.decoding_list = []
+        for i in self._names:
+            if self._df[i].dtype == "object":
+                column_index = range(len(self._df[i].unique()))
+                column_keys = self._df[i].unique()
+                encode_dict = dict(zip(column_keys, column_index))
+                decode_dict = dict(zip(column_index, column_keys))
+                self._df[i] = self._df[i].apply(
+                    self._code_transformation_to, dictionary_list=encode_dict
+                )
+                self.encoding_list.append(encode_dict)
+                self.decoding_list.append(decode_dict)
+        return self._df
+
+    def decode(self) -> DataFrame:
+        """Decodes the int type columns of the dataframe"""
+        j = 0
+        df_decoded = self._df.copy()
+        try:
+            number_of_columns = len(self.decoding_list[j])
+            for i in self._names:
+                if df_decoded[i].dtype == "int64":
+                    df_decoded[i] = df_decoded[i].apply(
+                        self._code_transformation_to, dictionary_list=self.decoding_list[j]
+                    )
+                    j += 1
+            return df_decoded
+        except AttributeError as e:
+            warning_type = "UserWarning"
+            msg = "It is not possible to decode the dataframe, since it has not been encoded"
+            msg += "Error: {%s}" % e
+            print(f"{warning_type}: {msg}")
+
+    def get_dictionaries(self) -> Tuple[List[dict], List[dict]]:
+        """Allows to return the list of dictionaries for encoding and decoding"""
+        try:
+            return self.encoding_list, self.decoding_list
+        except ValueError as e:
+            warning_type = "UserWarning"
+            msg = "It is not possible to return the list of dictionaries as they have not been created."
+            msg += "Error: {%s}" % e
+            print(f"{warning_type}: {msg}")
+
+    def _code_transformation_to(self, character: str, dictionary_list: List[dict]) -> int:
+        """Auxiliary function to perform data transformation using a dictionary
+
+        Parameters
+        ----------
+        character : str
+            A character data type.
+        dictionary_list : List[dict]
+            An object of dictionary type.
+
+        Returns
+        -------
+        dict_type[character] or np.nan if dict_type[character] doesn't exist.
+        """
+        try:
+            return dictionary_list[character]
+        except:
+            return np.nan
 
-    code_dicts : dict
-        An object of dictionary type to encodes.
-    """
-    df = data.copy()
-    names = data.columns
-    code_dicts = []
-    decode_dicts = []
-    for i in names:
-        if df[i].dtype == 'object':
-            index_of_name = range(len(df[i].unique()))
-            keys_of_name = df[i].unique()
-            code_dict = dict(zip(keys_of_name, index_of_name))
-            decode_dict = dict(zip(index_of_name, keys_of_name))
-            df[i] = df[i].apply(to_codes_transformation, dict_type=code_dict)
-            decode_dicts.append(decode_dict)
-            code_dicts.append(code_dict)
-    return df, decode_dicts, code_dicts
-
-def data_codeOrdecode(data, dict_types, d_type = 'decode'):
-    """Function that encodes or decodes according to a dictionary
 
-    Parameters
-    ----------
-    data : pd.DataFrame()
-        An object of type pandas dataframe.
-
-    dict_types : dict
-        An object of dictionary type to decodes or encodes.
-
-    Returns
-    -------
-    
-    df : pd.DataFrame()
-        The encoded or decoded input dataframe.
-    """
-    j = 0
-    df = data.copy()
-    names = df.columns
-    for i in names:
-        if d_type == 'decode':
-            if df[i].dtype == 'int64':
-                df[i] = df[i].apply(to_codes_transformation, dict_type=dict_types[j])
-                j += 1
-        else:
-            if df[i].dtype == 'object':
-                df[i] = df[i].apply(to_codes_transformation, dict_type=dict_types[j])
-                j += 1
-    return df
-
-#-------------------------------------------------------------------------
-if __name__ == '__main__':
+# -------------------------------------------------------------------------
+if __name__ == "__main__":
     # Generate data
     x = np.random.rand(3, 100)
-    y = 0.1*x[0, :] + 0.4*x[1, :] + 0.5*x[2, :]
-    importance = feature_importance(x, y)
+    y = 0.1 * x[0, :] + 0.4 * x[1, :] + 0.5 * x[2, :] + 0.1
+    linear_model = linear_regression()
+    linear_model.fit(x, y)
+    importance = linear_model.get_importances()
+    y_hat = linear_model.predict(x)
+
+    # Graph the data for visualization
+    plt.plot(x[0, :], y, "o", label="Original Data")
+    plt.plot(x[0, :], y_hat, "x", label="$\hat{y}$")
+    plt.legend()
+    plt.xlabel("$x$")
+    plt.ylabel("$y, $\hat{y}$")
+    plt.show()
 
     a = generate_series(1, 40, incline=False)
     # Graph the data for visualization
-    plt.plot(range(len(a[0, :])), a[0, :], label = 'Original Data')
+    plt.plot(range(len(a[0, :])), a[0, :], label="Original Data")
     plt.legend()
-    plt.xlabel('Time periods')
-    plt.ylabel('$y(t)$')
+    plt.xlabel("Time periods")
+    plt.ylabel("$y(t)$")
     plt.show()
 
     a_denoise = fft_denoise(a)
-    
-    plt.plot(range(len(a_denoise[0, :])), a_denoise[0, :], label = 'Denoise Data')
+
+    plt.plot(range(len(a_denoise[0, :])), a_denoise[0, :], label="Denoise Data")
     plt.legend()
-    plt.xlabel('Time periods')
-    plt.ylabel('$y(t)$')
+    plt.xlabel("Time periods")
+    plt.ylabel("$y(t)$")
     plt.show()
 
     # Calculate the autocorrelation of the data
     z = autocorr(a[0, :])
     z.plot()
-    #print(z())
+    # print(z())
 
     N = 1000
     mu = np.random.uniform(0, 10.0)
     sigma = np.random.uniform(0.1, 1.0)
     x = np.random.normal(mu, sigma, N)
-    f, cdf_, ox = cdf(x, plot = True)
-    invf, cdf_, ox = cdf(x, plot = True, inv = True)
+    f, cdf_, ox = cdf(x, plot=True)
+    invf, cdf_, ox = cdf(x, plot=True, inv=True)
```

### Comparing `likelihood-1.1.11/setup.py` & `likelihood-1.1.12/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="likelihood", # Replace with your own username
-    version="1.1.11",
+    version="1.1.12",
     author="J. A. Moreno-Guerra",
     author_email="jzs.gm27@gmail.com",
     description="A package that performs the maximum likelihood algorithm.",
     py_modules=["likelihood"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jzsmoreno/likelihood/",
```

