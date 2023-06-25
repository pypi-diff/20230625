# Comparing `tmp/airontools-0.1.8-py3-none-any.whl.zip` & `tmp/airontools-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,45 @@
-Zip file size: 16204 bytes, number of entries: 25
--rw-rw-r--  2.0 unx        0 b- defN 21-Jun-27 09:04 airontools/__init__.py
--rw-rw-r--  2.0 unx      183 b- defN 21-Jun-13 15:23 airontools/backend.py
--rw-rw-r--  2.0 unx     3120 b- defN 21-Oct-31 23:59 airontools/preprocessing.py
--rw-rw-r--  2.0 unx      506 b- defN 21-Aug-14 10:37 airontools/tools.py
--rw-rw-r--  2.0 unx      196 b- defN 21-Oct-17 10:34 airontools/devices/__init__.py
--rw-rw-r--  2.0 unx      209 b- defN 21-Oct-17 10:34 airontools/devices/utils_tf.py
--rw-rw-r--  2.0 unx       90 b- defN 21-Oct-17 13:33 airontools/devices/utils_torch.py
--rw-rw-r--  2.0 unx      346 b- defN 21-Nov-01 15:45 airontools/model_constructors/__init__.py
--rw-rw-r--  2.0 unx    21301 b- defN 21-Nov-01 22:27 airontools/model_constructors/constructors_tf.py
--rw-rw-r--  2.0 unx      811 b- defN 21-Nov-01 14:28 airontools/model_constructors/constructors_torch.py
--rw-rw-r--  2.0 unx     2217 b- defN 21-Nov-01 10:40 airontools/model_constructors/utils_tf.py
--rw-rw-r--  2.0 unx      175 b- defN 21-Oct-17 13:33 airontools/model_constructors/utils_torch.py
--rw-rw-r--  2.0 unx      237 b- defN 21-Nov-01 15:45 airontools/model_interactors/__init__.py
--rw-rw-r--  2.0 unx     1146 b- defN 21-Nov-01 22:27 airontools/model_interactors/model_interactors_tf.py
--rw-rw-r--  2.0 unx      396 b- defN 21-Oct-17 13:33 airontools/model_interactors/model_interactors_torch.py
--rw-rw-r--  2.0 unx      324 b- defN 21-Nov-01 15:45 airontools/visualization/__init__.py
--rw-rw-r--  2.0 unx     1011 b- defN 21-Oct-17 11:16 airontools/visualization/tensorboard_tf.py
--rw-rw-r--  2.0 unx       78 b- defN 21-Oct-17 13:40 airontools/visualization/tensorboard_torch.py
--rw-rw-r--  2.0 unx     1618 b- defN 21-Oct-17 10:34 airontools/visualization/utils_tf.py
--rw-rw-r--  2.0 unx       80 b- defN 21-Oct-17 13:40 airontools/visualization/utils_torch.py
--rw-rw-r--  2.0 unx     1525 b- defN 21-Nov-02 08:23 airontools-0.1.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3554 b- defN 21-Nov-02 08:23 airontools-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Nov-02 08:23 airontools-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 21-Nov-02 08:23 airontools-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2275 b- defN 21-Nov-02 08:23 airontools-0.1.8.dist-info/RECORD
-25 files, 41501 bytes uncompressed, 12430 bytes compressed:  70.0%
+Zip file size: 26879 bytes, number of entries: 43
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-05 18:06 airontools/__init__.py
+-rw-rw-r--  2.0 unx      183 b- defN 21-Nov-05 18:06 airontools/backend.py
+-rw-rw-r--  2.0 unx     3469 b- defN 21-Nov-16 21:37 airontools/preprocessing.py
+-rw-rw-r--  2.0 unx      506 b- defN 21-Nov-05 18:06 airontools/tools.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-16 16:50 airontools/constructors/__init__.py
+-rw-rw-r--  2.0 unx      219 b- defN 21-Nov-15 14:00 airontools/constructors/blocks/__init__.py
+-rw-rw-r--  2.0 unx     3354 b- defN 21-Nov-15 13:51 airontools/constructors/blocks/blocks_tf.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-15 12:45 airontools/constructors/blocks/blocks_torch.py
+-rw-rw-r--  2.0 unx      219 b- defN 21-Nov-16 17:02 airontools/constructors/layers/__init__.py
+-rw-rw-r--  2.0 unx    14119 b- defN 21-Nov-15 15:57 airontools/constructors/layers/layers_tf.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-15 12:45 airontools/constructors/layers/layers_torch.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-16 16:50 airontools/constructors/models/__init__.py
+-rw-rw-r--  2.0 unx      237 b- defN 21-Nov-16 15:23 airontools/constructors/models/general/__init__.py
+-rw-rw-r--  2.0 unx    10182 b- defN 21-Nov-15 15:57 airontools/constructors/models/general/general_tf.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-15 12:45 airontools/constructors/models/general/general_torch.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-16 16:50 airontools/constructors/models/supervised/__init__.py
+-rw-rw-r--  2.0 unx      287 b- defN 21-Nov-16 15:28 airontools/constructors/models/supervised/classification/__init__.py
+-rw-rw-r--  2.0 unx     4032 b- defN 21-Nov-16 19:38 airontools/constructors/models/supervised/classification/classification_tf.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-16 15:26 airontools/constructors/models/supervised/classification/classification_torch.py
+-rw-rw-r--  2.0 unx      378 b- defN 21-Nov-16 15:33 airontools/constructors/models/unsupervised/__init__.py
+-rw-rw-r--  2.0 unx     5400 b- defN 21-Nov-16 19:37 airontools/constructors/models/unsupervised/ae_tf.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-16 15:28 airontools/constructors/models/unsupervised/ae_torch.py
+-rw-rw-r--  2.0 unx     6121 b- defN 21-Nov-16 19:38 airontools/constructors/models/unsupervised/vae_tf.py
+-rw-rw-r--  2.0 unx        0 b- defN 21-Nov-16 15:28 airontools/constructors/models/unsupervised/vae_torch.py
+-rw-rw-r--  2.0 unx      215 b- defN 21-Nov-15 14:00 airontools/constructors/utils/__init__.py
+-rw-rw-r--  2.0 unx     2216 b- defN 21-Nov-15 15:58 airontools/constructors/utils/utils_tf.py
+-rw-rw-r--  2.0 unx      175 b- defN 21-Nov-05 18:06 airontools/constructors/utils/utils_torch.py
+-rw-rw-r--  2.0 unx      197 b- defN 21-Nov-15 14:00 airontools/devices/__init__.py
+-rw-rw-r--  2.0 unx      209 b- defN 21-Nov-05 18:06 airontools/devices/devices_tf.py
+-rw-rw-r--  2.0 unx       90 b- defN 21-Nov-05 18:06 airontools/devices/devices_torch.py
+-rw-rw-r--  2.0 unx      213 b- defN 21-Nov-07 11:47 airontools/interactors/__init__.py
+-rw-rw-r--  2.0 unx     1150 b- defN 21-Nov-15 15:57 airontools/interactors/interactors_tf.py
+-rw-rw-r--  2.0 unx      396 b- defN 21-Nov-05 18:06 airontools/interactors/interactors_torch.py
+-rw-rw-r--  2.0 unx      324 b- defN 21-Nov-05 18:06 airontools/visualization/__init__.py
+-rw-rw-r--  2.0 unx     1011 b- defN 21-Nov-15 15:57 airontools/visualization/tensorboard_tf.py
+-rw-rw-r--  2.0 unx       78 b- defN 21-Nov-05 18:06 airontools/visualization/tensorboard_torch.py
+-rw-rw-r--  2.0 unx     1557 b- defN 21-Nov-15 15:57 airontools/visualization/utils_tf.py
+-rw-rw-r--  2.0 unx       80 b- defN 21-Nov-05 18:06 airontools/visualization/utils_torch.py
+-rw-rw-r--  2.0 unx     1525 b- defN 21-Nov-16 23:03 airontools-0.1.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3529 b- defN 21-Nov-16 23:03 airontools-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Nov-16 23:03 airontools-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 21-Nov-16 23:03 airontools-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4191 b- defN 21-Nov-16 23:03 airontools-0.1.9.dist-info/RECORD
+43 files, 65965 bytes uncompressed, 19897 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -6,45 +6,99 @@
 
 Filename: airontools/preprocessing.py
 Comment: 
 
 Filename: airontools/tools.py
 Comment: 
 
