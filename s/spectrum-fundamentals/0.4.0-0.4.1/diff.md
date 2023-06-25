# Comparing `tmp/spectrum_fundamentals-0.4.0.tar.gz` & `tmp/spectrum_fundamentals-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.4.0.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.4.1.tar", max compression
```

## Comparing `spectrum_fundamentals-0.4.0.tar` & `spectrum_fundamentals-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/LICENSE
--rw-r--r--   0        0        0     2611 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/README.rst
--rw-r--r--   0        0        0     2367 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      940 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    11153 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1372 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0     7807 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    12452 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    14554 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1435 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    22868 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    22390 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0     9443 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2611 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/README.rst
+-rw-r--r--   0        0        0     2367 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      940 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    11160 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1372 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0     7807 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    12267 2023-06-25 12:04:29.968596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    14554 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1435 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    22868 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    22390 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0     9443 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2023-06-25 12:04:29.972596 spectrum_fundamentals-0.4.1/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.4.1/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.4.0/LICENSE` & `spectrum_fundamentals-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/README.rst` & `spectrum_fundamentals-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/pyproject.toml` & `spectrum_fundamentals-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.4.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.4.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamentals public repo"
 authors = ["WassimG <wassim.gabriel@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Initialize fundamentals."""
 __author__ = "Victor Giurcoiu"
 __email__ = "victor.giurcoiu@tum.de"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/annotation/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from spectrum_fundamentals import constants
 from spectrum_fundamentals.fragments import initialize_peaks
 
 logger = logging.getLogger(__name__)
 
 
 def match_peaks(
-    fragments_meta_data: pd.DataFrame,
+    fragments_meta_data: List[dict],
     peaks_intensity: np.ndarray,
     peaks_masses: np.ndarray,
     tmt_n_term: int,
     unmod_sequence: str,
     charge: int,
 ) -> List[Dict[str, Union[str, int, float]]]:
     """
@@ -33,15 +33,16 @@
     no_of_peaks = len(peaks_intensity)
     max_intensity = 1.0
     row_list = []
     temp_list = []
     next_start_peak = 0
     seq_len = len(unmod_sequence)
     matched_peak = False
-    for _, fragment in fragments_meta_data.iterrows():
+    fragment_no: float
+    for fragment in fragments_meta_data:
         min_mass = fragment["min_mass"]
         max_mass = fragment["max_mass"]
         fragment_no = fragment["no"]
         if matched_peak:
             start_peak = next_start_peak
         matched_peak = False
         while start_peak < no_of_peaks:
```

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/constants.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/fragments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
+from operator import itemgetter
 from typing import Dict, List, Optional, Tuple
 
 import numpy as np
-import pandas as pd
 
 from . import constants as constants
 
 logger = logging.getLogger(__name__)
 
 
 def _get_modifications(peptide_sequence: str) -> Optional[Tuple[Dict[int, float], int, str]]:
@@ -102,15 +102,15 @@
     for i in range(0, peptide_length):  # generate substrings
         forward_sum += constants.AA_MASSES[peptide_sequence[i]]  # sum left to right
         if i in modification_deltas:  # add mass of modification if present
             forward_sum += modification_deltas[i]
     return forward_sum + ion_type_offsets[0] + ion_type_offsets[1]
 
 
-def initialize_peaks(sequence: str, mass_analyzer: str, charge: int) -> Tuple[pd.DataFrame, int, str, float]:
+def initialize_peaks(sequence: str, mass_analyzer: str, charge: int) -> Tuple[List[dict], int, str, float]:
     """
     Generate theoretical peaks for a modified peptide sequence.
 
     :param sequence: Modified peptide sequence
     :param mass_analyzer: Type of mass analyzer used eg. FTMS, ITMS
     :param charge: Precursor charge
     :raises AssertionError:  if peptide sequence contained an unknown modification. TODO do this within the get_mod func.
@@ -119,21 +119,17 @@
     peptide_sequence = sequence
     modifications = _get_modifications(peptide_sequence)
     if modifications is None:
         raise AssertionError("Modification not found.")
     else:
         modification_deltas, tmt_n_term, peptide_sequence = modifications
 
-    col_dtypes = {"ion_type": str, "no": int, "charge": float, "mass": float, "min_mass": float, "max_mass": float}
     peptide_length = len(peptide_sequence)
-
     if peptide_length > 30:
-        df_out = pd.DataFrame(columns=col_dtypes.keys())
-        df_out = df_out.astype(col_dtypes)
-        return df_out, -1, "", 0.0
+        return [{}], -1, "", 0.0
 
     # initialize constants
     if int(round(charge)) <= 3:
         max_charge = int(round(charge))
     else:
         max_charge = 3
 
@@ -177,26 +173,25 @@
             # positive charge is introduced by protons (or H - ELECTRON_MASS)
             charge_delta = charge * constants.PARTICLE_MASSES["PROTON"]
             for ion_type in range(0, number_of_ion_types):  # generate all ion types
                 # Check for neutral loss here
                 mass = (ion_type_masses[ion_type] + charge_delta) / charge
                 min_mass, max_mass = get_min_max_mass(mass_analyzer, mass)
                 fragments_meta_data.append(
-                    [
-                        ion_types[ion_type],  # ion type
-                        i + 1,  # no
-                        charge,  # charge
-                        mass,  # mass
-                        min_mass,  # min mass
-                        max_mass,  # max mass
-                    ]
+                    {
+                        "ion_type": ion_types[ion_type],  # ion type
+                        "no": i + 1,  # no
+                        "charge": charge,  # charge
+                        "mass": mass,  # mass
+                        "min_mass": min_mass,  # min mass
+                        "max_mass": max_mass,  # max mass
+                    }
                 )
-    df_out = pd.DataFrame(data=fragments_meta_data, columns=col_dtypes.keys())
-    df_out.sort_values(by="mass", inplace=True)
-    return df_out, tmt_n_term, peptide_sequence, (forward_sum + ion_type_offsets[0] + ion_type_offsets[1])
+    fragments_meta_data = sorted(fragments_meta_data, key=itemgetter("mass"))
+    return fragments_meta_data, tmt_n_term, peptide_sequence, (forward_sum + ion_type_offsets[0] + ion_type_offsets[1])
 
 
 def get_min_max_mass(mass_analyzer: str, mass: float) -> Tuple[float, float]:
     """Helper function to get min and max mass based on mass analyzer.
 
     :param mass_analyzer: the type of mass analyzer used to determine the tolerance.
     :param mass: the theoretical fragment mass
```

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/percolator.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.4.1/spectrum_fundamentals/mod_string.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.4.0/PKG-INFO` & `spectrum_fundamentals-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-fundamentals
-Version: 0.4.0
+Version: 0.4.1
 Summary: Fundamentals public repo
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: WassimG
 Author-email: wassim.gabriel@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

