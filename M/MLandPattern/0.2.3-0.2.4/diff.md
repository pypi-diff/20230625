# Comparing `tmp/MLandPattern-0.2.3.tar.gz` & `tmp/MLandPattern-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.2.3.tar", last modified: Sun Jun 25 17:39:21 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.4.tar", last modified: Sun Jun 25 17:59:54 2023, max compression
```

## Comparing `MLandPattern-0.2.3.tar` & `MLandPattern-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:39:21.325367 MLandPattern-0.2.3/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:39:21.319216 MLandPattern-0.2.3/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    22003 2023-06-25 17:38:56.000000 MLandPattern-0.2.3/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.3/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:39:21.322121 MLandPattern-0.2.3/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-25 17:39:21.000000 MLandPattern-0.2.3/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 17:39:21.324015 MLandPattern-0.2.3/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.3/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-25 17:39:21.326186 MLandPattern-0.2.3/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-25 17:39:18.000000 MLandPattern-0.2.3/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:59:54.337662 MLandPattern-0.2.4/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:59:54.333913 MLandPattern-0.2.4/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    21989 2023-06-25 17:59:34.000000 MLandPattern-0.2.4/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.4/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 17:59:54.336558 MLandPattern-0.2.4/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 17:59:54.000000 MLandPattern-0.2.4/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-25 17:59:54.000000 MLandPattern-0.2.4/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-25 17:59:54.000000 MLandPattern-0.2.4/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-25 17:59:54.000000 MLandPattern-0.2.4/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 17:59:54.337270 MLandPattern-0.2.4/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.4/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-25 17:59:54.337823 MLandPattern-0.2.4/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-25 17:59:42.000000 MLandPattern-0.2.4/setup.py
```

### Comparing `MLandPattern-0.2.3/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.4/MLandPattern/MLandPattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     Calculates the Lineal Discriminant Analysis to perform dimension reduction
     :param matrix_values: matrix with the datapoints, with each row being a point
     :param label: vector with the label values associated with the dataset
     :param m: number of dimensions of the targeted sub-space
     :return: the LDA directions matrix (W), and the orthogonal sub-space of the directions (U)
     """
     class_labels = np.unique(label)
-    [Sw, Sb] = between_within_covariance(matrix_values, label, class_labels)
+    [Sw, Sb] = between_within_covariance(matrix_values, label)
     s, U = scipy.linalg.eigh(Sb, Sw)
     W = U[:, ::-1][:, 0:m]
     UW, _, _ = np.linalg.svd(W)
     U = UW[:, 0:m]
     return W, U
```