-Filename: airontools/devices/__init__.py
+Filename: airontools/constructors/__init__.py
+Comment: 
+
+Filename: airontools/constructors/blocks/__init__.py
+Comment: 
+
+Filename: airontools/constructors/blocks/blocks_tf.py
+Comment: 
+
+Filename: airontools/constructors/blocks/blocks_torch.py
+Comment: 
+
+Filename: airontools/constructors/layers/__init__.py
+Comment: 
+
+Filename: airontools/constructors/layers/layers_tf.py
+Comment: 
+
+Filename: airontools/constructors/layers/layers_torch.py
+Comment: 
+
+Filename: airontools/constructors/models/__init__.py
+Comment: 
+
+Filename: airontools/constructors/models/general/__init__.py
+Comment: 
+
+Filename: airontools/constructors/models/general/general_tf.py
 Comment: 
 
-Filename: airontools/devices/utils_tf.py
+Filename: airontools/constructors/models/general/general_torch.py
 Comment: 
 
-Filename: airontools/devices/utils_torch.py
+Filename: airontools/constructors/models/supervised/__init__.py
 Comment: 
 
-Filename: airontools/model_constructors/__init__.py
+Filename: airontools/constructors/models/supervised/classification/__init__.py
 Comment: 
 
-Filename: airontools/model_constructors/constructors_tf.py
+Filename: airontools/constructors/models/supervised/classification/classification_tf.py
 Comment: 
 
