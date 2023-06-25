# Comparing `tmp/balrogo-1.6.5.tar.gz` & `tmp/balrogo-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balrogo-1.6.5.tar", max compression
+gzip compressed data, was "balrogo-1.6.6.tar", max compression
```

## Comparing `balrogo-1.6.5.tar` & `balrogo-1.6.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1090 2020-11-09 15:43:31.991839 balrogo-1.6.5/LICENSE
--rw-r--r--   0        0        0     5130 2021-07-03 09:08:14.177776 balrogo-1.6.5/README.md
--rw-r--r--   0        0        0      153 2020-12-16 16:58:29.555231 balrogo-1.6.5/balrogo/__init__.py
--rwxr-xr-x   0        0        0    31398 2023-05-13 20:06:47.596043 balrogo-1.6.5/balrogo/angle.py
--rw-r--r--   0        0        0    88940 2023-05-13 20:06:47.596043 balrogo-1.6.5/balrogo/dynamics.py
--rwxr-xr-x   0        0        0    33854 2023-05-13 20:06:47.596043 balrogo-1.6.5/balrogo/gaia.py
--rwxr-xr-x   0        0        0     5538 2021-01-29 14:16:08.816985 balrogo-1.6.5/balrogo/hrd.py
--rwxr-xr-x   0        0        0    27818 2021-06-26 17:29:21.281211 balrogo-1.6.5/balrogo/marginals.py
--rw-r--r--   0        0        0    10097 2021-06-26 12:16:33.674788 balrogo-1.6.5/balrogo/mock.py
--rwxr-xr-x   0        0        0     5745 2021-01-29 14:16:08.816985 balrogo-1.6.5/balrogo/parallax.py
--rw-r--r--   0        0        0    52358 2023-05-13 20:06:47.596043 balrogo-1.6.5/balrogo/pm.py
--rw-r--r--   0        0        0   109400 2023-01-16 01:13:59.473054 balrogo-1.6.5/balrogo/position.py
--rw-r--r--   0        0        0      875 2023-05-13 20:06:47.596043 balrogo-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     6178 2023-05-13 20:07:00.158173 balrogo-1.6.5/setup.py
--rw-r--r--   0        0        0     6111 2023-05-13 20:07:00.158669 balrogo-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1090 2020-11-09 15:43:31.991839 balrogo-1.6.6/LICENSE
+-rw-r--r--   0        0        0     5130 2021-07-03 09:08:14.177776 balrogo-1.6.6/README.md
+-rw-r--r--   0        0        0      153 2020-12-16 16:58:29.555231 balrogo-1.6.6/balrogo/__init__.py
+-rwxr-xr-x   0        0        0    31398 2023-05-13 20:07:45.148112 balrogo-1.6.6/balrogo/angle.py
+-rw-r--r--   0        0        0    88940 2023-05-13 20:07:45.148112 balrogo-1.6.6/balrogo/dynamics.py
+-rwxr-xr-x   0        0        0    33854 2023-05-13 20:07:45.148112 balrogo-1.6.6/balrogo/gaia.py
+-rwxr-xr-x   0        0        0     5538 2021-01-29 14:16:08.816985 balrogo-1.6.6/balrogo/hrd.py
+-rwxr-xr-x   0        0        0    27818 2021-06-26 17:29:21.281211 balrogo-1.6.6/balrogo/marginals.py
+-rw-r--r--   0        0        0    10097 2021-06-26 12:16:33.674788 balrogo-1.6.6/balrogo/mock.py
+-rwxr-xr-x   0        0        0     5745 2021-01-29 14:16:08.816985 balrogo-1.6.6/balrogo/parallax.py
+-rw-r--r--   0        0        0    58579 2023-06-25 14:20:47.530000 balrogo-1.6.6/balrogo/pm.py
+-rw-r--r--   0        0        0   109400 2023-01-16 01:13:59.473054 balrogo-1.6.6/balrogo/position.py
+-rw-r--r--   0        0        0      875 2023-06-25 14:20:47.530000 balrogo-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0     6178 2023-06-25 14:20:54.651266 balrogo-1.6.6/setup.py
+-rw-r--r--   0        0        0     6111 2023-06-25 14:20:54.651558 balrogo-1.6.6/PKG-INFO
```

### Comparing `balrogo-1.6.5/LICENSE` & `balrogo-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/README.md` & `balrogo-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/angle.py` & `balrogo-1.6.6/balrogo/angle.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/dynamics.py` & `balrogo-1.6.6/balrogo/dynamics.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/gaia.py` & `balrogo-1.6.6/balrogo/gaia.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/hrd.py` & `balrogo-1.6.6/balrogo/hrd.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/marginals.py` & `balrogo-1.6.6/balrogo/marginals.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/mock.py` & `balrogo-1.6.6/balrogo/mock.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/parallax.py` & `balrogo-1.6.6/balrogo/parallax.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/balrogo/pm.py` & `balrogo-1.6.6/balrogo/pm.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,62 @@
     fac = gamma(-0.5 - slp_pm / 2) ** 2 / gamma(-1 - slp_pm / 2) ** 2
 
     pdf = fac * f / np.pi
 
     return pdf
 
 
