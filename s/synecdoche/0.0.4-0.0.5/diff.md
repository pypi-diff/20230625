# Comparing `tmp/synecdoche-0.0.4.tar.gz` & `tmp/synecdoche-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synecdoche-0.0.4.tar", last modified: Sat Jun 24 16:29:26 2023, max compression
+gzip compressed data, was "synecdoche-0.0.5.tar", last modified: Sun Jun 25 09:06:03 2023, max compression
```

## Comparing `synecdoche-0.0.4.tar` & `synecdoche-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-23 14:39:41.000000 synecdoche-0.0.4/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-24 16:29:26.308767 synecdoche-0.0.4/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      639 2023-06-23 21:57:45.000000 synecdoche-0.0.4/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-24 16:29:26.308767 synecdoche-0.0.4/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1447 2023-06-24 16:28:55.000000 synecdoche-0.0.4/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/synecdoche/
--rw-rw-r--   0 legion    (1000) legion    (1000)      129 2023-06-23 17:33:17.000000 synecdoche-0.0.4/synecdoche/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:39.000000 synecdoche-0.0.4/synecdoche/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1882 2023-06-24 15:43:56.000000 synecdoche-0.0.4/synecdoche/experimental.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8464 2023-06-24 15:43:08.000000 synecdoche-0.0.4/synecdoche/hyper.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/synecdoche.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      311 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       34 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       11 2023-06-24 16:29:26.000000 synecdoche-0.0.4/synecdoche.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:29:26.308767 synecdoche-0.0.4/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-23 17:42:50.000000 synecdoche-0.0.4/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:06:03.820424 synecdoche-0.0.5/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-23 14:39:41.000000 synecdoche-0.0.5/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-25 09:06:03.820424 synecdoche-0.0.5/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      639 2023-06-23 21:57:45.000000 synecdoche-0.0.5/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-25 09:06:03.820424 synecdoche-0.0.5/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1447 2023-06-25 09:05:31.000000 synecdoche-0.0.5/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:06:03.820424 synecdoche-0.0.5/synecdoche/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      129 2023-06-23 17:33:17.000000 synecdoche-0.0.5/synecdoche/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:39.000000 synecdoche-0.0.5/synecdoche/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1878 2023-06-25 06:59:47.000000 synecdoche-0.0.5/synecdoche/experimental.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8461 2023-06-25 08:43:37.000000 synecdoche-0.0.5/synecdoche/hyper.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:06:03.820424 synecdoche-0.0.5/synecdoche.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-25 09:06:03.000000 synecdoche-0.0.5/synecdoche.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      311 2023-06-25 09:06:03.000000 synecdoche-0.0.5/synecdoche.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-25 09:06:03.000000 synecdoche-0.0.5/synecdoche.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       34 2023-06-25 09:06:03.000000 synecdoche-0.0.5/synecdoche.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       11 2023-06-25 09:06:03.000000 synecdoche-0.0.5/synecdoche.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:06:03.820424 synecdoche-0.0.5/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-23 17:42:50.000000 synecdoche-0.0.5/tests/test_networks.py
```

### Comparing `synecdoche-0.0.4/LICENSE` & `synecdoche-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `synecdoche-0.0.4/PKG-INFO` & `synecdoche-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synecdoche
-Version: 0.0.4
+Version: 0.0.5
 Summary: Synecdoche: Hypernetworks for Haiku in JAX
 Home-page: https://github.com/kmheckel/synecdoche
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `synecdoche-0.0.4/README.md` & `synecdoche-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `synecdoche-0.0.4/setup.py` & `synecdoche-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "dm-haiku",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="synecdoche",
-    version="0.0.4",
+    version="0.0.5",
     description="Synecdoche: Hypernetworks for Haiku in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/synecdoche",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `synecdoche-0.0.4/synecdoche/experimental.py` & `synecdoche-0.0.5/synecdoche/experimental.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,14 @@
         layer_inputs = jnp.repeat(jnp.expand_dims(avg, 0), self.num_tgt_layers, 0)
         projections = hk.nets.MLP([self.embedding_dim, self.latent_dim, self.latent_dim])(layer_inputs)
 
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
         resized_tree = tree.tree_map(lambda layer, size: jnp.pad(layer[1,:size], 
-                                                                 (0,jnp.max(0,size-layer.size)), 
+                                                                 (0,max(0,size-layer.size)), 
                                                                  mode="wrap"), 
                                      rebuilt_tree, 
                                      self.tgt_sizes
                                     )
         net = tree.tree_map(jnp.reshape, resized_tree, self.target_layer_shapes)
         return net
```

### Comparing `synecdoche-0.0.4/synecdoche/hyper.py` & `synecdoche-0.0.5/synecdoche/hyper.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         # hypernetwork dimensions
         self.embedding_dim = embedding_dim
         self.hyper_out_dim = tree.tree_reduce(max, self.tgt_sizes)
         
     def __call__(self):
         embeddings = hk.get_parameter("w", [self.num_tgt_layers, self.embedding_dim],
                                       init=hk.initializers.TruncatedNormal())
+
         
         projections = jax.scipy.fft.idctn(embeddings, s=[self.num_tgt_layers, self.hyper_out_dim])
         # tgt_layers X max_layer_size matrix
         
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
@@ -181,14 +182,14 @@
         # tgt_layers X max_layer_size matrix
         
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
         # this is ugly... sorry...
         resized_tree = tree.tree_map(lambda layer, size: jnp.pad(layer[1,:size], 
-                                                                 (0,jnp.max(0,size-layer.size)), 
+                                                                 (0,max(0,size-layer.size)), 
                                                                  mode="wrap"), 
                                      rebuilt_tree, 
                                      self.tgt_sizes
                                     )
         net = tree.tree_map(jnp.reshape, resized_tree, self.target_layer_shapes)
         return net
```

### Comparing `synecdoche-0.0.4/synecdoche.egg-info/PKG-INFO` & `synecdoche-0.0.5/synecdoche.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synecdoche
-Version: 0.0.4
+Version: 0.0.5
 Summary: Synecdoche: Hypernetworks for Haiku in JAX
 Home-page: https://github.com/kmheckel/synecdoche
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

