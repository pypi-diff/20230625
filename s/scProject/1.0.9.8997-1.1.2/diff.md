# Comparing `tmp/scProject-1.0.9.8997.tar.gz` & `tmp/scProject-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/abaraban/PycharmProjects/scProject/dist/tmptgyuj8zs/scProject-1.0.9.8997.tar", last modified: Tue Jul  6 01:18:39 2021, max compression
+gzip compressed data, was "scProject-1.1.2.tar", last modified: Sat Jun 24 19:26:20 2023, max compression
```

## Comparing `scProject-1.0.9.8997.tar` & `scProject-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxr-xr-x   0 abaraban   (504) staff       (20)        0 2021-07-06 01:18:39.787132 scProject-1.0.9.8997/
--rw-r--r--   0 abaraban   (504) staff       (20)     1065 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/LICENSE
--rw-r--r--   0 abaraban   (504) staff       (20)       11 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/LICENSE.txt
--rw-r--r--   0 abaraban   (504) staff       (20)      624 2021-07-06 01:18:39.787213 scProject-1.0.9.8997/PKG-INFO
--rw-r--r--   0 abaraban   (504) staff       (20)      168 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/README.md
-drwxr-xr-x   0 abaraban   (504) staff       (20)        0 2021-07-06 01:18:39.784387 scProject-1.0.9.8997/scProject/
--rw-r--r--   0 abaraban   (504) staff       (20)       76 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/__init__.py
--rw-r--r--   0 abaraban   (504) staff       (20)     5903 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/matcher.py
--rw-r--r--   0 abaraban   (504) staff       (20)     4566 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/rg.py
--rw-r--r--   0 abaraban   (504) staff       (20)    19248 2021-07-06 00:34:46.000000 scProject-1.0.9.8997/scProject/stats.py
-drwxr-xr-x   0 abaraban   (504) staff       (20)        0 2021-07-06 01:18:39.786969 scProject-1.0.9.8997/scProject/test/
--rw-r--r--   0 abaraban   (504) staff       (20)        0 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/test/__init__.py
--rw-r--r--   0 abaraban   (504) staff       (20)      171 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/test/projection_object_test.py
--rw-r--r--   0 abaraban   (504) staff       (20)     2183 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/test/projection_test.py
--rw-r--r--   0 abaraban   (504) staff       (20)        0 2021-07-05 16:00:10.000000 scProject-1.0.9.8997/scProject/test/test_projection.py
--rw-r--r--   0 abaraban   (504) staff       (20)    16941 2021-07-06 00:59:23.000000 scProject-1.0.9.8997/scProject/viz.py
-drwxr-xr-x   0 abaraban   (504) staff       (20)        0 2021-07-06 01:18:39.785729 scProject-1.0.9.8997/scProject.egg-info/
--rw-r--r--   0 abaraban   (504) staff       (20)      624 2021-07-06 01:18:39.000000 scProject-1.0.9.8997/scProject.egg-info/PKG-INFO
--rw-r--r--   0 abaraban   (504) staff       (20)      411 2021-07-06 01:18:39.000000 scProject-1.0.9.8997/scProject.egg-info/SOURCES.txt
--rw-r--r--   0 abaraban   (504) staff       (20)        1 2021-07-06 01:18:39.000000 scProject-1.0.9.8997/scProject.egg-info/dependency_links.txt
--rw-r--r--   0 abaraban   (504) staff       (20)       10 2021-07-06 01:18:39.000000 scProject-1.0.9.8997/scProject.egg-info/top_level.txt
--rw-r--r--   0 abaraban   (504) staff       (20)       79 2021-07-06 01:18:39.787618 scProject-1.0.9.8997/setup.cfg
--rw-r--r--   0 abaraban   (504) staff       (20)      600 2021-07-06 01:16:59.000000 scProject-1.0.9.8997/setup.py
+drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:26:20.942992 scProject-1.1.2/
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     1065 2023-06-24 19:19:30.000000 scProject-1.1.2/LICENSE
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     2965 2023-06-24 19:26:20.943186 scProject-1.1.2/PKG-INFO
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     2516 2023-06-24 19:24:14.000000 scProject-1.1.2/README.md
+drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:26:20.938524 scProject-1.1.2/scProject/
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       76 2023-06-24 19:19:30.000000 scProject-1.1.2/scProject/__init__.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     5929 2023-06-24 19:19:30.000000 scProject-1.1.2/scProject/matcher.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     4572 2023-06-24 19:19:30.000000 scProject-1.1.2/scProject/rg.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)    19458 2023-06-24 19:19:30.000000 scProject-1.1.2/scProject/stats.py
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)    19166 2023-06-24 19:19:35.000000 scProject-1.1.2/scProject/viz.py
+drwxr-xr-x   0 WHITEKNIGHT2022   (501) staff       (20)        0 2023-06-24 19:26:20.942505 scProject-1.1.2/scProject.egg-info/
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     2965 2023-06-24 19:26:20.000000 scProject-1.1.2/scProject.egg-info/PKG-INFO
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)      295 2023-06-24 19:26:20.000000 scProject-1.1.2/scProject.egg-info/SOURCES.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)        1 2023-06-24 19:26:20.000000 scProject-1.1.2/scProject.egg-info/dependency_links.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)     1829 2023-06-24 19:26:20.000000 scProject-1.1.2/scProject.egg-info/requires.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       10 2023-06-24 19:26:20.000000 scProject-1.1.2/scProject.egg-info/top_level.txt
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)       79 2023-06-24 19:26:20.943928 scProject-1.1.2/setup.cfg
+-rw-r--r--   0 WHITEKNIGHT2022   (501) staff       (20)      752 2023-06-24 19:23:21.000000 scProject-1.1.2/setup.py
```

### Comparing `scProject-1.0.9.8997/LICENSE` & `scProject-1.1.2/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Goff Lab
+Copyright (c) 2023 Goff Lab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `scProject-1.0.9.8997/scProject/matcher.py` & `scProject-1.1.2/scProject/matcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Feature matching/mapping between source (annData) and target (patterns) datasets
 ##################
 import anndata as ad
 import scanpy as sc
 import numpy as np
 from scipy import sparse
 import pandas as pd
+import copy
 
 
 # class SourceTypeError(AssertionError):
 # 	"""Raised if source is not AnnData"""
 # 	print("Source data must be a valid AnnData object")
 
 def sourceIsValid(adata):
@@ -111,17 +112,17 @@
     :return: A tuple of two filtered AnnData objects
     """
 
     sourceIsValid(dataset)  # Make sure dataset is an AnnData object
     sourceIsValid(patterns)  # Make sure patterns is an AnnData object
     dataset.var = dataset.var.set_index(geneColumnName)
     overlap = dataset.var.index.intersection(patterns.var.index)
-    dataset_filtered = dataset[:, overlap]
+    dataset_filtered = dataset[:, overlap].copy()
     print(dataset_filtered.shape, "dataset filter shape")
-    patterns_filtered = patterns[:, overlap]
+    patterns_filtered = patterns[:, overlap].copy()
     print(patterns_filtered.shape, "patterns filter shape")
     dataset_filtered.X[dataset_filtered.X < 0] = 0
     patterns_filtered.X[patterns_filtered.X < 0] = 0
     # Normalize both dataset and pattern columns to 5 L1
     if sparse.issparse(patterns_filtered.X):
         patterns_filtered.X = patterns_filtered.X.toarray()
```