-Filename: airontools/model_constructors/constructors_torch.py
+Filename: airontools/constructors/models/supervised/classification/classification_torch.py
+Comment: 
+
+Filename: airontools/constructors/models/unsupervised/__init__.py
+Comment: 
+
+Filename: airontools/constructors/models/unsupervised/ae_tf.py
+Comment: 
+
+Filename: airontools/constructors/models/unsupervised/ae_torch.py
+Comment: 
+
+Filename: airontools/constructors/models/unsupervised/vae_tf.py
+Comment: 
+
+Filename: airontools/constructors/models/unsupervised/vae_torch.py
+Comment: 
+
+Filename: airontools/constructors/utils/__init__.py
+Comment: 
+
+Filename: airontools/constructors/utils/utils_tf.py
+Comment: 
+
+Filename: airontools/constructors/utils/utils_torch.py
+Comment: 
+
+Filename: airontools/devices/__init__.py
 Comment: 
 
-Filename: airontools/model_constructors/utils_tf.py
+Filename: airontools/devices/devices_tf.py
 Comment: 
 
-Filename: airontools/model_constructors/utils_torch.py
+Filename: airontools/devices/devices_torch.py
 Comment: 
 
-Filename: airontools/model_interactors/__init__.py
+Filename: airontools/interactors/__init__.py
 Comment: 
 
-Filename: airontools/model_interactors/model_interactors_tf.py
+Filename: airontools/interactors/interactors_tf.py
 Comment: 
 
-Filename: airontools/model_interactors/model_interactors_torch.py
+Filename: airontools/interactors/interactors_torch.py
 Comment: 
 
 Filename: airontools/visualization/__init__.py
 Comment: 
 
 Filename: airontools/visualization/tensorboard_tf.py
 Comment: 
@@ -54,23 +108,23 @@
 
 Filename: airontools/visualization/utils_tf.py
 Comment: 
 
 Filename: airontools/visualization/utils_torch.py
 Comment: 
 
-Filename: airontools-0.1.8.dist-info/LICENSE
+Filename: airontools-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: airontools-0.1.8.dist-info/METADATA
+Filename: airontools-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: airontools-0.1.8.dist-info/WHEEL
+Filename: airontools-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: airontools-0.1.8.dist-info/top_level.txt
+Filename: airontools-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: airontools-0.1.8.dist-info/RECORD
+Filename: airontools-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## airontools/preprocessing.py

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
-from sklearn.model_selection import KFold
 import random
 from random import seed
+from sklearn.model_selection import KFold
 
 
 def sub_sample(data, n):
     data_ = data.copy()
     data_.index = np.arange(data_.shape[0])
     return data.loc[:n-1, data_.columns]
 
@@ -44,16 +44,27 @@
         x_train += [input_data[train_inds, ...]]
         if val_ratio > 0:
             x_val += [input_data[val_inds, ...]]
         if output_data is not None:
             y_train += [output_data[train_inds, ...]]
         if val_ratio > 0 and output_data is not None:
             y_val += [output_data[val_inds, ...]]
+    # ToDo: improve next lines
+    if n_parallel_models == 1:
+        if len(x_train) > 0:
+            x_train = x_train[0]
+        if len(x_val) > 0:
+            x_val = x_val[0]
     returns = [x_train, x_val]
     if output_data is not None:
+        if n_parallel_models == 1:
+            if len(y_train) > 0:
+                y_train = y_train[0]
+            if len(y_val) > 0:
+                y_val = y_val[0]
         returns += [y_train, y_val]
     returns += [train_val_inds]
     return returns
 
 
 def update_specs(data_specs, input_data, output_data, cat_dictionary):
     """ Update specs given data specs and input and output data.
```

## airontools/devices/__init__.py

```diff
@@ -1,6 +1,6 @@
 from airontools.backend import get_backend
 BACKEND = get_backend()
-if BACKEND == 'tensorflow':
-    from airontools.devices.utils_tf import *
+if BACKEND == 'pytorch':
+    from airontools.devices.devices_torch import *
 else:
-    from airontools.devices.utils_torch import *
+    from airontools.devices.devices_tf import *
```

## airontools/visualization/tensorboard_tf.py

```diff
@@ -1,10 +1,10 @@
-from airontools.visualization.utils_tf import save_insights
-from airontools.model_constructors.utils_tf import get_latent_model
 from tensorflow.keras.models import Model
+from airontools.visualization.utils_tf import save_insights
+from airontools.constructors.utils.utils_tf import get_latent_model
 
 
 def get_insights(x, model, hidden_layer_names=None, **kwargs):
     """ Get insights of latent layers. Given input data and a model, this function makes use of tensorboard to get
     insights of the latent representations.
 
         Parameters:
