# Comparing `tmp/pymcabc-0.2.0.tar.gz` & `tmp/pymcabc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcabc-0.2.0.tar", last modified: Sun Apr  2 13:02:28 2023, max compression
+gzip compressed data, was "pymcabc-0.3.0.tar", last modified: Sun Jun 25 14:26:51 2023, max compression
```

## Comparing `pymcabc-0.2.0.tar` & `pymcabc-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:02:28.140804 pymcabc-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-02 13:02:19.000000 pymcabc-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-02 13:02:19.000000 pymcabc-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-02 13:02:28.140804 pymcabc-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-02 13:02:19.000000 pymcabc-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:02:28.140804 pymcabc-0.2.0/pymcabc/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/cross_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/decay_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/feynman_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/generate_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/identify_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-02 13:02:19.000000 pymcabc-0.2.0/pymcabc/save_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:02:28.140804 pymcabc-0.2.0/pymcabc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-02 13:02:28.000000 pymcabc-0.2.0/pymcabc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-02 13:02:28.000000 pymcabc-0.2.0/pymcabc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 13:02:28.000000 pymcabc-0.2.0/pymcabc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-02 13:02:28.000000 pymcabc-0.2.0/pymcabc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 13:02:28.000000 pymcabc-0.2.0/pymcabc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 13:02:28.140804 pymcabc-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-02 13:02:19.000000 pymcabc-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 13:02:28.140804 pymcabc-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-02 13:02:19.000000 pymcabc-0.2.0/tests/test_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.880414 pymcabc-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-25 14:26:43.000000 pymcabc-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-25 14:26:43.000000 pymcabc-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-25 14:26:51.876414 pymcabc-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-25 14:26:43.000000 pymcabc-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.876414 pymcabc-0.3.0/pymcabc/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/cross_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/decay_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/feynman_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/generate_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/identify_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-25 14:26:43.000000 pymcabc-0.3.0/pymcabc/save_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.876414 pymcabc-0.3.0/pymcabc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 14:26:51.000000 pymcabc-0.3.0/pymcabc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 14:26:51.880414 pymcabc-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-25 14:26:43.000000 pymcabc-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 14:26:51.876414 pymcabc-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_boost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_evengen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 14:26:43.000000 pymcabc-0.3.0/tests/test_plot.py
```

### Comparing `pymcabc-0.2.0/LICENSE` & `pymcabc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcabc-0.2.0/PKG-INFO` & `pymcabc-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.2.0
+Version: 0.3.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.2.0/README.md` & `pymcabc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pymcabc-0.2.0/pymcabc/cross_section.py` & `pymcabc-0.3.0/pymcabc/cross_section.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.2.0/pymcabc/decay_particle.py` & `pymcabc-0.3.0/pymcabc/decay_particle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,143 @@
 import math
 import random
 import json
-import numpy as np
 import pymcabc.constants
 from pymcabc.particle import Particle
 
 
 class DecayParticle:
     """
     decays particle
     """
 
     def __init__(self):
-        # self.Ecm = library["Ecm"][0]
         with open("library.json", "r") as f:
             library = json.load(f)
         self.mA = library["mA"][0]
         self.mB = library["mB"][0]
         self.mC = library["mC"][0]
         self.decay_process = library["decay_process"][0]
         self.decay1_mass = library["decay1_mass"][0]
         self.decay2_mass = library["decay2_mass"][0]
         self.massive = library["massive_mass"][0]
         self.delta = pymcabc.constants.delta
 
-    def rotate(self, pdecay: Particle, size: int):
+    def rotate(self, pdecay: Particle):
         """rotate particle"""
-        costh = (np.random.rand(size) * 2) - 1
-        sinth = np.sqrt(1 - costh**2)
-        phi = 2 * math.pi * np.random.rand(size)
-        sinPhi = np.sin(phi)
-        cosPhi = np.cos(phi)
+        costh = (2*random.random()) - 1
+        sinth = math.sqrt(1 - costh**2)
+        phi = 2 * math.pi * random.random()
+        sinPhi = math.sin(phi)
+        cosPhi = math.cos(phi)
+        pdecay_out = Particle(0,0,0,0)
+        pdecay_out.px = pdecay.pz * sinth *cosPhi
+        pdecay_out.py = pdecay.pz * sinth *sinPhi
+        pdecay_out.pz = pdecay.pz * costh
+        pdecay_out.E = pdecay.E 
+        
+        return pdecay_out
 
