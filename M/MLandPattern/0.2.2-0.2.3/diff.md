# Comparing `tmp/MLandPattern-0.2.2.tar.gz` & `tmp/MLandPattern-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.2.2.tar", last modified: Sun Jun 25 15:30:44 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.3.tar", last modified: Sun Jun 25 17:39:21 2023, max compression
```

## Comparing `MLandPattern-0.2.2.tar` & `MLandPattern-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 15:30:44.651630 MLandPattern-0.2.2/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 15:30:44.644349 MLandPattern-0.2.2/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    21938 2023-06-13 15:17:56.000000 MLandPattern-0.2.2/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.2/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 15:30:44.650589 MLandPattern-0.2.2/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 15:30:44.651290 MLandPattern-0.2.2/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.2/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-25 15:30:44.651772 MLandPattern-0.2.2/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-25 15:30:07.000000 MLandPattern-0.2.2/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:39:21.325367 MLandPattern-0.2.3/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:39:21.319216 MLandPattern-0.2.3/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    22003 2023-06-25 17:38:56.000000 MLandPattern-0.2.3/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.3/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:39:21.322121 MLandPattern-0.2.3/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 17:39:21.324015 MLandPattern-0.2.3/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.3/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-25 17:39:21.326186 MLandPattern-0.2.3/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-25 17:39:18.000000 MLandPattern-0.2.3/setup.py
```

### Comparing `MLandPattern-0.2.2/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.3/MLandPattern/MLandPattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,22 +121,23 @@
         return s, U
 
 
 def PCA(attribute_matrix, m):
     """
     Calculates the PCA dimension reduction of a matrix to a m-dimension sub-space
     :param attribute_matrix: matrix with the datapoints, with each row being a point
-    :param m: number of dimensions of the targeted sub-space
+    `param m` number of dimensions of the targeted sub-space
+    :return: The matrix P defined to do the PCA approximation
     :return: The dataset after the dimensionality reduction
     """
     DC = center_data(attribute_matrix)
     C = covariance(DC, 1)
     s, U = eigen(C)
     P = U[:, ::-1][:, 0:m]
-    return np.dot(P.T, attribute_matrix)
+    return P, np.dot(P.T, attribute_matrix)
 
 
 def covariance_within_class(matrix_values, label):
     """
     Calculates the average covariance within all the classes in a dataset
     :param matrix_values: matrix with the values associated to the parameters of the dataset
     :param label: vector with the label values associated with the dataset
```

