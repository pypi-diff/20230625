# Comparing `tmp/TorchSisso-1.0.9.tar.gz` & `tmp/TorchSisso-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSisso-1.0.9.tar", last modified: Fri Jun  9 14:26:49 2023, max compression
+gzip compressed data, was "TorchSisso-1.1.0.tar", last modified: Sun Jun 25 21:23:38 2023, max compression
```

## Comparing `TorchSisso-1.0.9.tar` & `TorchSisso-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-09 14:26:49.128782 TorchSisso-1.0.9/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-09 14:26:49.126790 TorchSisso-1.0.9/PKG-INFO
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-09 14:26:49.108788 TorchSisso-1.0.9/TorchSisso/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)    18780 2023-06-09 14:13:32.000000 TorchSisso-1.0.9/TorchSisso/FeatureSpaceConstruction.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8511 2023-06-09 14:15:23.000000 TorchSisso-1.0.9/TorchSisso/SISSO_REGRESSOR_TORCH.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      228 2023-06-08 12:10:38.000000 TorchSisso-1.0.9/TorchSisso/__init__.py
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)     5407 2023-06-09 14:24:20.000000 TorchSisso-1.0.9/TorchSisso/testRegressor.py
-drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-09 14:26:49.123787 TorchSisso-1.0.9/TorchSisso.egg-info/
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/PKG-INFO
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      303 2023-06-09 14:26:49.000000 TorchSisso-1.0.9/TorchSisso.egg-info/SOURCES.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/dependency_links.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/requires.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-09 14:26:48.000000 TorchSisso-1.0.9/TorchSisso.egg-info/top_level.txt
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-09 14:26:49.128788 TorchSisso-1.0.9/setup.cfg
--rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-09 14:26:42.000000 TorchSisso-1.0.9/setup.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-25 21:23:38.846594 TorchSisso-1.1.0/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-25 21:23:38.845596 TorchSisso-1.1.0/PKG-INFO
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-25 21:23:38.825595 TorchSisso-1.1.0/TorchSisso/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)    18880 2023-06-25 20:42:34.000000 TorchSisso-1.1.0/TorchSisso/FeatureSpaceConstruction.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     8606 2023-06-25 21:23:04.000000 TorchSisso-1.1.0/TorchSisso/SISSO_REGRESSOR_TORCH.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      228 2023-06-08 12:10:38.000000 TorchSisso-1.1.0/TorchSisso/__init__.py
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)     6903 2023-06-23 22:22:41.000000 TorchSisso-1.1.0/TorchSisso/testRegressor.py
+drwxr-x---   0 muthyala.7 (815005582) domain users (10000)        0 2023-06-25 21:23:38.841594 TorchSisso-1.1.0/TorchSisso.egg-info/
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      423 2023-06-25 21:23:38.000000 TorchSisso-1.1.0/TorchSisso.egg-info/PKG-INFO
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      303 2023-06-25 21:23:38.000000 TorchSisso-1.1.0/TorchSisso.egg-info/SOURCES.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)        1 2023-06-25 21:23:38.000000 TorchSisso-1.1.0/TorchSisso.egg-info/dependency_links.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       19 2023-06-25 21:23:38.000000 TorchSisso-1.1.0/TorchSisso.egg-info/requires.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       11 2023-06-25 21:23:38.000000 TorchSisso-1.1.0/TorchSisso.egg-info/top_level.txt
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)       38 2023-06-25 21:23:38.847594 TorchSisso-1.1.0/setup.cfg
+-rw-r-----   0 muthyala.7 (815005582) domain users (10000)      738 2023-06-25 21:23:29.000000 TorchSisso-1.1.0/setup.py
```

### Comparing `TorchSisso-1.0.9/TorchSisso/FeatureSpaceConstruction.py` & `TorchSisso-1.1.0/TorchSisso/FeatureSpaceConstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
       #getting list of cobinations without replacement using itertools 
       combinations1 = list(combinations(self.columns,2))
       combinations2 = torch.combinations(torch.arange(self.df_feature_values.shape[1]),2)
       comb_tensor = self.df_feature_values.T[combinations2,:]
       #Reshaping to match
       x_p = comb_tensor.permute(0,2,1)