+def pdf_field_stars_circ(Ux, Uy, mu_pmx, mu_pmy, sr_pmx, sr_pmy, rot_pm, slp_pm):
+    """
+    PDF of Milky Way field stars according to slightly different from
+    eq. 24 from Vitral 2021, such that the function does not assume a
+    2-D diamond shape at large radii.
+
+    Parameters
+    ----------
+    Ux : array_like
+        Array containting the data to be fitted, in x-direction.
+    Uy : array_like
+        Array containting the data to be fitted, in y-direction.
+    mu_pmx : float
+        Mean proper motion in x-direction.
+    mu_pmy :  float
+        Mean proper motion in y-direction.
+    sr_pmx : float
+        Scale radius in x-direction.
+    sr_pmy : float
+        Scale radius in y-direction.
+    rot_pm : float
+        Angle of rotation of the major axis' ellipse,
+        with respect to the x-direction.
+    slp_pm : float
+        Slope of the PDF.
+
+    Returns
+    -------
+    pdf : array_like
+        Array containing the PDF the Milky Way field stars.
+
+    """
+
+    x = (Ux - mu_pmx) * np.cos(rot_pm) + (Uy - mu_pmy) * np.sin(rot_pm)
+    y = -(Ux - mu_pmx) * np.sin(rot_pm) + (Uy - mu_pmy) * np.cos(rot_pm)
+
+    f1 = (x / sr_pmx) * (x / sr_pmx)
+    f2 = (y / sr_pmy) * (y / sr_pmy)
+
+    f = (1 + f1 * f2) ** (0.5 + slp_pm / 2) / (sr_pmx * sr_pmy)
+
+    fac = -0.5 * (3 + slp_pm)
+
+    pdf = fac * f / np.pi
+
+    return pdf
+
+
 def lngauss_1d(Ux, mu_pmx, sig_pm, mirror=False):
     """
     1D Log-Gaussian PDF in cartesian coordinates.
 
     Parameters
     ----------
     Ux : array_like
@@ -261,14 +309,71 @@
     den = 2 * np.pi * sig_pm * sig_pm
 
     pdf = np.exp(f1 + f2) / den
 
     return pdf
 
 
+def gaussh_1d(Ux, ex, mu, sig, h3, h4):
+
+    hi = np.asarray([1, 0, 0, h3, h4])
+
+    expterm = np.exp(-0.5 * ((Ux - mu) / np.sqrt(sig * sig + ex * ex)) ** 2)
+    den = 3 * np.sqrt(np.pi) * (4 + np.sqrt(6) * hi[4]) * (sig * sig + ex * ex) ** 4.5
+
+    num1_out = 6 * ex**4 * sig**2
+    num1_in1 = np.sqrt(2) * sig * (6 * sig + np.sqrt(3) * hi[3] * (Ux - mu))
+    num1_in2 = np.sqrt(3) * hi[4] * (2 * mu**2 - sig**2 + 2 * Ux**2 - 4 * mu * Ux)
+    num1 = num1_out * (num1_in1 + num1_in2)
+
+    num2_out = sig**4
+    num2_in1 = (
+        2
+        * np.sqrt(6)
+        * hi[3]
+        * sig
+        * (Ux - mu)
+        * (2 * mu**2 - 3 * sig**2 + 2 * Ux**2 - 4 * mu * Ux)
+    )
+    num2_in2 = (
+        np.sqrt(3)
+        * hi[4]
+        * (
+            4 * mu**4
+            - 12 * mu**2 * sig**2
+            + 3 * sig**4
+            + 4 * Ux**4
+            - 16 * mu * Ux**3
+            + 12 * Ux**2 * (2 * mu**2 - sig**2)
+            - 8 * Ux * (2 * mu**3 - 3 * mu * sig**2)
+        )
+    )
+    num2_in3 = 6 * np.sqrt(2) * sig**4
+    num2 = num2_out * (num2_in1 + num2_in2 + num2_in3)
+
+    num3_out = 2 * ex**2
+    num3_in1 = (
+        np.sqrt(6)
+        * hi[3]
+        * sig**3
+        * (Ux - mu)
+        * (2 * mu**2 - 3 * sig**2 + 2 * Ux**2 - 4 * mu * Ux)
+    )
+    num3_in2 = 12 * np.sqrt(2) * sig**6
+    num3 = num3_out * (num3_in1 + num3_in2)
+
+    num4 = 6 * np.sqrt(2) * ex**6 * sig * (np.sqrt(3) * hi[3] * (Ux - mu) + 4 * sig)
+
+    num5 = 3 * ex**8 * (np.sqrt(3) * hi[4] + 2 * np.sqrt(2))
+
+    gaussh = (expterm / den) * (num1 + num2 + num3 + num4 + num5)
+
+    return gaussh
+
+
 def global_pdf(
     Ux,
     Uy,
     ex,
     ey,
     exy,
     mu_pmx_go,
@@ -277,14 +382,15 @@
     mu_pmx_mw,
     mu_pmy_mw,
     sr_pmx_mw,
     sr_pmy_mw,
     rot_pm_mw,
     slp_pm_mw,
     frc_go_mw,
+    circ=False,
 ):
     """
     This function gives the sum of the PDF's from the galactic object
     (2D Gaussian) and Milky Way field stars.
 
     Parameters
     ----------
