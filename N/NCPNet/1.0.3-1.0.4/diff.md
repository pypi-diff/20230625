# Comparing `tmp/NCPNet-1.0.3.tar.gz` & `tmp/NCPNet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NCPNet-1.0.3.tar", last modified: Wed Jun 21 12:48:13 2023, max compression
+gzip compressed data, was "NCPNet-1.0.4.tar", last modified: Sun Jun 25 10:51:40 2023, max compression
```

## Comparing `NCPNet-1.0.3.tar` & `NCPNet-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     1073 2023-06-13 10:35:09.000000 NCPNet-1.0.3/LICENSE
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/NCPNet/
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)      160 2023-06-21 12:23:37.000000 NCPNet-1.0.3/NCPNet/__init__.py
--rw-rw-r--   0 wgj       (1024) wgj       (1025)       83 2023-06-21 12:27:02.000000 NCPNet-1.0.3/NCPNet/__main__.py
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/NCPNet/approaches/
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     4859 2023-06-13 03:06:30.000000 NCPNet-1.0.3/NCPNet/approaches/Decoder.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     5326 2023-06-13 02:30:59.000000 NCPNet-1.0.3/NCPNet/approaches/Encoder.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2921 2023-06-21 12:09:19.000000 NCPNet-1.0.3/NCPNet/approaches/PairEncoder.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)      217 2023-06-21 11:53:03.000000 NCPNet-1.0.3/NCPNet/approaches/__init__.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     6961 2023-06-21 11:58:54.000000 NCPNet-1.0.3/NCPNet/approaches/method.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)    27693 2023-06-21 12:26:48.000000 NCPNet-1.0.3/NCPNet/brain_data.py
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     2086 2023-06-21 12:33:41.000000 NCPNet-1.0.3/NCPNet/predict.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     4988 2023-06-13 03:06:48.000000 NCPNet-1.0.3/NCPNet/task.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)    22453 2023-06-21 02:52:51.000000 NCPNet-1.0.3/NCPNet/trainer.py
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2107 2023-06-20 10:43:06.000000 NCPNet-1.0.3/NCPNet/utils.py
-drwxrwxr-x   0 wgj       (1024) wgj       (1025)        0 2023-06-21 12:48:13.278123 NCPNet-1.0.3/NCPNet.egg-info/
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     3295 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/PKG-INFO
--rw-rw-r--   0 wgj       (1024) wgj       (1025)      450 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/SOURCES.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)        1 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/dependency_links.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)      180 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/requires.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)        7 2023-06-21 12:48:13.000000 NCPNet-1.0.3/NCPNet.egg-info/top_level.txt
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     3295 2023-06-21 12:48:13.278123 NCPNet-1.0.3/PKG-INFO
--rwxrwxr-x   0 wgj       (1024) wgj       (1025)     2797 2023-06-21 12:47:26.000000 NCPNet-1.0.3/README.md
--rw-rw-r--   0 wgj       (1024) wgj       (1025)       38 2023-06-21 12:48:13.278123 NCPNet-1.0.3/setup.cfg
--rw-rw-r--   0 wgj       (1024) wgj       (1025)     1128 2023-06-21 12:46:00.000000 NCPNet-1.0.3/setup.py
+drwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)        0 2023-06-25 10:51:40.777199 NCPNet-1.0.4/
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)     1073 2023-06-25 07:32:36.000000 NCPNet-1.0.4/LICENSE
+drwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)        0 2023-06-25 10:51:40.773199 NCPNet-1.0.4/NCPNet/
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)      175 2023-06-25 09:03:48.000000 NCPNet-1.0.4/NCPNet/__init__.py
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)       83 2023-06-25 07:32:36.000000 NCPNet-1.0.4/NCPNet/__main__.py
+drwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)        0 2023-06-25 10:51:40.777199 NCPNet-1.0.4/NCPNet/approaches/
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     4909 2023-06-25 08:35:28.000000 NCPNet-1.0.4/NCPNet/approaches/Decoder.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     5305 2023-06-25 08:57:39.000000 NCPNet-1.0.4/NCPNet/approaches/Encoder.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     2931 2023-06-25 08:36:29.000000 NCPNet-1.0.4/NCPNet/approaches/PairEncoder.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)      217 2023-06-25 07:32:36.000000 NCPNet-1.0.4/NCPNet/approaches/__init__.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     6774 2023-06-25 09:10:28.000000 NCPNet-1.0.4/NCPNet/approaches/method.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)    18713 2023-06-25 09:02:50.000000 NCPNet-1.0.4/NCPNet/brain_data.py
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)     9107 2023-06-25 09:02:38.000000 NCPNet-1.0.4/NCPNet/loader.py
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)     2111 2023-06-25 09:06:33.000000 NCPNet-1.0.4/NCPNet/predict.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     4988 2023-06-25 07:32:36.000000 NCPNet-1.0.4/NCPNet/task.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)    22453 2023-06-25 07:32:36.000000 NCPNet-1.0.4/NCPNet/trainer.py
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     2107 2023-06-25 07:32:36.000000 NCPNet-1.0.4/NCPNet/utils.py
+drwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)        0 2023-06-25 10:51:40.777199 NCPNet-1.0.4/NCPNet.egg-info/
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)     6723 2023-06-25 10:51:40.000000 NCPNet-1.0.4/NCPNet.egg-info/PKG-INFO
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)      467 2023-06-25 10:51:40.000000 NCPNet-1.0.4/NCPNet.egg-info/SOURCES.txt
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)        1 2023-06-25 10:51:40.000000 NCPNet-1.0.4/NCPNet.egg-info/dependency_links.txt
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)      187 2023-06-25 10:51:40.000000 NCPNet-1.0.4/NCPNet.egg-info/requires.txt
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)        7 2023-06-25 10:51:40.000000 NCPNet-1.0.4/NCPNet.egg-info/top_level.txt
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)     6723 2023-06-25 10:51:40.777199 NCPNet-1.0.4/PKG-INFO
+-rwxrwxr-x   0 wanguojia  (1013) wanguojia  (1013)     6225 2023-06-25 10:50:25.000000 NCPNet-1.0.4/README.md
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)       38 2023-06-25 10:51:40.777199 NCPNet-1.0.4/setup.cfg
+-rw-rw-r--   0 wanguojia  (1013) wanguojia  (1013)     1146 2023-06-25 10:36:40.000000 NCPNet-1.0.4/setup.py
```

### Comparing `NCPNet-1.0.3/LICENSE` & `NCPNet-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.3/NCPNet/approaches/Decoder.py` & `NCPNet-1.0.4/NCPNet/approaches/Decoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,28 @@
         x=x.sum(dim=-1)
         x=x.view(-1)
         x=torch.sigmoid(x)
         return x
 class mlp_predictor(torch.nn.Module):
     def __init__(self,config) -> None:
         super().__init__()