-        pdecay.px = pdecay.px * cosPhi - pdecay.py * sinPhi
-        pdecay.py = pdecay.px * sinPhi + pdecay.py * cosPhi
+    def decay(self, top: Particle):
+        """decay particle"""
 
-        pdecay.px = pdecay.px * costh - pdecay.pz * sinth
-        pdecay.pz = pdecay.px * sinth + pdecay.pz * costh
+        E1 = (top.mass()**2 - self.decay2_mass**2 + self.decay1_mass**2)/(2*top.mass())
+        
+        E2 =  top.mass() - E1
 
-        return pdecay
+        self.decay_p = math.sqrt((top.mass()**2  - (self.decay1_mass + self.decay2_mass)**2) * (top.mass()**2  - (self.decay1_mass - self.decay2_mass)**2)) / (2*top.mass())
 
-    def decay(self, top: Particle):
-        """decay particle"""
+        """ 
         self.decay_p = (
             1
             / (2 * top.mass())
-            * np.sqrt(
+            * math.sqrt(
                 (self.mA**4 + self.mB**4 + self.mC**4)
                 - 2
                 * (
                     self.mA**2 * self.mB**2
                     + self.mA**2 * self.mC**2
                     + self.mB**2 * self.mC**2
                 )
             )
         )
 
-        decay1 = Particle(-9, -9, -9, -9)
-        decay2 = Particle(-9, -9, -9, -9)
         # decay2.mass() = self.decay2_mass
 
-        E1 = np.sqrt(
+        E1 = math.sqrt(
             self.decay1_mass * self.decay1_mass + self.decay_p * self.decay_p
-        ) * np.ones(top.E.shape[0])
-        E2 = np.sqrt(
+        ) 
+        E2 = math.sqrt(
             self.decay2_mass * self.decay2_mass + self.decay_p * self.decay_p
-        ) * np.ones(top.E.shape[0])
+        ) 
+        """
 
-        decay1.set4momenta(E1, 0, self.decay_p, 0)
-        decay2.set4momenta(E2, 0, -self.decay_p, 0)
+        decay1 = Particle(0,0,0,0)
+        decay2 = Particle(0,0,0,0)
 
-        decay1 = self.rotate(decay1, size=top.E.shape[0])
-        decay2 = self.rotate(decay2, size=top.E.shape[0])
+        decay1.set4momenta(E1, 0, 0, self.decay_p)
+        decay2.set4momenta(E2, 0, 0, -self.decay_p)
+
+        decay1 = self.rotate(decay1)
+        decay2.set4momenta(E2, -decay1.px, -decay1.py, -decay1.pz)
+        #decay2 = self.rotate(decay2)
 
         return decay1, decay2
 
     def nearlyequal(self, a, b):
-        if abs(a - b) < 0.001:
+        if abs(a - b) < 1e-3:
             return True
         else:
             return False
 
     def prepare_decay(self, top: Particle):
         if self.decay_process != "NaN":
             # decay_process = decay_process.replace(" < "," ")
             # decay_process = decay_process.split(" ")
             # print(top.mass()[0], self.massive)
