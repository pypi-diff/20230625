# Comparing `tmp/lycoris_lora-0.1.7.dev6.tar.gz` & `tmp/lycoris_lora-0.1.7.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.7.dev6.tar", last modified: Sun Jun 25 04:19:21 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev7.tar", last modified: Sun Jun 25 13:21:46 2023, max compression
```

## Comparing `lycoris_lora-0.1.7.dev6.tar` & `lycoris_lora-0.1.7.dev7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.703789 lycoris_lora-0.1.7.dev6/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev6/Algo.md
--rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev6/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev6/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-25 04:19:21.703789 lycoris_lora-0.1.7.dev6/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.688784 lycoris_lora-0.1.7.dev6/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev6/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev6/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev6/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev6/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev6/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev6/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev6/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.696784 lycoris_lora-0.1.7.dev6/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev6/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev6/lycoris/ia3.py
--rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev6/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev6/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev6/lycoris/locon.py
--rw-rw-rw-   0        0        0     8254 2023-06-25 04:18:12.000000 lycoris_lora-0.1.7.dev6/lycoris/loha.py
--rw-rw-rw-   0        0        0    10194 2023-06-25 04:18:47.000000 lycoris_lora-0.1.7.dev6/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev6/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.702789 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 04:19:21.703789 lycoris_lora-0.1.7.dev6/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-25 04:18:33.000000 lycoris_lora-0.1.7.dev6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.703289 lycoris_lora-0.1.7.dev6/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev6/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev6/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.480754 lycoris_lora-0.1.7.dev7/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev7/Algo.md
+-rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev7/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev7/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-25 13:21:46.480754 lycoris_lora-0.1.7.dev7/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.464754 lycoris_lora-0.1.7.dev7/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev7/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev7/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev7/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev7/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev7/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev7/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev7/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.468254 lycoris_lora-0.1.7.dev7/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     6258 2023-06-25 13:20:45.000000 lycoris_lora-0.1.7.dev7/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev7/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    23175 2023-06-25 13:21:07.000000 lycoris_lora-0.1.7.dev7/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev7/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     4461 2023-06-25 13:17:36.000000 lycoris_lora-0.1.7.dev7/lycoris/locon.py
+-rw-rw-rw-   0        0        0     8817 2023-06-25 13:17:03.000000 lycoris_lora-0.1.7.dev7/lycoris/loha.py
+-rw-rw-rw-   0        0        0    10798 2023-06-25 13:17:55.000000 lycoris_lora-0.1.7.dev7/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev7/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.479754 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 13:21:46.480754 lycoris_lora-0.1.7.dev7/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-25 13:21:40.000000 lycoris_lora-0.1.7.dev7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.480254 lycoris_lora-0.1.7.dev7/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev7/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev7/tools/merge.py
```

### Comparing `lycoris_lora-0.1.7.dev6/.gitignore` & `lycoris_lora-0.1.7.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/Algo.md` & `lycoris_lora-0.1.7.dev7/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/Change.md` & `lycoris_lora-0.1.7.dev7/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/Demo.md` & `lycoris_lora-0.1.7.dev7/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/LICENSE.md` & `lycoris_lora-0.1.7.dev7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/README.md` & `lycoris_lora-0.1.7.dev7/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/better_conv.py` & `lycoris_lora-0.1.7.dev7/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/better_conv_extract.py` & `lycoris_lora-0.1.7.dev7/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/concept_neuron.py` & `lycoris_lora-0.1.7.dev7/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/locon_extract_test.py` & `lycoris_lora-0.1.7.dev7/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/locon_merge_test.py` & `lycoris_lora-0.1.7.dev7/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/singular_value_test.py` & `lycoris_lora-0.1.7.dev7/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.7.dev7/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/experiments/time_test.py` & `lycoris_lora-0.1.7.dev7/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev7/lycoris/dylora.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __init__(
         self, 
         lora_name, 
         org_module: nn.Module, 
         multiplier=1.0, 
         lora_dim=4, alpha=1, 
-        dropout=0.,
+        dropout=0., rank_dropout=0., module_dropout=0.,
         use_cp=False, 
         block_size=1,
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
```

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev7/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/kohya.py` & `lycoris_lora-0.1.7.dev7/lycoris/kohya.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
         network_dim = 4                     # default
     conv_dim = int(kwargs.get('conv_dim', network_dim) or network_dim)
     conv_alpha = float(kwargs.get('conv_alpha', network_alpha) or network_alpha)
     dropout = float(kwargs.get('dropout', 0.) or 0.)
+    rank_dropout = float(kwargs.get("rank_dropout", 0.) or 0.)
+    module_dropout = float(kwargs.get("module_dropout", 0.) or 0.)
     algo = (kwargs.get('algo', 'lora') or 'lora').lower()
     use_cp = (not kwargs.get('disable_conv_cp', True)
               or kwargs.get('use_conv_cp', False))
     block_size = int(kwargs.get('block_size', 4) or 4)
     network_module = {
         'lora': LoConModule,
         'locon': LoConModule,
@@ -62,15 +64,15 @@
         )
     else:
         network = LycorisNetwork(
             text_encoder, unet, 
             multiplier=multiplier, 
             lora_dim=network_dim, conv_lora_dim=conv_dim, 
             alpha=network_alpha, conv_alpha=conv_alpha,
-            dropout=dropout,
+            dropout=dropout, rank_dropout=rank_dropout, module_dropout=module_dropout,
             use_cp=use_cp,
             network_module=network_module,
             decompose_both=kwargs.get('decompose_both', False),
             factor=kwargs.get('factor', -1),
             block_size = block_size
         )
     
@@ -102,15 +104,16 @@
     def __init__(
         self, 
         text_encoder, unet, 
         multiplier=1.0, 
         lora_dim=4, conv_lora_dim=4, 
         alpha=1, conv_alpha=1,
         use_cp = False,
-        dropout = 0, network_module = LoConModule,
+        dropout = 0, rank_dropout = 0, module_dropout = 0,
+        network_module = LoConModule,
         **kwargs,
     ) -> None:
         super().__init__()
         self.multiplier = multiplier
         self.lora_dim = lora_dim
         self.conv_lora_dim = int(conv_lora_dim)
         if self.conv_lora_dim != self.lora_dim: 
@@ -122,14 +125,16 @@
         if self.alpha != self.conv_alpha: 
             print('Apply different alpha value for conv layer')
             print(f'Conv alpha: {conv_alpha}, Linear alpha: {alpha}')
         
         if 1 >= dropout >= 0:
             print(f'Use Dropout value: {dropout}')
         self.dropout = dropout
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
         
         # create module instances
         def create_modules(
             prefix, 
             root_module: torch.nn.Module, 
             target_replace_modules,
             target_replace_names = []
@@ -141,62 +146,68 @@
                     for child_name, child_module in module.named_modules():
                         lora_name = prefix + '.' + name + '.' + child_name
                         lora_name = lora_name.replace('.', '_')
                         if child_module.__class__.__name__ == 'Linear' and lora_dim>0:
                             lora = network_module(
                                 lora_name, child_module, self.multiplier, 
                                 self.lora_dim, self.alpha, 
-                                self.dropout, use_cp,
+                                self.dropout, self.rank_dropout, self.module_dropout, 
+                                use_cp,
                                 **kwargs
                             )
                         elif child_module.__class__.__name__ == 'Conv2d':
                             k_size, *_ = child_module.kernel_size
                             if k_size==1 and lora_dim>0:
                                 lora = network_module(
                                     lora_name, child_module, self.multiplier, 
                                     self.lora_dim, self.alpha, 
-                                    self.dropout, use_cp,
+                                    self.dropout, self.rank_dropout, self.module_dropout, 
+                                    use_cp,
                                     **kwargs
                                 )
                             elif conv_lora_dim>0:
                                 lora = network_module(
                                     lora_name, child_module, self.multiplier, 
                                     self.conv_lora_dim, self.conv_alpha, 
-                                    self.dropout, use_cp,
+                                    self.dropout, self.rank_dropout, self.module_dropout, 
+                                    use_cp,
                                     **kwargs
                                 )
                             else:
                                 continue
                         else:
                             continue
                         loras.append(lora)
                 elif name in target_replace_names:
                     lora_name = prefix + '.' + name
                     lora_name = lora_name.replace('.', '_')
                     if module.__class__.__name__ == 'Linear' and lora_dim>0:
                         lora = network_module(
                             lora_name, module, self.multiplier, 
                             self.lora_dim, self.alpha, 
-                            self.dropout, use_cp,
+                            self.dropout, self.rank_dropout, self.module_dropout, 
+                            use_cp,
                             **kwargs
                         )
                     elif module.__class__.__name__ == 'Conv2d':
                         k_size, *_ = module.kernel_size
                         if k_size==1 and lora_dim>0:
                             lora = network_module(
                                 lora_name, module, self.multiplier, 
                                 self.lora_dim, self.alpha, 
-                                self.dropout, use_cp,
+                                self.dropout, self.rank_dropout, self.module_dropout, 
+                                use_cp,
                                 **kwargs
                             )
                         elif conv_lora_dim>0:
                             lora = network_module(
                                 lora_name, module, self.multiplier, 
                                 self.conv_lora_dim, self.conv_alpha, 
-                                self.dropout, use_cp,
+                                self.dropout, self.rank_dropout, self.module_dropout, 
+                                use_cp,
                                 **kwargs
                             )
                         else:
                             continue
                     else:
                         continue
                     loras.append(lora)
```

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev7/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev7/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/locon.py` & `lycoris_lora-0.1.7.dev7/lycoris/locon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+from weakref import ref
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class LoConModule(nn.Module):
@@ -11,49 +12,53 @@
     """
 
     def __init__(
         self, 
         lora_name, org_module: nn.Module, 
         multiplier=1.0, 
         lora_dim=4, alpha=1, 
-        dropout=0.,
+        dropout=0., rank_dropout=0., module_dropout=0.,
         use_cp=False,
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
         self.lora_dim = lora_dim
         self.cp = False
 
-        if org_module.__class__.__name__ == 'Conv2d':
+        if isinstance(org_module, nn.Conv2d):
             # For general LoCon
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
             stride = org_module.stride
             padding = org_module.padding
             out_dim = org_module.out_channels
             if use_cp and k_size != (1, 1):
                 self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
                 self.lora_mid = nn.Conv2d(lora_dim, lora_dim, k_size, stride, padding, bias=False)
                 self.cp = True
             else:
                 self.lora_down = nn.Conv2d(in_dim, lora_dim, k_size, stride, padding, bias=False)
             self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
-        else:
+        elif isinstance(org_module, nn.Linear):
             in_dim = org_module.in_features
             out_dim = org_module.out_features
             self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
             self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
+        else:
+            raise NotImplementedError
         self.shape = org_module.weight.shape
         
         if dropout:
             self.dropout = nn.Dropout(dropout)
         else:
             self.dropout = nn.Identity()
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
         
         if type(alpha) == torch.Tensor:
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
@@ -89,16 +94,25 @@
             self.lora_down.weight *= ratio**(1/modules)
             if self.cp:
                 self.lora_mid.weight *= ratio**(1/modules)
         
         return scaled, orig_norm*ratio
 
     def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.org_forward(x)
         scale = self.scale * self.multiplier
         if self.cp:
-            return self.org_forward(x)  + self.dropout(
-                self.lora_up(self.lora_mid(self.lora_down(x))) * scale
-            )
+            mid = self.lora_mid(self.lora_down(x))
         else:
-            return self.org_forward(x)  + self.dropout(
-                self.lora_up(self.lora_down(x)) * scale
-            )
+            mid = self.lora_down(x)
+        
+        if self.rank_dropout and self.training:
+            drop = torch.rand(self.lora_dim, device=mid.device) < self.rank_dropout
+            if (dims:=len(x.shape)) == 4:
+                drop = drop.view(1, -1, 1, 1)
+            else:
+                drop = drop.view(*[1]*(dims-1), -1)
+            mid = mid * drop
+        
+        return self.org_forward(x) + self.dropout(self.lora_up(mid) * scale)
```

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/loha.py` & `lycoris_lora-0.1.7.dev7/lycoris/loha.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,15 +86,16 @@
     Hadamard product Implementaion for Low Rank Adaptation
     """
 
     def __init__(
         self, 
         lora_name, 
         org_module: nn.Module, 
-        multiplier=1.0, lora_dim=4, alpha=1, dropout=0.,
+        multiplier=1.0, lora_dim=4, alpha=1, 
+        dropout=0., rank_dropout=0., module_dropout=0.,
         use_cp=False,
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
         self.lora_dim = lora_dim
@@ -135,18 +136,19 @@
         else:
             self.hada_w1_a = nn.Parameter(torch.empty(shape[0], lora_dim))
             self.hada_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1]))
             
             self.hada_w2_a = nn.Parameter(torch.empty(shape[0], lora_dim))
             self.hada_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1]))
         
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-        else:
-            self.dropout = nn.Identity()
+        self.dropout = dropout
+        if rank_dropout:
+            print("[WARN]LoHa/LoKr haven't implemented rank dropout yet.")
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
         
         if type(alpha) == torch.Tensor:
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
@@ -177,14 +179,17 @@
             weight = make_weight(
                 self.hada_w1_a, self.hada_w1_b,
                 self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         if orig_weight is not None:
             weight = weight.reshape(orig_weight.shape)
+        if self.training and self.dropout:
+            drop = torch.rand(weight.size(0)) < self.dropout
+            weight *= drop.view(-1, [1]*len(weight.shape[1:])).to(weight.device)
         return weight
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
         desired = torch.clamp(norm, max=max_norm)
@@ -202,15 +207,21 @@
                 self.hada_t1 *= ratio**(1/modules)
                 self.hada_t2 *= ratio**(1/modules)
         
         return scaled, orig_norm*ratio
 
     @torch.enable_grad()
     def forward(self, x):
-        # print(torch.mean(torch.abs(self.orig_w1a.to(x.device) - self.hada_w1_a)), end='\r')
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.op(
+                    x,
+                    self.org_module[0].weight.data,
+                    None if self.org_module[0].bias is None else self.org_module[0].bias.data
+                )
         weight = (
             self.org_module[0].weight.data 
             + self.get_weight(self.org_module[0].weight.data) * self.multiplier
         )
         bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
         return self.op(
             x,
```

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev7/lycoris/lokr.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
 
     def __init__(
         self, 
         lora_name, org_module: nn.Module, 
         multiplier=1.0, 
         lora_dim=4, alpha=1, 
-        dropout=0.,
+        dropout=0., rank_dropout=0., module_dropout=0.,
         use_cp=False,
         decompose_both = False,
         factor:int=-1, # factorization factor
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
@@ -155,18 +155,18 @@
             else:
                 self.use_w2 = True
                 self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
 
             self.op = F.linear
             self.extra_args = {}
         
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-        else:
-            self.dropout = nn.Identity()
+        self.dropout = dropout
+        if rank_dropout:
+            print("[WARN]LyCORIS haven't implemented rank dropout yet.")
+        self.module_dropout = module_dropout
         
         if isinstance(alpha, torch.Tensor):
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         if self.use_w2 and self.use_w1:
             #use scale = 1
             alpha = lora_dim
@@ -210,14 +210,17 @@
             (self.lokr_w2 if self.use_w2 
              else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
              else self.lokr_w2_a@self.lokr_w2_b),
             torch.tensor(self.scale)
         )
         if orig_weight is not None:
             weight = weight.reshape(orig_weight.shape)
+        if self.training and self.dropout:
+            drop = torch.rand(weight.size(0)) < self.dropout
+            weight *= drop.view(-1, [1]*len(weight.shape[1:])).to(weight.device)
         return weight
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
         desired = torch.clamp(norm, max=max_norm)
@@ -239,14 +242,21 @@
                 self.lokr_w2_b  *= ratio**(1/modules)
             else:
                 self.lokr_w2 *= ratio**(1/modules)
         
         return scaled, orig_norm*ratio
 
     def forward(self, x):
+        if self.module_dropout and self.training:
+            if torch.rand(1) < self.module_dropout:
+                return self.op(
+                    x,
+                    self.org_module[0].weight.data,
+                    None if self.org_module[0].bias is None else self.org_module[0].bias.data
+                )
         weight = (
             self.org_module[0].weight.data 
             + self.get_weight(self.org_module[0].weight.data) * self.multiplier
         )
         bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
         return self.op(
             x,
```

### Comparing `lycoris_lora-0.1.7.dev6/lycoris/utils.py` & `lycoris_lora-0.1.7.dev7/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/setup.py` & `lycoris_lora-0.1.7.dev7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.7.dev6',
+    version='0.1.7.dev7',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.7.dev6/tools/extract_locon.py` & `lycoris_lora-0.1.7.dev7/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev6/tools/merge.py` & `lycoris_lora-0.1.7.dev7/tools/merge.py`

 * *Files identical despite different names*