```

## airontools/visualization/utils_tf.py

```diff
@@ -1,28 +1,28 @@
-import tempfile
-from airontools.tools import path_management
 import os
+import tempfile
 import tensorflow as tf
 from tensorboard.plugins import projector
+from airontools.tools import path_management
 
 
 def save_insights(embeddings, embeddings_names=None, metadata=None,
                   path=os.path.join(tempfile.gettempdir(), 'insights')):
     """ Save insights (embeddings or latent representations).
 
         Parameters:
             embeddings (list, array): Embeddings to be saved.
             embeddings_names (list, str): Embeddings names.
             metadata (list, array): Metadata.
             path (str): Path to save insights.
     """
 
     embeddings = embeddings if isinstance(embeddings, list) else [embeddings]
-    embeddings_names = embeddings_names if embeddings_names else list(['embeddings_' + str(i)
-                                                                       for i in range(len(embeddings))])
+    embeddings_names = embeddings_names if embeddings_names else \
+        list(['embeddings_' + str(i) for i in range(len(embeddings))])
 
     # Path management
     path_management(path)
 
     # Save metadata
     metadata_file_name = os.path.join(path, 'metadata.tsv')
     if metadata:
```

## Comparing `airontools/model_constructors/utils_tf.py` & `airontools/constructors/utils/utils_tf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+from sklearn.metrics import classification_report
 import tensorflow as tf
 from tensorflow.keras.models import Model
 from tensorflow.keras.mixed_precision import experimental as mixed_precision
 from tensorflow.keras import regularizers
 import tensorflow.keras.backend as k_bcknd
-from sklearn.metrics import classification_report
 import numpy as np
 
 
 def get_latent_model(model, layer_names):
     layer_names = layer_names if isinstance(layer_names, list) else [layer_names]
     return Model(inputs=model.inputs,
-                 outputs=[layer.outputs for layer in model.layers
+                 outputs=[layer.output for layer in model.layers
                           if any([layer_name in layer.name for layer_name in layer_names])])
 
 
 def set_precision(precision):
     if 'float16' in precision:
         if precision == 'mixed_float16':
             policy = mixed_precision.Policy('mixed_float16')
```

## Comparing `airontools/model_interactors/model_interactors_tf.py` & `airontools/interactors/interactors_tf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from tensorflow.keras.models import model_from_json, Model
-import tensorflow.keras.backend as bcknd
+import tensorflow.keras.backend as k_bcknd
 
 
 def save_model(model, name):
     model.save_weights(filepath=name + '_weights')
     with open(name + '_topology', "w") as json_file:
         json_file.write(model.to_json())
 
@@ -14,15 +14,15 @@
     json_file.close()
     model = model_from_json(loaded_model_json, custom_objects)
     model.load_weights(filepath=name + '_weights')
     return model
 
 
 def clear_session():
-    bcknd.clear_session()
+    k_bcknd.clear_session()
 
 
 def summary(model):
     """ Model summary.
 
         Parameters:
             model (Model): Model to summarize.
```

## Comparing `airontools-0.1.8.dist-info/LICENSE` & `airontools-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `airontools-0.1.8.dist-info/METADATA` & `airontools-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: airontools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Machine learning tools to complement the AIronSuit package.
 Home-page: https://github.com/AtrejuArtax/airontools
 Author: Claudi Ruiz Camps
 Author-email: claudi_ruiz@hotmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: sklearn
 
 # AIronTools
 
 AIronTools (Beta) is a Python library that provides the user with deep learning tools built to work with 
 [tensorflow](https://github.com/tensorflow/tensorflow) (or [pytorch](https://github.com/pytorch/pytorch) in the future) 
 as a backend.
 
 Key features:
 
 1. Model constructor that allows multiple models to be optimized in parallel across multiple GPUs. 
 2. Block constructor to build customised blocks/models.
 3. Layer constructor to build customised layers.
 4. Preprocessing utils.
-   
+
 ### Installation
 
 `pip install airontools`
 
 ### Custom Keras subclass to build a variational autoencoder (VAE) with airontools
 
 ``` python
```