@@ -315,14 +421,17 @@
     rot_pm_mw : float
         Angle of rotation of the Milky Way field stars' major axis' ellipse,
         with respect to the x-direction.
     slp_pm_mw : float
         Slope of the Milky Way field stars PDF.
     frc_go_mw : float
         Fraction of galactic objects by Milky Way stars.
+    circ : boolean, optional
+        True, if the user wants to use an interloper PDF with
+        ellipsoidal shape. The defualt is False.
 
     Returns
     -------
     array_like
         Sum of the PDF's from the galactic object
         (2D Gaussian) and Milky Way field stars.
 
@@ -336,22 +445,27 @@
     )
     sig_pm_go = np.sqrt(sig_pm_go * sig_pm_go + err)
 
     # PDF from galactic object
     pdf_go = frc_go_mw * gauss_2d(Ux, Uy, mu_pmx_go, mu_pmy_go, sig_pm_go)
 
     # PDF from Milky Way stars
-    pdf_mw = (1 - frc_go_mw) * pdf_field_stars(
-        Ux, Uy, mu_pmx_mw, mu_pmy_mw, sr_pmx_mw, sr_pmy_mw, rot_pm_mw, slp_pm_mw
-    )
+    if circ is True:
+        pdf_mw = (1 - frc_go_mw) * pdf_field_stars_circ(
+            Ux, Uy, mu_pmx_mw, mu_pmy_mw, sr_pmx_mw, sr_pmy_mw, rot_pm_mw, slp_pm_mw
+        )
+    else:
+        pdf_mw = (1 - frc_go_mw) * pdf_field_stars(
+            Ux, Uy, mu_pmx_mw, mu_pmy_mw, sr_pmx_mw, sr_pmy_mw, rot_pm_mw, slp_pm_mw
+        )
 
     return pdf_go + pdf_mw
 
 
-def likelihood_function(params, Ux, Uy, ex, ey, exy, values=None):
+def likelihood_function(params, Ux, Uy, ex, ey, exy, values=None, circ=False):
     """
     Computes minus the likelihood of the PM model from Vitral (2021).
 
     Parameters
     ----------
     params : array_like
         Array of parameters from the model.
@@ -365,14 +479,17 @@
         Data uncertainty in y-direction.
     exy : array_like
         Correlation of data uncertainty in x and y-direction.
     values : array_like, optional
         Array containing some of the parameters already fitted. If not fitted,
         they are filled with np.nan.
         The default is None.
+    circ : boolean, optional
+        True, if the user wants to use an interloper PDF with
+        ellipsoidal shape. The defualt is False.
 
     Returns
     -------
     L : float
         minus the logarithm of the likelihood function.
 
     """
@@ -411,14 +528,15 @@
         mu_pmx_mw,
         mu_pmy_mw,
         sr_pmx_mw,
         sr_pmy_mw,
         rot_pm_mw,
         slp_pm_mw,
         frc_go_mw,
