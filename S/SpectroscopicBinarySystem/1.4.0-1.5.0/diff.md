# Comparing `tmp/SpectroscopicBinarySystem-1.4.0.tar.gz` & `tmp/SpectroscopicBinarySystem-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.4.0.tar", last modified: Wed May 17 13:37:03 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.5.0.tar", last modified: Sun Jun 25 12:40:20 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.4.0.tar` & `SpectroscopicBinarySystem-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:37:03.836655 SpectroscopicBinarySystem-1.4.0/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     4710 2023-05-17 13:37:03.836655 SpectroscopicBinarySystem-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4319 2023-05-15 22:27:13.000000 SpectroscopicBinarySystem-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 13:37:03.834642 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4710 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-17 13:37:03.000000 SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-05-17 13:37:03.843117 SpectroscopicBinarySystem-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 13:37:03.835651 SpectroscopicBinarySystem-1.4.0/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    34755 2023-05-17 13:34:14.000000 SpectroscopicBinarySystem-1.4.0/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:40:20.726926 SpectroscopicBinarySystem-1.5.0/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4710 2023-06-25 12:40:20.726926 SpectroscopicBinarySystem-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4319 2023-06-25 07:59:28.000000 SpectroscopicBinarySystem-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 12:40:20.726926 SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4710 2023-06-25 12:40:20.000000 SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-06-25 12:40:20.000000 SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 12:40:20.000000 SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-06-25 12:40:20.000000 SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-25 12:40:20.000000 SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-06-25 12:40:20.739459 SpectroscopicBinarySystem-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 12:40:20.726926 SpectroscopicBinarySystem-1.5.0/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    33410 2023-06-25 12:39:12.000000 SpectroscopicBinarySystem-1.5.0/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.4.0/LICENSE` & `SpectroscopicBinarySystem-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.4.0/PKG-INFO` & `SpectroscopicBinarySystem-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.0)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.4)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.4.0/README.md` & `SpectroscopicBinarySystem-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.0)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.4)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.4.0/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.5.0/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.0)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.3.4)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.4.0/setup.cfg` & `SpectroscopicBinarySystem-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 342e 300d 0a61  rsion = 1.4.0..a
+00000030: 7273 696f 6e20 3d20 312e 352e 300d 0a61  rsion = 1.5.0..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.4.0/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.5.0/spectroscopicbinarysystem/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import re
 import os
+import csv
 import copy
 import math
 import warnings
-import pickle
-from hashlib import md5
 
 # numpy
 import numpy as np
 
 # astropy
 from astropy.io import fits
 from astropy.time import Time
 import astropy.units as u
 import astropy.wcs as fitswcs
-from astropy.time import Time
+from astropy.time import Time, TimeDelta
 from astropy.coordinates import SkyCoord, EarthLocation, SpectralCoord
 from astropy.modeling import models, fitting
 from astropy import constants as const
 
 # astroquery
 from astroquery.simbad import Simbad
 
@@ -57,15 +56,16 @@
         self._snr = 0.0
         self._line_fit_fwhm = 0.0
         self._phase = None
 
         spectrum_file = fits.open(filename)
 
         self._header = spectrum_file[0].header
-        self._jd = self._header['JD-OBS']
+        self._time = Time(self._header['DATE-OBS'], format='isot', scale='utc')
+        self._jd = self._time.jd
         self._observer = self._header['OBSERVER']
         with warnings.catch_warnings():  # Ignore warnings
             warnings.simplefilter('ignore')
 
             wcs_data = fitswcs.WCS(header={'CDELT1': self._header['CDELT1'], 'CRVAL1': self._header['CRVAL1'],
                                            'CUNIT1': 'Angstroms', 'CTYPE1': 'WAVE',
                                            'CRPIX1': self._header['CRPIX1']})
@@ -117,19 +117,18 @@
         return calibration_error
 
     def getSNR(self):
         return self._snr
 
     def getJD(self):
         """
-        Return 'JD-OBS' header field
         :return: float corresponding to the julian date of the observation
         :rtype: float
         """