+      del comb_tensor
       for op in operators_set:
           self.feature_values11 = torch.empty(self.df.shape[0],0).to(self.device)
           feature_names_11 = []
           if op =='+':
               sum = torch.sum(x_p,dim=2).T
               self.feature_values11 = torch.cat((self.feature_values11,sum),dim=1)
               feature_names_11.extend(list(map(lambda comb: '('+'+'.join(comb)+')', combinations1)))
@@ -202,14 +203,15 @@
               feature_names_11.extend(list(map(lambda comb: '('+'/'.join(comb[::-1])+')', combinations1)))
           elif op == '*':
               mul = torch.multiply(x_p[:,:,0],x_p[:,:,1]).T
               self.feature_values11 = torch.cat((self.feature_values11,mul),dim=1)
               feature_names_11.extend(list(map(lambda comb: '('+'*'.join(comb)+')', combinations1)))
           self.feature_values1 = torch.cat((self.feature_values1,self.feature_values11),dim=1)
           self.feature_names1.extend(feature_names_11)
+          del self.feature_values11, feature_names_11
               
       #Checking whether the lists are empty
       if len(self.feature_names1) == 0:
           return self.feature_values1, self.feature_names1
       else:
           #Removing Nan and inf columns from tenosr and corresponding variable name form the list
           #self.feature_values1 = torch.cat(self.feature_values2,dim=1)
@@ -218,15 +220,15 @@
           nan_or_inf_columns = nan_columns | inf_columns
     
           # Remove columns from tensor
           self.feature_values1 = self.feature_values1[:, ~nan_or_inf_columns]
     
           # Remove corresponding elements from list
           self.feature_names1 = [elem for i, elem in enumerate(self.feature_names1) if not nan_or_inf_columns[i]]