+        circ=circ,
     )
 
     # Transforms zero's in NaN
     f_i[f_i <= 0] = np.nan
 
     # Calculates the likelihood, taking out NaN's
     f_i = f_i[np.logical_not(np.isnan(f_i))]
@@ -688,14 +806,52 @@
     # Calculates the likelihood, taking out NaN's
     f_i = f_i[np.logical_not(np.isnan(f_i))]
     L = -np.sum(np.log(f_i))
 
     return L
 
 
+def likelihood_1gaussh1d(params, Ux, ex):
+    """
+    Computes minus the likelihood of one Gauss-Hermite.
+
+    Parameters
+    ----------
+    params : array_like
+        Array of parameters from the model.
+    Ux : array_like
+        Array containting the data to be fitted, in x-direction.
+    ex : array_like
+        Data uncertainty in x-direction.
+
+    Returns
+    -------
+    L : float
+        minus the logarithm of the likelihood function.
+    """
+
+    mu_pmx_go = params[0]  # mean from galactic object
+    sig_pm_go = params[1]  # dispersion from galactic object
+    h3 = params[2]
+    h4 = params[3]
+
+    # PDF from galactic object
+    pdf_go = gaussh_1d(Ux, ex, mu_pmx_go, sig_pm_go, h3, h4)
+
+    # Gets the PDF
+    f_i = pdf_go
+
+    # Transforms negatives in zeroes.
+    f_i[f_i <= 0] = 0
+
+    L = -np.sum(np.log(f_i))
+
+    return L
+
+
 def likelihood_prior(params, guess, bounds):
     """
     This function sets the prior probabilities for the MCMC.
 
     Parameters
     ----------
     params : array_like
@@ -726,15 +882,15 @@
         and (guess[9] - bounds[9] < params[9] < guess[9] + bounds[9])
     ):
         return 0.0
     else:
         return -np.inf
 
 
-def likelihood_prob(params, Ux, Uy, ex, ey, exy, guess, bounds):
+def likelihood_prob(params, Ux, Uy, ex, ey, exy, guess, bounds, circ=False):
     """
     This function gets the prior probability for MCMC.
 
     Parameters
     ----------
     params : array_like
         Array containing the fitted values.
@@ -748,25 +904,28 @@
         Data uncertainty in y-direction.
     exy : array_like
         Correlation of data uncertainty in x and y-direction.
     guess : array_like
         Array containing the initial guess of the parameters.
     bounds : array_like
         Array containing the interval of variation of the parameters.
+    circ : boolean, optional
+        True, if the user wants to use an interloper PDF with
+        ellipsoidal shape. The defualt is False.
 
     Returns
     -------
     log probability: float
         log-probability for the respective params.
     """
 
     lp = likelihood_prior(params, guess, bounds)
     if not np.isfinite(lp):
         return -np.inf
-    return lp - likelihood_function(params, Ux, Uy, ex, ey, exy)
+    return lp - likelihood_function(params, Ux, Uy, ex, ey, exy, circ=circ)
 
 
 def prob(Ux, Uy, ex, ey, exy, params, conv=True):
     """
     This function gives the probability of a certain star to belong to
     a galactic object. This is computed with distribution functions in
     proper motion space.
@@ -892,15 +1051,16 @@
     neighborhood = generate_binary_structure(2, 2)
 
     # apply the local maximum filter; all pixel of maximal value
     # in their neighborhood are set to 1
     local_max = maximum_filter(image, footprint=neighborhood) == image
     # local_max is a mask that contains the peaks we are
     # looking for, but also the background.
-    # In order to isolate the peaks we must remove the background from the mask.
+    # In order to isolate the peaks we must remove the background
+    # from the mask.
 
     # we create the mask of the background
     background = image == 0
 
     # a little technicality: we must erode the background in order to
     # successfully subtract it form local_max, otherwise a line will
     # appear along the background border (artifact of the local maximum filter)
@@ -1160,14 +1320,15 @@
     min_method="dif",
     conv=True,
     hybrid=True,
     values=None,
     ini=None,
     bounds=None,
     define_range=True,