-        self.mlp=torch.nn.Sequential(Linear(config['out_channels']*2,256,bias=True),Dropout(inplace=True),ReLU(inplace=True),\
-            Linear(256,128,bias=True),Dropout(inplace=True),ReLU(inplace=True),Linear(128,1,bias=False))
+        self.mlp=torch.nn.Sequential(Linear(config['out_channels']*2,256,bias=True),Dropout(config['dropout']),ReLU(config['dropout']),\
+            Linear(256,128,bias=True),Dropout(config['dropout']),ReLU(config['dropout']),Linear(128,1,bias=False))
    
     def forward(self,e1,e2):
         x=torch.cat((e1,e2),1)
         x=self.mlp(x)
         x=torch.sigmoid(x)
         x=x.view(-1)
         return x
 class mlptri_predictor(torch.nn.Module):
     def __init__(self,config) -> None:
         super().__init__()
-        self.mlp=torch.nn.Sequential(Linear(config['out_channels']*3,256,bias=True),Dropout(inplace=True),ReLU(inplace=True),\
-            Linear(256,128,bias=True),Dropout(inplace=True),ReLU(inplace=True),Linear(128,1,bias=False))
+        self.mlp=torch.nn.Sequential(Linear(config['out_channels']*3,256,bias=True),Dropout(config['dropout']),ReLU(config['dropout']),\
+            Linear(256,128,bias=True),Dropout(config['dropout']),ReLU(config['dropout']),Linear(128,1,bias=False))
     def forward(self,e1,e2,n):
         x=torch.cat((e1,e2,n),1)
         x=self.mlp(x)
         x=torch.sigmoid(x)
         x=x.view(-1)
         return x
 class lstm_predictor(torch.nn.Module):
