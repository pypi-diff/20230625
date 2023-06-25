# Comparing `tmp/lycoris_lora-0.1.7.dev5.tar.gz` & `tmp/lycoris_lora-0.1.7.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.7.dev5.tar", last modified: Sat Jun 24 18:14:40 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev6.tar", last modified: Sun Jun 25 04:19:21 2023, max compression
```

## Comparing `lycoris_lora-0.1.7.dev5.tar` & `lycoris_lora-0.1.7.dev6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.267951 lycoris_lora-0.1.7.dev5/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev5/Algo.md
--rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev5/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev5/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-24 18:14:40.267452 lycoris_lora-0.1.7.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.251449 lycoris_lora-0.1.7.dev5/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev5/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev5/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev5/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev5/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev5/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev5/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev5/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.254949 lycoris_lora-0.1.7.dev5/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev5/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev5/lycoris/ia3.py
--rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev5/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev5/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev5/lycoris/locon.py
--rw-rw-rw-   0        0        0     8518 2023-06-24 18:13:14.000000 lycoris_lora-0.1.7.dev5/lycoris/loha.py
--rw-rw-rw-   0        0        0    10339 2023-06-16 13:18:39.000000 lycoris_lora-0.1.7.dev5/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev5/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.266451 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-24 18:14:40.000000 lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:14:40.267951 lycoris_lora-0.1.7.dev5/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-24 18:14:34.000000 lycoris_lora-0.1.7.dev5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:14:40.266951 lycoris_lora-0.1.7.dev5/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev5/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev5/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.703789 lycoris_lora-0.1.7.dev6/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev6/Algo.md
+-rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev6/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev6/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-25 04:19:21.703789 lycoris_lora-0.1.7.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.688784 lycoris_lora-0.1.7.dev6/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev6/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev6/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev6/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev6/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev6/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev6/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev6/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.696784 lycoris_lora-0.1.7.dev6/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.7.dev6/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev6/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    22402 2023-06-16 11:27:54.000000 lycoris_lora-0.1.7.dev6/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev6/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     3844 2023-06-16 11:29:39.000000 lycoris_lora-0.1.7.dev6/lycoris/locon.py
+-rw-rw-rw-   0        0        0     8254 2023-06-25 04:18:12.000000 lycoris_lora-0.1.7.dev6/lycoris/loha.py
+-rw-rw-rw-   0        0        0    10194 2023-06-25 04:18:47.000000 lycoris_lora-0.1.7.dev6/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev6/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.702789 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 04:19:21.000000 lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 04:19:21.703789 lycoris_lora-0.1.7.dev6/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-25 04:18:33.000000 lycoris_lora-0.1.7.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:19:21.703289 lycoris_lora-0.1.7.dev6/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev6/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev6/tools/merge.py
```

### Comparing `lycoris_lora-0.1.7.dev5/.gitignore` & `lycoris_lora-0.1.7.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/Algo.md` & `lycoris_lora-0.1.7.dev6/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/Change.md` & `lycoris_lora-0.1.7.dev6/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/Demo.md` & `lycoris_lora-0.1.7.dev6/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/LICENSE.md` & `lycoris_lora-0.1.7.dev6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/README.md` & `lycoris_lora-0.1.7.dev6/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/better_conv.py` & `lycoris_lora-0.1.7.dev6/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/better_conv_extract.py` & `lycoris_lora-0.1.7.dev6/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/concept_neuron.py` & `lycoris_lora-0.1.7.dev6/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/locon_extract_test.py` & `lycoris_lora-0.1.7.dev6/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/locon_merge_test.py` & `lycoris_lora-0.1.7.dev6/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/singular_value_test.py` & `lycoris_lora-0.1.7.dev6/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.7.dev6/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/experiments/time_test.py` & `lycoris_lora-0.1.7.dev6/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev6/lycoris/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev6/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/kohya.py` & `lycoris_lora-0.1.7.dev6/lycoris/kohya.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev6/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev6/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/locon.py` & `lycoris_lora-0.1.7.dev6/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/loha.py` & `lycoris_lora-0.1.7.dev6/lycoris/loha.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,56 +3,54 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class HadaWeight(torch.autograd.Function):
     @staticmethod
-    def forward(ctx, orig_weight, w1a, w1b, w2a, w2b, scale=torch.tensor(1)):
+    def forward(ctx, w1a, w1b, w2a, w2b, scale=torch.tensor(1)):
         ctx.save_for_backward(w1a, w1b, w2a, w2b, scale)
         diff_weight = ((w1a@w1b)*(w2a@w2b)) * scale
-        
-        if isinstance(orig_weight, torch.Tensor):
-            orig_weight = orig_weight.reshape(diff_weight.shape)
-        return orig_weight + diff_weight
+        return diff_weight
 
     @staticmethod
     def backward(ctx, grad_out):
         (w1a, w1b, w2a, w2b, scale) = ctx.saved_tensors
         grad_out = grad_out * scale
         temp = grad_out*(w2a@w2b)
         grad_w1a = temp @ w1b.T
         grad_w1b = w1a.T @ temp
 
         temp = grad_out * (w1a@w1b)
         grad_w2a = temp @ w2b.T
         grad_w2b = w2a.T @ temp
         
         del temp