-            if self.nearlyequal(top.mass()[0], self.massive) and top.mass()[0] > (
-                self.decay1_mass + self.decay2_mass
-            ):
-                decay1, decay2 = self.decay(top)
-                decay1 = decay1.boost(top)
-                decay2 = decay2.boost(top)
-                return decay1, decay2
-            else:
-                output = np.ones(top.E.size) * (-9)
-                decay1 = Particle(output, output, output, output)
-                decay2 = Particle(output, output, output, output)
-                return decay1, decay2
+            decay_array1_px = [0]*len(top.px)
+            decay_array1_py = [0]*len(top.px)
+            decay_array1_pz = [0]*len(top.px)
+            decay_array1_E = [0]*len(top.px)
+
+            decay_array2_px = [0]*len(top.px)
+            decay_array2_py = [0]*len(top.px)
+            decay_array2_pz = [0]*len(top.px)
+            decay_array2_E = [0]*len(top.px)
+
+            for i in range(len(top.px)):
+                heavy_state = Particle(top.E[i],top.px[i], top.py[i],top.pz[i])
+                if self.nearlyequal(heavy_state.mass(), self.massive) and heavy_state.mass() > (
+                    self.decay1_mass + self.decay2_mass
+                ):
+
+                    decay1, decay2 = self.decay(heavy_state)
+                    decay1 = decay1.boost(heavy_state)
+                    decay2 = decay2.boost(heavy_state)
+                    
+                    decay_array1_px[i] = decay1.px
+                    decay_array1_py[i] = decay1.py
+                    decay_array1_pz[i] = decay1.pz
+                    decay_array1_E[i] = decay1.E
+
+                    decay_array2_px[i] = decay2.px
+                    decay_array2_py[i] = decay2.py
+                    decay_array2_pz[i] = decay2.pz
+                    decay_array2_E[i] = decay2.E
+                else:
+                    output = -9
+                    decay_array1_px[i] = output
+                    decay_array1_py[i] = output
+                    decay_array1_pz[i] = output
+                    decay_array1_E[i] = output
+
+                    decay_array2_px[i] = output
+                    decay_array2_py[i] = output
+                    decay_array2_pz[i] = output
+                    decay_array2_E[i] = output
+            
+            decay1 = Particle(decay_array1_E,decay_array1_px, decay_array1_py, decay_array1_pz)
+            decay2 = Particle(decay_array2_E,decay_array2_px, decay_array2_py, decay_array2_pz)
+            return decay1, decay2
+
+
+
```

### Comparing `pymcabc-0.2.0/pymcabc/feynman_diagram.py` & `pymcabc-0.3.0/pymcabc/feynman_diagram.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,24 +11,35 @@
 
     def __init__(self):
         with open("library.json", "r") as f:
             library = json.load(f)
 
         process = library["process"]
         mediator = library["mediator"][0]
+        channel = library["channel"][0]
         process = process[0].replace(">", mediator)
         self.process = process.split()
-
-        for p in library["process_type"][0]:
-            if p == "s":
-                self.s_chan()
-            elif p == "t":
-                self.t_chan()
-            elif p == "u":
-                self.u_chan()
+        if channel == "none":
+            for p in library["process_type"][0]:
+                if p == "s":
+                    self.s_chan()
+                elif p == "t":
+                    self.t_chan()
+                elif p == "u":
+                    self.u_chan()
+                else:
+                    print("Possible channels: s, t, and u")
+                    return 0
+        else:
+            if channel == "s":
+                    self.s_chan()
+            if channel == "t":
+                    self.t_chan()
+            if channel == "u":
+                    self.u_chan()
             else:
                 print("Possible channels: s, t, and u")
                 return
 
     def s_chan(self):
         fig = plt.figure(figsize=(5.0, 5.0))
         ax = fig.add_axes([0, 0, 1, 1], frameon=False)
```

### Comparing `pymcabc-0.2.0/pymcabc/generate_event.py` & `pymcabc-0.3.0/pymcabc/generate_event.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.2.0/pymcabc/identify_process.py` & `pymcabc-0.3.0/pymcabc/identify_process.py`

 * *Files identical despite different names*

### Comparing `pymcabc-0.2.0/pymcabc/particle.py` & `pymcabc-0.3.0/pymcabc/particle.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,48 +56,61 @@
 
     def pT(self):
         """returns particle's transverse momentum"""
         return np.sqrt(self.px**2 + self.py**2)
 
     def mass(self):
         """returns particle's mass"""
