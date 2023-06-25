# Comparing `tmp/spyx-0.0.7.tar.gz` & `tmp/spyx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyx-0.0.7.tar", last modified: Fri Jun 23 20:21:32 2023, max compression
+gzip compressed data, was "spyx-0.0.8.tar", last modified: Sat Jun 24 16:27:19 2023, max compression
```

## Comparing `spyx-0.0.7.tar` & `spyx-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.7/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:21:32.839973 spyx-0.0.7/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.7/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 20:21:32.839973 spyx-0.0.7/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-23 20:20:57.000000 spyx-0.0.7/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/spyx/
--rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.7/spyx/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.7/spyx/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.7/spyx/activation.py
--rw-rw-r--   0 legion    (1000) legion    (1000)    12319 2023-06-22 22:55:28.000000 spyx-0.0.7/spyx/data.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2690 2023-06-23 20:19:39.000000 spyx-0.0.7/spyx/loss.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     7303 2023-06-23 19:28:10.000000 spyx-0.0.7/spyx/nn.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/spyx.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-23 20:21:32.000000 spyx-0.0.7/spyx.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:21:32.839973 spyx-0.0.7/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.7/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.8/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-24 16:27:19.542202 spyx-0.0.8/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.8/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-24 16:27:19.542202 spyx-0.0.8/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-24 16:26:55.000000 spyx-0.0.8/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/spyx/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.8/spyx/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.8/spyx/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.8/spyx/activation.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)    12388 2023-06-24 10:16:27.000000 spyx-0.0.8/spyx/data.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2707 2023-06-24 16:23:53.000000 spyx-0.0.8/spyx/loss.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8325 2023-06-24 16:22:34.000000 spyx-0.0.8/spyx/nn.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/spyx.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.8/tests/test_networks.py
```

### Comparing `spyx-0.0.7/LICENSE` & `spyx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spyx-0.0.7/PKG-INFO` & `spyx-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spyx-0.0.7/README.md` & `spyx-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spyx-0.0.7/setup.py` & `spyx-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "numpy",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="spyx",
-    version="0.0.7",
+    version="0.0.8",
     description="Spyx: SNNs in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/spyx",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `spyx-0.0.7/spyx/activation.py` & `spyx-0.0.8/spyx/activation.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.7/spyx/data.py` & `spyx-0.0.8/spyx/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,16 @@
         tensor = tensor[:self.sample_T,:]
         return np.minimum(tensor, 1)
     
 
 class SHD_loader():
     """
     Dataloading wrapper for the Spiking Heidelberg Dataset.
+
+    https://zenkelab.org/resources/spiking-heidelberg-datasets-shd/
     """
 
 
     # Change this to allow a config dictionary of 
     def __init__(self, batch_size=128, sample_T = 100):        
         shd_timestep = 1e-6
         shd_channels = 700
```

### Comparing `spyx-0.0.7/spyx/loss.py` & `spyx-0.0.8/spyx/loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import jax
 import jax.numpy as jnp
 import optax
 
 # need to make these consistent...
 
 @jax.jit
-def SRR_MSE(avg_spike_counts, target_count):
+def mse_spike_count_reg(avg_spike_counts, target_count):
     """Spike rate regularization based on mean squared error from target rate."""
 
     flat = jnp.concatenate(jax.tree_util.tree_flatten(avg_spike_counts)[0])
     return jnp.sum(optax.l2_loss(flat, jnp.array([target_count]*flat.shape[0])))
 
 @jax.jit
-def SRR_INV(avg_spike_counts, time_len):
+def inverse_spike_count_reg(avg_spike_counts, time_len):
     """
     Spike rate regularization based on an inverse function that strongly
     discourages neurons from silencing and gradually penalizes higher spike rates.
     
     """
 
     flat = jnp.concatenate(jax.tree_util.tree_flatten(avg_spike_counts)[0])
@@ -31,40 +31,37 @@
     Used in combination with a Leaky-Integrate neuron model as the final layer.
 
     """
 
     preds = jnp.argmax(jnp.sum(traces, axis=-2), axis=-1)
     return jnp.sum(preds == targets) / traces.shape[0], preds
 
+# should expose the smoothing rate and allow for users to partial it away or possibly schedule it...
 @jax.jit
-def integral_xentropy(traces, targets):
+def integral_crossentropy(traces, targets, smoothing=0.3):
     """
     Calculate the crossentropy between the integral of membrane potentials.