-        return float(self._header['JD-OBS'])
+        return float(self._jd)
 
     def getHeader(self):
         return self._header
 
     def getDate(self):
         """
         Return 'DATE-OBS' header field
@@ -162,17 +161,17 @@
         return self._basename
 
     def findRVCorrection(self):
         """
         Compute radial velocity correction in function of the target and the location of the observer
         :return: None
         """
-        t = Time(self._header['JD-OBS'], format='jd', scale='utc')
+        t = Time(self._jd, format='jd', scale='utc')
         loc = EarthLocation(
-            self._header['GEO_LONG'], self._header['GEO_LAT'], self._header['GEO_ELEV'] * u.m)
+            float(self._header['GEO_LONG']), float(self._header['GEO_LAT']), float(self._header['GEO_ELEV']) * u.m)
         vcorr = self._skycoord.radial_velocity_correction(
             kind=self._conf["RV_CORR_TYPE"], obstime=t, location=loc)
         self._rv_corr = vcorr.to(u.km / u.s)
 
     def getRVCorrection(self):
         return self._rv_corr
 
@@ -244,25 +243,14 @@
                 fwhm = g_fit.fwhm
 
         self._debug_line_fitting = (spec1d_line, y_fit, extract_region(Spectrum1D(
             flux=spec1_gsmooth.flux, wcs=self.wcs), sr_w1))
         self._center_of_line = center.value
         self._line_fit_fwhm = fwhm.value
 
-    def asdict(self):
-        return {'jd': self.getJD(),
-                'date': self.getDate(),
-                'observer': self.getObserver(),
-                'instrument': self.getInstrument(),
-                'basename': self.getBaseName(),
-                'rv': self.getRV(),
-                'error': self.getError(),
-                'center': self.getCenterOfLine(),
-                'phase': self.getPhase()}
-
     def __str__(self):
         return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- snr: {self._snr}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n- error: {self.getError()}\n"
 
 #
 
 
 class SpectroscopicBinarySystem:
@@ -279,46 +267,39 @@
     :param t0: Allow to fix Periastron epoch T0 if known (julian date)
     :param period: If the period of the orbit is already known use this param (period in days).
     :param perdiod_guess: If the period is uncertain use this param (period in days).
     :param conf: Allow to customize additionnal parameters (see self._conf default value below)
     :param debug: Allow to activate log and some additional plots for debug purpose
     """
 
-    def __init__(self, object_name, spectra_path, t0=None, period=None, period_guess=None, conf=None, verbose=False, debug=False, nocache=False):
+    def __init__(self, object_name, spectra_path, t0=None, period=None, period_guess=None, conf=None, verbose=False, debug=False):
 
         self._conf = {"LAMBDA_REF": 6562.82,
                       "LINE_FIT_MODEL": "gaussian",
                       "LINE_FIT_FWHM": 3.0,
                       "LINE_FIT_GAUSS_SMOOTH_STD": 10,
                       "RV_CORR_TYPE": "barycentric",
                       "SB_TYPE": 1}
 
         self._sb_spectra = []
-        self._sb_spectra_dict = []
         self._spectra_filename = []
         self._orbital_solution = None
         self._spectra_path = spectra_path
         self._object_name = object_name
         self._type = type
-        self._nocache = nocache
         self._t0 = t0
         self._period = period
         self._period_guess = period_guess
         self._debug = debug
         self._verbose = verbose
         self._residuals = []
-        self._key = str(self._conf).encode()
-        for root, dirs, files in os.walk(self._spectra_path):
-            for file in files:
-                regex = re.compile('(.*).fit')
-                if (re.match(regex, file)):
-                    spectrum_filename = os.path.join(
-                        self._spectra_path, file)
-                    self._key += spectrum_filename.encode()
-        self._key = md5(self._key).hexdigest()
+        self._results_csv_filename = os.path.join(
+            self._spectra_path, 'sbss_results.csv')
+        self._bss_filename = os.path.join(
+            self._spectra_path, 'binarystarsolver_results.txt')
 
         # load user configuration or defaults
         if conf:
             self._conf.update(conf)
 
         print('** SpectroscopicBinarySystem **')
         self.__findObjectCoordinate()
@@ -330,46 +311,28 @@
         self._skycoord = None
         if result_table := Simbad.query_object(self._object_name):
             ra = result_table[0]['RA']
             dec = result_table[0]['DEC']
             self._skycoord = SkyCoord(f'{ra} {dec}', unit=(u.hourangle, u.deg))
 
     def __loadSpectra(self):