+    circ=False,
 ):
     """
     Calls a maximum likelihood fit of the proper motion paramters of
     the joint distribution of galactic object plus Milky Way stars.
 
     Parameters
     ----------
@@ -1203,14 +1364,17 @@
     bounds : array_like, optional
         Bounds used in the MLE fit.
         The default is None.
     define_range : boolean, optional
         True, if the user wishes that automatic ranges be defined.
         Good choice for data containing clear outliers.
         The default is True.
+    circ : boolean, optional
+        True, if the user wants to use an interloper PDF with
+        ellipsoidal shape. The defualt is False.
 
 
     Returns
     -------
     results : 10D-array
         Best fit parameters of the proper motion model.
     var : 10D-array
@@ -1352,15 +1516,17 @@
             eXY = np.zeros(len(X))
         else:
             eXY = eXY[idxpm]
 
     if hybrid is True:
         if min_method == "dif":
             mle_model = differential_evolution(
-                lambda c: likelihood_function(c, X, Y, eX, eY, eXY, values=values),
+                lambda c: likelihood_function(
+                    c, X, Y, eX, eY, eXY, values=values, circ=circ
+                ),
                 bounds,
             )
             results = mle_model.x
 
         else:
 
             ini = np.asarray(
@@ -1374,39 +1540,42 @@
                     ini[5],
                     0,
                     ini[6],
                     ini[7],
                 ]
             )
             mle_model = minimize(
-                lambda c: likelihood_function(c, X, Y, eX, eY, eXY, values=values),
+                lambda c: likelihood_function(
+                    c, X, Y, eX, eY, eXY, values=values, circ=circ
+                ),
                 ini,
                 method=min_method,
                 bounds=bounds,
             )
             results = mle_model["x"]
 
         hfun = ndt.Hessian(
-            lambda c: likelihood_function(c, X, Y, eX, eY, eXY, values=values),
+            lambda c: likelihood_function(
+                c, X, Y, eX, eY, eXY, values=values, circ=circ
+            ),
             full_output=True,
         )
 
         hessian_ndt, info = hfun(results)
         for i in range(len(values) - 1, -1, -1):
             if np.logical_not(np.isnan(values[i])):
                 hessian_ndt = np.delete(hessian_ndt, i, axis=1)
                 hessian_ndt = np.delete(hessian_ndt, i, axis=0)
                 results[i] = values[i]
         try:
             var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
         except np.linalg.LinAlgError as err:
             if "Singular matrix" in str(err):
-                print(
-                    "WARNING: Errors are deprecated --> assigning uncertainties as -1."
-                )
+                print("WARNING: Errors are deprecated")
+                print("--> assigning uncertainties as -1.")
                 var = -np.ones(len(results))
             else:
                 raise ValueError("Error when computing uncertainties.")
     else:
         mle_model = differential_evolution(
             lambda c: likelihood_gauss2d(c, X, Y, eX, eY, eXY, values=values), bounds
         )
@@ -1422,26 +1591,32 @@
                 hessian_ndt = np.delete(hessian_ndt, i, axis=1)
                 hessian_ndt = np.delete(hessian_ndt, i, axis=0)
                 results[i] = values[i]
         try:
             var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
         except np.linalg.LinAlgError as err:
             if "Singular matrix" in str(err):
-                print(
-                    "WARNING: Errors are deprecated --> assigning uncertainties as -1."
-                )
+                print("WARNING: Errors are deprecated")
+                print("--> assigning uncertainties as -1.")
                 var = -np.ones(len(results))
             else:
                 raise ValueError("Error when computing uncertainties.")
 
     return results, var
 
 
 def gauss_likelihood(
-    X, eX=None, conv=True, hybrid=True, lngauss=False, mirror=None, dgauss=False
+    X,
+    eX=None,
+    conv=True,
+    hybrid=True,
+    lngauss=False,
+    mirror=None,
+    dgauss=False,
+    hermite=False,
 ):
     """
     Calls a maximum likelihood fit of two (or one) Gaussian 1D fields.
 
     Parameters
     ----------
     X : array_like
@@ -1460,14 +1635,19 @@
         Log-Gaussian distribution. The default is False.
     mirror : Boolean
         True, if the Log-Gaussian is mirrored with respect to the
         y-axis. The default is None.
     dgauss : Boolean
         True, if user wishes to model interlopers with a
         double Gaussian distribution. The default is False.
+    hermite : Boolean
+        True, if user wishes to model the source with a
+        Gauss-Hermite function (up to order 4). Only available
+        for non hybrid treatment.
+        The default is False.
 
     Returns
     -------
     results : array
         Best fit parameters of the proper motion model.
     var : array
         Uncertainty of the fits.