### Comparing `scProject-1.0.9.8997/scProject/rg.py` & `scProject-1.1.2/scProject/rg.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from sklearn import linear_model
 import numpy as np
 
 
 def NNLR_ElasticNet(dataset_filtered, patterns_filtered, projectionName, alpha, L1, layer=False, iterations=10000, positive=True):
     """ This method performs an elastic net regression from sci-kit learn. Currently it only takes in dense matrices.
 
-    :param dataset_filtered: AnnData object cells x genes
-    :param patterns_filtered: AnnData object features x genes
+    :param dataset_filtered: AnnData object genes x samples
+    :param patterns_filtered: AnnData object genes x features
     :param projectionName: index of the projection in dataset_filtered.obsm
     :type projectionName: String
     :param alpha: regularization parameter
     :type alpha: double
     :param L1: regularization parameter
     :type L1: double
     :param layer: Layer of dataset to regress on string
@@ -35,16 +35,16 @@
         print(model.coef_.shape)
 
 
 # still experimenting with this but same idea as NNLR_Elastic net, but implements a lasso regression instead
 def NNLR_positive_Lasso(dataset_filtered, patterns_filtered, projectionName, alpha, layer=False, iterations=10000):
     """This method performs a positive lasso regression from sci-kit learn.
 
-    :param dataset_filtered: AnnData object cells x genes
-    :param patterns_filtered: AnnData object features x genes
+    :param dataset_filtered: AnnData object genes x samples
+    :param patterns_filtered: AnnData object genes x features
     :param projectionName: index of the projection in dataset_filtered.obsm
     :param alpha: regularization parameter
     :param layer: Layer with which to perform the regression
     :param iterations: number of iterations while performing the regression
     :return: void, the dataset_filtered is mutated and the projection is stored in dataset_filtered.obsm[projectionName]
     """
     matcher.sourceIsValid(dataset_filtered)
@@ -62,16 +62,16 @@
 
 
 # still experimenting with this but same idea as NNLR_Elastic net, but implements ordinary least squares from scipy no
 # regularization
 def NNLR_LeastSquares(dataset_filtered, patterns_filtered, projectionName):
     """This performs a non negative least squares regression using Scipy.
 