-        return grad_out, grad_w1a, grad_w1b, grad_w2a, grad_w2b, None
+        return grad_w1a, grad_w1b, grad_w2a, grad_w2b, None
 
 
 class HadaWeightCP(torch.autograd.Function):
     @staticmethod
-    def forward(ctx, orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale=torch.tensor(1)):
+    def forward(ctx, t1, w1a, w1b, t2, w2a, w2b, scale=torch.tensor(1)):
         ctx.save_for_backward(t1, w1a, w1b, t2, w2a, w2b, scale)
         
         rebuild1 = torch.einsum('i j k l, j r, i p -> p r k l', t1, w1b, w1a)
         rebuild2 = torch.einsum('i j k l, j r, i p -> p r k l', t2, w2b, w2a)
         
-        return orig_weight + rebuild1*rebuild2*scale
+        return rebuild1*rebuild2*scale
 
     @staticmethod
     def backward(ctx, grad_out):
         (t1, w1a, w1b, t2, w2a, w2b, scale) = ctx.saved_tensors
+        grad_out = grad_out * scale
         
         temp = torch.einsum('i j k l, j r -> i r k l', t2, w2b)
         rebuild = torch.einsum('i j k l, i r -> r j k l', temp, w2a)
         
-        grad_w = rebuild*grad_out*scale
+        grad_w = rebuild*grad_out
         del rebuild
         
         grad_w1a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
         grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w1a.T)
         del grad_w, temp
         
         grad_w1b = torch.einsum('i r k l, i j k l -> r j', t1, grad_temp)
@@ -68,23 +66,23 @@
         grad_w2a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
         grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w2a.T)
         del grad_w, temp
         
         grad_w2b = torch.einsum('i r k l, i j k l -> r j', t2, grad_temp)
         grad_t2 = torch.einsum('i j k l, j r -> i r k l', grad_temp, w2b.T)
         del grad_temp
-        return grad_out, grad_t1, grad_w1a, grad_w1b, grad_t2, grad_w2a, grad_w2b, None
+        return grad_t1, grad_w1a, grad_w1b, grad_t2, grad_w2a, grad_w2b, None
 
 
-def make_weight(orig_weight, w1a, w1b, w2a, w2b, scale):
-    return HadaWeight.apply(orig_weight, w1a, w1b, w2a, w2b, scale)
+def make_weight(w1a, w1b, w2a, w2b, scale):
+    return HadaWeight.apply(w1a, w1b, w2a, w2b, scale)
 
 
-def make_weight_cp(orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale):
-    return HadaWeightCP.apply(orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale)
+def make_weight_cp(t1, w1a, w1b, t2, w2a, w2b, scale):
+    return HadaWeightCP.apply(t1, w1a, w1b, t2, w2a, w2b, scale)
 
 
 class LohaModule(nn.Module):
     """
     Hadamard product Implementaion for Low Rank Adaptation
     """
 
@@ -167,22 +165,20 @@
 
     def apply_to(self):
         self.org_module[0].forward = self.forward
 
     def get_weight(self, orig_weight=None):
         if self.cp:
             weight = make_weight_cp(
-                0, 
                 self.hada_t1, self.hada_w1_a, self.hada_w1_b,
                 self.hada_t1, self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         else:
             weight = make_weight(
-                0, 
                 self.hada_w1_a, self.hada_w1_b,
                 self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         if orig_weight is not None:
             weight = weight.reshape(orig_weight.shape)
         return weight
```

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev6/lycoris/lokr.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,21 @@
 
 
 def make_weight_cp(t, wa, wb):
     rebuild2 = torch.einsum('i j k l, i p, j r -> p r k l', t, wa, wb) # [c, d, k1, k2]
     return rebuild2
 
 
-def make_kron(orig_weight, w1, w2, scale):
+def make_kron(w1, w2, scale):
     if len(w2.shape) == 4:
         w1 = w1.unsqueeze(2).unsqueeze(2)
     w2 = w2.contiguous()
     rebuild = torch.kron(w1, w2)
     
-    if isinstance(orig_weight, torch.Tensor):
-        rebuild = rebuild.reshape(orig_weight.shape)
-    return orig_weight + rebuild*scale
+    return rebuild*scale
 
 
 class LokrModule(nn.Module):
     """
     modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
         and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
         and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
@@ -204,15 +202,14 @@
     # Same as locon.py
     def apply_to(self):
         self.org_forward = self.org_module[0].forward
         self.org_module[0].forward = self.forward
     
     def get_weight(self, orig_weight = None):
         weight = make_kron(
-            0, 
             self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
             (self.lokr_w2 if self.use_w2 
              else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
              else self.lokr_w2_a@self.lokr_w2_b),
             torch.tensor(self.scale)
         )
         if orig_weight is not None:
```

### Comparing `lycoris_lora-0.1.7.dev5/lycoris/utils.py` & `lycoris_lora-0.1.7.dev6/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.7.dev6/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/setup.py` & `lycoris_lora-0.1.7.dev6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.7.dev5',
+    version='0.1.7.dev6',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.7.dev5/tools/extract_locon.py` & `lycoris_lora-0.1.7.dev6/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev5/tools/merge.py` & `lycoris_lora-0.1.7.dev6/tools/merge.py`

 * *Files identical despite different names*