@@ -1583,23 +1763,36 @@
             ]
         else:
             ranges = [
                 min(ini[0], ini[2]) - 5 * max(ini[1], ini[3]),
                 max(ini[0], ini[2]) + 5 * max(ini[1], ini[3]),
             ]
     else:
-        # Gets the initial guess of the parameters
-        ini = np.asarray([np.median(X), np.std(X)])
+        if hermite is True:
+            # Gets the initial guess of the parameters
+            ini = np.asarray([np.median(X), np.std(X), 0, 0])
 
-        bounds = [
-            (ini[0] - 3 * ini[1], ini[0] + 3 * ini[1]),
-            (0.1 * ini[1], 10 * ini[1]),
-        ]
+            bounds = [
+                (ini[0] - 3 * ini[1], ini[0] + 3 * ini[1]),
+                (0.1 * ini[1], 10 * ini[1]),
+                (-0.5, 0.5),
+                (-0.5, 0.5),
+            ]
+
+            ranges = [ini[0] - 3 * ini[1], ini[0] + 3 * ini[1]]
+        else:
+            # Gets the initial guess of the parameters
+            ini = np.asarray([np.median(X), np.std(X)])
+
+            bounds = [
+                (ini[0] - 3 * ini[1], ini[0] + 3 * ini[1]),
+                (0.1 * ini[1], 10 * ini[1]),
+            ]
 
-        ranges = [ini[0] - 3 * ini[1], ini[0] + 3 * ini[1]]
+            ranges = [ini[0] - 3 * ini[1], ini[0] + 3 * ini[1]]
 
     idx_x = np.intersect1d(np.where(X < ranges[1]), np.where(X > ranges[0]))
 
     X = X[idx_x]
 
     if conv is False:
         eX = np.zeros(len(X))
@@ -1646,22 +1839,36 @@
             hfun = ndt.Hessian(
                 lambda c: likelihood_2gauss1d(c, X, eX), full_output=True
             )
             hessian_ndt, info = hfun(results)
             var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
 
     else:
-        mle_model = differential_evolution(
-            lambda c: likelihood_1gauss1d(c, X, eX), bounds
-        )
-        results = mle_model.x
+        if hermite is True:
+            mle_model = differential_evolution(
+                lambda c: likelihood_1gaussh1d(c, X, eX), bounds
+            )
+            results = mle_model.x
 
-        hfun = ndt.Hessian(lambda c: likelihood_1gauss1d(c, X, eX), full_output=True)
-        hessian_ndt, info = hfun(results)
-        var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
+            hfun = ndt.Hessian(
+                lambda c: likelihood_1gaussh1d(c, X, eX), full_output=True
+            )
+            hessian_ndt, info = hfun(results)
+            var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
+        else:
+            mle_model = differential_evolution(
+                lambda c: likelihood_1gauss1d(c, X, eX), bounds
+            )
+            results = mle_model.x
+
+            hfun = ndt.Hessian(
+                lambda c: likelihood_1gauss1d(c, X, eX), full_output=True
+            )
+            hessian_ndt, info = hfun(results)
+            var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
 
     if lngauss is False:
         return results, var
     else:
         return results, var, mirror
 
 
@@ -1673,14 +1880,15 @@
     eXY=None,
     conv=True,
     nwalkers=None,
     steps=1000,
     ini=None,
     bounds=None,
     use_pool=False,
+    circ=False,
 ):
     """
     MCMC routine based on the emcee package (Foreman-Mackey et al, 2013).
 
     The user is strongly encouraged to provide initial guesses,
     which can be derived with the "maximum_likelihood" method,
     previously checked to provide reasonable fits.
@@ -1717,14 +1925,17 @@
         respect to the initial guesses.
         The order of parameters should be the same returned by the method
         "maximum_likelihood".
         The default is None.
     use_pool : boolean, optional
         "True", if the user whises to use full CPU power of the machine.
         The default is False.
+    circ : boolean, optional
+        True, if the user wants to use an interloper PDF with
+        ellipsoidal shape. The defualt is False.
 
     Returns
     -------
     chain : array_like
         Set of chains from the MCMC.
 
     """
@@ -1733,34 +1944,32 @@
         ini = initial_guess(X, Y)
         ini = np.asarray(
             [ini[0], ini[1], ini[2], ini[3], ini[4], ini[5], ini[5], 0, ini[6], ini[7]]
         )
 
     if bounds is None:
 
