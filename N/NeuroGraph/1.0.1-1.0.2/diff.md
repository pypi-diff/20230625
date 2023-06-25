# Comparing `tmp/NeuroGraph-1.0.1.tar.gz` & `tmp/NeuroGraph-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NeuroGraph-1.0.1.tar", last modified: Fri Jun 23 22:15:51 2023, max compression
+gzip compressed data, was "dist/NeuroGraph-1.0.2.tar", last modified: Sun Jun 25 20:17:26 2023, max compression
```

## Comparing `NeuroGraph-1.0.1.tar` & `NeuroGraph-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,18 @@
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      158 2023-06-23 22:05:06.000000 NeuroGraph-1.0.1/NeuroGraph/__init__.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     4564 2023-06-23 18:40:47.000000 NeuroGraph-1.0.1/NeuroGraph/benchmarks_main.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     3372 2023-06-23 20:45:01.000000 NeuroGraph-1.0.1/NeuroGraph/load_dynamic_benchmarks_example.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     3383 2023-06-23 21:15:03.000000 NeuroGraph-1.0.1/NeuroGraph/main.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     4470 2023-06-21 23:13:52.000000 NeuroGraph-1.0.1/NeuroGraph/neurograph.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     2710 2023-06-22 21:53:48.000000 NeuroGraph-1.0.1/NeuroGraph/neurograph_dynamic.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)     3262 2023-06-23 15:52:48.000000 NeuroGraph-1.0.1/NeuroGraph/preprocess.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)    40900 2023-06-23 20:13:12.000000 NeuroGraph-1.0.1/NeuroGraph/preprocess_fmri.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)    10571 2023-06-23 20:10:30.000000 NeuroGraph-1.0.1/NeuroGraph/process_dynamic.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      432 2023-06-23 20:21:28.000000 NeuroGraph-1.0.1/NeuroGraph/setup.py
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      142 2023-06-23 21:46:04.000000 NeuroGraph-1.0.1/NeuroGraph/test.py
-drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph.egg-info/
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      493 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph.egg-info/PKG-INFO
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      477 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph.egg-info/SOURCES.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph.egg-info/dependency_links.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       53 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph.egg-info/requires.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       11 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/NeuroGraph.egg-info/top_level.txt
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      493 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/PKG-INFO
--rw-rw-r--   0 anwar     (1000) anwar     (1000)       38 2023-06-23 22:15:51.000000 NeuroGraph-1.0.1/setup.cfg
--rw-rw-r--   0 anwar     (1000) anwar     (1000)      796 2023-06-23 22:15:22.000000 NeuroGraph-1.0.1/setup.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     1067 2023-06-24 14:47:00.000000 NeuroGraph-1.0.2/LICENSE.txt
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/NeuroGraph/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        0 2023-06-25 15:58:57.000000 NeuroGraph-1.0.2/NeuroGraph/__init__.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     7067 2023-06-25 18:10:54.000000 NeuroGraph-1.0.2/NeuroGraph/datasets.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)    51030 2023-06-25 15:59:31.000000 NeuroGraph-1.0.2/NeuroGraph/preprocess.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      151 2023-06-25 20:10:33.000000 NeuroGraph-1.0.2/NeuroGraph/test.py
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)     3284 2023-06-25 20:10:42.000000 NeuroGraph-1.0.2/NeuroGraph/utils.py
+drwxrwxr-x   0 anwar     (1000) anwar     (1000)        0 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      309 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)        1 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       53 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/requires.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       11 2023-06-25 20:17:25.000000 NeuroGraph-1.0.2/NeuroGraph.egg-info/top_level.txt
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      519 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/PKG-INFO
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      169 2023-06-25 16:17:37.000000 NeuroGraph-1.0.2/README.md
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)       38 2023-06-25 20:17:26.000000 NeuroGraph-1.0.2/setup.cfg
+-rw-rw-r--   0 anwar     (1000) anwar     (1000)      797 2023-06-25 18:33:47.000000 NeuroGraph-1.0.2/setup.py
```

### Comparing `NeuroGraph-1.0.1/NeuroGraph/neurograph.py` & `NeuroGraph-1.0.2/NeuroGraph/datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from torch_geometric.data import Data, InMemoryDataset
 from torch_geometric.data import InMemoryDataset, download_url
 import os,glob
 import torch
 import zipfile
 
