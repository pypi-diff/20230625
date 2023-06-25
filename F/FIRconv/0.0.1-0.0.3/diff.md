# Comparing `tmp/FIRconv-0.0.1.tar.gz` & `tmp/FIRconv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\FIRconv-0.0.1.tar", last modified: Sun Mar 12 17:40:23 2023, max compression
+gzip compressed data, was "FIRconv-0.0.3.tar", last modified: Sun Jun 25 16:23:16 2023, max compression
```

## Comparing `FIRconv-0.0.1.tar` & `FIRconv-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 17:40:23.000000 FIRconv-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv/
--rw-rw-rw-   0        0        0    16595 2023-03-12 13:48:40.000000 FIRconv-0.0.1/FIRconv/FIRconv.py
--rw-rw-rw-   0        0        0       22 2023-03-12 17:14:23.000000 FIRconv-0.0.1/FIRconv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-03-12 17:40:23.000000 FIRconv-0.0.1/FIRconv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3321 2023-03-12 17:40:23.000000 FIRconv-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2240 2023-03-12 16:39:44.000000 FIRconv-0.0.1/README.md
--rw-rw-rw-   0        0        0      677 2023-03-12 17:40:23.000000 FIRconv-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-03-12 17:40:04.000000 FIRconv-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-12 17:40:23.000000 FIRconv-0.0.1/tests/
--rw-rw-rw-   0        0        0     2282 2023-03-12 13:50:37.000000 FIRconv-0.0.1/tests/ALgorithms_validation.py
--rw-rw-rw-   0        0        0     1842 2023-03-12 13:50:27.000000 FIRconv-0.0.1/tests/testFIR.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:23:16.697563 FIRconv-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-25 16:23:16.679364 FIRconv-0.0.3/FIRconv/
+-rw-rw-rw-   0        0        0    17293 2023-06-25 15:23:33.000000 FIRconv-0.0.3/FIRconv/FIRconv.py
+-rw-rw-rw-   0        0        0       22 2023-05-09 21:48:03.000000 FIRconv-0.0.3/FIRconv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:23:16.695731 FIRconv-0.0.3/FIRconv.egg-info/
+-rw-rw-rw-   0        0        0     2799 2023-06-25 16:23:16.000000 FIRconv-0.0.3/FIRconv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-25 16:23:16.000000 FIRconv-0.0.3/FIRconv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:23:16.000000 FIRconv-0.0.3/FIRconv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-25 16:23:16.000000 FIRconv-0.0.3/FIRconv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-25 16:23:16.000000 FIRconv-0.0.3/FIRconv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-05-09 21:48:03.000000 FIRconv-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2799 2023-06-25 16:23:16.698134 FIRconv-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2241 2023-05-09 21:48:03.000000 FIRconv-0.0.3/README.md
+-rw-rw-rw-   0        0        0      677 2023-06-25 16:23:16.709859 FIRconv-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-06-25 16:22:14.000000 FIRconv-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `FIRconv-0.0.1/FIRconv/FIRconv.py` & `FIRconv-0.0.3/FIRconv/FIRconv.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,22 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 '''
 
 import numpy as np
-from numpy.core.numeric import Inf
 from numpy.fft import fft, ifft
 from copy import deepcopy
 
 
 class FIRfilter:
-    def __init__(self, method="overlap-save", blockSize=512, h=None, partition=None, normalize=True):
+    def __init__(self, method="overlap-save", blockSize=512, h=None, partition=None, normalize=True, xfadeLen=None):
         '''
-        Performs real-time convolution via FIR filters. This class is a wrapper for the pyFIRfilter()
+        Performs real-time convolution with FIR filters. This class is a wrapper for the pyFIRfilter()
         which allows for smooth crossover when changing filters at runtime. For most cases this class
         should be prefered.
 
         Parameters
         ----------
         method : str, optional
             The FIR method to use, available ones are 'overlap-save', 'overlap-add',
@@ -54,37 +53,43 @@
         partition : int, optional
             Partition size for the UPOLS filter. For general use it is recommended that
             you supply the impulse response instead of the partion size at class initilization,
             by doing this, the optimal partition size will be calculated by default.
         normalize : bool, optional
             Indicate if output should be normalized or not. If True the frame output is going to
             be normalized to be below 1. The default is True.
+        xfadeLen : int, optional 
+            Sets the length of the crossfading when switching filters. If None it is set to 
+            (block_size / 2)
 
         Returns
         -------
         FIRfilter.process(x, h) returns the convolution of block x with impulse response h.
         Output has the same size as x and type: np.array
 
         '''
         self.B = blockSize
         self.currentFIR = pyFIRfilter(method, blockSize, h, partition, normalize)
         self.futureFIR = pyFIRfilter(method, blockSize, h, partition, normalize)
-        # self.Xfader = Crossfader(N_cross=B, N_ch=self.N_ch)
+
         self.current_h = h
         self.flagIRchanged = False
         self.lockXfade = False  # it will only allow for new position after crossfading in done
-
+        if xfadeLen is None:
+            self.xfadeLen = self.B//2
+        else:
+            self.xfadeLen = xfadeLen
     def process(self, x, h=None):
         # initialize crossfader now that we know the number of channels in the input
         if not hasattr(self, 'Xfader'):
             if np.ndim(x) == 0:
                 Nch = 1
             else:
                 Nch = x.shape[-1]
-            self.Xfader = Crossfader(N_cross=2*self.B, N_ch=Nch)
+            self.Xfader = Crossfader(N_cross=self.xfadeLen, N_ch=Nch)
 
 
         if h is not None and np.any(h != self.current_h):   # check if the impulse response h has changed
             self.flagIRchanged = True
 
         if self.flagIRchanged and not self.lockXfade:
             self.future_h = h
@@ -113,28 +118,29 @@
     '''
     Simple FIR object.
     '''
     def __init__(self, method, blockSize, h, partition, normalize):
         self.method = method.lower()
         self.B = blockSize                # block size (audio input len, which will also be the output size)
         self.stored_h = h        # save IR for comparison next frame (optional input)
-        self.partition = partition  # partition size (UPOLS)
+        self.LEN_partitions = partition  # partition size (UPOLS)
         self.normalize = normalize
         self.NFFT = None          # fft/ifft size
         self.flagHchanged = True  # check if the IR changed or it's still the same
         self.Nh = h.shape[0]
+        self.input_buffer = None
         self._generate_ref()
 
         validMethods = ['overlap-save', 'overlap-add', 'ols', 'ola', 'upols']
         error_msg = f'Unknown FIRfilter method: "{self.method}", \n Supported methods are: {validMethods}'
         assert self.method in validMethods, error_msg
 
         if ('upols' in self.method) and (partition is None) and (h is not None):
-            self.partition, self.NFFT = self._optimize_UPOLS_parameters(self.Nh, self.B)
-            # print(f'partition size: {self.partition} \n nfft: {self.NFFT}')
+            self.LEN_partitions, self.NFFT = self._optimize_UPOLS_parameters(self.Nh, self.B)
+            # print(f'partition size: {self.LEN_partitions} \n nfft: {self.NFFT}')
 
     def _pad_the_end(self, x, new_length):
         if x.shape[0] < new_length:
             output = np.squeeze(np.zeros((new_length, self.N_ch)))
             output[:x.shape[0], ...] = x
         else:
             output = x
@@ -166,17 +172,17 @@
     def _optimize_UPOLS_parameters(self, N, B):
         '''brute-force the optimal parameters for UPOLS
             N: IR length
             B: buffer size
         '''
         def cost(B, N, L, K):
             # theoretical time estimates for each operation, pag. 211
-            return 1 / B * (1.68 * K * np.log2(K) + 3.49 * K * np.log2(K) + 6 * ((K + 1) / 2) + ((N / L) - 1) * 8 * ((K + 1) / 2))
+            return 1. / B * (1.68 * K * np.log2(K) + 3.49 * K * np.log2(K) + 6. * ((K + 1.) / 2.) + ((N / L) - 1.) * 8. * ((K + 1.) / 2.))
 
-        c_opt = Inf
+        c_opt = np.Inf
         rang = np.array([2**k for k in range(0, int(np.log2(N)))]).astype('int')
         for L in rang:
             d_max = B - np.gcd(L, B)
             K_min = int(B + L + d_max - 1)
             K_max = int(2**np.ceil(np.log2(K_min)))
             k_sort = np.sort([K_min, K_max])
             if k_sort[0] == k_sort[1]:
@@ -196,26 +202,26 @@
         if self.flagHchanged:  # store the IR fft
             self.H = fft(self.stored_h, self.NFFT, axis=0)
             self.flagHchanged = False
         return ifft(X * self.H, axis=0).real
 
     def _OLA(self, x):
         if self.NFFT is None:
-            self.NFFT = self.B + self.stored_h.shape[0] - 1
+            self.NFFT = self.B + self.Nh - 1
             self.left_overs = np.squeeze(np.zeros((self.NFFT, self.N_ch)))
             self.len_y_left = self.NFFT - self.B
 
         # Fast convolution
         y = self._fft_conv(x)
 
         # Overlap-Add the partial convolution result
         out = y[:self.B, ...] + self.left_overs[:self.B, ...]
 
         self.left_overs = np.roll(self.left_overs, -self.B, axis=0)  # flush the buffer
-        self.left_overs[-self.B:, ...] = 0
+        self.left_overs[-self.B:, ...] = 0.
         self.left_overs[:self.len_y_left, ...] = self.left_overs[:self.len_y_left, ...] + y[self.B:, ...]
         if self.normalize:
             return self._normalize_output(out)
         else:
             return out
 
     def _OLS(self, x):
@@ -234,63 +240,58 @@
         if self.normalize:
             return self._normalize_output(out[-self.B:, ...])
         else:
             return out[-self.B:, ...]
 
     def _UPOLS(self, x, h):
         if self.flagHchanged:  # only run on on initial call
-            Nh = self.Nh
-            if self.partition is None:
+            if (self.LEN_partitions is None) or (self.NFFT is None):
                 print('Running UPOLS parameter optimization, this may take a few minutes to run deppending on the length of the impulse respose, to avoid this optimization prcedure, simply declare a "partition" value at the class initialization')
-                self.partition, self.NFFT = self._optimize_UPOLS_parameters(Nh, self.B)
-                L_partit = self.partition
-            else:
-                L_partit = self.partition
-                dmax = self.B - np.gcd(L_partit, self.B)
-                self.NFFT = self.B + L_partit + dmax
-
-            self.P = int(np.ceil(Nh / L_partit))  # number of partitions done
-            self.input_buffer = np.squeeze(np.zeros((self.NFFT, self.N_ch)))  # Initialize input buffer
-            # Initialize filter and FDL
-            self.nm = np.zeros((self.P,))  # tells us which FDL positions should be used
-            self.H = np.zeros((self.P, self.NFFT, self.N_ch), dtype='complex_')  # partitioned filters (freq domain)
-            if self.N_ch == 1:
-                self.H = np.squeeze(self.H, axis=-1)
+                self.LEN_partitions, self.NFFT = self._optimize_UPOLS_parameters(self.Nh, self.B)
+                # dmax = self.B - np.gcd(self.LEN_partitions, self.B)
+                # self.NFFT = self.B + self.LEN_partitions + dmax
+            elif self.input_buffer is None:  # initialize variables that depend only on the size of stuff
+                self.input_buffer = np.squeeze(np.zeros((self.NFFT, self.N_ch)))  # Initialize input buffer
+                self.N_partitions = int(np.ceil(self.Nh / self.LEN_partitions))  # number of partitions done
+                # Initialize filter and FDL
+                self.H = np.zeros((self.N_partitions, self.NFFT, self.N_ch), dtype=complex)  # partitioned filters (freq domain)
+                # calculate remainder delays
+                m = np.arange(self.N_partitions)
+                self.pre_delays = np.mod(m * self.LEN_partitions, self.B)    
+                self.active_FDL_idx = (m * self.LEN_partitions // self.B).astype(int)  # # tells us which FDL positions should be used (FDL active slots)        
+                self.FDL = np.zeros((max(self.active_FDL_idx) + 1, self.NFFT, self.N_ch), dtype=complex)  # delay line
+                if self.N_ch == 1:
+                    self.FDL = np.squeeze(self.FDL, axis=-1)
+                if np.ndim(self.FDL) == 1:
+                    self.FDL = np.expand_dims(self.FDL, axis=0)  # case self.active_FDL_idx==0
+                if self.N_ch == 1:
+                    self.H = np.squeeze(self.H, axis=-1)
 
             # (1) split original filter into P length-L sub filters
-            for m, ii in enumerate(range(0, Nh, L_partit)):
+            for m, ii in enumerate(range(0, self.Nh, self.LEN_partitions)):
                 try:
-                    h_partit = h[ii:(ii + L_partit), ...]
-                except Exception:
-                    h_partit = self._pad_the_end(h[ii:, ...], L_partit)
+                    h_partit = h[ii:(ii + self.LEN_partitions), ...]
+                except Exception:  # triggers length of IR is not a multiple of the number of partitions 
+                    h_partit = self._pad_the_end(h[ii:, ...], self.LEN_partitions)
 
                 # (2) incorporate "remainder delays"
-                dm = np.mod(m * L_partit, self.B)
-                h_pad = self._pad_beginning(h_partit, dm)
+                h_pad = self._pad_beginning(h_partit, self.pre_delays[m])
                 self.H[m, ...] = fft(h_pad, n=self.NFFT, axis=0)
-                self.nm[m] = np.floor(m * L_partit / self.B)  # FDL active slots
-            self.nm = self.nm.astype(int)
-            self.FDL = np.zeros((max(self.nm) + 1, self.NFFT, self.N_ch), dtype='complex_')  # delay line
-            if self.N_ch == 1:
-                self.FDL = np.squeeze(self.FDL, axis=-1)
-
-            if np.ndim(self.FDL) == 1:
-                self.FDL = np.expand_dims(self.FDL, axis=0)  # case self.nm==0
-
+            # Flag that the required changes have been made to accomodate the new filter
             self.flagHchanged = False
-
+            
         # (3) Sliding window of the input
         self.input_buffer = np.roll(self.input_buffer, shift=-self.B, axis=0)  # previous contents are shifted B samples to the left
         self.input_buffer[-self.B:, ...] = x  # next length-B input block is stored rightmost
         # (4) Stream
         self.FDL = np.roll(self.FDL, shift=1, axis=0)  # shift the FDL to create space for current input
         self.FDL[0, ...] = fft(self.input_buffer, axis=self.fftAxis)  # add current buffer to the first FDL slot
         # convo
         # note: the sum is done in the frequency domain (yep!)
-        out = ifft(np.sum(self.FDL[self.nm, ...] * self.H, axis=0), axis=self.fftAxis).real
+        out = ifft(np.sum(self.FDL[self.active_FDL_idx, ...] * self.H, axis=0), axis=self.fftAxis).real
 
         if self.normalize:
             return self._normalize_output(out[-self.B:, ...])
         else:
             return out[-self.B:]
 
     def process(self, x, h=None):
@@ -337,15 +338,15 @@
 
         '''
         if self.reset_faders:
             self._reset_fader_funcs()
 
         frame_sz = A.shape[0]
         # (1) - Case the length of the xfade is longer than the frame
-        if self.xfade_up.shape[0] > frame_sz:
+        if self.xfade_up.shape[0] >= frame_sz:
             C = (A * self.xfade_down[:frame_sz, ...]) + (B * self.xfade_up[:frame_sz, ...])
             # Delete the fader part that was already used
             self.xfade_up = np.delete(self.xfade_up, range(frame_sz), axis=0)
             self.xfade_down = np.delete(self.xfade_down, range(frame_sz), axis=0)
             self.isDone = False
 
         # (2) - Case the length of the xfade is smaller than the frame
```