@@ -76,15 +76,15 @@
         x=x.view(-1)
         return x
 
 class joint_predictor(torch.nn.Module):
     def __init__(self,config) -> None:
         super().__init__()
         self.model_config = config
-        self.mlp=torch.nn.Sequential(Linear(config['out_channels']*2,256,bias=True),Dropout(inplace=True),ReLU(inplace=True),\
+        self.mlp=torch.nn.Sequential(Linear(config['out_channels']*2,256,bias=True),Dropout(config['dropout']),ReLU(config['dropout']),\
             Linear(256,config['out_channels'],bias=True))
         self.lin1=torch.nn.Linear(config['out_channels'],1,bias=True)
 
     def forward(self,x1,x2,x3):
         x=torch.cat((x1,x2),1)
         p1=self.mlp(x)
         p=torch.stack([p1,x3],dim=1)
```

### Comparing `NCPNet-1.0.3/NCPNet/approaches/Encoder.py` & `NCPNet-1.0.4/NCPNet/approaches/Encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import torch.nn.functional as F
 import numpy as np
 from torch_geometric.nn.conv import MessagePassing
 class node_attr_encoder(torch.nn.Module):
     def __init__(self, config):
         super(node_attr_encoder, self).__init__()
         self.model_config = config
-        self.drop1 = torch.nn.Dropout(inplace=True)
+        self.drop1 = torch.nn.Dropout(config['dropout'])
         if (self.model_config['num_node']) is None or (self.model_config['use_type_info']):
             self.x_embddings = torch.nn.Linear(self.model_config['type_dim'], self.model_config['dim'], bias=False)
         else:
             self.x = torch.nn.Parameter(
                 torch.empty(size=(self.model_config['num_node'], self.model_config['dim']), dtype=torch.float32),
                 requires_grad=True)
             xavier_normal_(self.x)
@@ -30,15 +30,15 @@
     def __init__(self,conv:MessagePassing,use_type_info=None,activation='relu',dropout='0.5'):
         self.conv=conv
         if activation=='relu':
             self.activ=torch.nn.ReLU()
         else:
             pass
         if dropout is not None:
-            self.drop=torch.nn.Dropout(inplace=True)
+            self.drop=torch.nn.Dropout(dropout)
     def forward(self, x=None, edge_index=None,
                 edge_weight = None):
         x=self.conv(x,edge_index,edge_weight=edge_weight)
         if hasattr(self,'activ'):
             x=self.activ(x)
         x=self.activ(x)
         if hasattr(self,'drop'):
@@ -50,15 +50,15 @@
         super().__init__()
         self.model_config = config
         self.node_attr_layer=node_attr_encoder(config)
         self.conv1=GCNConv(self.model_config['dim'], self.model_config['hidden_channels'])
         
         
         self.relu1=torch.nn.ReLU()
-        self.drop1=torch.nn.Dropout(inplace=True)
+        self.drop1=torch.nn.Dropout(config['dropout'])
         self.conv2 = GCNConv(self.model_config['hidden_channels'], self.model_config['out_channels'])
 
     def forward(self,x=None, edge_index=None):
 
         x=self.node_attr_layer(x)
        
         x=self.conv1(x,edge_index)
@@ -72,15 +72,15 @@
         super().__init__()
         self.model_config = config
         self.node_attr_layer=node_attr_encoder(config)
         
         #self.convs = torch.nn.ModuleList()
         self.conv1=torch.nn.Linear(self.model_config['dim'], self.model_config['hidden_channels'])
         self.relu1=torch.nn.ReLU()
-        self.drop1=torch.nn.Dropout(inplace=True)
+        self.drop1=torch.nn.Dropout(config['dropout'])
         self.conv2=torch.nn.Linear(self.model_config['hidden_channels'], self.model_config['out_channels'])
     def forward(self,x=None, edge_index=None):
         x=self.node_attr_layer(x)
         x=self.conv1(x)
         x=self.relu1(x)
         x=self.drop1(x)
         x=self.conv2(x)
@@ -94,15 +94,15 @@
         self.hidden=config['hidden_channels']
         self.out_channel=config['out_channels']
         self.conv1=GCNConv(self.model_config['dim'], self.out_channel)
         self.convs = torch.nn.ModuleList()
         for i in range(self.num_layers - 1):
             self.convs.append(Sequential(
                         ReLU(),
-                        torch.nn.Dropout(inplace=True),
+                        torch.nn.Dropout(config['dropout']),
                         GCNConv(self.out_channel,self.out_channel),
                     ))
     def forward(self,x=None, edge_index=None):
         x=self.node_attr_layer(x)
         x=self.conv1(x,edge_index)
         for conv in self.convs:
             x=conv[0](x)
@@ -130,12 +130,8 @@
                         ReLU()
                     ), train_eps=True))
     def forward(self,x=None, edge_index=None):
         x=self.node_attr_layer(x)
         x=self.conv1(x,edge_index)
         for conv in self.convs:
             x=conv(x,edge_index)