-        # try:
-        #    x = math.sqrt(self.E**2 - sum([self.px**2, self.py**2, self.pz**2]))
-        #    return x
-        # except:
-        #    return 0
-        x = self.E**2 - self.px**2 - self.py**2 - self.pz**2
-        if x[0] < 0:
-            x = np.zeros(self.E.size())
-        else:
-            x = np.sqrt(x)
+        try:
+            x = self.E**2 - self.px**2 - self.py**2 - self.pz**2
+            if x < 0:
+                x = 0
+            else:
+                x = math.sqrt(x)
+        except:
+            x = [0]*len(self.px)
+            for i in range(len(x)):
+                x[i] = self.E[i]**2 - self.px[i]**2 - self.py[i]**2 - self.pz[i]**2
+                print(x[i])
+                if x[i] < 0:
+                    x[i] = 0
+                else:
+                    x[i] = math.sqrt(x)
         return x
 
     def set4momenta(self, new_E, new_px, new_py, new_pz):
         """assign new four momentum to an existing particle"""
         self.px = new_px
         self.py = new_py
         self.pz = new_pz
         self.E = new_E
 
     def boost(self, other):
         """
         boosts a particle four momentum.
          # boost motivated from ROOT TLorentzVector class
+
+         other is used to boost
         """
-        new = Particle(-9, -9, -9, -9)
-        new_other = Particle(-9, -9, -9, -9)
+        new = Particle(0., 0., 0., 0.)
+        new_other = Particle(0., 0., 0., 0.)
+        
         new_other.set4momenta(
             other.E, other.px / other.E, other.py / other.E, other.pz / other.E
         )
-        beta = new_other.p()
-        gamma = 1.0 / np.sqrt(1 - beta**2)
-        gamma_2 = (gamma - 1.0) / beta
+        beta = new_other.p2()
+        gamma = 1.0 / math.sqrt(1.0 - beta)
+
+        if beta>0:
+            gamma_2 = (gamma - 1.0) / beta
+        else:
+            gamma_2 = 0.0
+
 
         dotproduct = (
             self.px * new_other.px + self.py * new_other.py + self.pz * new_other.pz
         )
         new.px = self.px + (gamma_2 * dotproduct + gamma * self.E) * new_other.px
         new.py = self.py + (gamma_2 * dotproduct + gamma * self.E) * new_other.py
         new.pz = self.pz + (gamma_2 * dotproduct + gamma * self.E) * new_other.pz
         new.E = gamma * (self.E + dotproduct)
-        return new
+        return new
```

### Comparing `pymcabc-0.2.0/pymcabc/plotting.py` & `pymcabc-0.3.0/pymcabc/plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     def plot(data, key):
         plt.hist(data, bins=40, color=None)
         label = key.replace("_", " ")
         plt.xlabel(label)
         plt.ylabel("Events")
-        plt.show()
+        #plt.show()
         plt.savefig(key + ".png")
 
     def file(filename="ABC_events.root"):
         # if ".root" in filename:
         file = uproot.open(filename)
         tree = file["events"]
         branches = tree.arrays()
```

### Comparing `pymcabc-0.2.0/pymcabc/save_events.py` & `pymcabc-0.3.0/pymcabc/save_events.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,24 +20,29 @@
 
     def __init__(
         self,
         Nevent: int,
         boolDecay: bool = True,
         boolDetector: bool = True,
         boolTruth: bool = True,
+        detector_sigma = 1.,
+        detector_factor=1.,
     ):
         """
          saving events
         Parameters:
             Nevent (int): number of events to generate
             boolDecay (bool): optional.  decay particles or not
             boolDetector (bool): optional.  gaussian smearing on particles
             boolTruth (bool): optional.  save truth events
         """
         self.Nevent = Nevent
+        self.detector_sigma  = detector_sigma
+        self.detector_factor  = detector_factor
+
         with open("library.json", "r") as f:
             library = json.load(f)
         self.w_max = library["w_max"][0]
         self.Ecm = library["Ecm"][0]
         input_string = library["process"][0]
         input_string = input_string.replace(" > ", " ")
         input_string = input_string.split(" ")
@@ -83,16 +88,16 @@
                 self.output_2 + "_Px": self.top2.px,
                 self.output_2 + "_Py": self.top2.py,
                 self.output_2 + "_Pz": self.top2.pz,
             }
 
         if self.boolDecay == False or self.decay_process == "NaN":
             if self.boolDetector == True:
-                self.top1 = Detector().gauss_smear(self.top1)
-                self.top2 = Detector().gauss_smear(self.top2)
+                self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
+                self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
 
             file = uproot.recreate(name)
             file["events"] = {
                 self.output_1 + "_E": self.top1.E,
                 self.output_1 + "_Px": self.top1.px,
                 self.output_1 + "_Py": self.top1.py,
                 self.output_1 + "_Pz": self.top1.pz,
@@ -103,25 +108,27 @@
             }
         else:
             file = uproot.recreate(name)
             top1 = self.top1
             top2 = self.top2
             decay1, decay2 = DecayParticle().prepare_decay(top1)
             decay3, decay4 = DecayParticle().prepare_decay(top2)