### Comparing `FIRconv-0.0.1/FIRconv.egg-info/PKG-INFO` & `FIRconv-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,62 @@
-Metadata-Version: 2.1
-Name: FIRconv
-Version: 0.0.1
-Summary: Python implementation of real-time convolution for auralization
-Home-page: https://github.com/davircarvalho/FIRconv
-Author: Davi Carvalho
-Author-email: r.davicarvalho@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/davircarvalho/FIRconv/issues
-Description: # FIRconv
-        
-        <p align="left">
-          <a href="https://github.com/davircarvalho/FIRconv/releases/" target="_blank">
-            <img alt="GitHub release" src="https://img.shields.io/github/v/release/davircarvalho/FIRconv?include_prereleases&style=flat-square">
-          </a>
-        
-          <a href="https://github.com/davircarvalho/FIRconv/commits/master" target="_blank">
-            <img src="https://img.shields.io/github/last-commit/davircarvalho/FIRconv?style=flat-square" alt="GitHub last commit">
-          </a>
-        
-          <a href="https://github.com/davircarvalho/FIRconv/issues" target="_blank">
-            <img src="https://img.shields.io/github/issues/davircarvalho/FIRconv?style=flat-square&color=red" alt="GitHub issues">
-          </a>
-        
-          <a href="https://github.com/davircarvalho/FIRconv/blob/master/LICENSE" target="_blank">
-            <img alt="LICENSE" src="https://img.shields.io/github/license/davircarvalho/FIRconv?style=flat-square&color=yellow">
-          <a/>
-        
-        </p>
-        <hr>
-        
-        
-        Python implementations of Finite Impulse Response (FIR) filters for real-time convolutions.
-        
-        The algorithms are mainly *(but not strictly)* the ones described in **WEFERS, Frank. Partitioned convolution algorithms for real-time auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://publications.rwth-aachen.de/record/466561/files/466561.pdf?subformat=pdfa&version=1).
-        
-        
-        # Current algorithms
-        - Overlap-add (OLA);
-        - Overlap-save (OLS);
-        - Uniformily Partitioned Overlap-Save (UPOLS) (generalized version)
-        
-        # Instalation
-        Use pip to install FIRconv:
-        ```
-        $ pip install FIRconv
-        ```
-        
-        # Getting started
-        Bellow there's a pseudo-code showing how to setup a basic use of FIRconv for real time convolutions.
-        
-        ```python
-        from FIRconv import FIRfilter
-        import numpy as np
-        
-        # Initialize FIR filter
-        bufferSize = 2**10
-        method = 'upols'
-        FIRfilter(method, bufferSize, h=IR)
-        
-        while True:
-          output = FIRfilter.process(audio)
-          play(output)
-        
-        
-        ```
-        
-        
-        - For more in-depth examples have a look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/FIRconv/blob/main/Algorithms_validation.py)
-        ___________________________________________________________________
-        Collaborations are more than welcome!
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# FIRconv
+
+<p align="left">
+  <a href="https://github.com/davircarvalho/FIRconv/releases/" target="_blank">
+    <img alt="GitHub release" src="https://img.shields.io/github/v/release/davircarvalho/FIRconv?include_prereleases&style=flat-square">
+  </a>
+
+  <a href="https://github.com/davircarvalho/FIRconv/commits/master" target="_blank">
+    <img src="https://img.shields.io/github/last-commit/davircarvalho/FIRconv?style=flat-square" alt="GitHub last commit">
+  </a>
+
+  <a href="https://github.com/davircarvalho/FIRconv/issues" target="_blank">
+    <img src="https://img.shields.io/github/issues/davircarvalho/FIRconv?style=flat-square&color=red" alt="GitHub issues">
+  </a>
+
+  <a href="https://github.com/davircarvalho/FIRconv/blob/master/LICENSE" target="_blank">
+    <img alt="LICENSE" src="https://img.shields.io/github/license/davircarvalho/FIRconv?style=flat-square&color=yellow">
+  <a/>
+
+</p>
+<hr>
+
+
+Python implementations of Finite Impulse Response (FIR) filters for real-time convolutions.
+
+The algorithms are mainly *(but not strictly)* the ones described in **WEFERS, Frank. Partitioned convolution algorithms for real-time auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://publications.rwth-aachen.de/record/466561/files/466561.pdf?subformat=pdfa&version=1).
+
+
+# Current algorithms
+- Overlap-add (OLA);
+- Overlap-save (OLS);
+- Uniformily Partitioned Overlap-Save (UPOLS) (generalized version)
+
+# Installation
+Use pip to install FIRconv:
+```
+$ pip install FIRconv
+```
+
+# Getting started
+Bellow there's a pseudo-code showing how to setup a basic use of FIRconv for real time convolutions.
+
+```python
+from FIRconv import FIRfilter
+import numpy as np
+
+# Initialize FIR filter
+bufferSize = 2**10
+method = 'upols'
+FIRfilter(method, bufferSize, h=IR)
+
+while True:
+  output = FIRfilter.process(audio)
+  play(output)
+
+
+```
+
+
+- For more in-depth examples have a look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/FIRconv/blob/main/Algorithms_validation.py)
+___________________________________________________________________
+Collaborations are more than welcome!
```

#### html2text {}

```diff
@@ -1,29 +1,22 @@
-Metadata-Version: 2.1 Name: FIRconv Version: 0.0.1 Summary: Python
-implementation of real-time convolution for auralization Home-page: https://
-github.com/davircarvalho/FIRconv Author: Davi Carvalho Author-email:
-r.davicarvalho@gmail.com License: UNKNOWN Project-URL: Bug Tracker, https://
-github.com/davircarvalho/FIRconv/issues Description: # FIRconv
+# FIRconv
 [GitHub_release] [GitHub_last_commit] [GitHub_issues]
 [LICENSE]
 ===============================================================================
 Python implementations of Finite Impulse Response (FIR) filters for real-time
 convolutions. The algorithms are mainly *(but not strictly)* the ones described
 in **WEFERS, Frank. Partitioned convolution algorithms for real-time
 auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://
 publications.rwth-aachen.de/record/466561/files/
 466561.pdf?subformat=pdfa&version=1). # Current algorithms - Overlap-add (OLA);
 - Overlap-save (OLS); - Uniformily Partitioned Overlap-Save (UPOLS)