-        bounds = np.asarray(
-            [
-                ini[2],
-                ini[2],
-                ini[2] * 0.5,
-                ini[5],
-                ini[6],
-                ini[5] * 0.5,
-                ini[6] * 0.5,
-                np.pi / 2,
-                1,
-                ini[9] * 0.1,
-            ]
-        )
+        bounds = [
+            (ini[0] - 3 * ini[2], ini[0] + 3 * ini[2]),
+            (ini[1] - 3 * ini[2], ini[1] + 3 * ini[2]),
+            (0.1 * ini[2], 10 * ini[2]),
+            (ini[3] - 5 * ini[5], ini[3] + 5 * ini[5]),
+            (ini[4] - 5 * ini[5], ini[4] + 5 * ini[5]),
+            (0.1 * ini[5], 10 * ini[5]),
+            (0.1 * ini[5], 10 * ini[5]),
+            (-np.pi / 2, np.pi / 2),
+            (-20, -3),
+            (0.01, 1),
+        ]
 
     ndim = len(ini)  # number of dimensions.
     if nwalkers is None or nwalkers < 2 * ndim:
         nwalkers = int(2 * ndim + 1)
 
-    pos = [ini + 1e-3 * bounds * np.random.randn(ndim) for i in range(nwalkers)]
+    pos = [ini + 1e-3 * ini * np.random.randn(ndim) for i in range(nwalkers)]
 
     if conv is False:
         eX = np.zeros(len(X))
         eY = np.zeros(len(X))
         eXY = np.zeros(len(X))
     else:
         if eX is None:
@@ -1775,21 +1984,21 @@
     if use_pool:
 
         with Pool() as pool:
             sampler = emcee.EnsembleSampler(
                 nwalkers,
                 ndim,
                 likelihood_prob,
-                args=(X, Y, eX, eY, eXY, ini, bounds),
+                args=(X, Y, eX, eY, eXY, ini, bounds, circ),
                 pool=pool,
             )
             sampler.run_mcmc(pos, steps)
     else:
 
         sampler = emcee.EnsembleSampler(
-            nwalkers, ndim, likelihood_prob, args=(X, Y, eX, eY, eXY, ini, bounds)
+            nwalkers, ndim, likelihood_prob, args=(X, Y, eX, eY, eXY, ini, bounds, circ)
         )
         sampler.run_mcmc(pos, steps)
 
     chain = sampler.chain
 
     return chain