-    :param dataset_filtered: AnnData object cells x genes
-    :param patterns_filtered: AnnData object features x genes
+    :param dataset_filtered: AnnData object genes x samples
+    :param patterns_filtered: AnnData object genes x features
     :param projectionName: index of the projection in dataset_filtered.obsm
     :return: void, the dataset_filtered is mutated and the projection is stored in dataset_filtered.obsm[projectionName]
     """
     matcher.sourceIsValid(dataset_filtered)
     matcher.sourceIsValid(patterns_filtered)
     print(patterns_filtered.X.shape[0], "patterns", dataset_filtered.X.T.shape[1], "data")
     pattern_matrix = np.zeros([patterns_filtered.X.shape[0], dataset_filtered.X.T.shape[1]])
```

### Comparing `scProject-1.0.9.8997/scProject/stats.py` & `scProject-1.1.2/scProject/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import matplotlib.pyplot as plt
 import scipy.stats
 from . import matcher
 from scipy.stats import t
 from scipy.sparse import issparse
 import math
 import pandas as pd
+import os
 
 
 def importantGenes(patterns_filtered, featureNumber, threshold):
     """Returns the list of genes that are expressed greater than threshold in the feature.
 
     :param patterns_filtered: AnnData object features x genes
     :param featureNumber: Which pattern you want to examine
@@ -233,31 +234,31 @@
         C2CovM = np.cov(C2Dense, rowvar=False, bias=False)
     else:
         C2CovM = np.cov(cluster2.X, rowvar=False, bias=False)
 
     pooled = ((n1 - 1) * C1CovM + (n2 - 1) * C2CovM) / (n1 + n2 - 2)
 
     list1 = []
-    count = 0
+
     for i in range(dimensionality):
         pooledVar = pooled[i, i]
         scale = tval * math.sqrt(((1 / n1) + (1 / n2)) * pooledVar)
 
         diff = MeanDiff[0, i]
         plusminus[0, i] = diff - scale
         plusminus[1, i] = diff + scale
         if plusminus[0, i] < 0 and plusminus[1, i] < 0:
-            if verbose is 0:
+            if verbose == 0:
                 print('Gene Name: {0} Mean Difference: {1} Low: {2} High {3}'.format(cluster1.var[varName][i], diff,
                                                                                      plusminus[0, i], plusminus[1, i]))
             gene = cluster1.var[varName][i]
             list1.append(gene)
 
         if plusminus[0, i] > 0 and plusminus[1, i] > 0:
-            if verbose is 0:
+            if verbose == 0:
                 print('Gene Name: {0} Mean Difference: {1} Low: {2} High {3}'.format(cluster1.var[varName][i], diff,
                                                                                      plusminus[0, i], plusminus[1, i]))
             gene = cluster1.var[varName][i]
             list1.append(gene)
 
     data = pd.DataFrame(np.transpose(plusminus), index=cluster1.var[varName], columns=['Low', 'High'])
     filt = ((data['High'] > 0) & (data['Low'] > 0)) | ((data['High'] < 0) & (data['Low'] < 0))