-        return x
-
-
-if __name__=='__main__':
-    pass
+        return x
```

### Comparing `NCPNet-1.0.3/NCPNet/approaches/PairEncoder.py` & `NCPNet-1.0.4/NCPNet/approaches/PairEncoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     def __init__(self,config) -> None:
         super().__init__()
         self.model_config = config
         self.lookupneigh=Lookup_neighbor_embedding(config)
         self.conv1=torch.nn.Conv1d(config['out_channels'],int(config['out_channels']*0.5),kernel_size=1,bias=False)
 
         self.act_f1=nn.LeakyReLU(0.05)
-        self.dp1=torch.nn.Dropout(inplace=True)
+        self.dp1=torch.nn.Dropout(config['dropout'])
         
         self.conv2=torch.nn.Conv1d(int(config['out_channels']*0.5),config['out_channels']-int(config['out_channels']*0.5),kernel_size=1,bias=False)
         self.act_f2=nn.LeakyReLU(0.05)
-        self.dp2=torch.nn.Dropout(inplace=True)
+        self.dp2=torch.nn.Dropout(config['dropout'])
     def forward(self,z,neighbor=None):
         if len(neighbor.squeeze())==0:
             return torch.zeros(size=(len(neighbor),self.model_config['out_channels']))
         else:
             x=self.lookupneigh(z,neighbor)
             x=x.permute((0,2,1)).contiguous()
             x=self.conv1(x)
```

### Comparing `NCPNet-1.0.3/NCPNet/approaches/method.py` & `NCPNet-1.0.4/NCPNet/approaches/method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 
 import torch
-#from torch_geometric.nn import GCNConv
-#from torch.nn import Sequential, Linear, BatchNorm1d, ReLU,LayerNorm
-
 from .Encoder import GCN,GCN2,MLP,node_attr_encoder
 from .Decoder import LinkPred
 from .PairEncoder import NeighEnco,NeighEnco2
 from os.path import join
 import pickle
 import yaml
 import os
 from NCPNet.utils import edge_index2Graph
-from NCPNet.brain_data import LinkPred_PairNeigh_Loader
+from NCPNet.loader import LinkPred_PairNeigh_Loader
 import random
 class Net(torch.nn.Module):
     def __init__(self,config,cache_nxg=False):
         super(Net,self).__init__()
         self.config=config
         node_encoder=self.config['node_encoder']
         if 'pair_encoder' in self.config:
@@ -23,15 +20,14 @@
             self.use_pair_enco=True
             if'gamma' in self.config:
                 self.gamma=self.config['gamma']
             else:
                 self.gamma=0.5
         else:
             self.use_pair_enco=False
-
         decoder=self.config['Model']
         namespace=globals()
         if decoder in namespace and node_encoder in namespace:
             Deco_cls,node_Enco_cls=namespace[decoder],namespace[node_encoder]
             self.Deco,self.node_Enco=Deco_cls(config),node_Enco_cls(config)
         else:
             raise ModuleNotFoundError('%s or %s not found'%(decoder,node_encoder))
@@ -56,17 +52,15 @@
         if not hasattr(self,'train_edges'):
             self.X=torch.nn.parameter.Parameter(data=self.train_data.data.x.detach(),requires_grad=False)
             with torch.no_grad():
                 z=self.node_Enco(x=self.X,edge_index=self.train_data.data.edge_index)
                 self.z=torch.nn.parameter.Parameter(data=z.detach(),requires_grad=False)
             
     def forward(self,*args,**kwargs):
-
         z=self.node_Enco(x=kwargs['x'],edge_index=kwargs['edge_index'])