-    right now has a fixed value for label smoothing to discourage silencing 
+    Allows for label smoothing to discourage silencing 
     the other neurons in the readout layer.
+
+    Attributes:
+        traces: the output of the final layer of the SNN
+        targets: the integer labels for each class
+        smoothing: [optional] rate at which to smooth labels.
     """
 
     logits = jnp.sum(traces, axis=-2) # time axis.
-    labels = optax.smooth_labels(jax.nn.one_hot(targets, logits.shape[-1]), 0.3)
+    labels = optax.smooth_labels(jax.nn.one_hot(targets, logits.shape[-1]), smoothing)
     return optax.softmax_cross_entropy(logits, labels).mean() #change to mean
 
 
-@jax.jit
-def regularized_xentropy(traces, targets, avg_spike_counts, time_steps, r):
-    """
-    Weighted loss of integral crossentropy plus inverse spike rate regularization.
-    """
-
-    xe = integral_xentropy(traces, targets)
-    reg = SRR_INV(avg_spike_counts, time_steps)
-    return xe + r*reg
 
 # needs fixing.
 @jax.jit
-def exponential_integral_xentropy(spikes, targets):
+def exp_integral_crossentropy(spikes, targets):
     """
     Integral crossentropy with exponential weighting to promote pushing voltage
     deflections and therefore spikes to earlier in the network rollout.
 
     Still under construction.
 
     Adapted from:
```

### Comparing `spyx-0.0.7/spyx/nn.py` & `spyx-0.0.8/spyx/nn.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,42 @@
         # calculate whether spike is generated, and update membrane potential
         Vout = self.beta*Vin + x
         return Vout, Vout
     
     def initial_state(self, batch_size):
         return jnp.zeros([batch_size, self.layer_size], dtype=jnp.float32)
 
+class IF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
+    """
+    Integrate and Fire neuron model 
+    
+
+    Attributes:
+        hidden_size: Size of preceding layer's outputs
+        threshold: threshold for reset. Defaults to 1.
+        activation: spyx.activation function, default is Heaviside with Straight-Through-Estimation.
+    """
+
+    def __init__(self, hidden_size, threshold=1, 
+                 activation = Heaviside(),
+                 name="LIF"):
+        super().__init__(name=name)
+        self.hidden_size = hidden_size
+        self.threshold = threshold
+        self.act = activation
+    
+    def __call__(self, x, V):
+        # calculate whether spike is generated, and update membrane potential
+        spikes = self.act(V - self.threshold)
+        V = (V + x - spikes*self.threshold).astype(jnp.float16)
+        
+        return spikes, V
+
+    def initial_state(self, batch_size): # figure out how to make dynamic...
+        return jnp.zeros([batch_size, self.hidden_size], dtype=jnp.float16)
 
 
 class LIF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
     """
     Leaky Integrate and Fire neuron model inspired by the implementation in
     snnTorch:
 
@@ -118,14 +146,15 @@
         V = (beta*V + x - spikes*self.threshold).astype(jnp.float16)
         
         return spikes, V
 
     def initial_state(self, batch_size): # figure out how to make dynamic...
         return jnp.zeros([batch_size, self.hidden_size], dtype=jnp.float16)
 
+
 class RLIF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
     """
     Recurrent LIF Neuron adapted from snnTorch:
 
     https://snntorch.readthedocs.io/en/latest/snn.neurons_rleaky.html
     """
 
@@ -152,17 +181,15 @@
         V = (beta*V + x + recurrent*spikes - spikes*self.threshold).astype(jnp.float16)
         
         return spikes, V
 
     def initial_state(self, batch_size):
         return jnp.zeros([batch_size, self.hidden_size], dtype=jnp.float16)
 
-
-
-# Synaptic Conductance a.k.a CoBa
+# Current Based (CuBa)
 class SC(hk.RNNCore): 
     """
     Conductance based neuron modeling synaptic conductance.
 
     Adapted from snnTorch:
 
     https://snntorch.readthedocs.io/en/latest/snn.neurons_synaptic.html
```

### Comparing `spyx-0.0.7/spyx.egg-info/PKG-INFO` & `spyx-0.0.8/spyx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