-        """
-        Load all spectra and create SBSpectrum1D objects
-        """
-        pickle_file = os.path.join(
-            self._spectra_path, f"{self._key}_spectra.pickle")
-        if os.path.exists(pickle_file) and not self._nocache:
-            with open(pickle_file, "rb") as infile:
-                self._sb_spectra_dict = pickle.load(infile)
-        else:
-            self._sb_spectra = []
-            self._sb_spectra_dict = []
-            for root, dirs, files in os.walk(self._spectra_path):
-                for file in files:
-                    regex = re.compile('(.*).fit')
-                    if (re.match(regex, file)):
-                        spectrum_filename = os.path.join(
-                            self._spectra_path, file)
-                        sbSpec1D = SBSpectrum1D(
-                            spectrum_filename, self._skycoord, self._conf)
-                        self._sb_spectra.append(sbSpec1D)
-                        self._sb_spectra_dict.append(sbSpec1D.asdict())
-                        if self._verbose:
-                            print(sbSpec1D)
-            if not self._nocache:
-                with open(pickle_file, "wb") as outfile:
-                    pickle.dump(self._sb_spectra_dict, outfile)
+        for root, dirs, files in os.walk(self._spectra_path):
+            for file in files:
+                regex = re.compile('(.*).fit')
+                if (re.match(regex, file)):
+                    spectrum_filename = os.path.join(self._spectra_path, file)
+                    sbSpec1D = SBSpectrum1D(
+                        spectrum_filename, self._skycoord, self._conf)
+                    self._sb_spectra.append(sbSpec1D)
+                    if self._verbose:
+                        print(sbSpec1D)
 
         if self._verbose:
-            print(f'key : {self._key}')
-            print(f'{len(self._sb_spectra_dict)} processed spectra')
-
-        if self._debug and self._sb_spectra:
+            print(f'{len(self._sb_spectra)} processed spectra')
+        if self._debug:
             plt.rcParams['font.size'] = '6'
             plt.rcParams['font.family'] = 'monospace'
 
             paginate_sb_spectra = [self._sb_spectra[i:i+16]
                                    for i in range(0, len(self._sb_spectra), 16)]
             for page, spectra in enumerate(paginate_sb_spectra):
                 fig, axs = plt.subplots(4, 4, figsize=(
@@ -407,15 +370,15 @@
 
     def getObservationCount(self):
         """
         Return the count of processed spectra
         :return: count
         :rtype: int
         """
-        return len(self._sb_spectra_dict)
+        return len(self._sb_spectra)
 
     def __getPhase(self, jd0, period, jd):
         """
         Compute the phase of a given JD
         :param jd0: JD of the first observation
         :param period: period of the orbit
         :param jd: JD to compute the phase
@@ -439,93 +402,90 @@
         M = 2 * np.pi * ((t - t0) % 1)
         # Eccentric anomaly
         E = utilities.eccentric_anomaly_from_mean(e, M, tolerance=0.00001)
         # True anomaly
         f = utilities.true_anomaly_from_eccentric(e, E)
         return (K * (e * np.cos(w) + np.cos(w + f)) + v0)
 
-    def __solveSystem(self):
+    def solveSystem(self):
         """
         Compute the orbital solution with BinaryStarSolver
         """
-        pickle_file = os.path.join(
-            self._spectra_path, f"{self._key}_orbital.pickle")
-        if os.path.exists(pickle_file) and not self._nocache:
-            with open(pickle_file, "rb") as infile:
-                self._orbital_solution = pickle.load(infile)
-                params, err, cov = self._orbital_solution
-        else:
-            # write result file for BinaryStarSolver
-            with open(f'{self._spectra_path}/sbs_results.txt', 'w') as f:
-                for s in self._sb_spectra:
-                    error = 1 / s.getError() if s.getError() else 1
-                    output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)} {error}"
-                    f.write(output + '\n')
-
-            # [γ, K, ω, e, T0, P, a, f(M)]
-            try:
-                params, err, cov = StarSolve(
-                    data_file=f"{self._spectra_path}/sbs_results.txt",
-                    star="primary",
-                    Period=self._period,
-                    Pguess=self._period_guess,
-                    covariance=True,
-                    graphs=False,
-                )
-            except:
-                print(
-                    'An exception occurred : the calculation of the orbital solution failed')
-                exit()
-
-            self._orbital_solution = (params, err, cov)
-
-            if not self._nocache:
-                with open(pickle_file, "wb") as outfile:
-                    pickle.dump(self._orbital_solution, outfile)
+        # write result file for BinaryStarSolver
+        with open(self._bss_filename, 'w') as f:
+            for s in self._sb_spectra:
+                error = 1 / s.getError() if s.getError() else 1
+                output = f"{float(s.getJD()) - 2400000.0} {round(s.getRV(), 3)} {error}"
+                f.write(output + '\n')
+
+        # [γ, K, ω, e, T0, P, a, f(M)]
+        try:
+            params, err, cov = StarSolve(
+                data_file=self._bss_filename,
+                star="primary",
+                Period=self._period,
+                Pguess=self._period_guess,
+                covariance=True,
+                graphs=False,
+            )
+        except:
+            print(
+                'An exception occurred : the calculation of the orbital solution failed')
+            exit()
+
+        self._orbital_solution = (params, err, cov)
 
         # If self._t0 compute phase delta between T0 of the model and the fixed value
         if self._t0:
             t0 = self._t0
             phase1 = self.__getPhase(
                 t0, self._orbital_solution[0][5], self._orbital_solution[0][4]+2400000)
             phase2 = 1.0
             self._v0 = phase1 - phase2
         # Else use t0 compute by the model
         else:
             self._t0 = self._orbital_solution[0][4] + 2400000
             self._v0 = 0
 
         period = self._orbital_solution[0][5]
-        if self._sb_spectra:
-            for s in self._sb_spectra:
-                # compute phase of the sytem
-                s.setPhase(self.__getPhase(float(self._t0), period, s.getJD()))
-
-        for s in self._sb_spectra_dict:
+        for s in self._sb_spectra:
             # compute phase of the sytem
-            jd = s['jd']
-            s['phase'] = self.__getPhase(float(self._t0), period, jd)
+            jd = s.getJD()
+            phase = self.__getPhase(float(self._t0), period, jd)
+            s.setPhase(phase)
             if self._verbose:
-                print(f"{s['basename']} phase : {s['phase']}")
+                print(f"{s.getBaseName()} phase : {phase}")
+
+        # export all results
+        res = [['FILE', 'JD-OBS', 'DATE-OBS', 'EXPTIME', 'OBSERVER',
+                'INSTRUMENT', 'PHASE', 'CENTER', 'RV', 'ERROR']]
+        for s in self._sb_spectra:
+            res.append([s.getBaseName(), s.getJD(), s.getDate(), s.getHeader()['EXPTIME'], s.getObserver(), s.getInstrument(
+            ), s.getPhase(), s.getCenterOfLine(), s.getRV(), s.getError()])
+
+        with open(self._results_csv_filename, 'w') as f:
+            mywriter = csv.writer(
+                f, delimiter=',', quoting=csv.QUOTE_NONNUMERIC)
+            mywriter.writerows(res)
 
         print(
-            f'{self._object_name} orbital solution with {len(self._sb_spectra_dict)} spectra',
+            f'{self._object_name} orbital solution with {len(self._sb_spectra)} spectra',
             f'- γ = {params[0]} ± {err[0]}',
             f'- K = {params[1]} ± {err[1]}',
             f'- ω = {params[2]} ± {err[2]}',
             f'- e = {params[3]} ± {err[3]}',
             f'- T0 = {params[4]} ± {err[4]}',
             f'- P = {params[5]} ± {err[5]}',
             f'- a = {params[6]} ± {err[6]}',
             f'- f(M) = {params[7]} ± {err[7]}',
             f'- Error sums = {sum(err)}',
             sep='\n')
 
     def getOrbitalSolution(self):
-        self.__solveSystem()
+        self.solveSystem()
         return self._orbital_solution
 
     def __findNearest(self, array, value):
         """
         Find the nearest value in an array
         :param array: array for search
         :param value: value to find
@@ -546,65 +506,64 @@
         marker_index = {}
         color_number = 0
 
         cmap = plt.get_cmap('tab20')
         markers_style = ["o", "v", "^", "s", "D", "P", "X"]
 
         # define colors (max 60 distinct observers)
-        colors = cmap((np.arange(20)).astype(int), alpha=1)
-        + cmap((np.arange(20)).astype(int), alpha=.75)
-        + cmap((np.arange(20)).astype(int), alpha=.5)
+        colors = np.concatenate((cmap((np.arange(20)).astype(int), alpha=1), cmap(
+            (np.arange(20)).astype(int), alpha=.75), cmap((np.arange(20)).astype(int), alpha=.5)))
 
         # sort sb spectra by observer name
-        self._sb_spectra_dict.sort(key=lambda x: x['observer'])
+        self._sb_spectra.sort(key=lambda x: x.getObserver())
 
-        for s in self._sb_spectra_dict:
+        for s in self._sb_spectra:
 
             # get the observer
-            obs = s['observer']
+            obs = s.getObserver()
             if (obs not in observers.keys()):
                 observers[obs] = colors[color_number]
                 color_number += 1
                 if not group_by_instruments:
-                    axs[0].errorbar(s['phase'], s['rv'], yerr=0,
+                    axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
                                     fmt='o', ecolor='k', label=obs, capsize=0, color=observers[obs], lw=.7, markersize=5)
             elif not group_by_instruments:
-                axs[0].errorbar(s['phase'], s['rv'], yerr=0,
+                axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
                                 fmt='o', ecolor='k', capsize=0, color=observers[obs], lw=.7, markersize=5)
             color = observers[obs]
 
             # get the instrument
             if (group_by_instruments):
-                label = f"{obs} - {s['instrument'][:30]}…"
+                label = f"{obs} - {s.getInstrument()[:30]}…"
                 if label not in instruments.keys():
                     if obs not in marker_index:
                         marker_index[obs] = 0
                     instruments[label] = markers_style[marker_index[obs]]
                     marker_index[obs] += 1
-                    axs[0].errorbar(s['phase'], s['rv'], yerr=0, label=label, ecolor='k',
-                                    capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
+                    axs[0].errorbar(s.getPhase(), s.getRV(
+                    ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=5)
                 else:
-                    axs[0].errorbar(s['phase'], s['rv'], yerr=0,
+                    axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
                                     fmt=instruments[label], ecolor='k', capsize=0, color=color, lw=.7, markersize=5)
 
-            xindex = self.__findNearest(self._model_x, s['phase'])
-            delta = s['rv'] - self._model_y[xindex]
+            xindex = self.__findNearest(self._model_x, s.getPhase())
+            delta = s.getRV() - self._model_y[xindex]
             self._residuals.append(delta)
             fmt = instruments[label] if group_by_instruments else 'o'
-            error = s['error']
+            error = s.getError()
             capsize = 3 if error else 0
-            axs[1].errorbar(s['phase'], delta,
-                            yerr=s['error'], fmt=fmt, ecolor='k', capsize=capsize, color=color, lw=.7, markersize=5)
+            axs[1].errorbar(s.getPhase(), delta,
+                            yerr=s.getError(), fmt=fmt, ecolor='k', capsize=capsize, color=color, lw=.7, markersize=5)
 
         print(
             f'- Residual standard deviation : {np.std(self._residuals)}')
 
     def plotRadialVelocityCurve(self, title="", subtitle="", rv_y_multiple=10, residual_y_multiple=None, savefig=False, dpi=150, font_family='monospace', font_size=9, group_by_instruments=False):
         if not self._orbital_solution:
-            self.__solveSystem()
+            self.solveSystem()
 
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
         fig, axs = plt.subplots(2, 1, figsize=(12, 7), gridspec_kw={
             'height_ratios': [4, 1]}, sharex=True)
         axs[1].set_xlabel('Phase', fontdict=None,
                           labelpad=None, fontname='monospace', size=8)
@@ -660,15 +619,15 @@
         :param font_family:
         :param font_size:
         :param show:
         :return: fig
         """
 
         if not self._orbital_solution:
-            self.__solveSystem()
+            self.solveSystem()
 
         fig = go.Figure()
 
         # plot orbital solution
         self._model_x = np.arange(0, 1.011, 0.001)
 
         self._model_y = list(map(lambda x: self.__computeRadialVelocityCurve(x, self._v0, self._orbital_solution[0][1],
@@ -684,63 +643,67 @@
         instruments = {}
         color_number = 0
         period = self._orbital_solution[0][5]
 
         cmap = plt.get_cmap('tab20')
 
         # define colors (max 60 distinct observers)
-        colors = cmap((np.arange(20)).astype(int), alpha=1)
-        + cmap((np.arange(20)).astype(int), alpha=.75)
-        + cmap((np.arange(20)).astype(int), alpha=.5)
+        colors = np.concatenate((cmap((np.arange(20)).astype(int), alpha=1), cmap(
+            (np.arange(20)).astype(int), alpha=.75), cmap((np.arange(20)).astype(int), alpha=.5)))
 
         markers_style = ['circle', 'square',
                          'diamond', 'triangle-up', 'triangle-down']
 
-        for s in self._sb_spectra_dict:
+        for s in self._sb_spectra:
+            # compute phase of the sytem
+            jd = s.getJD()
+            phase = self.__getPhase(float(self._t0), period, jd)
+            s.setPhase(phase)
+
             # get the observer
-            obs = s['observer']
+            obs = s.getObserver()
             if (obs not in observers.keys()):
                 rgb = colors[color_number][:3] * 255
                 str_rgb = ",".join([str(rgb[0]), str(rgb[1]), str(rgb[2])])
                 observers[obs] = f'rgba({str_rgb}, {colors[color_number][3]})'
                 color_number += 1
             color = observers[obs]
 
             if group_by_instrument:
                 # get the instrument
-                label = f"{obs} - {s['instrument'][:30]}…"
+                label = f"{obs} - {s.getInstrument()[:30]}…"
                 if label in instruments:
                     fig.add_trace(
-                        go.Scatter(x=[s['phase']],
-                                   y=[s['rv']],
+                        go.Scatter(x=[phase],
+                                   y=[s.getRV()],
                                    mode='markers',
                                    marker_symbol=instruments[label],
                                    marker=dict(color=color,
                                                size=8),
                                    showlegend=False))
                 else:
                     if obs not in marker_index:
                         marker_index[obs] = 0
                     instruments[label] = markers_style[marker_index[obs]]
                     marker_index[obs] += 1
                     fig.add_trace(
-                        go.Scatter(x=[s['phase']],
-                                   y=[s['rv']],
+                        go.Scatter(x=[phase],
+                                   y=[s.getRV()],
                                    mode='markers',
                                    name=label,
                                    marker_symbol=instruments[label],
                                    marker=dict(color=color,
                                                size=8),
                                    showlegend=True))
             else:  # no grouping
                 # set label to date
-                label = f"{obs} - {s['date']}"
+                label = f"{obs} - {s.getDate()}"
                 fig.add_trace(
-                    go.Scatter(x=[s['phase']],
-                               y=[s['rv']],
+                    go.Scatter(x=[phase],
+                               y=[s.getRV()],
                                mode='markers',
                                name=label,
                                marker_symbol='circle',
                                marker=dict(color=color,
                                            size=8),
                                showlegend=False))
 
@@ -808,20 +771,16 @@
         :param font_size:
         :param show:
         :return: fig
         """
         plt.rcParams['font.size'] = font_size
         plt.rcParams['font.family'] = font_family
 
-        self._nocache = True
-        if not self._sb_spectra:
-            self.__loadSpectra()
-            self.__solveSystem()
-        elif not self._orbital_solution:
-            self.__solveSystem()
+        if not self._orbital_solution:
+            self.solveSystem()
 
         # sort sb spectra by phase
         self._sb_spectra.sort(key=lambda x: x.getPhase())
 
         # create y axis range (phase)
         y_phase = np.arange(0, 1.01, 0.015)
         # create x axis range (wavelength) and convert to km/s
@@ -866,7 +825,17 @@
         plt.yticks(np.arange(0, 1.01, 0.1))
         if savefig:
             plt.savefig(
                 f'{self._spectra_path}/{self._object_name}_2d_spectrum_result.png', dpi=dpi)
         plt.show()
 
         return spec2d
+
+
+def printPhaseEphem(jd0, period, start_date=None, step_in_days=1, count_in_days=20):
+    st = Time(start_date, format='isot', scale='utc')
+    for i in range(0, count_in_days, step_in_days):
+        dt = TimeDelta(i * 3600 * 24, format='sec')
+        ft = st + dt
+        jd = ft.jd
+        phase = (jd - jd0) / period % 1
+        print(f'date (UT) = {ft} phase = {phase:.2f}')
```