-
 class NeuroGraphStatic(InMemoryDataset):
+
     r"""
-    Graph-based neuroimaging benchmark datasets, *.e.g.*,
+    Graph-based neuroimaging benchmark datasets, e.g.,
     :obj:`"HCPGender"`, :obj:`"HCPAge"`, :obj:`"HCPActivity"`,
     :obj:`"HCP-WM"`, or :obj:`"HCP-FI"`
 
-
     Args:
         root (str): Root directory where the dataset should be saved.
         name (str): The `name
             <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
             dataset.
         transform (callable, optional): A function/transform that takes in an
             :obj:`torch_geometric.data.Data` object and returns a transformed
@@ -30,23 +29,22 @@
             value, indicating whether the data object should be included in the
             final dataset. (default: :obj:`None`)
         return: Pytorch geometric dataset
     """
 
     def __init__(self, root, dataset_name,transform=None, pre_transform=None, pre_filter=None):
         self.root, self.name = root, dataset_name
-        super().__init__(root, transform, pre_transform, pre_filter)
         self.root = root
         self.urls = {"HCPGender":'https://vanderbilt.box.com/shared/static/r6hlz2arm7yiy6v6981cv2nzq3b0meax.zip',
                     "HCPActivity":'https://vanderbilt.box.com/shared/static/b4g59ibn8itegr0rpcd16m9ajb2qyddf.zip',
                     "HCPAge":'https://vanderbilt.box.com/shared/static/lzzks4472czy9f9vc8aikp7pdbknmtfe.zip',
                     "HCPWM":'https://vanderbilt.box.com/shared/static/xtmpa6712fidi94x6kevpsddf9skuoxy.zip',
                     "HCPFI":'https://vanderbilt.box.com/shared/static/g2md9h9snh7jh6eeay02k1kr9m4ido9f.zip'
                     }
-        
+        super().__init__(root, transform, pre_transform, pre_filter)
         self.data, self.slices = torch.load(self.processed_paths[0])
 
     @property
     def raw_dir(self):
         return os.path.join(self.root,self.name, self.name+'raw')
     
     @property
@@ -95,7 +93,64 @@
 
         if self.pre_transform is not None:
             data_list = [self.pre_transform(data) for data in data_list]
 
         data, slices = self.collate(data_list)
         torch.save((data, slices), self.processed_paths[0])
        