```

### Comparing `balrogo-1.6.5/balrogo/position.py` & `balrogo-1.6.6/balrogo/position.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.6.5/pyproject.toml` & `balrogo-1.6.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balrogo"
-version = "1.6.5"
+version = "1.6.6"
 description = "Bayesian Astrometric Likelihood Recovery of Galactic Objects"
 authors = ["Eduardo Vitral <vitral@iap.fr>", "Alexandre Macedo <arj.macedo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/eduardo-vitral/balrogo"
 
 [tool.poetry.dependencies]
```

### Comparing `balrogo-1.6.5/setup.py` & `balrogo-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'shapely>=1.6.4,<2.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib_metadata>=3.3.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'balrogo',
-    'version': '1.6.5',
+    'version': '1.6.6',
     'description': 'Bayesian Astrometric Likelihood Recovery of Galactic Objects',
     'long_description': '# BALRoGO\n\n[![pipeline status](https://gitlab.com/eduardo-vitral/balrogo/badges/master/pipeline.svg)](https://gitlab.com/eduardo-vitral/balrogo/-/commits/master)\n[![coverage report](https://gitlab.com/eduardo-vitral/balrogo/badges/master/coverage.svg)](https://gitlab.com/eduardo-vitral/balrogo/-/commits/master)\n[![pypi](https://img.shields.io/pypi/v/balrogo.svg)](https://pypi.python.org/pypi/balrogo/)\n[![python](https://img.shields.io/pypi/pyversions/balrogo.svg)](https://pypi.python.org/pypi/balrogo)\n[![license](http://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)\n\n<!-- markdownlint-disable-next-line no-inline-html -->\n<img alt="logo" align="right" src="https://gitlab.com/eduardo-vitral/balrogo/-/raw/master/logo.png" width="20%" />\n\nBALRoGO: Bayesian Astrometric Likelihood Recovery of Galactic Objects.\n\n- Specially developed to handle data from the Gaia space mission.\n- Extracts galactic objects such as globular clusters and dwarf galaxies from data contaminated by interlopers.\n- Uses a combination of Bayesian and non-Bayesian approaches.\n- Provides:\n  - Fits of proper motion space.\n  - Fits of surface density.\n  - Fits of object center.\n  - Confidence regions for the color-magnitude diagram and parallaxes.\n\nIf something does not work, please [file an issue](https://gitlab.com/eduardo-vitral/balrogo/-/issues).\n\n## Attribution\n\nPlease cite [us](https://academic.oup.com/mnras/article-abstract/504/1/1355/6237524?redirectedFrom=fulltext) if you find this code useful in your research. The BibTeX entry for the paper is:\n\n```bibtex\n@ARTICLE{Vitral21,\n   author = {{Vitral}, Eduardo},\n    title = "BALRoGO: Bayesian Astrometric Likelihood Recovery of Galactic Objects - Global properties of over one hundred globular clusters with Gaia EDR3",\n  journal = {\\mnras},\n     year = 2021,\n    month = jun,\n   volume = {504},\n   number = {1},\n    pages = {1355-1369},\n      doi = {10.1093/mnras/stab947},\n   eprint = {2102.04841},\n   adsurl = {https://ui.adsabs.harvard.edu/abs/2021MNRAS.504.1355V},\n}\n```\n\n## Quick overview\n\nBALRoGO has nine modules that perform different tasks:\n\n- ***angle.py*** : This module contains the main functions concerning angular tansformations, sky projections and spherical trigonomtry.\n- ***gaia.py*** : This module contains the main functions concerning the handling of the Gaia mission data.\n- ***hrd.py*** : This module contains the main functions concerning the color magnitude diagram (CMD). It provides a Kernel Density Estimation (KDE) of the CMD distribution.\n- ***marginals.py*** : This module is based on the Python corner package (Copyright 2013-2016 Dan Foreman-Mackey & contributors, The Journal of Open Source Software): https://joss.theoj.org/papers/10.21105/joss.00024\nI have done some modifications on it so it allows some new features and so it takes into account some choices as default. I thank Gary Mamon for his good suggestions concerning the plot visualization.\n-  ***parallax.py*** : This module contains the main functions concerning parallax information. It provides a kernel density estimation of the distance distribution, as well as a fit of the mode of this distribution.\n- ***pm.py*** : This module contains the main functions concerning proper motion data. It provides MCMC and maximum likelihood fits of proper motions data, as well as robust initial guesses for those fits.\n- ***position.py*** : This module contains the main functions concerning positional information. It provides MCMC and maximum likelihood fits of surface density, as well as robust initial guesses for the (RA,Dec) center of the source.\n- ***mock.py*** : This module handles mock data sets. It converts 3D coordinates to sky coordinates and is able to add realistic errors to proper motions. It is also able to generate Milky Way interlopers.\n- ***dynamics.py*** : This module handles conversions from celestial coordinates to plane of sky coordinates (vPOSr,vPOSt), as well as allows computation of dispersion profiles in different ways. Also computes the velocity anisotropy from cartesian data.\n\n## Installation\n\nBALRoGO is available through [pip](https://pypi.org/project/balrogo/). The quickiest way to install it is to type the following command in your terminal:\n\n```terminal\npip install balrogo\n```\n\nIf you are using [Anaconda](https://www.anaconda.com/), you might want to install it directly in your Anaconda bin path:\n\n```terminal\ncd path/anaconda3/bin/\npip install balrogo\n```\n\nFor updated versions of the code, you can do the same as above, but instead of using `pip install balrogo`, you should type:\n\n```terminal\npip install --upgrade balrogo\n```\n\n### Using BALRoGO on [*Gaia*](https://www.cosmos.esa.int/web/gaia/data-access) data\n\nFor quick tutorial of BALRoGO applied to *Gaia* data, please click [here](https://gitlab.com/eduardo-vitral/balrogo/-/blob/master/GAIA.md).\n\n## License\n\nCopyright (c) 2020 Eduardo Vitral & Alexandre Macedo.\n\nBALRoGO is free software made available under the [MIT License](LICENSE). The BALRoGO logo is licensed under a [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by/4.0/).\n',
     'author': 'Eduardo Vitral',
     'author_email': 'vitral@iap.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/eduardo-vitral/balrogo',
```

### Comparing `balrogo-1.6.5/PKG-INFO` & `balrogo-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balrogo
-Version: 1.6.5
+Version: 1.6.6
 Summary: Bayesian Astrometric Likelihood Recovery of Galactic Objects
 Home-page: https://gitlab.com/eduardo-vitral/balrogo
 License: MIT
 Author: Eduardo Vitral
 Author-email: vitral@iap.fr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

