# Comparing `tmp/lycoris_lora-0.1.7.dev7.tar.gz` & `tmp/lycoris_lora-0.1.7.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.7.dev7.tar", last modified: Sun Jun 25 13:21:46 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev8.tar", last modified: Sun Jun 25 13:28:00 2023, max compression
```

## Comparing `lycoris_lora-0.1.7.dev7.tar` & `lycoris_lora-0.1.7.dev8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.480754 lycoris_lora-0.1.7.dev7/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev7/Algo.md
--rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev7/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev7/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-06-25 13:21:46.480754 lycoris_lora-0.1.7.dev7/PKG-INFO
--rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.464754 lycoris_lora-0.1.7.dev7/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev7/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev7/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev7/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev7/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev7/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev7/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev7/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.468254 lycoris_lora-0.1.7.dev7/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/lycoris/__init__.py
--rw-rw-rw-   0        0        0     6258 2023-06-25 13:20:45.000000 lycoris_lora-0.1.7.dev7/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev7/lycoris/ia3.py
--rw-rw-rw-   0        0        0    23175 2023-06-25 13:21:07.000000 lycoris_lora-0.1.7.dev7/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev7/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     4461 2023-06-25 13:17:36.000000 lycoris_lora-0.1.7.dev7/lycoris/locon.py
--rw-rw-rw-   0        0        0     8817 2023-06-25 13:17:03.000000 lycoris_lora-0.1.7.dev7/lycoris/loha.py
--rw-rw-rw-   0        0        0    10798 2023-06-25 13:17:55.000000 lycoris_lora-0.1.7.dev7/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev7/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.479754 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      773 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-25 13:21:46.000000 lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 13:21:46.480754 lycoris_lora-0.1.7.dev7/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-06-25 13:21:40.000000 lycoris_lora-0.1.7.dev7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 13:21:46.480254 lycoris_lora-0.1.7.dev7/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev7/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev7/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:28:00.595277 lycoris_lora-0.1.7.dev8/
+-rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev8/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.7.dev8/Algo.md
+-rw-rw-rw-   0        0        0      618 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev8/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.7.dev8/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev8/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-06-25 13:28:00.594778 lycoris_lora-0.1.7.dev8/PKG-INFO
+-rw-rw-rw-   0        0        0     7396 2023-06-05 03:31:07.000000 lycoris_lora-0.1.7.dev8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 13:28:00.580774 lycoris_lora-0.1.7.dev8/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev8/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.7.dev8/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.7.dev8/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.7.dev8/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.7.dev8/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev8/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.7.dev8/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.7.dev8/experiments/time_test.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:28:00.584778 lycoris_lora-0.1.7.dev8/lycoris/
+-rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev8/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     6258 2023-06-25 13:20:45.000000 lycoris_lora-0.1.7.dev8/lycoris/dylora.py
+-rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.7.dev8/lycoris/ia3.py
+-rw-rw-rw-   0        0        0    23175 2023-06-25 13:21:07.000000 lycoris_lora-0.1.7.dev8/lycoris/kohya.py
+-rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.7.dev8/lycoris/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev8/lycoris/kohya_utils.py
+-rw-rw-rw-   0        0        0     4461 2023-06-25 13:17:36.000000 lycoris_lora-0.1.7.dev8/lycoris/locon.py
+-rw-rw-rw-   0        0        0     8827 2023-06-25 13:27:40.000000 lycoris_lora-0.1.7.dev8/lycoris/loha.py
+-rw-rw-rw-   0        0        0    10808 2023-06-25 13:27:52.000000 lycoris_lora-0.1.7.dev8/lycoris/lokr.py
+-rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-0.1.7.dev8/lycoris/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:28:00.593777 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-06-25 13:28:00.000000 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2023-06-25 13:28:00.000000 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 13:28:00.000000 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-25 13:28:00.000000 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 13:28:00.000000 lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.7.dev8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 13:28:00.595277 lycoris_lora-0.1.7.dev8/setup.cfg
+-rw-rw-rw-   0        0        0      547 2023-06-25 13:27:58.000000 lycoris_lora-0.1.7.dev8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 13:28:00.594778 lycoris_lora-0.1.7.dev8/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.7.dev8/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-0.1.7.dev8/tools/merge.py
```

### Comparing `lycoris_lora-0.1.7.dev7/.gitignore` & `lycoris_lora-0.1.7.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/Algo.md` & `lycoris_lora-0.1.7.dev8/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/Change.md` & `lycoris_lora-0.1.7.dev8/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/Demo.md` & `lycoris_lora-0.1.7.dev8/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/LICENSE.md` & `lycoris_lora-0.1.7.dev8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/README.md` & `lycoris_lora-0.1.7.dev8/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/better_conv.py` & `lycoris_lora-0.1.7.dev8/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/better_conv_extract.py` & `lycoris_lora-0.1.7.dev8/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/concept_neuron.py` & `lycoris_lora-0.1.7.dev8/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/locon_extract_test.py` & `lycoris_lora-0.1.7.dev8/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/locon_merge_test.py` & `lycoris_lora-0.1.7.dev8/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/singular_value_test.py` & `lycoris_lora-0.1.7.dev8/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/sparse_bias_test.py` & `lycoris_lora-0.1.7.dev8/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/experiments/time_test.py` & `lycoris_lora-0.1.7.dev8/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev8/lycoris/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev8/lycoris/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/kohya.py` & `lycoris_lora-0.1.7.dev8/lycoris/kohya.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev8/lycoris/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev8/lycoris/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/locon.py` & `lycoris_lora-0.1.7.dev8/lycoris/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/loha.py` & `lycoris_lora-0.1.7.dev8/lycoris/loha.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,16 +179,16 @@
             weight = make_weight(
                 self.hada_w1_a, self.hada_w1_b,
                 self.hada_w2_a, self.hada_w2_b,
                 scale = torch.tensor(self.scale),
             )
         if orig_weight is not None:
             weight = weight.reshape(orig_weight.shape)
-        if self.training and self.dropout:
-            drop = torch.rand(weight.size(0)) < self.dropout
+        if self.training and self.rank_dropout:
+            drop = torch.rand(weight.size(0)) < self.rank_dropout
             weight *= drop.view(-1, [1]*len(weight.shape[1:])).to(weight.device)
         return weight
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
```

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev8/lycoris/lokr.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,16 +210,16 @@
             (self.lokr_w2 if self.use_w2 
              else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
              else self.lokr_w2_a@self.lokr_w2_b),
             torch.tensor(self.scale)
         )
         if orig_weight is not None:
             weight = weight.reshape(orig_weight.shape)
-        if self.training and self.dropout:
-            drop = torch.rand(weight.size(0)) < self.dropout
+        if self.training and self.rank_dropout:
+            drop = torch.rand(weight.size(0)) < self.rank_dropout
             weight *= drop.view(-1, [1]*len(weight.shape[1:])).to(weight.device)
         return weight
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
```

### Comparing `lycoris_lora-0.1.7.dev7/lycoris/utils.py` & `lycoris_lora-0.1.7.dev8/lycoris/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-0.1.7.dev8/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/setup.py` & `lycoris_lora-0.1.7.dev8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='lycoris_lora',
     packages=['lycoris'],
-    version='0.1.7.dev7',
+    version='0.1.7.dev8',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-0.1.7.dev7/tools/extract_locon.py` & `lycoris_lora-0.1.7.dev8/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-0.1.7.dev7/tools/merge.py` & `lycoris_lora-0.1.7.dev8/tools/merge.py`

 * *Files identical despite different names*