-
             if self.boolDetector == True:
-                # if decay1.px[0] == -9 and decay1.E[0] == -9:
-                self.top1 = Detector().gauss_smear(self.top1)
-                # if decay2.px[0] == -9 and decay2.E[0] == -9:
-                self.top2 = Detector().gauss_smear(self.top2)
-                # else:
-                decay1 = Detector().gauss_smear(decay1)
-                decay2 = Detector().gauss_smear(decay2)
-                decay3 = Detector().gauss_smear(decay3)
-                decay4 = Detector().gauss_smear(decay4)
+
+                if decay1.px[0] == -9 and decay1.E[0] == -9:
+                    self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
+                if decay2.px[0] == -9 and decay2.E[0] == -9:
+                    self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
+                #self.top1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top1)
+                #self.top2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(self.top2)
+
+                decay1 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay1)
+                decay2 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay2)
+                decay3 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay3)
+                decay4 = Detector(self.detector_sigma,self.detector_factor).gauss_smear(decay4)
 
             file["events"] = {
                 self.output_1 + "_E": self.top1.E,
                 self.output_1 + "_Px": self.top1.px,
                 self.output_1 + "_Py": self.top1.py,
                 self.output_1 + "_Pz": self.top1.pz,
                 self.output_1 + "_E_decay_" + self.decayed1: decay1.E,
@@ -140,40 +147,8 @@
                 self.output_2 + "_Px_decay_" + self.decayed1: decay3.px,
                 self.output_2 + "_Py_decay_" + self.decayed1: decay3.py,
                 self.output_2 + "_Pz_decay_" + self.decayed1: decay3.pz,
                 self.output_2 + "_E_decay_" + self.decayed2: decay4.E,
                 self.output_2 + "_Px_decay_" + self.decayed2: decay4.px,
                 self.output_2 + "_Py_decay_" + self.decayed2: decay4.py,
                 self.output_2 + "_Pz_decay_" + self.decayed2: decay4.pz,
-            }
-
-
-"""drop support for csv file
-    def to_csv(self):
-
-        data = list(
-            zip(
-                self.top1.E,
-                self.top1.px,
-                self.top1.py,
-                self.top1.pz,
-                self.top2.e,
-                self.top2.px,
-                self.top2.py,
-                self.top2.pz,
-            )
-        )
-
-        column_name = [
-            self.output_1 + "_Energy",
-            self.output_1 + "_Px",
-            self.output_1 + "_Py",
-            self.output_1 + "_Pz",
-            self.output_2 + "_E",
-            self.output_2 + "_Px",
-            self.output_2 + "_Py",
-            self.output_2 + "_Pz",
-        ]
-        df = pd.DataFrame(data, columns=column_name)
-        df.reset_index(drop=True, inplace=True)
-        df.to_csv("ABC_events.csv", index=False)
-"""
+            }
```

### Comparing `pymcabc-0.2.0/pymcabc.egg-info/PKG-INFO` & `pymcabc-0.3.0/pymcabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcabc
-Version: 0.2.0
+Version: 0.3.0
 Summary: Monte Carlo Event Generator for the ABC theory
 Home-page: https://github.com/amanmdesai/pymcabc
 Author: Aman Desai
 Author-email: amanmukeshdesai@gmail.com
 Maintainer: Aman Desai
 Maintainer-email: amanmukeshdesai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymcabc-0.2.0/setup.py` & `pymcabc-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md','r') as file:
     long_description = file.read()
 
 setuptools.setup(
 name="pymcabc",
-version="0.2.0",
+version="0.3.0",
 description= "Monte Carlo Event Generator for the ABC theory",
 author="Aman Desai",
 author_email="amanmukeshdesai@gmail.com",
 maintainer="Aman Desai",
 maintainer_email="amanmukeshdesai@gmail.com",
 url = "https://github.com/amanmdesai/pymcabc",
 long_description=long_description,
```

