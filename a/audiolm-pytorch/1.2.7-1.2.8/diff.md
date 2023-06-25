# Comparing `tmp/audiolm-pytorch-1.2.7.tar.gz` & `tmp/audiolm-pytorch-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.2.7.tar", last modified: Wed Jun 21 13:38:24 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.8.tar", last modified: Sun Jun 25 16:41:44 2023, max compression
```

## Comparing `audiolm-pytorch-1.2.7.tar` & `audiolm-pytorch-1.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    68033 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 13:38:24.000000 audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 13:38:24.378648 audiolm-pytorch-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-21 13:38:09.000000 audiolm-pytorch-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:41:44.662612 audiolm-pytorch-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 16:41:44.662612 audiolm-pytorch-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:41:44.658612 audiolm-pytorch-1.2.8/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68033 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30358 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:41:44.658612 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:41:44.662612 audiolm-pytorch-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/setup.py
```

### Comparing `audiolm-pytorch-1.2.7/LICENSE` & `audiolm-pytorch-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/PKG-INFO` & `audiolm-pytorch-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.7
+Version: 1.2.8
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.7/README.md` & `audiolm-pytorch-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/attend.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/audiolm_pytorch.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/encodec.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
             encodec_codebook = rearrange(encodec_codebook, '... -> 1 ...')
             vq_codebook.copy_(encodec_codebook)
 
     @property
     def seq_len_multiple_of(self):
         return reduce(lambda x, y: x * y, self.strides)
 
+    @property
+    def downsample_factor(self):
+        return self.seq_len_multiple_of
+
     def forward(
         self,
         x,
         return_encoded = False,
         **kwargs
     ):
```

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/hubert_kmeans.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,19 @@
     def groups(self):
         return 1
 
     @property
     def codebook_size(self):
         return self.kmeans.n_clusters
 
+    @property
+    def downsample_factor(self):
+        # todo: double check
+        return 320
+
     @torch.no_grad()
     def forward(
         self,
         wav_input,
         flatten = True,
         input_sample_hz = None
     ):
```

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/soundstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,14 +679,18 @@
             *self.decoder_film.parameters()
         ]
 
     @property
     def seq_len_multiple_of(self):
         return functools.reduce(lambda x, y: x * y, self.strides)
 
+    @property
+    def downsample_factor(self):
+        return self.seq_len_multiple_of
+
     def process_input(
         self,
         x,
         input_sample_hz = None,
         curtail_from_left = False
     ):
         x, ps = pack([x], '* n')
```

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.8/audiolm_pytorch/vq_wav2vec.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,14 +47,19 @@
         assert hasattr(self.model, 'vector_quantizer') and hasattr(self.model.vector_quantizer, 'embedding'), 'the vq wav2vec model does not seem to be valid'
 
     @property
     def groups(self):
         return self.model.vector_quantizer.groups
 
     @property
+    def downsample_factor(self):
+        # todo: double check architecture
+        return 80
+
+    @property
     def codebook_size(self):
         return self.model.vector_quantizer.embedding.shape[0]
 
     @torch.no_grad()
     def forward(
         self,
         wav_input,
```

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.7
+Version: 1.2.8
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.7/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.7/setup.py` & `audiolm-pytorch-1.2.8/setup.py`

 * *Files identical despite different names*