@@ -324,15 +325,15 @@
     MeanDiff = (C1Mean - C2Mean)
     feature = patterns_filtered[(featureNumber - 1)].copy()
     # construct weighted Mean Difference using specified feature
     curNorm = np.linalg.norm(np.reshape(feature.X, -1), ord=1)
     numNonzero = np.count_nonzero(feature.X)
     normalized = feature.X * (numNonzero / curNorm)
     drivers = np.multiply(np.reshape(normalized, -1), np.reshape(MeanDiff, -1))
-    drivers = np.reshape(drivers, (1, 2412))
+    drivers = np.reshape(drivers, (1, drivers.shape[0]))
     feature.X = normalized
 
     plusminus = np.zeros((2, drivers.shape[1]))
     n1 = cluster1.shape[0]
     n2 = cluster2.shape[0]
     pVal = 1 - alpha
     boncorrect = pVal / (2 * dimensionality)
@@ -347,15 +348,15 @@
         C2CovM = np.cov(C2Dense)
     else:
         C2CovM = np.cov(cluster2.X, rowvar=False, bias=False)
 
     pooled = ((n1 - 1) * C1CovM + (n2 - 1) * C2CovM) / (n1 + n2 - 2)
 
     list1 = []
-    count = 0
+
     for i in range(dimensionality):
         pooledVar = pooled[i, i]
         scale = tval * math.sqrt(((1 / n1) + (1 / n2)) * pooledVar)
 
         diff = drivers[0, i]
         plusminus[0, i] = diff - scale
         plusminus[1, i] = diff + scale
@@ -377,15 +378,15 @@
 
     filtStand = ((standardBon['High'] > 0) & (standardBon['Low'] > 0)) | (
             (standardBon['High'] < 0) & (standardBon['Low'] < 0))
     filtDriver = ((driverBon['High'] > 0) & (driverBon['Low'] > 0)) | (
             (driverBon['High'] < 0) & (driverBon['Low'] < 0))
 
     commonGenes = set(standardBon[filtStand].index).intersection(set(driverBon[filtDriver].index))
-    intersection = standardBon.loc[commonGenes]
+    intersection = standardBon.loc[list(commonGenes)]
 
     if display:
         if path is None:
             raise ValueError("Path Cannot Be None When Display is True")
         mapper = dict(zip(cluster1.var.index, cluster1.var['gene_short_name']))
         geneShorts = [mapper[i] for i in feature.var.index]
         feature.var.index = geneShorts
@@ -423,13 +424,18 @@
             plt.annotate(txt, (mean, patternWeight + .5), fontsize=annotationSize)
             plt.plot((low, high), (patternWeight, patternWeight), '-', color='black')
         plt.plot(x1, y1, color='black')
         plt.ylim(bottom=-.25, top=max(sigPatternWeight.values)[0] + 10)
         plt.title("Latent Space " + str(featureNumber), fontsize=titleFontsize)
         plt.xlabel("Log 2 Fold Change", fontsize=axisFontsize)
         plt.ylabel("L1 Adjusted Pattern Weight", fontsize=axisFontsize)
+        # Directory path and filename
+        directory = os.path.dirname(path)
+        # Create the directory if it doesn't exist
+        if not os.path.exists(directory):
+            os.makedirs(directory)
         plt.savefig(path)
 
     return intersection, driverBon, standardBon
 
 
     # return pd.DataFrame(np.transpose(plusminus), index=cluster1.var[varName], columns=['Low', 'High'])
```

### Comparing `scProject-1.0.9.8997/scProject/viz.py` & `scProject-1.1.2/scProject/viz.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import matplotlib.pyplot as plt
 import matplotlib.colors as clrs
 from scipy import stats
 import numpy as np
 import umap
 import seaborn as sns
 import matplotlib.patches as mpatches