-        #x1=self.Deco(z,edge_label_index=kwargs['edge_label_index'])
         if self.use_pair_enco:
 
             out=self.Deco(z,edge_label_index=kwargs['edge_label_index'],neighbor=kwargs['neighbor'])
         else:
             out=self.Deco(z,edge_label_index=kwargs['edge_label_index'])
         return out
     def _create_setnxg(self,nxg):
@@ -158,11 +152,10 @@
                 pickle.dump((self,train_data,self.config),pkl)
             else:
                 pickle.dump((self,self.config),pkl)
     @staticmethod
     def loadfrom(filepath):
         with open(filepath,'rb') as fin:
             model,train_data,config=pickle.load(fin)
-
         if model.train_data is None:
             model.train_data=train_data
         return model
```

### Comparing `NCPNet-1.0.3/NCPNet/brain_data.py` & `NCPNet-1.0.4/NCPNet/brain_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -39,32 +39,32 @@
         if device is None:
             self.device='cpu'
         else:
             self.device=device
         if process:
             self._process()
         if restore_split is None:
-            self.data, self.slices = torch.load(self.processed_paths[0],map_location=self.device)
+            self._data, self.slices = torch.load(self.processed_paths[0],map_location=self.device)
         elif isinstance(restore_split,str):
-            self.data= torch.load(restore_split,map_location=self.device)
-        self.data, self.slices = self.collate([self.data])
+            self._data= torch.load(restore_split,map_location=self.device)
+        self._data, self.slices = self.collate([self._data])
 
     @property
     def num_edges(self):
-        return self.data.edge_index.size(0)
+        return self._data.edge_index.size(0)
     @property
     def edge_index(self):
-        return self.data.edge_index
+        return self._data.edge_index
     @property
     def y(self):
-        return self.data.y
+        return self._data.y
     
     @property
     def num_nodes(self):
-        return self.data.num_nodes
+        return self._data.num_nodes
     @property
     def raw_dir(self) -> str:
         return osp.join(self.root, 'raw')
 
     @property
     def processed_dir(self) -> str:
         return osp.join(self.root, 'processed')
@@ -204,234 +204,28 @@
                     train_edge_index.append([n1,n2])
         train_edge_index=torch.tensor(train_edge_index).T
 
         total_edges=test_edge_index.size(1)+train_edge_index.size(1)
         if test_edge_index.size(1)>int(total_edges*0.1):
             test_edge_index=test_edge_index[:,:int(total_edges*0.1)]
 
-        test_edge_index=test_edge_index.to(device=self.data.x.device)
-        train_edge_index=train_edge_index.to(device=self.data.x.device)
+        test_edge_index=test_edge_index.to(device=self._data.x.device)
+        train_edge_index=train_edge_index.to(device=self._data.x.device)
 
 
-        test_data=Data(x=self.data.x,y=self.data.y,edge_index=test_edge_index,neu2ID=neu2ID,label2ID=label2ID)
-        train_data=Data(x=self.data.x,y=self.data.y,edge_index=train_edge_index,neu2ID=neu2ID,label2ID=label2ID)
+        test_data=Data(x=self._data.x,y=self._data.y,edge_index=test_edge_index,neu2ID=neu2ID,label2ID=label2ID)
+        train_data=Data(x=self._data.x,y=self._data.y,edge_index=train_edge_index,neu2ID=neu2ID,label2ID=label2ID)
         return train_data,test_data
 
 
 
 
 
     def __repr__(self) -> str:
         return 'HemiBrain'