-(generalized version) # Instalation Use pip to install FIRconv: ``` $ pip
+(generalized version) # Installation Use pip to install FIRconv: ``` $ pip
 install FIRconv ``` # Getting started Bellow there's a pseudo-code showing how
 to setup a basic use of FIRconv for real time convolutions. ```python from
 FIRconv import FIRfilter import numpy as np # Initialize FIR filter bufferSize
 = 2**10 method = 'upols' FIRfilter(method, bufferSize, h=IR) while True: output
 = FIRfilter.process(audio) play(output) ``` - For more in-depth examples have a
 look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/
 testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/
 FIRconv/blob/main/Algorithms_validation.py)
 ___________________________________________________________________
-Collaborations are more than welcome! Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Collaborations are more than welcome!
```

### Comparing `FIRconv-0.0.1/PKG-INFO` & `FIRconv-0.0.3/FIRconv.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,77 @@
 Metadata-Version: 2.1
 Name: FIRconv
-Version: 0.0.1
+Version: 0.0.3
 Summary: Python implementation of real-time convolution for auralization
 Home-page: https://github.com/davircarvalho/FIRconv
 Author: Davi Carvalho
 Author-email: r.davicarvalho@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davircarvalho/FIRconv/issues
-Description: # FIRconv
-        
-        <p align="left">
-          <a href="https://github.com/davircarvalho/FIRconv/releases/" target="_blank">
-            <img alt="GitHub release" src="https://img.shields.io/github/v/release/davircarvalho/FIRconv?include_prereleases&style=flat-square">
-          </a>
-        
-          <a href="https://github.com/davircarvalho/FIRconv/commits/master" target="_blank">
-            <img src="https://img.shields.io/github/last-commit/davircarvalho/FIRconv?style=flat-square" alt="GitHub last commit">
-          </a>
-        
-          <a href="https://github.com/davircarvalho/FIRconv/issues" target="_blank">
-            <img src="https://img.shields.io/github/issues/davircarvalho/FIRconv?style=flat-square&color=red" alt="GitHub issues">
-          </a>
-        
-          <a href="https://github.com/davircarvalho/FIRconv/blob/master/LICENSE" target="_blank">
-            <img alt="LICENSE" src="https://img.shields.io/github/license/davircarvalho/FIRconv?style=flat-square&color=yellow">
-          <a/>
-        
-        </p>
-        <hr>
-        
-        
-        Python implementations of Finite Impulse Response (FIR) filters for real-time convolutions.
-        
-        The algorithms are mainly *(but not strictly)* the ones described in **WEFERS, Frank. Partitioned convolution algorithms for real-time auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://publications.rwth-aachen.de/record/466561/files/466561.pdf?subformat=pdfa&version=1).
-        
-        
-        # Current algorithms
-        - Overlap-add (OLA);
-        - Overlap-save (OLS);
-        - Uniformily Partitioned Overlap-Save (UPOLS) (generalized version)
-        
-        # Instalation
-        Use pip to install FIRconv:
-        ```
-        $ pip install FIRconv
-        ```
-        
-        # Getting started
-        Bellow there's a pseudo-code showing how to setup a basic use of FIRconv for real time convolutions.
-        
-        ```python
-        from FIRconv import FIRfilter
-        import numpy as np
-        
-        # Initialize FIR filter
-        bufferSize = 2**10
-        method = 'upols'
-        FIRfilter(method, bufferSize, h=IR)
-        
-        while True:
-          output = FIRfilter.process(audio)
-          play(output)
-        
-        
-        ```
-        
-        
-        - For more in-depth examples have a look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/FIRconv/blob/main/Algorithms_validation.py)
-        ___________________________________________________________________
-        Collaborations are more than welcome!
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FIRconv
+
+<p align="left">
+  <a href="https://github.com/davircarvalho/FIRconv/releases/" target="_blank">
+    <img alt="GitHub release" src="https://img.shields.io/github/v/release/davircarvalho/FIRconv?include_prereleases&style=flat-square">
+  </a>
+
+  <a href="https://github.com/davircarvalho/FIRconv/commits/master" target="_blank">
+    <img src="https://img.shields.io/github/last-commit/davircarvalho/FIRconv?style=flat-square" alt="GitHub last commit">
+  </a>
+
+  <a href="https://github.com/davircarvalho/FIRconv/issues" target="_blank">
+    <img src="https://img.shields.io/github/issues/davircarvalho/FIRconv?style=flat-square&color=red" alt="GitHub issues">
+  </a>
+
+  <a href="https://github.com/davircarvalho/FIRconv/blob/master/LICENSE" target="_blank">
+    <img alt="LICENSE" src="https://img.shields.io/github/license/davircarvalho/FIRconv?style=flat-square&color=yellow">
+  <a/>
+
+</p>
+<hr>
+
+
+Python implementations of Finite Impulse Response (FIR) filters for real-time convolutions.
+
+The algorithms are mainly *(but not strictly)* the ones described in **WEFERS, Frank. Partitioned convolution algorithms for real-time auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://publications.rwth-aachen.de/record/466561/files/466561.pdf?subformat=pdfa&version=1).
+
+
+# Current algorithms
+- Overlap-add (OLA);
+- Overlap-save (OLS);
+- Uniformily Partitioned Overlap-Save (UPOLS) (generalized version)
+
+# Installation
+Use pip to install FIRconv:
+```
+$ pip install FIRconv
+```
+
+# Getting started
+Bellow there's a pseudo-code showing how to setup a basic use of FIRconv for real time convolutions.
+
+```python
+from FIRconv import FIRfilter
+import numpy as np
+
+# Initialize FIR filter
+bufferSize = 2**10
+method = 'upols'
+FIRfilter(method, bufferSize, h=IR)
+
+while True:
+  output = FIRfilter.process(audio)
+  play(output)
+
+
+```
+
+
+- For more in-depth examples have a look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/FIRconv/blob/main/Algorithms_validation.py)
+___________________________________________________________________
+Collaborations are more than welcome!
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: FIRconv Version: 0.0.1 Summary: Python
+Metadata-Version: 2.1 Name: FIRconv Version: 0.0.3 Summary: Python
 implementation of real-time convolution for auralization Home-page: https://
 github.com/davircarvalho/FIRconv Author: Davi Carvalho Author-email:
-r.davicarvalho@gmail.com License: UNKNOWN Project-URL: Bug Tracker, https://
-github.com/davircarvalho/FIRconv/issues Description: # FIRconv
+r.davicarvalho@gmail.com Project-URL: Bug Tracker, https://github.com/
+davircarvalho/FIRconv/issues Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE # FIRconv
 [GitHub_release] [GitHub_last_commit] [GitHub_issues]
 [LICENSE]
 ===============================================================================
 Python implementations of Finite Impulse Response (FIR) filters for real-time
 convolutions. The algorithms are mainly *(but not strictly)* the ones described
 in **WEFERS, Frank. Partitioned convolution algorithms for real-time
 auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://
 publications.rwth-aachen.de/record/466561/files/
 466561.pdf?subformat=pdfa&version=1). # Current algorithms - Overlap-add (OLA);
 - Overlap-save (OLS); - Uniformily Partitioned Overlap-Save (UPOLS)
-(generalized version) # Instalation Use pip to install FIRconv: ``` $ pip
+(generalized version) # Installation Use pip to install FIRconv: ``` $ pip
 install FIRconv ``` # Getting started Bellow there's a pseudo-code showing how
 to setup a basic use of FIRconv for real time convolutions. ```python from
 FIRconv import FIRfilter import numpy as np # Initialize FIR filter bufferSize
 = 2**10 method = 'upols' FIRfilter(method, bufferSize, h=IR) while True: output
 = FIRfilter.process(audio) play(output) ``` - For more in-depth examples have a
 look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/
 testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/
 FIRconv/blob/main/Algorithms_validation.py)
 ___________________________________________________________________
-Collaborations are more than welcome! Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Collaborations are more than welcome!
```