+import os
 
 
 def pearsonMatrix(dataset_filtered, patterns_filtered, cellTypeColumnName, num_cell_types, projectionName, plotName,
                   plot, row_cluster=True, col_cluster=True, path=None, display=True, dpi=300, xtickSize=8, ytickSize=8):
     """This method finds the pearson correlation coefficient between every pattern and every cell type
 
     :param dataset_filtered: Anndata object cells x genes
@@ -89,18 +90,26 @@
                     xticklabels=dataset_filtered.obs[cellTypeColumnName].unique(),
                     yticklabels=y_ticks)
         plt.tick_params(axis='y', labelsize=ytickSize)
         plt.tick_params(axis='x', labelsize=xtickSize)
     if path is None and display is True:
         plt.show()
     if path is not None and display is False:
+        # Create the directory if it doesn't exist
+        directory = os.path.dirname(path)
+        if not os.path.exists(directory):
+            os.makedirs(directory)
         plt.savefig(path, dpi=dpi)
         plt.close()
     if path is not None and display is True:
         plt.show()
+        # Create the directory if it doesn't exist
+        directory = os.path.dirname(path)
+        if not os.path.exists(directory):
+            os.makedirs(directory)
         plt.savefig(path, dpi=dpi)
 
 
 def UMAP_Projection(dataset_filtered, cellTypeColumnName, projectionName, UMAPName, n_neighbors, metric='euclidean',
                     plot=True, colorScheme='Paired', pointSize=.5, subset=None, path=None, display=True, dpi=300):
     """This method projects the pattern matrix down into 2 dimensional space. Make sure the colorScheme chosen has
     enough colors for every cell type.
@@ -161,16 +170,24 @@
             handles.append(mpatches.Patch(color=(sns.color_palette(colorScheme, n_colors=numTypes)[i]),
                                           label=dataset_filtered.obs[cellTypeColumnName].unique()[i]))
         plt.legend(handles=handles, title="Cell Types", fontsize='xx-small', loc='best')
         if display is True and path is None:
             plt.show()
         if display is True and path is not None:
             plt.show()
+            # Create the directory if it doesn't exist
+            directory = os.path.dirname(path)
+            if not os.path.exists(directory):
+                os.makedirs(directory)
             plt.savefig(path, dpi=dpi)
         if display is False and path is not None:
+            # Create the directory if it doesn't exist
+            directory = os.path.dirname(path)
+            if not os.path.exists(directory):
+                os.makedirs(directory)
             plt.savefig(path, dpi=dpi)
             plt.close()
     else:
         subsetted = dataset_filtered[dataset_filtered.obs[cellTypeColumnName].isin(subset)]
         color = matcher.mapCellNamesToInts(subsetted, cellTypeColumnName)
         nd = subsetted.obsm[UMAPName]
         numTypes = subsetted.obs[cellTypeColumnName].unique().shape[0]
@@ -186,16 +203,24 @@
             handles.append(mpatches.Patch(color=(sns.color_palette(colorScheme, n_colors=numTypes)[i]),
                                           label=subsetted.obs[cellTypeColumnName].unique()[i]))
         plt.legend(handles=handles, title="Cell Types", fontsize='xx-small', loc='best')
         if display is True and path is None:
             plt.show()
         if display is True and path is not None:
             plt.show()
+            # Create the directory if it doesn't exist
+            directory = os.path.dirname(path)
+            if not os.path.exists(directory):
+                os.makedirs(directory)
             plt.savefig(path, dpi=dpi)
         if display is False and path is not None:
+            # Create the directory if it doesn't exist
+            directory = os.path.dirname(path)
+            if not os.path.exists(directory):
+                os.makedirs(directory)
             plt.savefig(path, dpi=dpi)
             plt.close()
 
 
 def featurePlots(dataset_filtered, num_patterns, projectionName, UMAPName, vmin=.00000000001, clip=99.5,
                  zeroColor='dimgrey', obsColumn=None, cmap='viridis', pointSize=.1, subset=None,
                  path=None, display=True, dpi=300):
@@ -237,16 +262,24 @@
                         cmap=colors, vmin=vmin, vmax=np.percentile(feature, clip), s=pointSize)
             plt.colorbar()
             print("Number of nonzero cells " + str(np.count_nonzero(feature)))
             if path is None:
                 plt.show()
             if path is not None and display is True:
                 plt.show()
+                # Create the directory if it doesn't exist
+                directory = os.path.dirname(path)
+                if not os.path.exists(directory):
+                    os.makedirs(directory)
                 plt.savefig(path + str(i) + ".png", dpi=dpi)
             if path is not None and display is False:
+                # Create the directory if it doesn't exist
+                directory = os.path.dirname(path)
+                if not os.path.exists(directory):
+                    os.makedirs(directory)
                 plt.savefig(path + str(i) + ".png", dpi=dpi)
                 plt.close()
     else:
         colors = plt.get_cmap(cmap)
         colors.set_under(zeroColor)
         for i in range(num_patterns):
             feature = pattern_matrix[:, i]
@@ -255,16 +288,24 @@
                         vmax=np.percentile(feature, clip), s=pointSize)
             plt.colorbar()
             print("Number of nonzero cells " + str(np.count_nonzero(feature)))
             if path is None:
                 plt.show()
             if path is not None and display is True:
                 plt.show()
+                # Create the directory if it doesn't exist
+                directory = os.path.dirname(path)
+                if not os.path.exists(directory):
+                    os.makedirs(directory)
                 plt.savefig(path + str(i + 1) + ".png", dpi=dpi)
             if path is not None and display is False:
+                # Create the directory if it doesn't exist
+                directory = os.path.dirname(path)
+                if not os.path.exists(directory):
+                    os.makedirs(directory)
                 plt.savefig(path + str(i + 1) + ".png", dpi=dpi)
                 plt.close()
 
 
 def patternWeightDistribution(dataset_filtered, projectionName, patterns, obsColumn, subset, numBins=100):
     """
 
@@ -278,15 +319,15 @@
     """
     subset = dataset_filtered[dataset_filtered.obs[obsColumn].isin(list(subset))]
     print("This subset has shape:", subset.shape)
 
     for i in patterns:
         filte = subset.obsm[projectionName][:, i-1] > 0
         maxval = np.max(subset.obsm[projectionName][:, i-1][filte])
-        if maxval is 0:
+        if maxval == 0:
             print("Feature " + str(i) + " is all 0 in this subset")
             continue
         bins = np.arange(0, maxval+1, (maxval + 1) / numBins)
 
         plt.title("Feature " + str(i))
         plt.hist(subset.obsm[projectionName][:, i-1][filte], bins=bins)
         plt.show()
@@ -313,45 +354,53 @@
     zipperWeighted = zip(list(wCIs.index), wCIs['Low'], wCIs['High'])
 
     counter = len(wCIs) - 1
     genes = []
     for geneName, low, high in zipperWeighted:
         genes.insert(0, geneName)
         plt.plot((low, high), (counter, counter), '-', color='blue')
-        if counter is 1:
+        if counter == 1:
             plt.plot((float(low + high) / 2.0), counter, 'o', color='blue', label=pointLabel)
         else:
             plt.plot((float(low + high) / 2.0), counter, 'o', color='blue')
         counter -= 1
 
     plt.title(weightTitle)
     plt.plot((0, 0), (0, numGenesToPlot), '--', color='black')
     plt.ylim(top=numGenesToPlot)
     plt.ylim(bottom=-1)
     plt.legend()
     plt.yticks(range(len(genes)), genes)
+    # Create the directory if it doesn't exist
+    directory = os.path.dirname(pathForWeight)
+    if not os.path.exists(directory):
+        os.makedirs(directory)
     plt.savefig(pathForWeight, dpi=300, bbox_inches='tight')
     plt.show()
 
     bCIs = projectionDriverOutput[2].loc[wCIs.index]
 
     zipperBCI = zip(list(bCIs.index), bCIs['Low'], bCIs['High'])
 
     counter = len(wCIs) - 1
     genes = []
     for geneName, low, high in zipperBCI:
         genes.insert(0, geneName)
         plt.plot((low, high), (counter, counter), '-', color='blue')
-        if counter is 1:
+        if counter == 1:
             plt.plot((float(low + high) / 2.0), counter, 'o', color='blue', label=pointLabel)
         else:
             plt.plot((float(low + high) / 2.0), counter, 'o', color='blue')
         counter -= 1
 
     plt.title(bonTitle)
     plt.plot((0, 0), (0, numGenesToPlot), '--', color='black')
     plt.ylim(top=numGenesToPlot)
     plt.ylim(bottom=-1)
     plt.legend()
     plt.yticks(range(len(genes)), genes)
+    # Create the directory if it doesn't exist
+    directory = os.path.dirname(pathForBon)
+    if not os.path.exists(directory):
+        os.makedirs(directory)
     plt.savefig(pathForBon, dpi=300, bbox_inches='tight')
     plt.show()
```