+class NeuroGraphDynamic():
+
+    r"""
+    Graph-based neuroimaging benchmark datasets, *.e.g.*,
+    :obj:`"DynHCPGender"`, :obj:`"DynHCPAge"`, :obj:`"DynHCPActivity"`,
+    :obj:`"DynHCP-WM"`, or :obj:`"DynHCP-FI"`
+
+
+    Args:
+        root (str): Root directory where the dataset should be saved.
+        name (str): The `name
+            <https://anwar-said.github.io/anwarsaid/neurograph.html/>`_ of the
+            dataset.
+        
+        return: a list of graphs in pyg format. Each graph has dynamic graphs batched in pyg batch 
+    """
+
+    def __init__(self,root, name):
+        self.root = root
+        self.name = name
+        self.urls = {"DynHCPGender":'https://vanderbilt.box.com/shared/static/mj0z6unea34lfz1hkdwsinj7g22yohxn.zip',
+                    "DynHCPActivity":'https://vanderbilt.box.com/shared/static/2so3fnfqakeu6hktz322o3nm2c8ocus7.zip',
+                    "DynHCPAge":'https://vanderbilt.box.com/shared/static/195f9teg4t4apn6kl6hbc4ib4g9addtq.zip',
+                    "DynHCPWM":'https://vanderbilt.box.com/shared/static/mxy8fq3ghm60q6h7uhnu80pgvfxs6xo2.zip',
+                    "DynHCPFI":'https://vanderbilt.box.com/shared/static/un7w3ohb2mmyjqt1ou2wm3g87y1lfuuo.zip'
+                    }
+        if self.urls.get(name):
+            self.download(self.urls.get(name))
+        else:
+            print('dataset not found! The name of the datasets are: "DynHCPGender","DynHCPActivity","DynHCPAge","DynHCPWM","DynHCPFI"')
+        self.dataset, self.labels = self.load_data()
+    
+    def download(self,url):
+        
+        download_url(url, os.path.join(self.root, self.name))
+        basename = os.path.basename(url)
+        with zipfile.ZipFile(os.path.join(self.root,self.name,basename), 'r') as file:
+            file.extractall(os.path.join(self.root,self.name,os.path.dirname(basename)))
+            # self.remove(os.path.join(self.raw_dir,basename))
+    def load_data(self):
+        if self.name=='DynHCPActivity':
+            dataset_raw = torch.load(os.path.join(self.root,self.name,self.name,"processed", self.name+".pt"))
+            dataset,labels = [],[]
+            for v in dataset_raw:
+                batches = v.get('batches')
+                if len(batches)>0:
+                    for b in batches:
+                        y = b.y[0].item()
+                        dataset.append(b)
+                        labels.append(y)
+        else:
+            dataset = torch.load(os.path.join(self.root,self.name,self.name,"processed", self.name+".pt"))
+            labels = dataset['labels']
+            dataset = dataset['batches']
+        return dataset,labels
+    
+
```

### Comparing `NeuroGraph-1.0.1/NeuroGraph/preprocess.py` & `NeuroGraph-1.0.2/NeuroGraph/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from nilearn.datasets import fetch_atlas_schaefer_2018
 from nilearn.image import load_img
 from nilearn.connectome import ConnectivityMeasure
 from scipy.stats import zscore
 import torch
 from torch_geometric.data import Data
 
+
 def preprocess(fmri,regs, n_rois =1000):
     """
     Preprocess fMRI data using NeuroGraph preprocessing pipeline
 
     Args:
 
     fmri (numpy array): fmri image
@@ -53,27 +54,29 @@
     np.fill_diagonal(fc, 0)
 
     # zscored upper triangle
     zd_fc *= 1 - np.tri(*zd_fc.shape, k=-1)
     np.fill_diagonal(zd_fc, 0)
     corr = fc + zd_fc
     return corr
+
+
 def construct_Adj(corr, threshold=5):
     """
     create adjacency matrix from functional connectome matrix
     
     Args:
-
+    
     corr (n x n numpy matrix): functional connectome matrix
 
     Threshold (int (1- 100)): threshold for controling graph density. 
 
     the more higher the threshold, the more denser the graph. default: 5 
-    
     """
+
     corr_matrix_copy = corr.copy()
     threshold = np.percentile(corr_matrix_copy[corr_matrix_copy > 0], 100 - threshold)
     corr_matrix_copy[corr_matrix_copy < threshold] = 0
     corr_matrix_copy[corr_matrix_copy >= threshold] = 1
     return corr_matrix_copy
 
 def construct_data(corr, label, threshold = 5):
@@ -85,15 +88,16 @@
 
     Threshold (int (1- 100)): threshold for controling graph density. 
 
     the more higher the threshold, the more denser the graph. default: 5 
 
     
     """
-    A = corr.copy()
+    
+    A = torch.tensor(corr.copy())
     threshold = np.percentile(A[A > 0], 100 - threshold)
     A[A < threshold] = 0
     A[A >= threshold] = 1
     edge_index = A.nonzero().t().to(torch.long)
     data = Data(x = corr, edge_index=edge_index, y = label)
     return data
```

### Comparing `NeuroGraph-1.0.1/setup.py` & `NeuroGraph-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='NeuroGraph',
-    version='1.0.1',
+    version='1.0.2',
     description='A Python package for graph-based Neuroimaging benchmarks and tools',
     author='Anwar Said',
     author_email='<anwar.said@vanderbilt.edu>',
     packages=['NeuroGraph'],
     install_requires=[
         # List any dependencies your package requires
         'boto3==1.26.158',
@@ -19,8 +19,8 @@
      classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering',
     ],
-)
+)
```