### Comparing `FIRconv-0.0.1/README.md` & `FIRconv-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: FIRconv
+Version: 0.0.3
+Summary: Python implementation of real-time convolution for auralization
+Home-page: https://github.com/davircarvalho/FIRconv
+Author: Davi Carvalho
+Author-email: r.davicarvalho@gmail.com
+Project-URL: Bug Tracker, https://github.com/davircarvalho/FIRconv/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FIRconv
 
 <p align="left">
   <a href="https://github.com/davircarvalho/FIRconv/releases/" target="_blank">
     <img alt="GitHub release" src="https://img.shields.io/github/v/release/davircarvalho/FIRconv?include_prereleases&style=flat-square">
   </a>
 
@@ -27,15 +42,15 @@
 
 
 # Current algorithms
 - Overlap-add (OLA);
 - Overlap-save (OLS);
 - Uniformily Partitioned Overlap-Save (UPOLS) (generalized version)
 
-# Instalation
+# Installation
 Use pip to install FIRconv:
 ```
 $ pip install FIRconv
 ```
 
 # Getting started
 Bellow there's a pseudo-code showing how to setup a basic use of FIRconv for real time convolutions.
```

#### html2text {}

```diff
@@ -1,19 +1,26 @@
-# FIRconv
+Metadata-Version: 2.1 Name: FIRconv Version: 0.0.3 Summary: Python
+implementation of real-time convolution for auralization Home-page: https://
+github.com/davircarvalho/FIRconv Author: Davi Carvalho Author-email:
+r.davicarvalho@gmail.com Project-URL: Bug Tracker, https://github.com/
+davircarvalho/FIRconv/issues Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+markdown License-File: LICENSE # FIRconv
 [GitHub_release] [GitHub_last_commit] [GitHub_issues]
 [LICENSE]
 ===============================================================================
 Python implementations of Finite Impulse Response (FIR) filters for real-time
 convolutions. The algorithms are mainly *(but not strictly)* the ones described
 in **WEFERS, Frank. Partitioned convolution algorithms for real-time
 auralization. Logos Verlag Berlin GmbH, 2015**. found [here](http://
 publications.rwth-aachen.de/record/466561/files/
 466561.pdf?subformat=pdfa&version=1). # Current algorithms - Overlap-add (OLA);
 - Overlap-save (OLS); - Uniformily Partitioned Overlap-Save (UPOLS)