-
-class LinkPred_Loader:
-    def __init__(self,config,dataset: InMemoryDataset):
-        self.dataset=dataset
-        self.loader_config=config
-        if 'negtive_num' in self.loader_config:
-            self.negtive_num=self.loader_config['negtive_num']
-        else:
-            self.negtive_num=1
-
-        if 'batch_size' in self.loader_config:
-            self.batch_size=self.loader_config['batch_size']
-        else:
-            if dataset.edge_index.size(1)*(self.negtive_num+1)*self.loader_config['dim']<int(8*1024*1024*1024/12):
-                self.batch_size=dataset.edge_index.size(1)
-            else:
-                self.batch_size=min(500000,dataset.edge_index.size(1))
-        self.step=0
-    def __iter__(self):
-        self.step=0
-
-        neg_edge_index = negative_sampling(
-            edge_index=self.dataset.edge_index, num_nodes=self.dataset.num_nodes,
-            num_neg_samples=self.dataset.edge_index.size(1)*self.negtive_num, method='sparse')
-        self.edge_label_index = torch.cat(
-            [self.dataset.edge_index, neg_edge_index],
-            dim=-1
-        )
-        
-        self.edge_label = torch.cat([
-            self.dataset.edge_index.new_ones(self.dataset.edge_index.size(1),dtype=torch.float32),neg_edge_index.new_zeros(neg_edge_index.size(1),dtype=torch.float32)
-        ], dim=0)
-        perm = torch.randperm(self.edge_label_index.size(1),device=self.edge_label.device)
-        self.batch_index=torch.split(perm,self.batch_size)
-        # split_num=ceil(self.edge_label_index.size(1)/self.batch_size)
-        # self.batchs_edge_index=torch.hsplit(self.edge_label_index,split_num)
-        self.edge_label_index=self.edge_label_index.T
-        self.edge_label=self.edge_label.T
-        return self
-    def __next__(self):
-        if self.step>=len(self.batch_index):
-            raise StopIteration
-        else:
-            ind=self.batch_index[self.step]
-            edge_label_index=torch.nn.functional.embedding(ind,self.edge_label_index)
-            edge_label_index=edge_label_index.T
-            edge_label=torch.nn.functional.embedding(ind,self.edge_label)
-            edge_label=edge_label.T
-            batch=(self.dataset.x,self.dataset.edge_index,self.dataset.edge_attr,edge_label_index,edge_label)
-            self.step+=1
-        return batch
-    def __len__(self):
-        return len(self.batch_index)
-class LinkPred_PairNeigh_Loader(LinkPred_Loader):
-    def __init__(self,config,dataset: InMemoryDataset,nxg:nx.Graph,hop=1):
-        self.dataset=dataset
-        self.loader_config=config
-        if 'negtive_num' in self.loader_config:
-            self.negtive_num=self.loader_config['negtive_num']
-        else:
-            self.negtive_num=1
-
-        if 'batch_size' in self.loader_config:
-            self.batch_size=self.loader_config['batch_size']
-        else:
-            if dataset.edge_index.size(1)*(self.negtive_num+1)*self.loader_config['dim']<int(8*1024*1024*1024/12):
-                self.batch_size=dataset.edge_index.size(1)
-            else:
-                self.batch_size=min(500000,dataset.edge_index.size(1))
-        self.nxg={}
-        for n in nxg.nodes():
-            self.nxg[n]=set(nxg[n])
-        for i in range(dataset.num_nodes):
-            if i not in self.nxg:
-                self.nxg[i]=set([])
-        for i in range(hop-1):
-            for n in self.nxg.keys():
-                q=list(self.nxg[n])
-                for j in q:
-                    if j !=n:
-                        for kj in self.nxg[j]:
-                            if kj not in self.nxg[n] and kj!=n:
-                                self.nxg[n].add(kj)
-        self.cached_nxg_neighbors=None
-        self.step=0
-        self.max_pad_num=None
-    
-    def get_neighboor(self,edge_index,mode='inter',max_num=30):
-        edge_index_list=edge_index.cpu().T.tolist()
-        res=[]
-        
-     
-        if mode=='inter':
-  
-            for edges in edge_index_list:
-                u,v=tuple(edges)
-                u_set,v_set=self.nxg[u],self.nxg[v]
-
-                pair=u_set.intersection(v_set)
-                pair=pair.difference({u,v})
-                neigh=list(pair)
-                if len(neigh)>max_num:
-                    #random.sample(neigh,max_num)
-                    res.append(random.sample(neigh,max_num))
-                else:
-                    res.append(neigh)
-        res=[torch.tensor(i,dtype=torch.int32)+1 for i in res]
-        out=torch.nn.utils.rnn.pad_sequence(res,batch_first=False).T
-        return out
-    def __iter__(self):
-        self.step=0
-        neg_edge_index = negative_sampling(
-            edge_index=self.dataset.edge_index, num_nodes=self.dataset.num_nodes,
-            num_neg_samples=self.dataset.edge_index.size(1)*self.negtive_num, method='sparse')
-        if self.cached_nxg_neighbors is None:
-            self.cached_nxg_neighbors=self.get_neighboor(self.dataset.edge_index)
-
-        neg_nxg_neighbors=self.get_neighboor(neg_edge_index)
-
-        if neg_nxg_neighbors.size(1)<self.cached_nxg_neighbors.size(1):
-            d=self.cached_nxg_neighbors.size(1)-neg_nxg_neighbors.size(1)
-            neg_nxg_neighbors=torch.cat([neg_nxg_neighbors,torch.zeros(size=(neg_nxg_neighbors.size(0),d),dtype=torch.int32)],dim=1)
-        elif neg_nxg_neighbors.size(1)>self.cached_nxg_neighbors.size(1):
-            d=neg_nxg_neighbors.size(1)-self.cached_nxg_neighbors.size(1)
-            self.cached_nxg_neighbors=torch.cat([self.cached_nxg_neighbors,torch.zeros(size=(self.cached_nxg_neighbors.size(0),d),dtype=torch.int32)],dim=1)
-        assert self.cached_nxg_neighbors.size(1)==neg_nxg_neighbors.size(1)
-
-        self.neighbors=torch.cat([self.cached_nxg_neighbors,neg_nxg_neighbors],dim=0)
-        self.neighbors=self.neighbors.to(device=self.loader_config['device'])
-        self.edge_label_index = torch.cat(
-            [self.dataset.edge_index, neg_edge_index],
-            dim=-1
-        )
-        
-        self.edge_label = torch.cat([
-            self.dataset.edge_index.new_ones(self.dataset.edge_index.size(1),dtype=torch.float32),neg_edge_index.new_zeros(neg_edge_index.size(1),dtype=torch.float32)
-        ], dim=0)
-        perm = torch.randperm(self.edge_label_index.size(1),device=self.edge_label.device)
-        self.batch_index=torch.split(perm,self.batch_size)
-        # split_num=ceil(self.edge_label_index.size(1)/self.batch_size)
-        # self.batchs_edge_index=torch.hsplit(self.edge_label_index,split_num)
-        self.edge_label_index=self.edge_label_index.T
-        self.edge_label=self.edge_label.T
-        return self
-    def __next__(self):
-        if self.step>=len(self.batch_index):
-            raise StopIteration
-        else:
-            ind=self.batch_index[self.step]
-            edge_label_index=torch.nn.functional.embedding(ind,self.edge_label_index)
-            edge_label_index=edge_label_index.T
-            edge_label=torch.nn.functional.embedding(ind,self.edge_label)
-            #edge_label=self.edge_label[ind]
-            edge_label=edge_label.T
-            batch_neighbor=torch.nn.functional.embedding(ind,self.neighbors)
-            batch=(self.dataset.x,self.dataset.edge_index,self.dataset.edge_attr,edge_label_index,edge_label,batch_neighbor)
-            self.step+=1
-        return batch
-    def __len__(self):
-        return len(self.batch_index)
-
-class NodeCla_Loader:
-    '''for small graph'''
-    def __init__(self,dataset: InMemoryDataset):
-        self.dataset=dataset
-        self.batch_num=1
-        self.step=0
-    def __iter__(self):
-        self.step=0
-        return self
-    def __next__(self):
-        if self.step >= self.batch_num:
-            raise StopIteration
-        batch=(self.dataset.x, self.dataset.edge_index,self.dataset.edge_attr,self.dataset.y,self.dataset.train_mask,self.dataset.test_mask)
-        self.step+=1
-        return batch
-class Scale_NodeCla_Loader:
-    def __init__(self,dataset: InMemoryDataset,subgraph_num=40,shuffle=True):
-        self.dataset=dataset
-        self.batch_num=subgraph_num
-        self.step=0
-        self.subgraph_num=subgraph_num
-        self.chunk_size=int(self.dataset.edge_index.size()[1]/self.subgraph_num)
-        self.shuffle=shuffle
-        #self.update()
-    def update(self):
-        edge_index=self.dataset.edge_index
-        edge_idx=np.arange(0,edge_index.size()[1])
-        if self.shuffle:
-            np.random.shuffle(edge_idx)
-        device=edge_index.data.device
-        self.iter_idx=torch.split(torch.from_numpy(edge_idx).to(device=device),self.chunk_size)
-    def __iter__(self):
-        self.update()
-        return self
-    def __next__(self):
-        if self.step >= self.batch_num:
-            raise StopIteration
-        else:
-            batch_id=self.iter_idx[self.step]
-            batch_edge_index=torch.nn.functional.embedding(batch_id,self.dataset.edge_index.T)
-            batch_edge_index=batch_edge_index.T
-            batch=(self.dataset.x, batch_edge_index,self.dataset.edge_attr,self.dataset.y,self.dataset.train_mask,self.dataset.test_mask)
-            self.step+=1
-        return batch
-
 class Celegans19(InMemoryDataset):
     r"""
     Args:
         root (string): Root directory where the dataset should be saved.
         name (string): The name of the dataset (:obj:`"Male"`,
             :obj:`"Hermaphrodite"`).
         transform (callable, optional): A function/transform that takes in an
@@ -508,14 +302,17 @@
             Neuron2ID={k:v for v,k in enumerate(Neuron2Type.keys())}
             self.neu2ID_dict=Neuron2ID
             type_set=set(Neuron2Type.values())
             Type2id={k:v for v,k in enumerate(type_set)}
             self.label2ID_dict=Type2id
         return self.label2ID_dict
     @property
+    def num_nodes(self):
+        return self._data.num_nodes
+    @property
     def typedim(self):
         if hasattr(self,'cache_type_dim'):
             return self.cache_type_dim
         else:
             label2ID=self.label2ID
             self.cache_type_dim=len(label2ID.keys())
             return self.cache_type_dim
@@ -643,16 +440,14 @@
         if process:
             self._process()
         if restore_split is None:
             self.data, self.slices = torch.load(self.processed_paths[0],map_location=self.device)
         elif isinstance(restore_split,str):
             self.data= torch.load(restore_split,map_location=self.device)
         self.data, self.slices = self.collate([self.data])
-    
-    
 class NxGraph(InMemoryDataset):
     url=None
     def __init__(self, root: Optional[str] = None, nxg='barbell',transform: Optional[Callable] = None, pre_transform: Optional[Callable] = None, pre_filter: Optional[Callable] = None,**kwargs):
         
         
         self.kwargs=kwargs
         if isinstance(nxg,str):
```

### Comparing `NCPNet-1.0.3/NCPNet/predict.py` & `NCPNet-1.0.4/NCPNet/predict.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import sys
 import os.path as osp
 
 import traceback
 import copy
 import argparse
 import yaml
-from NCPNet.brain_data import HemiBrain,LinkPred_Loader,Celegans19,LinkPred_PairNeigh_Loader
-
+from NCPNet.brain_data import HemiBrain,Celegans19
+from NCPNet.loader import LinkPred_Loader,LinkPred_PairNeigh_Loader
 import torch_geometric.transforms as T
 from NCPNet.approaches import Net
 from NCPNet.utils import load_config,edge_index2Graph
 from NCPNet.task import Base_Task
 from torch_geometric.loader import RandomNodeSampler,NeighborLoader
 from torch_geometric.transforms import RandomLinkSplit
 from NCPNet.trainer import LinkPred_trainer
```

### Comparing `NCPNet-1.0.3/NCPNet/task.py` & `NCPNet-1.0.4/NCPNet/task.py`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.3/NCPNet/trainer.py` & `NCPNet-1.0.4/NCPNet/trainer.py`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.3/NCPNet/utils.py` & `NCPNet-1.0.4/NCPNet/utils.py`

 * *Files identical despite different names*

### Comparing `NCPNet-1.0.3/setup.py` & `NCPNet-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name='NCPNet',
-    version='1.0.3',
+    version='1.0.4',
     author='Guojia Wan',
     author_email='guojiawan@whu.edu.cn',
     description='Learning synapse-level brain circuit networks. Include training, inferring, evaluation, and visualization.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/mxz12119/NCPNet',
     packages=find_packages(),
-    setup_requires=['torch==1.8.0'],
+    setup_requires=['torch>=2.0.1'],
     install_requires=[
-        'torch_geometric==2.0.1',
-        'torch-cluster==1.5.9',
-        'torch-sparse==0.6.12',
-        'torch-scatter==2.0.8',
-        'navis==1.3.1',
+        'torch_geometric>=2.3.1',
+        'torch-cluster>=1.6.1',
+        'torch-sparse>=0.6.17',
+        'torch-scatter>=2.1.1',
+        'navis==1.4.0',
         'neuprint-python==0.4.25',
         'networkx',
         'tqdm',
         'tensorboardx',
         'pandas',
         'numpy',
         'scikit-learn',
-        'zmq'
+        'zmq',
+        'pyyaml'
     ],
     python_requires='>=3.7',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```