-    
+          
           #Returning the dataframe created
           return self.feature_values1,self.feature_names1 #created_space
   
 
   '''
   ##########################################################################################################
 
@@ -249,20 +251,22 @@
     space_created = torch.cat((self.df_feature_values,values,values1), dim=1).to(self.device)
     self.columns = self.columns + names + names1 
     del values, values1, names, names1
     print('First Feature Space building is completed with features count: ',int(space_created.shape[1]))
     print('Time for phi1 creation is: ',round(time.time() - start_time,3),' seconds')
     #Update the columns according to the new phi created for the next phase features
     self.df_feature_values = (space_created).to(self.device)
+    del space_created
+
     #Creating the phi2 based on the space created 
     start_time = time.time()
     values, names = self.combinations(basic_operators)
     values1, names1 = self.single_variable(other_operators)
-    space_created_2 = torch.cat((space_created,values,values1), dim=1).to(self.device)
-    del space_created,values,values1
+    space_created_2 = torch.cat((self.df_feature_values,values,values1), dim=1).to(self.device)
+    del values,values1
     self.columns = self.columns + names + names1 
     del names, names1
     #######################
     #code to remove duplicate columns from dataframe
     #########################
     #Converting tensor to numpy and then dataframe to remove duplicates
     space = pd.DataFrame(space_created_2.cpu(),columns = self.columns)
```

### Comparing `TorchSisso-1.0.9/TorchSisso/SISSO_REGRESSOR_TORCH.py` & `TorchSisso-1.1.0/TorchSisso/SISSO_REGRESSOR_TORCH.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,21 @@
 import time 
 import torch.nn as nn
 import torch.optim as optim
 import itertools
 import pdb
 class SISSORegressor:
     
-    def __init__(self,x,y,names,dimension=1,sis_features=20,method='L0',device='cpu'):
+    def __init__(self,x,y,names,dimension=1,sis_features=20,device='cpu'):
         self.device = device
         self.x = x.to(self.device)
         self.y = y.to(self.device)
         self.names = names
         self.dimension = dimension
         self.sis_features = sis_features
-        self.method = method 
         self.x_mean = self.x.mean(dim=0)
         self.x_std = self.x.std(dim=0)
         self.y_mean = self.y.mean()
         self.y_centered = self.y - self.y_mean
         self.x_standardized = ((self.x - self.x_mean)/self.x_std)
         self.scores = []
         self.indices = torch.arange(1, (self.dimension*self.sis_features+1)).view(self.dimension*self.sis_features,1).to(self.device)
@@ -116,16 +115,16 @@
                 self.indices = torch.cat((self.indices,sorted_indices),dim=1)
                 #selected_index = self.indices[0,0]
                 selected_index = self.indices[0,1]
                 x_in = self.x[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias = torch.cat((torch.ones_like(x_in), x_in), dim=1).to(self.device)
                 #Calculate the intercept and coefficient, Non standardized
-                #coef1, _, _, _ = torch.linalg.lstsq(x_with_bias, self.y)
-                coef1 = torch.pinverse(x_with_bias).to(self.device) @ self.y
+                coef1, _, _, _ = torch.linalg.lstsq(x_with_bias, self.y)
+                #coef1 = torch.pinverse(x_with_bias).to(self.device) @ self.y
                 #Calculate the residuals based on the standardized and centered values
                 x_in1 = self.x_standardized[:, int(selected_index)].unsqueeze(1)
                 # Add a column of ones to x for the bias term
                 x_with_bias1 = torch.cat((torch.ones_like(x_in1), x_in1), dim=1)
                 #coef, _, _, _ = torch.linalg.lstsq(x_with_bias1, self.y_centered)
                 coef = torch.pinverse(x_with_bias1).to(self.device) @ self.y_centered
                 self.residual = (self.y_centered - (coef[1]*self.x_standardized[:, int(selected_index)])).unsqueeze(1).T
@@ -138,28 +137,30 @@
                     print('Equation: ', equation)
                     print('RMSE: ', rmse)
                 else:
                     equation = str(float(coefficient)) + '*' + str(self.names[int(selected_index)])  + str(float(intercept))
                     print('Equation: ', equation)
                     print('RMSE: ', rmse)
                 print('Time taken to generate one dimensional equation: ', time.time()-start_1D,'seconds')
+                if self.device == 'cuda':torch.cuda.empty_cache()
             else:
                 start = time.time()
                 rmse,terms,intercept,coefs = self.higher_dimension(i)
                 equation =''
                 for k in range(len(terms)):
                     print(f'{k+1} term in the equation is {terms[k]}')
                     if coefs.flatten()[k] > 0:
-                        equation = equation + ' + ' + (str(terms[k])) 
+                        equation = equation + ' + ' + (str(terms[k]))+'  '
                     else:
                         equation = equation + (str(terms[k])) + '  '
                 print('Equation: ',equation[:len(equation)-1])
                 print('Intercept:', float(intercept))
                 print('RMSE:',float(rmse))
                 print(f'Time taken for {i} dimension is: ', time.time()-start)
+                if self.device == 'cuda': torch.cuda.empty_cache()
         return float(rmse),equation
```

### Comparing `TorchSisso-1.0.9/setup.py` & `TorchSisso-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import setuptools
 
 
 setuptools.setup(
     name="TorchSisso",
-    version="1.0.9",
+    version="1.1.0",
     author="Madhav Muthyala",
     author_email="madhavreddymuthyala@gmail.com",
     description="GPU Supported Sure Independence Screening and Sparsifying Operator Package",
     url="https://github.com/MR1319/TorchSisso",
     packages=setuptools.find_packages(),
     install_requires=[
         "torch",
```