-(generalized version) # Instalation Use pip to install FIRconv: ``` $ pip
+(generalized version) # Installation Use pip to install FIRconv: ``` $ pip
 install FIRconv ``` # Getting started Bellow there's a pseudo-code showing how
 to setup a basic use of FIRconv for real time convolutions. ```python from
 FIRconv import FIRfilter import numpy as np # Initialize FIR filter bufferSize
 = 2**10 method = 'upols' FIRfilter(method, bufferSize, h=IR) while True: output
 = FIRfilter.process(audio) play(output) ``` - For more in-depth examples have a
 look at [testFIR.py](https://github.com/davircarvalho/FIRconv/blob/main/
 testFIR.py) or [Algorithms_validationpy](https://github.com/davircarvalho/
```

### Comparing `FIRconv-0.0.1/setup.cfg` & `FIRconv-0.0.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 4952 636f 6e76 0d0a 7665 7273   = FIRconv..vers
-00000020: 696f 6e20 3d20 302e 302e 310d 0a61 7574  ion = 0.0.1..aut
+00000020: 696f 6e20 3d20 302e 302e 330d 0a61 7574  ion = 0.0.3..aut
 00000030: 686f 7220 3d20 4461 7669 2043 6172 7661  hor = Davi Carva
 00000040: 6c68 6f0d 0a61 7574 686f 725f 656d 6169  lho..author_emai
 00000050: 6c20 3d20 722e 6461 7669 6361 7276 616c  l = r.davicarval
 00000060: 686f 4067 6d61 696c 2e63 6f6d 0d0a 6465  ho@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 5079 7468  scription = Pyth
 00000080: 6f6e 2069 6d70 6c65 6d65 6e74 6174 696f  on implementatio
 00000090: 6e20 6f66 2072 6561 6c2d 7469 6d65 2063  n of real-time c
```

### Comparing `FIRconv-0.0.1/setup.py` & `FIRconv-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name="FIRconv",
     description="Python implementation of real-time convolution for auralization",
     author="Davi Carvalho",
     url="https://github.com/davircarvalho/FIRconv",
     author_email="r.davicarvalho@gmail.com",
-    version="0.0.1",
+    version="0.0.3",
     install_requires=[
         "numpy"
         #"librosa",
         #"pyaudio",
         #"matplotlib"
     ],
     packages=find_namespace_packages(include='FIRconv.*'),
```

